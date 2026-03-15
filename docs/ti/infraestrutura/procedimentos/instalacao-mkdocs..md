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

🔑 Token: ****************************************

⚠️ IMPORTANTE: Nunca insira tokens reais ou senhas diretamente nos arquivos .md. O GitHub possui um sistema de varredura (Secret Scanning) que bloqueia o envio caso detecte chaves expostas.

Sincronização via Terminal

git add .
git commit -m "docs: descrição da alteração"
git push origin main


Sincronização via GitHub Desktop

Realize o Commit to main.

No menu Repository, selecione Pull para sincronizar.

🛠️ Solução de Problemas (Troubleshooting)

Erro: "Push blocked: secret detected"

Se o GitHub bloquear seu envio com esta mensagem, significa que ele detectou um token de acesso (PAT) ou senha no histórico de commits ou no texto do arquivo.

Como resolver:

Remova o segredo: Localize o arquivo mencionado no erro (ex: instalacao-mkdocs..md) e substitua o token real por asteriscos ****.

Novo Commit: Salve o arquivo e faça um novo commit.

Revogação: Por segurança, acesse sua conta no GitHub e revogue o token detectado, gerando um novo.

Bypass (Não recomendado): Caso tenha certeza de que é um falso positivo ou uma informação pública, você pode clicar no link de "Bypass" fornecido na interface do GitHub Desktop para forçar o envio, mas o ideal é sempre remover o dado sensível.