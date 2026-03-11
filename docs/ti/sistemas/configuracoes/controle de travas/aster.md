# Procedimento de Cadastro de Representantes

[cite_start]Este documento detalha o fluxo de processos para o cadastro de representantes (pessoa física ou jurídica) nas plataformas empresariais da Globo Pharma[cite: 3, 4].

---

## 1. Início do Processo
[cite_start]O processo é iniciado com a abertura de um **Informe de Contratação**, conforme o tipo de vínculo[cite: 6]:

* [cite_start]**Recursos Humanos (RH):** Para representantes com vínculo empregatício, seguindo o procedimento `IT-INF-000043-GERENCIAMENTO DE USUÁRIOS`[cite: 7].
* [cite_start]**Área Comercial:** Para representantes Pessoa Jurídica (PJ) que não possuem vínculo direto com o RH[cite: 8].

---

## 2. Configuração nos Sistemas

[cite_start]O cadastro envolve a configuração sequencial em quatro sistemas principais[cite: 10]:

### 2.1. Active Directory (AD)
* [cite_start]**Aplicabilidade:** Apenas para representantes que utilizarão recursos internos, como computador ou o portal de chamados GLPI[cite: 12].
* [cite_start]**Ação:** Criar o usuário para acesso à rede e serviços internos conforme a "MATRIZ DE ACESSOS"[cite: 13, 14].

### 2.2. SAP Business One (SAP B1)
[cite_start]O cadastro no SAP B1 é fundamental para a gestão operacional e de vendas[cite: 17]. Os campos devem seguir o padrão da empresa:

* [cite_start]**Código do Usuário:** Nome e último nome[cite: 18].
* [cite_start]**Nome do Usuário:** Nome completo, em letras maiúsculas e sem acentuação[cite: 19].
* [cite_start]**E-mail:** Pode ser o e-mail interno (@globopharma.com.br) ou pessoal[cite: 20].
* [cite_start]**Departamento:** Selecionar obrigatoriamente "REPRESENTANTES"[cite: 21].
* [cite_start]**Comprador:** Adicionar o código do comprador previamente cadastrado no menu "Vendedores/Compradores" (responsabilidade da Área Comercial)[cite: 22].

### 2.3. Portal ASTER
[cite_start]O portal utiliza o e-mail registrado no SAP B1 como identificador[cite: 68].

1.  [cite_start]Acesse o sistema ASTER e entre na aba **Usuários**[cite: 69, 70].
2.  [cite_start]Clique em **Adicionar novo usuário**[cite: 86].
3.  [cite_start]Preencha o campo **E-mail**[cite: 90].
4.  [cite_start]No campo **Nome**, preencha exatamente como cadastrado no SAP B1[cite: 94].
5.  [cite_start]Defina uma **Senha inicial**[cite: 96].
6.  [cite_start]**Permissões:** Utilize as configurações do perfil "PERFIL REPRESENTANTES" como base para cópia[cite: 100].
7.  [cite_start]**Sincronização:** No perfil do representante no ASTER, altere o campo `salespersonCode` para o mesmo valor do campo **Comprador** registrado no SAP B1[cite: 116].

---

## 3. Cadastro no BI "Globo Vendedores" (Power BI)
[cite_start]Esta etapa finaliza o acesso do representante aos relatórios de vendas personalizados[cite: 168].

1.  [cite_start]Acesse o endereço do [Power BI](https://app.powerbi.com) e faça login[cite: 169, 175].
2.  [cite_start]Acesse o menu **Workspaces** > **Meu workspace**[cite: 176, 198].
3.  [cite_start]Abra o relatório **PBI Globo Pharma Vendedores**[cite: 222].
4.  [cite_start]Clique no botão **Editar**[cite: 248].
5.  [cite_start]Aplique o filtro de **Vendedores**, adicionando o nome do representante a ser cadastrado[cite: 264].
6.  [cite_start]Vá em **Arquivo > Salvar como** e salve na pasta "Vendedores" com o nome do representante como título[cite: 288, 311].
7.  [cite_start]Vá em **Arquivo > Inserir relatório > Publicar na web** e copie o link gerado[cite: 312, 339].

### 3.1. Vinculação Final no SAP
1.  [cite_start]Retorne ao SAP B1 no menu **Vendedores/Compradores**[cite: 356].
2.  [cite_start]Localize o representante e, na coluna **Link Power BI**, cole o link copiado[cite: 359].
3.  [cite_start]**Nota:** Remova a parte inicial do link (mantenha apenas a partir do prefixo `eyJrljoi...`)[cite: 359].

---

## 4. Modelos de Aprovação
[cite_start]Após a inclusão do código BI, é necessário configurar as autorizações[cite: 362]:

1.  [cite_start]Acesse a tela de **Modelos de aprovação**[cite: 362].
2.  [cite_start]Adicione o representante em todos os modelos que possuem o prefixo **"PV"** (Ex: `PV DESVIO DE LIMITE`, `PV BONIFICAÇÃO`, etc.)[cite: 362, 406, 417].