🚀 5. Deploy com Nginx (Produção)Para disponibilizar a documentação na rede, geramos os arquivos estáticos e configuramos o Nginx.Gerar Build:Bashsource venv/bin/activate
mkdocs build
Os arquivos finais estarão na pasta /var/www/mkdocs-site/site.Configurar Virtual Host:Crie o arquivo /etc/nginx/sites-available/mkdocs:Nginxserver {
    listen 80;
    server_name docs.seu-dominio.internal; # Altere para o seu DNS

    root /var/www/mkdocs-site/site;
    index index.html;

    location / {
        try_files $uri $uri/ =404;
    }
}
Ativar Site:Bashsudo ln -s /etc/nginx/sites-available/mkdocs /etc/nginx/sites-enabled/
sudo nginx -t
sudo systemctl restart nginx
🔄 6. Comandos de ManutençãoObjetivoComandoAtivar ambientesource venv/bin/activateTestar localmentemkdocs serve -a 0.0.0.0:8000Atualizar Sitemkdocs buildAdicionar Pluginspip install <nome-do-plugin>Nota: Lembre-se de configurar o backup da pasta /var/www/mkdocs-site/docs ou manter o projeto sincronizado via Git.