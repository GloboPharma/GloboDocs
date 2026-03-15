Documentação de Instalação – Servidor Debian 13 com MkDocs e GitHub Desktop
1. Objetivo

Este documento descreve o processo de instalação e configuração de um servidor Debian 13 para hospedagem de documentação utilizando MkDocs e sincronização com repositório GitHub através do GitHub Desktop.

O objetivo é permitir a edição local da documentação e sincronização automática com o repositório remoto.

2. Pré-requisitos

Antes de iniciar, garantir que o servidor possua:

Debian 13 instalado

Usuário com privilégios sudo

Acesso à internet

Python 3 instalado

Git instalado

3. Atualizar o Sistema

Atualizar os pacotes do sistema.

sudo apt update
sudo apt upgrade -y
4. Instalar dependências

Instalar Python, pip e git.

sudo apt install -y python3 python3-pip git

Verificar instalação:

python3 --version
pip3 --version
git --version
5. Instalar MkDocs

Instalar o MkDocs utilizando pip.

pip install mkdocs

Verificar instalação:

mkdocs --version

Opcionalmente instalar o tema Material:

pip install mkdocs-material

Tema utilizado pelo Material for MkDocs.

6. Criar projeto MkDocs

Criar um novo projeto de documentação.

mkdocs new documentacao

Estrutura criada:

documentacao/
├── docs/
│   └── index.md
└── mkdocs.yml

Entrar no diretório:

cd documentacao
7. Testar servidor local

Executar o servidor de testes:

mkdocs serve -a 0.0.0.0:8000

Acessar no navegador:

http://IP_DO_SERVIDOR:8000
8. Criar repositório no GitHub

Acessar o GitHub

Criar um novo repositório

Definir nome do projeto (ex: documentacao)

Não inicializar com README

9. Inicializar Git no projeto

No diretório do projeto:

git init
git add .
git commit -m "Primeira versão da documentação"

Adicionar repositório remoto:

git remote add origin https://github.com/USUARIO/documentacao.git

Enviar arquivos:

git branch -M main
git push -u origin main
10. Sincronização utilizando GitHub Desktop

Instalar o GitHub Desktop na estação de trabalho.

Passos:

Abrir o GitHub Desktop

Fazer login com a conta do GitHub

Selecionar Clone Repository

Escolher o repositório criado

Editar arquivos .md localmente

Realizar commit

Clicar em Push origin

Fluxo de trabalho:

Editar documentação
      ↓
Commit no GitHub Desktop
      ↓
Push para GitHub
      ↓
Servidor sincronizado
11. Gerar versão estática da documentação

Para gerar o site estático:

mkdocs build

Arquivos gerados:

site/
12. Publicação (Opcional)

Publicar diretamente no GitHub Pages:

mkdocs gh-deploy

Isso cria automaticamente a branch gh-pages.

13. Estrutura recomendada da documentação
docs/
├── index.md
├── instalacao.md
├── servidores.md
├── procedimentos.md
└── troubleshooting.md
14. Boas práticas

Usar Markdown padrão

Criar uma página por procedimento

Usar imagens para diagramas

Versionar sempre no GitHub

Se quiser, posso também te ajudar a montar:

Estrutura profissional de documentação (padrão DevOps / SRE)

Automação de deploy com GitHub Actions

Servidor Debian servindo MkDocs via Nginx

Sincronização automática do repositório no servidor

Posso inclusive te gerar um repositório modelo completo de documentação com MkDocs pronto para usar.