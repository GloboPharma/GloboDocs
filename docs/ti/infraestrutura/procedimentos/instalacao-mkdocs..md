# Documentação Técnica: Implantação e Operação do GloboDocs

[cite_start]Esta documentação descreve o processo de acesso, instalação, inicialização e organização estrutural do ambiente **GloboDocs**, garantindo a padronização operacional, rastreabilidade e segurança[cite: 1, 3].

---

## 1. Informações do Ambiente

### 1.1 Host
[cite_start]O sistema está hospedado em um servidor com as seguintes especificações[cite: 5, 6]:

| Parâmetro | Valor |
| :--- | :--- |
| **Hostname** | [cite_start]VS-DOCS-01 [cite: 6] |
| **Endereço IP** | [cite_start]10.11.0.149 [cite: 6] |
| **Sistema Operacional** | [cite_start]Debian 13 [cite: 6] |

### 1.2 Acesso ao Sistema (SSH)
[cite_start]O acesso remoto deve ser realizado via protocolo SSH utilizando as credenciais abaixo[cite: 8, 9]:

| Perfil | Usuário | Senha |
| :--- | :--- | :--- |
| **Operacional** | `globo` | [cite_start]`Pharma2026` [cite: 9] |
| **Administrativo** | `root` | [cite_start]`Caravela424` [cite: 9] |

### 1.3 Acesso Web
[cite_start]O serviço de documentação está disponível na rede interna[cite: 10, 11]:

* [cite_start]**Serviço:** MkDocs [cite: 11]
* [cite_start]**Porta:** 8000 [cite: 11]
* [cite_start]**URL:** [http://10.11.0.149:8000](http://10.11.0.149:8000) [cite: 11]

---

## 2. Instalação e Configuração

### 2.1 Dependências de Sistema
[cite_start]Para preparar o ambiente Debian, instale os pacotes Python necessários[cite: 12, 13]:

```bash
sudo apt update [cite: 14]
sudo apt install python3 python3-pip python3-dev -y [cite: 15]
2.2 Criação do Projeto MkDocs
Comando para gerar a estrutura base do projeto:

Bash
# Exemplo executado no diretório /opt [cite: 19]
mkdocs new GloboDocs [cite: 17]
3. Operação do Serviço
3.1 Inicialização
O serviço deve ser executado a partir do diretório /GloboDocs/GloboDocs.


Ativar o ambiente virtual: 

Bash
source .venv/bin/activate [cite: 25]

Inicializar o serviço: 

Bash
mkdocs serve -a 10.11.0.149:8000 [cite: 26, 28]
4. Estrutura de Conteúdo
4.1 Organização de Diretórios
Os documentos devem ser organizados por departamentos:

Bash
mkdir -p docs/producao docs/garantia docs/ti docs/gentegestao docs/financeiro docs/fiscal docs/comercial [cite: 44]
4.2 Configuração de Navegação
As novas seções devem ser declaradas no arquivo mkdocs.yml sob o campo nav:.

5. Integração com GitHub
5.1 Credenciais e Sincronização

Usuário: GloboPharma 
+1


Senha: Pha@2026 


Token de Acesso: inserrir o token de acesso 

5.2 Fluxo de Atualização (Git CLI)
Para atualizar o repositório via linha de comando:


Adicionar alterações: git add . 


Criar commit: git commit -m "docs: descrição" 


Enviar para o servidor: git push origin main 

5.3 Fluxo via GitHub Desktop
Abrir o GitHub Desktop.

Clicar em Commit to main.

No menu superior, clicar em Repository e selecionar Pull para sincronizar e atualizar a base no servidor.
+1

⚠️ Aviso: Mantenha o Token de acesso em segurança. Caso necessário, gere um novo no portal do GitHub do GloboPharma.


**Gostaria que eu formatasse esse arquivo para ser usado especificamente como o `README.md` do seu repositório no GitHub?**