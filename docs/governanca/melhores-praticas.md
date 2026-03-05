#Boas Práticas de Documentação (Docs-as-Code)
 Seguir estas diretrizes garante que a documentação do GloboDocs permaneça atualizada, fácil de navegar e com aparência profissional.

##1. Melhores Práticas de Escrita (Markdown)

Links Relativos: Utilize links internos relativos para garantir que funcionem tanto localmente quanto no site publicado.

Exemplo: [texto](arquivo.md) ou [texto](../pasta/arquivo.md).


Imagens e Recursos: Armazene imagens e arquivos estáticos na subpasta docs/assets/ e referencie-os com caminhos relativos.


Sintaxe Limpa: Evite misturar abas e espaços; utilize sempre espaços para indentação (padrão de 2 ou 4).

!!! tip "Dica: Uso de Admonitions"
Utilize blocos de advertência ou notas para destacar informações importantes como avisos, dicas ou notas específicas.

##2. Fluxo de Trabalho e Revisão

Revisão por Pares (PRs): Toda alteração deve passar por um Pull Request e ser revisada por outro membro da equipe, tratando o documento como código.


Pré-visualização Local: Sempre utilize o comando mkdocs serve para visualizar as alterações em tempo real antes de enviar ao repositório.


Documentação Automática: Para projetos em Python, utilize o plugin mkdocstrings para gerar documentação a partir do código automaticamente.

##3. Automação e Deploy (CI/CD)

Pipeline de CI/CD: Configure GitHub Actions ou GitLab CI para construir e implantar a documentação automaticamente ao realizar o push na branch principal (main ou master).


Publicação: Utilize o comando mkdocs gh-deploy para publicar o site diretamente no GitHub Pages.


Validação: Configure a automação para verificar links quebrados durante o processo de build.

##4. Regras Gerais e Estrutura

Pastas Ocultas: Não inicie nomes de pastas ou arquivos com ponto (ex: .manual.md), pois o MkDocs os ignora.


Organização de Diretórios: Nunca coloque o diretório de saída (site_dir) dentro da pasta de documentos (docs_dir) para evitar erros de recursão.

Estrutura de Conteúdo: Busque seguir a divisão em quatro partes:

Tutoriais: Aprendizado prático orientado a lições.

Guias de "Como Fazer": Passos para resolver problemas específicos.

Referência Técnica: Descrição teórica e técnica.


Explicação: Discussão de conceitos e arquitetura.








# Matriz RACI: Atribuição e Responsabilidades

## Atribuição de Responsabilidades

A **Matriz RACI** é uma ferramenta estratégica utilizada pela **Globo Pharma** para organizar e priorizar as ações de seus colaboradores. Ela serve para alinhar as funções em um projeto, processo ou serviço, garantindo que cada 
membro esteja ciente das atribuições que lhe foram designadas.

## 🧩 O que é a Matriz RACI?

A sigla RACI é um acrônimo dos termos em inglês que definem os papéis de cada atividade:

| Sigla | Papel | Descrição | Comunicação |
| :---: | :--- | :--- | :--- |
| **R** | **Responsável** | Quem executa efetivamente a atividade ou elemento do projeto. | **Execução** |
| **A** | **Autoridade** | Quem aprova formalmente a entrega e tem autoridade final. | **Aprovação** |
| **C** | **Consultado** | Quem deve ser consultado em caso de dúvidas ou mudanças (via de mão dupla). | **Consulta** |
| **I** | **Informado** | Quem deve ser notificado sobre resultados, sem necessidade de resposta. | **Informação** |

---

## 📈 Benefícios do Modelo

A implementação desta matriz no **GloboDocs** traz ganhos operacionais diretos:

* **Aumento no Engajamento:** Reduz dúvidas e confusões, diminuindo o estresse e aumentando o envolvimento da equipe.
* **Treinamento Eficiente:** Foca nas competências que agregam valor real à função executada, evitando perda de tempo.
* **Economia de Tempo:** Apenas os colaboradores envolvidos no processo específico são convocados para reuniões.
* **Redução de Frustração:** Elimina o problema de não saber quem procurar para obter soluções em níveis hierárquicos superiores.

---

## 🛠️ Guia de Implementação

Para aplicar o modelo na prática, podem ser utilizadas planilhas, editores de texto ou softwares de gestão.

### 1. Identificação Estratégica
* Identifique os projetos vinculados aos objetivos estratégicos da organização.
* Liste as etapas e tarefas principais verticalmente.
* Defina quem executa (R), quem aprova (A) e quem será consultado (C) ou informado (I).

!!! warning "Regra de Ouro da Governança"
    Para toda atividade, deve existir pelo menos um **R** e exatamente um **A**. **Nunca** designe mais de um aprovador para a mesma atividade.

### 2. Alinhamento e Reuniões
* Realize reuniões regulares com todos os identificados na matriz para que fiquem cientes de suas responsabilidades.
* **Nota:** Pessoas marcadas como **I** (Informados) nem sempre precisam participar de todas as reuniões.
* O modelo deve ser priorizado em processos críticos e de alto valor estratégico para a empresa.

---

## 📝 Exemplo Prático: Sistemas (SAP / BEAS)

Abaixo, um modelo de preenchimento para as tecnologias do portal:

| Atividade / Processo | Gestor de TI | Analista de Sistemas | Diretor Operacional | Usuário Chave |
| :--- | :---: | :---: | :---: | :---: |
| **Configuração de Módulo SAP** | **A** | **R** | **I** | **C** |
| **Manutenção Corretiva BEAS** | **A** | **R** | **I** | **I** |
| **Aprovação de Mudança (RFC)** | **R** | **C** | **A** | **C** |

---
## Atribuição de Responsabilidades

## 📚 Controle de Versão

| Versão | Data | Autor | Descrição | Aprovação |
|--------|------|------|-----------|-----------|
| 1.0 | 2026-02-12 | TI Corporativo | Criação inicial | Diretoria Operacional |

---

## 🕘 Histórico de Alterações

| Data | Versão | Alteração | Responsável |
|------|--------|----------|-------------|
| 2026-02-12 | 1.0 | Publicação inicial | Gestão de TI |

---

## 🔐 Classificação Documental

Nível: **Interno**

### Diretrizes
- Uso restrito a colaboradores autorizados
- Proibida distribuição externa
- Armazenar apenas em repositórios corporativos

---

## 🔗 Integração com ITSM

Esta matriz suporta:

- Gestão de Mudanças (RFC)
- Definição de aprovadores CAB
- Identificação de stakeholders
- Comunicação estruturada

Alterações devem seguir fluxo formal de Change Management.

---

## 📖 Referências Normativas

- ITIL 4  
- COBIT 2019  
- ISO/IEC 20000  

Base conceitual — não implica certificação formal.

---
## Atribuição de Responsabilidades

Documento: GOV-RACI-001  
Owner: Gestão de TI  
Aprovador: Diretoria Operacional  
Classificação: Interno  
Versão: 1.0  
Data de Vigência: 2026-02-12  
Próxima Revisão: 2027-02  

Última atualização: 2026
