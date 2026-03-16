# Documentação de Instalação – Servidor Debian com MkDocs e GitHub Desktop

## 1. Objetivo

Este documento descreve o processo de instalação e configuração de um servidor **Debian 13** para hospedagem de documentação utilizando **MkDocs** e sincronização com repositório **GitHub** através do **GitHub Desktop**.

O objetivo é permitir a edição local da documentação e sincronização com o repositório remoto.

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

## 15. Inicialização do Serviço MkDocs

Para operar o sistema, acesse o diretório base da aplicação:
`cd /GloboDocs/GloboDocs`

---

### 15.1. Execução do Serviço

Siga os passos abaixo para ativar o ambiente e colocar o site no ar:

### 15.2 Ativar o virtualenv
```bash
Comando: source .venv/bin/activate
```
### 15.3  Inicializar o serviço
```bash
Comando: mkdocs serve -a 10.11.0.149:8000.
```
- Exemplo no terminal:
```bash
  root@VS-DOCS-01:~/GloboDocs/GloboDocs# mkdocs serve -a 10.11.0.149:8000
```

### 15.4 Sincronização com GitHub

Após realizar as alterações locais, envie os arquivos para o repositório remoto:
```bash
Comando: git push origin main
```
Dados de Autenticação:

- Login: GloboPharma
- Token: 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

⚠️ Nota: Caso o token expire, você deve gerar um novo no portal do GitHub da conta GloboPharma/GloboDocs.

---

## 16. Boas práticas

- Usar **Markdown padrão**
- Criar uma página por procedimento
- Usar imagens para diagramas
- Versionar sempre no GitHub

---

## 17. Referências Utilizadas

Este projeto de implantação baseia-se nas seguintes fontes de referência:

- Documentação Oficial MkDocs: Guia de implantação e deploy (https://www.mkdocs.org/user-guide/deploying-your-docs/).
- Blog Remontti: Guia prático de instalação em ambiente Linux (https://blog.remontti.com.br/6110).
- Guia Interno GloboDocs: Documentação técnica de implantação e operação v.2026.

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Marcelo Diniz**

- GitHub: [@GloboPharma](https://github.com/GloboPharma)
- Email: marcelo.diniz@globopharma.com.br

---

<div align="center">
  Made with  by Marcelo Diniz
</div>