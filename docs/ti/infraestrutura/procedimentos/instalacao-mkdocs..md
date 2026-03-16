# Documentação de Instalação – Servidor Debian 13 com MkDocs e GitHub Desktop

## 1. Objetivo

Este documento descreve o processo de instalação e configuração de um servidor **Debian 13** para hospedagem de documentação utilizando **MkDocs** e sincronização com repositório **GitHub** através do **GitHub Desktop**.

O objetivo é permitir a edição local da documentação e sincronização com o repositório remoto.

Esta documentação estabelece as diretrizes para instalação, operação e manutenção do ambiente GloboDocs, visando a padronização, segurança e rastreabilidade dos processos.
---

## 2. Pré-requisitos

Antes de iniciar, garantir que o servidor possua:

- Sistema Operacional: Debian 13 
- Usuário com privilégios **sudo**
- Acesso à internet
- Python: Python 3 
- Pip: Gerenciador de pacotes pip para Python.
- Git instalado
- Permissões: Acesso root ou sudo pode ser necessário caso não utilize um ambiente virtual. 

---

## 3. Atualizar o Sistema

Atualizar os pacotes do sistema.

```bash
sudo apt update
sudo apt upgrade -y
```

---

## 4. Instalar dependências

Instalar Python, pip e git.

```bash
sudo apt install -y python3 python3-pip git
```

Verificar instalação:

```bash
python3 --version
pip3 --version
git --version
```

---

## 5. Instalar MkDocs

Instalar o MkDocs utilizando pip.

```bash
pip install mkdocs
```

Verificar instalação:

```bash
mkdocs --version
```

Opcionalmente instalar o tema Material.

```bash
pip install mkdocs-material
```

---

## 6. Criar projeto MkDocs

Criar um novo projeto de documentação.

```bash
mkdocs new GloboDocs
```

Estrutura criada:

```
GloboDocs/
├── docs/
│   └── index.md
└── mkdocs.yml
```

Entrar no diretório:

```bash
cd GloboDocs/GloboDocs
```

---

## 7. Testar servidor local

Executar o servidor de testes:

```bash
mkdocs serve -a 10.11.0.149:8000
```

Acessar no navegador:

```
http://10.11.0.149:8000
```

---

## 8. Criar repositório no GitHub

1. Acessar https://github.com
2. Criar um novo repositório
3. Definir nome do projeto ('GloboDocs`)
4. Não inicializar com README

---

## 9. Inicializar Git no projeto

No diretório do projeto:

```bash
git init
git add .
git commit -m "Primeira versão da documentação"
```

Adicionar repositório remoto:

```bash
git remote add origin https://github.com/GloboPharma/GloboDocs.git
```

Enviar arquivos:

```bash
git branch -M main
git push -u origin main
```

---

## 10. Sincronização utilizando GitHub Desktop

Instalar o **GitHub Desktop** na estação de trabalho.

Passos:

1. Abrir o GitHub Desktop
2. Fazer login com a conta do GitHub "(Github -> USER: GloboPharma  e SENHA: Pha@2026)"
3. Selecionar **Clone Repository**
4. Escolher o repositório criado
5. Editar arquivos `.md` localmente
6. Realizar commit
7. Clicar em **Push origin**

Fluxo de trabalho:

```
Editar documentação
      ↓
Commit no GitHub Desktop
      ↓
Push para GitHub
      ↓
Servidor sincronizado
```

---

## 11. Gerar versão estática da documentação

Para gerar o site estático:

```bash
mkdocs build
```

Arquivos gerados:

```
site: http://globodocs.globopharma.com.br:8000
```

---

## 12. Publicação (Opcional)

Publicar diretamente no GitHub Pages:

```bash
mkdocs gh-deploy
```

Isso cria automaticamente a branch `gh-pages`.

---

## 13. Estrutura recomendada da documentação

```
docs/
├── index.md
├── Governanca
├── Administrativo
├── Fabrica
├── Projetos
├── Templates
└── Base de Conhecimento
```

---


## 14. Credenciais de Acesso (SSH)

O acesso ao servidor é restrito via SSH através das seguintes contas:


| Perfil | Usuário | Senha |
| :--- | :--- | :--- |
| Operacional | globo | Pharma2026 |
| Administrativo | root | Caravela424 |

## 15. Inicialização e Execução do Serviço MkDocs 

1. Inicialização do Serviço MkDocs

 Acessar o diretório /GloboDocs/GloboDocs
__________________________________________________________

2 Execução dos comandos a seguir:

 2.1 Ativar o virtualenv
     Executar o comando: source .venv/bin/activate
     Incializar o serviço: mkdocs serve -a 10.11.0.149:8000
     Exemplo:
     root@VS-DOCS-01:~/GloboDocs/GloboDocs# mkdocs serve -a 10.11.0.149:8000
____________________________________________________________________________

3. Envia as alterações para o GitHub
   
   git push origin main
Sincronização:
   Login: GloboPharma

⚠️ Token: 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

Ou gerar um novo token no portal do Github do GloboPharma/GloboDocs
________________________________________________________________________

## 16. Boas práticas

- Usar **Markdown padrão**
- Criar uma página por procedimento
- Usar imagens para diagramas
- Versionar sempre no GitHub

---