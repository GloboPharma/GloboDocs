
!!! warning "Título do aviso"
    Esta pagina ainda está em processo de publicação.
    Após validação o procedimento será incluso.

# Procedimento para Renovação do Certificado SSL

Este manual descreve as etapas necessárias para a atualização da assinatura TLS/SSL e instalação do novo certificado no servidor via WebHost Manager (WHM).

## 1. Visão Geral
* [cite_start]**Domínio:** `*.globopharma.com.br` [cite: 3, 4]
* [cite_start]**Número do Pedido:** 121551 [cite: 4]
* [cite_start]**Vencimento Atual:** 30 de março de 2026 [cite: 4]
* [cite_start]**Data Recomendada para Atualização:** Até 10/03/2026 [cite: 3]

## 2. Geração da Solicitação de Assinatura (CSR)
Para iniciar o processo, é necessário gerar uma nova CSR no servidor:

1. [cite_start]Acesse o link de suporte da Sectigo: [Como gerar CSR](https://www.sectigo.com.br/suporte/como-gerar-csr.php)[cite: 5].
2. [cite_start]Selecione o servidor **Web Host Manager (WHM)**[cite: 5].
3. [cite_start]Siga as instruções na tela do WHM[cite: 6]:
    * [cite_start]Insira o domínio: `globopharma.com.br`[cite: 6].
    * [cite_start]Preencha as informações de contato e empresa (Globo Pharma)[cite: 6].
    * [cite_start]Defina uma senha para os segredos compartilhados[cite: 6].
4. Clique em **Criar**. [cite_start]O sistema gerará a **CSR** e a **Chave Privada**[cite: 6].

> **Importante:** Salve a Chave Privada em um local seguro. [cite_start]Ela será necessária na etapa de instalação[cite: 165].

## 3. Solicitação de Reemissão
Com a CSR em mãos:
1. [cite_start]Acesse o link de reposição: [Sectigo Reposição](https://www.sectigo.com.br/reposicao)[cite: 3].
2. [cite_start]Cole o conteúdo da CSR gerada (incluindo as tags `-----BEGIN CERTIFICATE REQUEST-----`)[cite: 7, 86].
3. [cite_start]Aguarde o e-mail de confirmação com o novo certificado[cite: 163].

## 4. Instalação do Certificado no WHM
Após receber o e-mail com o certificado, siga estes passos para instalação:

1. [cite_start]Acesse a interface **Instalar um certificado SSL em um domínio** no WHM[cite: 163].
2. [cite_start]**Campo Certificado:** Abra o novo arquivo de certificado no Bloco de Notas, copie todo o conteúdo e cole neste campo[cite: 164].
3. [cite_start]**Campo Chave Privada:** Cole a chave gerada no momento da requisição (Passo 2)[cite: 165].
4. [cite_start]**Campo Pacote de Autoridade de Certificação (CABUNDLE):** Cole o pacote de raízes enviado por e-mail[cite: 165, 167].
    * [cite_start]*Nota: Caso não tenha recebido, acione o suporte da Sectigo*[cite: 165].
5. [cite_start]Clique em **Instalar**[cite: 166].

## 5. Histórico de Solicitações
* [cite_start]**Solicitação anterior:** Gerada com sucesso para `globopharma.com.br`[cite: 6].
* [cite_start]**Nova solicitação (09/03/2026):** Atualizada para o domínio wildcard `*.globopharma.com.br`[cite: 85].