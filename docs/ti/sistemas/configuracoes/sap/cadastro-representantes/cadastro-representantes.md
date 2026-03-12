# Procedimento de Cadastro de Representantes (Portal ASTER e SAP B1)

Este documento detalha o fluxo de processos para o cadastro de representantes no portal **ASTER** e no sistema **SAP B1**, conforme realizado pela **Globo Pharma**. O objetivo é garantir um procedimento padronizado e eficiente para a integração de novos representantes (pessoa física ou jurídica) nas plataformas empresariais.

---
## 1. Início do Processo
O processo é iniciado com a abertura de um **Informe de Contratação**, que pode ser:

1. **Aberto pelo Recursos Humanos (RH):** Para representantes com vínculo empregatício. (Seguindo o procedimento `IT-INF-000043-GERENCIAMENTO DE USUÁRIOS`).
2. **Aberto pela Área Comercial:** Para representantes Pessoa Jurídica (PJ) que não possuem vínculo direto com o RH.

---

## 2. Fluxo de Cadastro Passo a Passo
O cadastro do representante envolve a configuração em três sistemas principais: **Active Directory (AD)**, **SAP B1** e **Portal ASTER**, seguido pela configuração no **Power BI**.

### 2.1. Criação de Usuário no Active Directory (AD)

* **Aplicabilidade:** Apenas para representantes que utilizarão recursos internos da Globo Pharma, como computador ou o portal de chamados GLPI.
* **Ação:** Criar o usuário no AD para acesso à rede e serviços internos (Cadastro realizado conforme a **“MATRIZ DE ACESSOS”**).


![hhh](GloboDocs/docs/imagens/usuário-ad.png)


### 2.2. Cadastro no SAP B1
[cite_start]Configurações obrigatórias para gestão operacional[cite: 17]:
* [cite_start]**Código do Usuário**: Nome e último nome (padrão Globo Pharma)[cite: 18].
* [cite_start]**Nome do Usuário**: Nome completo, em maiúsculas e sem acentuação[cite: 19].
* [cite_start]**E-mail**: Pode ser @globopharma.com.br ou pessoal[cite: 20].
* [cite_start]**Departamento**: Selecionar obrigatoriamente "REPRESENTANTES"[cite: 21, 48].
* [cite_start]**Comprador**: Adicionar o código numérico previamente cadastrado pela Área Comercial (ex: código 87 ou 26)[cite: 22, 59, 158].

### 2.3. Cadastro no Portal ASTER
[cite_start]O sistema utiliza o e-mail do SAP B1 como identificador[cite: 68].
1.  [cite_start]Acessar a aba **Usuários** no ASTER[cite: 70].
2.  [cite_start]Adicionar novo usuário e preencher o e-mail[cite: 86, 90].
3.  [cite_start]O campo **Nome** deve ser idêntico ao cadastrado no SAP B1[cite: 94].
4.  [cite_start]Definir senha inicial[cite: 96].
5.  [cite_start]**Permissões**: Copiar as configurações do perfil "PERFIL REPRESENTANTES"[cite: 100].
6.  [cite_start]**Sincronização**: No perfil do usuário, alterar o campo `salespersonCode` para o mesmo valor do campo **Comprador** do SAP B1[cite: 116, 124].

---

## 3. Cadastro no Power BI (Relatórios de Vendas)
[cite_start]Finaliza o acesso aos relatórios personalizados[cite: 168].
1.  [cite_start]Acessar o menu **Workspaces** > **Meu workspace**[cite: 176, 198].
2.  [cite_start]Abrir o relatório **PBI Globo Pharma Vendedores**[cite: 222].
3.  [cite_start]Clicar em **Editar** e aplicar o filtro com o nome do representante[cite: 248, 264].
4.  [cite_start]**Salvar como**: Na pasta "Vendedores", use o nome do representante como título do arquivo[cite: 288, 311].
5.  [cite_start]**Publicar**: Vá em Arquivo > Inserir relatório > **Publicar na web**[cite: 312].
6.  [cite_start]**Link**: Copie o link gerado[cite: 339].

---

## 4. Integração Final e Aprovações

### Vinculação do Link no SAP B1
1.  [cite_start]Acesse o menu **Vendedores/Compradores** no SAP B1[cite: 356].
2.  [cite_start]Localize o representante e cole o link do Power BI na respectiva coluna[cite: 359].
3.  [cite_start]**Atenção**: Remova a parte inicial da URL, mantendo o conteúdo a partir do prefixo `eyJrljoi...`[cite: 359].

### Modelos de Aprovação
* [cite_start]Acessar a tela de modelos de aprovação e incluir o novo representante em todos os modelos que possuem o prefixo **"PV"** (Pedido de Venda)[cite: 362, 371].
* [cite_start]Exemplos de modelos: `PV 150aimi`, `PV ACIMA 1m`, `PV DESVIO DE LIMITE`, entre outros[cite: 395, 399, 406].

---