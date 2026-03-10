
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

5. Checklist de Verificação
[ ] CSR gerada com os dados corretos da empresa? 

[ ] Chave privada salva com segurança? 

[ ] Domínio wildcard (*) incluído na solicitação? 

[ ] Instalação confirmada no WHM?

![Sectigo Logo](docs/imagens/sectigo-logo.png)