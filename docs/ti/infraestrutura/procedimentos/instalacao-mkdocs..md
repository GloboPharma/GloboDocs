<div align="center">
  <img src="http://globodocs.globopharma.com.br:8000/GloboPharma/GloboDocs/assets/Logo-BR-GD.jpg" alt="Documentação Técnica — Implantação e Operação do GloboDocs Logo" width="200"/>
</div>

# Documentação Técnica — Implantação e Operação do GloboDocs

Documentar o processo de acesso, instalação, inicialização e organização estrutural do ambiente GloboDocs hospedado em servidor Debian, garantindo padronização operacional, rastreabilidade e segurança.

## 📋 Prerequisites

1. Requisitos de Infraestrutura (Host)
    Sistema Operacional: Servidor com Debian 13.
    Identificação: Hostname definido como VS-DOCS-01.
    Rede: Endereço IP fixo 10.11.0.149.

2. Requisitos de Software e Linguagem
    Linguagem de Programação: Python 3
    Gerenciador de Pacotes: python3-pip.
    Bibliotecas de Desenvolvimento: python3-dev.
    Framework de Documentação: MkDocs.
    Ambiente Isolado: Utilização de um ambiente virtual (virtualenv ou .venv) para     execução do serviço.

3. Requisitos de Acesso e Segurança
    Protocolo de Comunicação: Acesso remoto via SSH.
    Contas de Usuário: Disponibilidade de perfis "Operacional" (usuário globo) e "Administrativo" (usuário root).
    Porta de Rede: Liberação da porta 8000 para tráfego HTTP.

4. Requisitos de Integração (Versionamento)Ferramenta de Controle: 
    Git para integração com repositório remoto.
    Plataformas: Conta no GitHub (Usuário GloboPharma) e uso do software GitHub Desktop.
    Autenticação: Token de acesso pessoal (PAT) do GitHub para sincronização segura.

## 🔧 Installation

```bash
Etapa 1: Preparação do Sistema Operacional
Esta fase garante que o servidor Debian tenha os repositórios atualizados e as ferramentas base para o Python.

  Atualização de repositórios: sudo apt update.
  Instalação de pacotes essenciais: sudo apt install python3 python3-pip python3-dev -y.

Etapa 2: Criação da Estrutura do Projeto
Comandos utilizados para gerar o diretório base e a estrutura de arquivos do MkDocs.
  Criação do projeto: mkdocs new GloboDocs. 
  Acesso ao diretório do projeto: cd /GloboDocs/GloboDocs (conforme o caminho de execução padrão).

Etapa 3: Preparação do Ambiente de Execução
Procedimentos para isolar as dependências e preparar o serviço para inicialização.
  Ativação do ambiente virtual: source .venv/bin/activate.
  Comando de inicialização: mkdocs serve -a 10.11.0.149:8000.

Etapa 4: Organização Estrutural de Conteúdo
Criação manual da árvore de diretórios para os departamentos da empresa.

Criação de diretórios setoriais: ```bash
mkdir -p docs/producao docs/garantia docs/ti docs/gentegestao docs/financeiro docs/fiscal docs/comercial
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Marcelo Diniz**

- GitHub: [@GloboPharma](https://github.com/GloboPharma)

---

<div align="center">
  Made with ❤️ by Marcelo Diniz
</div>