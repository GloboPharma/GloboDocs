
!!! warning "Título do aviso"
    Esta pagina ainda está em processo de publicação.
    Após validação o procedimento será incluso.

# Procedimento: Renovação de Certificado SSL (WHM)

Este manual descreve o procedimento operacional padrão para a renovação de certificados SSL/TLS para os domínios da Globo Pharma, utilizando a plataforma Sectigo e o painel WebHost Manager (WHM).
---

## 1. Dados do Certificado (Referência 2026)
[cite_start]O certificado SSL protege o domínio e deve ser atualizado periodicamente para evitar interrupções nos serviços[cite: 3].

* **Domínio:** `*.globopharma.com.br`[cite: 3, 4].
* **Número do Pedido:** 121551[cite: 4].
* **Vencimento Original:** 30 de março de 2026[cite: 4].
* **Data Limite Recomendada:** 10 de março de 2026[cite: 3].

---

## 2. Geração da Solicitação de Assinatura (CSR)
A geração da CSR é o primeiro passo para informar à autoridade certificadora os dados do servidor.

1.  Acesse o portal de suporte da Sectigo para geração de CSR:(https://www.sectigo.com.br/suporte/como-gerar-csr.php).
2.  No WHM, acesse a interface Gerar uma Solicitação de Assinatura e Certificado SSL..
3.  Preencha as informações conforme os padrões da empresa:

-----------------FINALIZAR APARTIR DESTA PARTE ----------------------
    * [cite_start]**E-mail:** marcelo.diniz@globopharma.com.br[cite: 6].
4.  [cite_start]Configure as **Informações do Certificado**[cite: 6]:
    * [cite_start]**Domínios:** `globopharma.com.br`[cite: 6].
    * [cite_start]**Cidade:** Sao Jose da Lapa[cite: 6].
    * [cite_start]**Estado:** Minas Gerais[cite: 6].
    * [cite_start]**País:** BR (Brasil)[cite: 6].
    * [cite_start]**Empresa:** Globo Pharma[cite: 6].
5.  [cite_start]Clique em **Criar** para gerar os códigos[cite: 6].

> [cite_start]**Atenção:** Ao finalizar, o sistema exibirá a **CSR**, a **Chave Privada** e o **Certificado Autoassinado**. [cite_start]Salve a Chave Privada em local seguro, pois ela é necessária para a instalação final[cite: 165].

---

## 3. Reposição e Reemissão
[cite_start]Após gerar a nova CSR, o certificado deve ser reemitido pela autoridade certificadora[cite: 3].

1.  [cite_start]Acesse o link: [https://www.sectigo.com.br/reposicao](https://www.sectigo.com.br/reposicao)[cite: 3].
2.  [cite_start]Cole a CSR gerada (incluindo as tags `-----BEGIN CERTIFICATE REQUEST-----`)[cite: 86].
3.  [cite_start]A Sectigo enviará um código de verificação para os e-mails administrativos do domínio (ex: `admin@dominio.com.br`, `postmaster@dominio.com.br`).
4.  [cite_start]Após a validação, o novo certificado será enviado para o e-mail cadastrado.

---

## 4. Instalação do Novo Certificado
[cite_start]Com os arquivos em mãos, acesse a interface **Instalar um certificado SSL em um domínio** no WHM[cite: 163].

### Passo a Passo da Instalação:
1.  [cite_start]**Domínio:** Selecione o domínio correspondente[cite: 163].
2.  [cite_start]**Certificado (CRT):** Abra o novo certificado recebido por e-mail no Bloco de Notas, copie e cole todo o conteúdo no campo[cite: 164].
3.  [cite_start]**Chave Privada (KEY):** Cole a chave privada que foi gerada no momento da criação da CSR (Passo 2)[cite: 165].
4.  [cite_start]**Pacote de Autoridade de Certificação (CABUNDLE):** Cole o "Pacote de Raízes" encaminhado por e-mail pela Sectigo[cite: 165, 167].
5.  [cite_start]Clique em **Instalar**[cite: 166].

---

## 5. Referências Técnicas (Exemplos)

### Exemplo de CSR (Solicitação)
```text
-----BEGIN CERTIFICATE REQUEST-----
MIIDRTCCAi0CAQAwgbIxHTAbBgNVBAMMFCouZ2xvYm9waGFybWEuY29tLmJyMSQw
IgYJKoZIhvcNAQkBFhV0aUBnbG9ib3BoYXJtYS5jb20uYnIxFTATBgNVBAgMDE1p
...
-----END CERTIFICATE REQUEST-----