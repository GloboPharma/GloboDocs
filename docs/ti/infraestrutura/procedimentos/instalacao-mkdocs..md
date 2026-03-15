# 📚 GloboDocs — Central de Documentação

[cite_start]Este repositório contém a infraestrutura e o conteúdo da documentação técnica da **GloboPharma**, gerenciada via **MkDocs** e hospedada em ambiente Debian[cite: 1, 3, 6].

---

## 🖥️ Informações do Ambiente

| Recurso | Detalhes |
| :--- | :--- |
| **Hostname** | [cite_start]`VS-DOCS-01` [cite: 6] |
| **Endereço IP** | [cite_start]`10.11.0.149` [cite: 6] |
| **Sistema Operacional** | [cite_start]`Debian 13` [cite: 6] |
| **Interface Web** | [cite_start][http://10.11.0.149:8000](http://10.11.0.149:8000) [cite: 11] |

### [cite_start]🔐 Acesso via SSH [cite: 8]
| Perfil | Usuário | Senha |
| :--- | :--- | :--- |
| **Operacional** | [cite_start]`globo` [cite: 9] | `**********` |
| **Administrativo** | [cite_start]`root` [cite: 9] | `***********` |

---

## 🛠️ Configuração e Instalação

### 1. Preparação do Python [cite: 13]
Instalação das dependências necessárias para rodar o MkDocs no servidor[cite: 12, 15]:
```bash
sudo apt update
sudo apt install python3 python3-pip python3-dev -y
2. Inicialização do Projeto Para criar a estrutura base do projeto (Exemplo em /opt):Bashmkdocs new GloboDocs
🚀 Operação do ServiçoPara iniciar o servidor de documentação, acesse o diretório /GloboDocs/GloboDocs  e execute os comandos abaixo:Ativar Ambiente Virtual:Bashsource .venv/bin/activate
Subir o Servidor:Bashmkdocs serve -a 10.11.0.149:8000
📂 Estrutura de Conteúdo Os documentos estão organizados por departamentos para facilitar a navegação e padronização:Comando para criar as pastas setoriais:Bashmkdir -p docs/producao docs/garantia docs/ti docs/gentegestao docs/financeiro docs/fiscal docs/comercial
Navegação : Edite o arquivo mkdocs.yml na seção nav: para registrar novos arquivos.🔄 Fluxo de Atualização (GitHub) CredenciaisUsuário: GloboPharma Senha: ********🔑 Token: **************************************** Nota: Caso necessário, gere um novo token no portal do GitHub.Sincronização via Terminal Bashgit add .
git commit -m "docs: descrição da alteração"
git push origin main
Sincronização via GitHub Desktop Realize o Commit to main.No menu Repository, selecione Pull para sincronizar e atualizar a base de dados do servidor.⚠️ Nota: Esta documentação é de uso restrito para garantir a segurança operacional.