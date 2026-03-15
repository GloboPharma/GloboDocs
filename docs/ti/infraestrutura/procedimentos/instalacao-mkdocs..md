# 📖 Modelo de Configuração e Instalação: MkDocs

Este documento descreve o padrão de instalação e configuração do MkDocs no servidor virtualizado **VM-DOCS-01**, hospedado no cluster **GP-VMS-02**.

## 🖥️ Informações do Ambiente
* **Hostname:** `VM-DOCS-01`
* **Host Físico/Grupo:** `GP-VMS-02`
* **Sistema Operacional:** Debian GNU/Linux 13 (Trixie)
* **Servidor Web:** Nginx
* **Referências:** [Remontti Blog](https://blog.remontti.com.br/6110) | [MkDocs User Guide](https://www.mkdocs.org/user-guide/deploying-your-docs/)

---

## 🛠️ 1. Preparação do Servidor

Atualize o sistema e instale as dependências necessárias para o Python e o servidor web.

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install python3 python3-venv python3-pip nginx git -y

📦 2. Instalação do MkDocs (Ambiente Virtual)
Seguindo as normas do Debian 13 para evitar conflitos com o apt, utilizaremos um ambiente virtual (venv).

Bash
# Definir diretório da aplicação
sudo mkdir -p /var/www/mkdocs-site
sudo chown $USER:$USER /var/www/mkdocs-site
cd /var/www/mkdocs-site

# Criar e ativar o ambiente virtual
python3 -m venv venv
source venv/bin/activate

# Instalar MkDocs e o tema Material
pip install mkdocs mkdocs-material

🏗️ 3. Estrutura do Projeto
Inicie um novo projeto no diretório atual:

Bash
mkdocs new .
Arquivos Gerados:
mkdocs.yml: Configurações de tema, plugins e navegação.

docs/: Pasta contendo os arquivos .md da sua documentação.

⚙️ 4. Configuração do mkdocs.yml
Abaixo, um modelo base configurado com o tema Material (recomendado):

YAML
site_name: Documentação Técnica - GP-VMS
site_url: [http://docs.seu-dominio.internal](http://docs.seu-dominio.internal)
repo_url: [https://github.com/seu-usuario/repo](https://github.com/seu-usuario/repo)

theme:
  name: material
  palette:
    - scheme: default
      primary: indigo
      accent: indigo
    - scheme: slate
      primary: blue
      accent: blue
  features:
    - navigation.tabs
    - search.suggest
    - search.highlight

nav:
  - Home: index.md
  - Servidores:
    - VM-DOCS-01: servidores/docs-01.md
  - Redes: rede/topologia.md
  
  O Gemini disse
Aqui está o conteúdo estruturado em formato Markdown (.md), pronto para ser copiado e salvo como um arquivo de documentação (ex: INSTALL_MKDOCS.md) ou utilizado no seu repositório de infraestrutura.

Markdown
# 📖 Modelo de Configuração e Instalação: MkDocs

Este documento descreve o padrão de instalação e configuração do MkDocs no servidor virtualizado **VM-DOCS-01**, hospedado no cluster **GP-VMS-02**.

## 🖥️ Informações do Ambiente
* **Hostname:** `VM-DOCS-01`
* **Host Físico/Grupo:** `GP-VMS-02`
* **Sistema Operacional:** Debian GNU/Linux 13 (Trixie)
* **Servidor Web:** Nginx
* **Referências:** [Remontti Blog](https://blog.remontti.com.br/6110) | [MkDocs User Guide](https://www.mkdocs.org/user-guide/deploying-your-docs/)

---

## 🛠️ 1. Preparação do Servidor

Atualize o sistema e instale as dependências necessárias para o Python e o servidor web.

```bash
sudo apt update && sudo apt upgrade -y
sudo apt install python3 python3-venv python3-pip nginx git -y
📦 2. Instalação do MkDocs (Ambiente Virtual)
Seguindo as normas do Debian 13 para evitar conflitos com o apt, utilizaremos um ambiente virtual (venv).

Bash
# Definir diretório da aplicação
sudo mkdir -p /var/www/mkdocs-site
sudo chown $USER:$USER /var/www/mkdocs-site
cd /var/www/mkdocs-site

# Criar e ativar o ambiente virtual
python3 -m venv venv
source venv/bin/activate

# Instalar MkDocs e o tema Material
pip install mkdocs mkdocs-material
🏗️ 3. Estrutura do Projeto
Inicie um novo projeto no diretório atual:

Bash
mkdocs new .
Arquivos Gerados:
mkdocs.yml: Configurações de tema, plugins e navegação.

docs/: Pasta contendo os arquivos .md da sua documentação.

⚙️ 4. Configuração do mkdocs.yml
Abaixo, um modelo base configurado com o tema Material (recomendado):

YAML
site_name: Documentação Técnica - GP-VMS
site_url: [http://docs.seu-dominio.internal](http://docs.seu-dominio.internal)
repo_url: [https://github.com/seu-usuario/repo](https://github.com/seu-usuario/repo)

theme:
  name: material
  palette:
    - scheme: default
      primary: indigo
      accent: indigo
    - scheme: slate
      primary: blue
      accent: blue
  features:
    - navigation.tabs
    - search.suggest
    - search.highlight

nav:
  - Home: index.md
  - Servidores:
    - VM-DOCS-01: servidores/docs-01.md
  - Redes: rede/topologia.md

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