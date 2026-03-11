# Boas Práticas de Documentação (Docs-as-Code)

Seguir estas diretrizes garante que a documentação do GloboDocs permaneça atualizada, fácil de navegar e com aparência profissional.

## 1. Melhores Práticas de Escrita (Markdown)

**Links Relativos:**  
Utilize links internos relativos para garantir que funcionem tanto localmente quanto no site publicado.

Exemplo:  
`[texto](arquivo.md)` ou `[texto](../pasta/arquivo.md)`

**Imagens e Recursos:**  
Armazene imagens e arquivos estáticos na subpasta `docs/assets/` e referencie-os com caminhos relativos.

**Sintaxe Limpa:**  
Evite misturar abas e espaços; utilize sempre espaços para indentação (padrão de 2 ou 4).

!!! tip "Dica: Uso de Admonitions"
    Utilize blocos de advertência ou notas para destacar informações importantes como avisos, dicas ou notas específicas.

---

## 2. Fluxo de Trabalho e Revisão

**Revisão por Pares (PRs):**  
Toda alteração deve passar por um Pull Request e ser revisada por outro membro da equipe, tratando o documento como código.

**Pré-visualização Local:**  
Sempre utilize o comando mkdocs serve para visualizar as alterações em tempo real antes de enviar ao repositório.

**Documentação Automática:**  
Para projetos em Python, utilize o plugin mkdocstrings para gerar documentação a partir do código automaticamente.

---

##3. Automação e Deploy (CI/CD

**Pipeline de CI/CD:**  
Configure GitHub Actions ou GitLab CI para construir e implantar a documentação automaticamente ao realizar o push na branch principal (main ou master).

**Publicação**  
Utilize o comando mkdocs gh-deploy para publicar o site diretamente no GitHub Pages.

**Validação:**  
Configure a automação para verificar links quebrados durante o processo de build.

---

##4. Regras Gerais e Estrutura

**Pastas Ocultas:**  
Não inicie nomes de pastas ou arquivos com ponto (ex: .manual.md), pois o MkDocs os ignora.

**Organização de Diretórios:**  
Nunca coloque o diretório de saída (site_dir) dentro da pasta de documentos (docs_dir) para evitar erros de recursão.


**Estrutura de Conteúdo:**
 Busque seguir a divisão em quatro partes:
 
1.  **Tutoriais:**  Aprendizado prático orientado a lições.
2.  **Guias de "Como Fazer":**  Passos para resolver problemas específicos.
3.  **Referência Técnica:**  Descrição teórica e técnica.
4.  **Explicação:**  Discussão de conceitos e arquitetura.


---

**Última atualização: 2026**
