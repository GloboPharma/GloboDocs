📚 GloboDocs — Central de Documentação

Este repositório contém a infraestrutura e o conteúdo da documentação técnica da GloboPharma, gerenciada via MkDocs e hospedada em ambiente Debian.

🖥️ Informações do Ambiente

Recurso

Detalhes

Hostname

VS-DOCS-01

Endereço IP

10.11.0.149

Sistema Operacional

Debian 13

Interface Web

http://10.11.0.149:8000

🔐 Acesso via SSH

Perfil

Usuário

Senha

Operacional

globo

**********

Administrativo

root

***********

🛠️ Configuração e Instalação

1. Preparação do Python

Instalação das dependências necessárias para rodar o MkDocs no servidor:

sudo apt update
sudo apt install python3 python3-pip python3-dev -y


2. Inicialização do Projeto

Para criar a estrutura base do projeto:

mkdocs new GloboDocs


🚀 Operação do Serviço

Para iniciar o servidor de documentação, acesse o diretório /GloboDocs/GloboDocs e execute:

Ativar Ambiente Virtual:

source .venv/bin/activate


Subir o Servidor:

mkdocs serve -a 10.11.0.149:8000


📂 Estrutura de Conteúdo

Os documentos estão organizados por departamentos para facilitar a navegação:

Comando para criar as pastas setoriais:

mkdir -p docs/producao docs/garantia docs/ti docs/gentegestao docs/financeiro docs/fiscal docs/comercial


Navegação: Edite o arquivo mkdocs.yml na seção nav: para registrar novos arquivos.

🔄 Fluxo de Atualização (GitHub)

Credenciais e Segurança

Usuário: GloboPharma

Senha: ********

🔑 Token: inserir o tokem

(O token deve ser configurado localmente ou via variável de ambiente para evitar bloqueios de segurança).

Sincronização via Terminal

git add .
git commit -m "docs: correção de segurança e atualização"
git push origin main


Sincronização via GitHub Desktop

Realize o Commit to main.

No menu Repository, selecione Pull para sincronizar.

⚠️ Nota de Segurança: O GitHub bloqueia pushes com tokens expostos. Sempre mascare ou utilize variáveis de ambiente para chaves de acesso.