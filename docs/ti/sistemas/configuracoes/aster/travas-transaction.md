Travas no ASTER

Nesse cenário de teste, realizamos os testes aplicando as travas existentes no banco de dados migrando-as para a tela de Travas Transaction do ASTER.
Nas imagens abaixo, constará as imagens das travas acontecendo junto com a informação da trava correspondente e a localização da trava no ASTER.


## SPS-0001 - Necessário informar todos os dados de endereço!

### ASTER - Trava 1

- **Campo: Tipo de logradouro**


30


- **Campo: Rua/caixa postal**




- **Campo: Rua n°**


31


- **Campo: CEP**


- **Campos: Estado - Município**


32


- **Campo: ID do endereço**


- **Campo: País/região**


> OBS: Em qualquer um dos campos de endereço se estiver vazio ocorrerá a trava e campo País/região = ‘BR’.

33


## SPS-0003 - Verifica preenchimento de campos obrigatórios para itens de materiais.
### ASTER - Trava 4 - INATIVA

- **Campo: Item de venda**


34


- **Campo: Classificação de itens p/ impostos**


35


- **Campo: Nº do item**


36


- **Campo: Descrição**


37


- **Campo: Nome da UM de compras**


38


- **Campo: Nome da UM de vendas**


39


- **Campo: Nome da UM**


40


## SPS-0010 - Preencha o campo razão social do PN

### ASTER - Trava 6

- **Campo: Razão Social**

> OBS: A Ausência de informação no campo Razão Social causará a trava.

41


## SPS-0027 - Quando Produto Acabado, Preencha o campo Grupo Determinação

### ASTER - Trava 7

- **Campo: Grupo Determinação**

> OBS: No cadastro do item ou atualização de itens de material do tipo produto acabado, o preenchimento do campo Grupo Determinação de torna obrigatório.

42


## SPS-0028 - Preencha o campo Possui Suframa?

### ASTER - Trava 8

- **Campos: Possui Suframa? e Código**


> OBS: Caso o PN seja do tipo Cliente se torna obrigatório o preenchimento do Possui Suframa?

43


## SPS-00154- Não permite adicionar Pedido de Venda sem Lista de Preço.

### ASTER - Trava 9

- **Campo: SPS – Lista de Preço**


- **Campo: Utilização**


44


- **Campo: Grupo de Itens**


- **Campo: SPS_BonificacaoExtra**


45


- **Campo: Bonificação Trade?**


46


## SPS-00155- Não permite adicionar Nota Fiscal sem Lista de Preço.

### ASTER - Trava 10

- **Campo: SPS – Lista de Preço**


- **Campo: SPS – Utilização**


47


- **Campo: Grupo de itens**



## SPS-00156- Não permite adicionar Pedido de Devolução sem Lista de Preço.

### ASTER - Trava 11

- **Campos: SPS – Lista de Preço**


48


- **Campos: Utilização**


## SPS-0029 - Preencha o campo Possui Regime?

### ASTER - Trava 12

- **Campos: Possui Regime Especial? e Código**

> OBS: Caso o PN seja do tipo Cliente se torna obrigatório o preenchimento do Possui Regime Especial?

49


## SPS-0030 - Este PN Possui Regime, preencha Nº Regime

### ASTER - Trava 13

- **Campos: Nº Regime Especial e Possui Regime Especial?**

> OBS: Caso o PN seja do tipo Cliente e o campo Possui Regime Especial? Estiver igual a “Sim” se torna obrigatório o preenchimento do campo Nº Regime Especial.

50


## SPS-0031 - Preencha o campo Distribuidor Hospitalar?

### ASTER - Trava 14

- **Campo: Distribuidor Hospitalar?**

> OBS: Caso o PN seja do tipo cliente se torna obrigatório o preenchimento do campo Distribuidor Hospitalar?

51


## SPS-00157- Não permite adicionar Devolução de Nota Fiscal de Saída sem Lista de Preço.
### ASTER - Trava 15

- **Campos: SPS – Lista de Preço**


- **Campos: SPS – Utilização**




52


## SPS-0158- Impede inserção de Cotação de Compras sem certificado AE

### ASTER - Trava 16

- **Campo: Produto Controlado**



- **Campo: Orgão Regulador**


53


- **Campo: Autorização Especial para substâncias sujeitas a controle especial (AE)**





54


## SPS-0041 - Não é permitido adicionar NF de Entrada sem Pedido de Compra Vinculado!
### ASTER - Trava 17

- **Campo: Tipo de Item/Serviço**


- **Campo: Modelo**


55


- **Campo: Uso Principal**


> OBS: É obrigatório adição de NF de entrada somente proveniente de Pedido de venda, com uso principal específicos, modelo diferente de CTe selecionado e tipo do item igual a item.

56


## SPS-0159- Impede inserção de PC sem certificado AE

### ASTER - Trava 18

- **Campo: Produto Controlado**


- **Campo: Órgão Regulador**


57


- **Campo: Autorização Especial para substâncias sujeitas a controle Especial (AE)**



58


## SPS-0161- Não permite adicionar Solicitação de Compra sem o centro de custo vinculado.
### ASTER - Trava 19

- **Campo: Utilização**




- **Campo: Projeto**


59


## SPS-00163- Não permite adicionar PC fabricante com pendências documentais

### ASTER - Trava 20

- **Campo: U_SPS_Fabric**


- **Campo: Status da Linha**


60


- **Campo: Alvarás Aptos**



61


## SPS-0165- Impede fabricante divergente do informado no pedido de compras.

### ASTER - Trava 21

- **Campo: Cód. Fabricante**



- **Campo: Nome do Fabricante**


62




## SPS-0166- Impede fabricante com descrição divergente do cadastro do PN.
### ASTER - Trava 22

- **Campo: Nome do Fabricante**


63


## SPS-0167- Impede inserção de recebimento sem pedido de compras.

### ASTER - Trava 23

- **Campo: Referência base**


## SPS-0168- Não permite adicionar Solicitação de Compra sem preço.

### ASTER - Trava 24

- **Campo: Preço**


64


## SPS-00169- Não permite adicionar esboço PV se o cliente possuir pendências em documentos regulatórios.
### ASTER - Trava 25

- **Campo: Produto Controlado**




- **Campo: Alvarás Aptos**


65


- **Campo: Adicionar ESBOÇO**




## SPS-00170- Não permite adicionar NF se o cliente possuir pendências em documentos regulatórios.
### ASTER - Trava 26

- **Campo: Produto Controlado**


66


- **Campo: Alvarás Aptos**

- **Campo: Status**


67



## SPS-171- Não permite adicionar Talão com Preço Unitário 10x maior que a lista de preço.
### ASTER - Trava 27

- **Campo: Preço Unitário**


68


- **Campo: Lista de preços**


> OBS: Lista de preços diferente da lista 6 (Hospitalar).
## SPS-00174- Não permite adicionar CV se o cliente possuir pendências em documentos regulatórios.
### ASTER - Trava 28

- **Campo: Produto Controlado**


69


- **Campo: Alvarás Aptos**





70


## SPS-0175- Não permite adicionar Esboço de Solicitação de Compra sem projeto caso seja compra P&D.
### ASTER - Trava 29

- **Campo: Projeto**



- **Campo: Utilização**

> OBS: Utilização igual a Compra P&D.

71


## SPS-00178- Impede inserção de usuário duplicado na etapa.

### ASTER - Trava 30

- **Campo: Usuário Inserido/Removido**


> OBS: Ação deve ser diferente de R.

72


## SPS-00179- Não permite alterar pedido de transferência de outros solicitantes.
### ASTER - Trava 31

- **Campo: Ordem de produção**




- **Campo: Para depósito**


73


- **Campo: Status**




## SPS-00180- Não permite realizar transferência se o item não estiver no pedido base.
### ASTER - Trava 32

- **Campo: Ordem de produção**


74


- **Campo: Para depósito**




- **Campo: Nº do item**

> OBS: Trava não funcional, aceita a inclusão de outro item que não está no pedido.


75


## SPS-0042 - Não é permitido adicionar Pedido de Compra sem Centro de Custo vinculado!
### ASTER - Trava 33

- **Campo: Centro de Custo**



- **Campo: ID BR Supply**


76


- **Campo: Item**

Itens que não estão presentes na tabela "SPS_APROV_SBUGRPN2"
> OBS: Trava Ocorre quando os Campos Centro de custo e ID BR Supply não estão preenchidos e apenas itens fora da tabela "SPS_APROV_SBUGRPN2".

77


## SPS-00181- Não permite remover linha da transferência e adicionar novamente.

### ASTER - Trava 34

- **Campo: Ordem de produção**



- **Campo: Para depósito**


78




79


## SPS-0186- Impede inserção de Oferta de Compras sem certificado do exército.

### ASTER - Trava 35

- **Campo: Produto Controlado**



- **Campo: Orgão Regulador**


80


- **Campo: Licença de funcionamento Exército**



81


## SPS-0187- Impede inserção de Pedido de Compras sem certificado do exército.

### ASTER - Trava 36

- **Campo: Produto Controlado**



- **Campo: Órgão Regulador**


82


- **Campo: Licença de funcionamento Exército**



83


## SPS-0188- Impede inserção de Nota Fiscal de Entrada sem certificado do exército.
### ASTER - Trava 37

- **Campo: Produto Controlado**



- **Campo: Órgão Regulador**


84


- **Campo: Licença de funcionamento Exército**


85


## SPS-0948- Impede inserção de lote com status liberado.

### ASTER - Trava 38

- **Campo: Status**


86


- **Campo: Assinatura do usuário**



> OBS: Assinatura do usuário deve ser diferente de 205 – Portal Aster.


- **Campo: Nº do Item**


87


## SPS-0043 - Não é permitido adicionar NF de Entrada sem Centro de Custo vinculado!
### ASTER - Trava 39

- **Campo: Centro de Custo**

- **Campo: Item de estoque**


88


- **Campo: Item**

Itens que não estão presentes na tabela "SPS_APROV_SBUGRPN2"
> OBS: A trava ocorre quando o item não é controlado por estoque e está sem o centro de custo preenchido na linha da nota fiscal de entrada e apenas itens fora da tabela "SPS_APROV_SBUGRPN2".

89


## SPS-0189- Não é possível pedir transferência diretamente do recebimento para produção.
### ASTER - Trava 40

- **Campo: Do depósito**



- **Campo: Para depósito**


90


## SPS-00191- Não permite adicionar Devolução sem preencher informações do lote.
### ASTER - Trava 41

- **Campo: Lote Fornec/Lote Pai**



- **Campo: Data de fabricação**




91


- **Campo: Data de vencimento**


- **Campo: Data de admissão**


92




## SPS-0048 - Não é permitido adicionar Pedido de Devolução sem informar Motivo da Devolução!
### ASTER - Trava 42

- **Campo: Motivo Devolução**


> OBS: Trava é acionado quando o pedido de devolução é adicionado ou atualizado com campo Motivo Devolução vazio.

93


## SPS-00192 - Não permite adicionar Lote Duplicado.

### ASTER - Trava 43

> OBS: Trava obsoleta, o processo está voltado para devolução de mercadoria dentro do processo de compra, onde o lote do produto já está criado.


## SPS-0003 - Informar campos obrigatórios!

### ASTER - Trava 44 – INATIVA

- **Campo: Código NCM**

Cadastro de item.

94


- **Campo: Item de venda**

Cadastro de item.
- **Campo: Nº do item/Descrição**

Cadastro de item.

95


- **Campo: Nome da UM de compras**

Cadastro de item.
- **Campo: Nome da UM de vendas**

Cadastro de item.

96


- **Campo: Nome da UM**


Cadastro de item.
- **Campo: Serviço/Código NCM**


Cadastro de item.
> OBS: Bloqueia o cadastro quando o item de venda está flegado, classe de serviço, com NCM preenchido, e não possui preenchimento obrigatório nos seguintes campos: Código

97


do item, Descrição do item, Unidade de medida de compra, Unidade de medida de venda, Unidade de medida de estoque. (Trava sem sentido)


## SPS-0004 - Chave de Acesso Deve Conter 44 Dígitos!

### ASTER - Trava 45 - INATIVA

- **Campo: Chave de Acesso**

Nota Fiscal de Entrada.
- **Campo: Modelo**

Valores: 39 - NFe (55) | 45 - CT-e | 44 - Modelo CT-e

98


Nota Fiscal de Entrada.
> OBS: Bloqueia o documento quando o Model é 44, 45 ou 39 e a chave de acesso não possui 44 caracteres para o DocEntry informado.

99


## SPS-0012 - O setores Contábil, Financeiro, Garantia e Comercial precisa validar o PN: Salvar com o Status de Inativo (FORNECEDOR)
### ASTER - Trava 46 – INATIVA

- **Campos: Validação Controladoria - Validação Qualidade - Validação Comercial - Validação Fiscal – Código/Tipo**

Cadastro de Fornecedor.
- **Campo: Validação**


100


Cadastro de Fornecedor.
> OBS: Bloqueia a adição ou atualização do cadastro de fornecedor se o Tipo do PN = ‘Fornecedor’, ativo e os campos, Validação Controladoria diferente de 'Y' ou Validação Qualidade diferente de 'Y' ou Validação Comercial diferente de 'Y' ou Validação Fiscal diferente de 'Y'.
## SPS-0012 - O setores Contábil, Financeiro, Garantia e Comercial precisa validar o PN: Salvar com o Status de Inativo (CLIENTE)
### ASTER - Trava 47 – INATIVA

- **Campos: Validação Controladoria - Validação Qualidade - Validação Comercial - Validação Fiscal – Código/Tipo**


Cadastro de Fornecedor.

101


- **Campos: Validação**


Cadastro de Fornecedor.
> OBS: Bloqueia a adição ou atualização do cadastro de fornecedor se o Tipo do PN = ‘Cliente’, ativo e os campos, Validação Controladoria diferente de 'Y' ou Validação Qualidade diferente de 'Y' ou Validação Comercial diferente de 'Y' ou Validação Fiscal diferente de 'Y'.

102


## SPS-0049 - Não é permitido adicionar Devolução sem informar Motivo da Devolução!
### ASTER - Trava 48

- **Campo: Motivo Devolução**

> OBS: Trava é acionado quando a Devolução de Nota Fiscal de Saída é adicionado ou atualizado com campo Motivo Devolução vazio.

103


## SPS-0050 - Não é permitido adicionar Devolução sem informar Motivo da Devolução!
### ASTER - Trava 49

- **Campo: Motivo Devolução**


104


## SPS-00193-	Impede	inserção	de	data	de	vencimento	menor	que fabricação/admissão.
### ASTER - Trava 50

- **Campo: Data de vencimento**


105


## SPS-0194- Não permite adicionar Devolução com o Código Identificador Adicional ou Código SAP divergente do Item.
### ASTER - Trava 51

- **Campo: SPS – Grupo N1**

- **Campo: Tipo de Produção**


106


> OBS: Tipo de Produção 0 - Produção Interna ou 3 - Produção Parcial Interna.
- **Campos: Identificador adicional e Lote**



107


## SPS-0194B- Não permite adicionar Devolução com o Código Identificador Adicional ou Código SAP divergente do Item.
### ASTER - Trava 52

- **Campo: SPS – Grupo N1**

- **Campo: Tipo de Produção**


108


> OBS: Tipo de Produção 0 - Produção Interna ou 3 - Produção Parcial Interna.


- **Campos: Identificador adicional e Lote**



109


## SPS-0196 - Não permite adicionar solicitações de transferência com lote vencido.
### ASTER - Trava 53

- **Campo: Para depósito**

- **Campo: Lote p/ Teste**


110




## SPS-00197 - Não permite adicionar transferência com lote vencido.

### ASTER - Trava 54

- **Campo: Para depósito**

> OBS: Depósitos 01.22 e 01.39

111


- **Campo: Lote p/ Teste**



112


## SPS-00197 -	Não permite adicionar NF com utilização de Venda e Bonificação.
### ASTER - Trava 55

- **Campo: Utilização**


113


## SPS-0198 - Não permite adicionar Pedido de Devolução sem informar NF de Origem.
### ASTER - Trava 56

- **Campo: SPS – NF de Origem**


- **Campo: Utilização**


114


## SPS-0199 - Não permite adicionar Pedido de Devolução sem informar NF de Origem.
### ASTER - Trava 57

- **Campo: SPS – NF de Origem**


- **Campo: SPS – Utilização**


115


## SPS-00200 - Quando Nota for de Bonificação, em Prestações precisa estar selecionado Aplicar imposto proporcionalmente.
### ASTER - Trava 58

- **Campo: Utilização**


- **Campo: Aplicar imposto na 1ª prestação**


116


- **Campo: Prestações**


> OBS: Maior ou igual a 2 prestações.


117


## SPS-00201 - Trava duplicidade n NF, Serie e PN.

### ASTER - Trava 59

- **Campo: Serial**

- **Campo: Fornecedor**


118


- **Campo: Modelo**



## SPS-0202 - Impede adicionar Nota Fiscal com "Nome da UM" em branco.

### ASTER - Trava 60

- **Campo: Nome da UM**


119


- **Campo: Modelo**


## SPS-0203 - Impede Cancelar Adiantamento com Numeração Fiscal.

### ASTER - Trava 61

- **Campo: Nº NF SeqCode**


120


- **Campo: Modelo**



121


## SPS-0204 - Impede lançar nota Fiscal de Entrada sem CST de PIS.

### ASTER - Trava 62

- **Campo: CST para PIS**


- **Campo: Modelo**


> OBS: Modelo 18 - Modelo 21,21 - Nota Fiscal de Servi,39 - NFe (55),45 - CT-e,46 - NFS-e,56 - NF3-e 66.

122




## SPS-0205 - Impede lançar nota Fiscal de Entrada sem CST de COFINS.

### ASTER - Trava 63

- **Campo: CST para COFINS**


123


- **Campo: Modelo**


> OBS: Modelo 18 - Modelo 21,21 - Nota Fiscal de Servi,39 - NFe (55),45 - CT-e,46 - NFS-e,56 - NF3-e 66.


124


## SPS-0206 - Impede lançar nota Fiscal de Entrada sem CST de IPI.

### ASTER - Trava 64

- **Campo: CST para IPI**



- **Campo: Modelo**


> OBS: Modelo 39 - NFe (55).

125


## SPS-0207 - Impede lançar nota Fiscal de Entrada sem CST de ICMS.

### ASTER - Trava 65

- **Campo: CST para ICMS**


126


- **Campo: Modelo**


> OBS: Modelo 18 - Modelo 21,39 - NFe (55),45 - CT-e, 56 - NF3-e 66.


127


## SPS-0208- Não permite adicionar pedido de venda sem autorização na utilização.
### ASTER - Trava 66 - INATIVA

- **Campo: Assinatura de Usuário**

> OBS: A trava é acionada quando a assinatura do usuário é diferente de 205 (Portal Aster), e o UserId na tabela SPS_PV_AUT é diferente da Assinatura do usuário.

128


## SPS-0209- Utilizações remessa p/descarte e venda de sucata só podem ser usados nos depósitos 01.03 e 01.09.
### ASTER - Trava 67

- **Campo: Utilização**

> OBS: Remessa p/ descarte ou Venda de sucata.

129


- **Campo: Depósito**

> OBS: Depósito diferente do 01.03 - INSUMOS REPROVADOS e 01.09 - PRODUTO ACABADO REPROVADO.

130


## SPS-0208- Impede adicionar Devolução com qualquer depósito que não seja '01.08'.
### ASTER - Trava 68

- **Campo: Depósito**


131


## SPS-00209- Trava duplicidade Pedido de Devolução nNF, Serie e PN.

### ASTER - Trava 69

- **Campo: Status**

> OBS: A trava é acionada quando já existe um Pedido de devolução para o cliente, com o mesmo documento base e o Pedido de devolução não está Cancelado.

132


## SPS-00210- Impede de cancelar NF de entrada, caso exista ordem CQ criada para o recebimento.
### ASTER - Trava 70 - INATIVA

- **Campo: DocEntry**


133


## SPS-00216- Impede de cancelar NF de entrada, caso exista ordem CQ criada para o recebimento.
### ASTER - Trava 71- INATIVA

- **Campo: Motivo Cancelamento**


134


## SPS-0211- Impede Lançar Pedido de Transferência para Consumo Interno sem Centro de Custo.
### ASTER - Trava 72

- **Campo: Para depósito**


- **Campo: Centro de Custo**


135


## SPS-0212- Impede Lançar Esboço de Pedido de Transferência para Consumo Interno sem Centro de Custo.
### ASTER - Trava 73

- **Campo: Para depósito**



- **Campo: Centro de Custo**


136


## SPS-0214- Impede Lançar Esboço de Transferência para Consumo Interno sem Centro de Custo.
### ASTER - Trava 74

- **Campo: Para depósito**



- **Campo: Centro de Custo**


137


## SPS-00215- Não permite criar pedido de venda com quantidade diferente das transferências vinculadas.
### ASTER - Trava 75

- **Campo: Quantidade**



138


## SPS-00216- Impede de cancelar NF de entrada, caso exista ordem CQ criada para o recebimento.
### ASTER - Trava 76

- **Campo: Motivo Cancelamento**


139


## SPS-00216- Não permite adicionar NF de Entrega Futura sem preencher informações do lote.
### ASTER - Trava 77

- **Campo: Modulo NF de entrega futura**



- **Campo: Administrar item por**


140




## SPS-00217- Não permite adicionar NF de Entrega Futura com quantidade de lote diferente da quantidade vendida.
### ASTER - Trava 78

- **Campo: Quantidade**


141





## SPS-00218- Não permite adicionar Pedido de Compra com o campo "Código do Fabricante" vazio.
### ASTER - Trava 79

- **Campo: Cód. Fabricante**


142


## SPS-00219- Não permite adicionar Pedido de Compra com o campo "Nome do Fabricante" vazio.
### ASTER - Trava 80 - INATIVA

- **Campo: Nome do Fabricante**


143


## SPS-00218- Não permite realizar transferência se trocar o lote do item com correção de teor.
### ASTER - Trava 81

- **Campo: Ordem de produção**



- **Campo: SPS - Lote**


144


- **Campo: SPS - Lote**



## SPS-00220- Valida e Obriga os depósitos de origem para solicitação "Restore" - 01.22.
### ASTER - Trava 82 - INATIVA

- **Campo: Tipo da Solicitação**


145


- **Campo: Do depósito**




## SPS-00221- Valida e Obriga os depósitos de origem para solicitação "Restore" - 01.39.
### ASTER - Trava 83 - INATIVA

- **Campo: Tipo da Solicitação**


146


- **Campo: Para depósito**

## SPS-00230- Não permite adicionar entrada de mercadorias de produto controlado na rotina de pesagem do WMS.
### ASTER - Trava 84

- **Campo: Produto Controlado**


147


- **Campo: Tipo da Solicitação**



## SPS-00219- Não permite realizar transferência para produção com lote de revisão de embalagem bloqueada.
### ASTER - Trava 85

- **Campo: Restrição Revisão Embalagem**


148


- **Campo: Quantidade**




- **Campo: Depósito**


> OBS: Depósitos: 01.22, 01.23, 01.24, 01.25, 01.26, 01.27 e 01.28.

149


## SPS-00220- Não permite realizar transferências do WMS com lote vencido.

### ASTER - Trava 86

- **Campo: Depósito**

> OBS: Depósitos 01.22 e 01.39.


- **Campo: Tipo da Solicitação**


> OBS: Tipo da Solicitação diferente de Transferência.

150


- **Campo: Data de Vencimento**



151


## SPS-00221- Não permite realizar transferências do WMS com restrições no lote.
### ASTER - Trava 87

- **Campo: Para depósito**




- **Campo: Tipo da Solicitação**


152


- **Campo: Status**


> OBS: Status - Diferente de Liberado.


- **Campo: Status 2**

> OBS: Status 2 – Diferente de Aprovado.

153


- **Campo: Status 2**



## SPS-0222- Impede criar Pedido de Transferência de complemento com item diferente de Material de Embalagem.
### ASTER - Trava 88

- **Campo: OP Complementar**


154


- **Campo: Grupo de Itens**



> OBS: Diferente de Material de Embalagem.


- **Campo: Ordem de produção**


155


## SPS-0223- Impede criar Pedido de Transferência de complemento com itens não pertencentes a OP.
### ASTER - Trava 89

- **Campo: OP Complementar**


156


- **Campo: Ordem de produção**




- **Campo: Grupo de Itens**


157




## SPS-0224- Impede criar Pedido de Transferência de complemento com lote em branco.
### ASTER - Trava 90

- **Campo: OP Complementar**


158


- **Campo: Ordem de produção**



- **Campo: Grupo de Itens**


159


- **Campo: Administrar item por**



- **Campo: SPS – Lote**


160


## SPS-0225- Impede criar transferência de complemento com lote não pertencente ao item.
ASTER – Trava 91

- **Campo: OP Complementar**



- **Campo: Ordem de produção**


161


- **Campo: Grupo de Itens**



- **Campo: Administrar item por**


162


- **Campo: SPS – Lote**



## SPS-0226- Impede criar Transferência de Estoque de devolução com item diferente de Material de Embalagem.
ASTER – Trava 92

- **Campo: Tipo da Solicitação**


> OBS: Retorno Estoque ou Sobra em Campanha.

163


- **Campo: Grupo de Itens**

> OBS: Grupo não deve ser MATERIAL DE EMBALAGEM ou INDUSTRIALIZACAO POR ENCOMENDA.


- **Campo: Ordem de produção**


164


## SPS-0227- Impede criar Transferência de Estoque para posição diferente de "01.39-SOBRAEMB" para requisição de Retorno de Estoque.
ASTER – Trava 93

- **Campo: Tipo da Solicitação**

- **Campo: Grupo de Itens**


165


- **Campo: Ordem de produção**

- **Campo: Para depósito**


166


- **Campo: Primeiro para posição no depósito**



## SPS-0228- Impede criar Transferência de Estoque para posição diferente de "01.39-SOBRAEMB" para requisição de Retorno de Estoque.
ASTER – Trava 94

- **Campo: Tipo da Solicitação**


167


- **Campo: Grupo de Itens**



- **Campo: Ordem de produção**


168


- **Campo: Para depósito**

- **Campo: Primeiro para posição no depósito**


169


## SPS-0229- Impede criar Pedido de Transferência de Estoque para lotes que não tenham quantidade suficiente disponível.
ASTER – Trava 95

- **Campo: SPS - Lote**

- **Campo: Depósito**


170


- **Campo: Quantidade**


- **Campo: Tipo da Solicitação**


171


- **Campo: OP Complementar**



## SPS-00222- Não permite adicionar Liberação de Produção com Data de Entrega menor do que Hoje.
ASTER – Trava 96

- **Campo: Data de Liberação**


172


- **Campo: Tipo da Solicitação**


> OBS: Tipo da Solicitação Produção ou Separação Produção.

173


## SPS-0223- Não permite adicionar Esboço de Venda em duplicidade.

ASTER – Trava 97 - INATIVA

- **Campo: Data de lançamento**

- **Campo: Nº do item**


174


- **Campo: Total a pagar**

- **Campo: Status**

> OBS: Status deve ser diferente de ‘C’

175


- **Campo: Utilização**

- **Campo: Quantidade**



> OBS: O Status da Autorização deve estar Recusado.

176








## SPS-0224- Impede lançar Pedido de Devolução de Mercadorias com o Liberar Lote vazio.
ASTER – Trava 98

- **Campo: Liberar Lote**


177


- **Campo: Liberar Utilização**

> OBS: Utilização diferente de Armazenagem, Perda de Mercadoria, Remessa p/descarte, Conserto ou reparo, Exportacao, Remessa p/teste, Ret.Demonstracao, Amostra Gratis, Retorno Comodato, Devoluções compra, Comodato, Outras Saidas.

178


## SPS-0225- Impede lançar Pedido de Devolução de Mercadorias com a Utilização vazio.
ASTER – Trava 99

- **Campo: Uso principal**


179


## SPS-00226- Não permite adicionar Pedido de Devolução de Mercadorias sem lote alocado.
ASTER – Trava 100

- **Campo: Utilização**

- **Campo: Administrar item por**


180





## SPS-0231- Impede adicionar ou atualizar o PN com Necessário Agendamento
= "Sim" com os campos de agendamento vazios.

ASTER – Trava 101

- **Campo: Necessário Agendamento**


181


- **Campo: Meio de Comunicação**



- **Campo: E-mail Agendamento**


182


- **Campo: Telefone/Whatsapp Agendamento**

- **Campo: Link Portal de Agendamento**


183


- **Campo: Observação Agendamento**




- **Campo: Tipo**


184


## SPS-0228- Impede adicionar ou atualizar o PN de Possui Suframa = "Sim" com o campo Suframa vazio.
ASTER – Trava 102

- **Campo: Possui Suframa?**


185


- **Campo: SUFRAMA**

- **Campo: Tipo**


186


## SPS-0224- Não permite adicionar Nota Fiscal de Saída com Impostos Tributados = 0.
ASTER – Trava 103

- **Campo: Imposto**


- **Campo: Alíquota**


187





## SPS-0051 - Informar Motivo referente ao Desconto!

### ASTER - Trava 104

- **Campo: Assunto**

Valores: 3 Desconto.


188


- **Campo: Motivo Desconto**

> OBS: Se o campo assunto estiver como desconto é obrigatório preencher o Motivo de Desconto.
## SPS-0052 - Informar o Representante

### ASTER - Trava 105

- **Campo: Tipo**

Valores: 1 Trade Marketing | 2 Comissão | 3 Cancelamento Pedido | 5 SAC.

189


- **Campo: Representante**

> OBS: Trava ocorre quando um dos valores acima, estiver setado no campo Assunto se torna obrigatório informar Representante.
## SPS-0053 - Informar o Cliente que irá receber a Transferência da Verba

### ASTER - Trava 106

- **Campo: Tipo**

Valores: 1 Trade Marketing.

190


- **Campo: Assunto**

Valores: 1 Transf. de Saldo.


191


- **Campo: Destino Verba**

> OBS: Se o campo “Assunto” contive o valor “Transf. de Saldo.” e o campo “Tipo” contiver o valor “Trade Marketing.” O campo “Destino Verba” se torna obrigatório.


## SPS-0054 - Informar o % de Comissão Diferenciada!

### ASTER - Trava 107

- **Campo: Comissão Diferenciada?**

Valores: Y Sim.

192


- **Campo: % Comissão Diferenciada**

> OBS: Se o campo “Comissão Diferenciada?” se torna obrigatório o preenchimento do campo “% Comissão Diferenciada”.

193


## SPS-0055 - Não é permitido vincular fornecedor / fabricante que não seja qualificado!
### ASTER - Trava 108

- **Campo: Validação Controladoria**



194


- **Campo: Validação Qualidade**

- **Campo: Validação Comercial**


195


- **Campo: Validação Suprimentos**



## SPS-0056 - Não é permitido adicionar Solicitação de Compra sem Centro de Custo vinculado!
### ASTER - Trava 109

- **Campo: Centro de Custo**

Os itens não pertencentes à tabela “SPS_APROV_SBUGRPN2”.

196


> OBS: Trava para obrigar o preenchimento do Centro de Custo na linha da solicitação de compra, para itens fora da tabela “SPS_APROV_SBUGRPN2”.


## SPS-0057 - Não é permitido adicionar Pedido de compra com o fornecedor divergente do fornecedor qualificado!
### ASTER - Trava 110

- **Campo: Cód. Fabricante**


197


- **Campo: SPS - Grupo N3**


Valores: exceto esses, 'MPA','MPA4','MPD','MPD4','MPB','MPB4', no cadastro de item.
> OBS: Se o item informado na linha do pedido de compra estiver fora da exceção do campo “SPS - Grupo N3” no cadastro do item, citado acima, o campo “Cód. Fabricante” na linha do pedido de compra, precisa conter o mesmo fornecedor do cabeçalho do pedido de compra.

198


## SPS-0105- Não permite adicionar Pedido de Compra vinculado um contrato Guarda-chuva com o saldo maior do que o planejado.
ASTER – Trava 111

- **Campo: Total a pagar**


199


## SPS-0058 - Não é permitido adicionar Pedido de compra com o campo Incoterms vazio!
### ASTER - Trava 112

- **Campo: Incoterms**

> OBS: Trava para obrigar o preenchimento do campo “Incoterms” em todos os pedidos de compra.

200


## SPS-0061 - Não é permitido adicionar Recebimento de Mercadoria com o campo Incoterms vazio!
### ASTER - Trava 113

- **Campo: Incoterms**


> OBS: Trava para obrigar o preenchimento do campo “Incoterms” em todos os recebimentos de mercadorias.

201


## SPS-00106- Não permite criar Atividade sem vincular Cliente.

ASTER – Trava 114

- **Campo: Código do PN**



- **Campo: Tipo**


> OBS: Tipo Trade Marketing e Cancelamento de Pedido.

202




## SPS-0062 - Não é permitido adicionar NF de Entrada com o campo Incoterms vazio!
### ASTER - Trava 115

- **Campo: Incoterms**

> OBS: Trava para obrigar o preenchimento do campo “Incoterms” em todas as NF de Entrada.

203


## SPS-0068 - Não é permitido adicionar Pedido de Compra que possui contrato guarda chuva com condições de pagamento divergente!
### ASTER - Trava 116

- **Campo: Condições de pagamento**

Condições de pagamento do contrato guarda-chuva.
- **Campo: Condições de pagamento**

Condições de pagamento do pedido de compra.

204


> OBS: Trava que exige que a condições de pagamento do contrato guarda-chuva setado no pedido de compra seja igual a condição de pagamento no pedido de compra.


## SPS-0107- Impede inserção de Cotação de Vendas sem certificado AE.

ASTER – Trava 117

- **Campo: Produto Controlado**



- **Campo: Autorização de funcionamento da Anvisa (AFE)**


205




## SPS-0108- Impede inserção de PV sem certificado AE.

ASTER – Trava 118

- **Campo: Produto Controlado**


206


- **Campo: Autorização de funcionamento da Anvisa (AFE)**



207


## SPS-0069 - Não é permitido adicionar Pedido de Compra que possui contrato guarda chuva com o tipo de envio divergente
### ASTER - Trava 119

- **Campo: Tipo de envio**


Tipo de envio do contrato guarda-chuva.
- **Campo: Tipo de envio**


Tipo de envio do pedido de compra.

208


> OBS: Trava que exige que o Tipo de envio do contrato guarda-chuva setado no pedido de compra seja igual o Tipo de envio no pedido de compra.
## SPS-0109- Impede inserção NF de Saída sem certificado AE.

ASTER – Trava 120

- **Campo: Produto Controlado**

- **Campo: Autorização de funcionamento da Anvisa (AFE)**


209




## SPS-00111- Não permite adicionar Pedido sem % de Verba Diferenciada quando o campo "Comissão Diferenciada" está igual a Sim.
ASTER – Trava 121

- **Campo: Verba Diferenciada?**


210


- **Campo: % Verba Diferenciada**


211


## SPS-0070 - Não é permitido adicionar Pedido de Compra com o preço divergente do planejado no contrato guarda-chuva
### ASTER - Trava 122

- **Campo: Preço unitário**

Preço unitário do contrato guarda-chuva.


- **Campo: Preço unitário**


212


Preço unitário do pedido de compra.

> OBS: Trava que exige que o Preço unitário do contrato guarda-chuva setado no pedido de compra seja igual o Preço unitário no pedido de compra.


## SPS-00112- Não permite liberar Ordem de Despacho quando documentos com condição A Vista não estão Pagos.
ASTER – Trava 123

- **Campo: Situação**


213


- **Campo: Condições de pagamento**





- **Campo: Valor Aplicado**


214




## SPS-00113- Não permite adicionar recebimento sem preencher informações do lote.
ASTER – Trava 124

- **Campo: Lote Fabricante**


215


- **Campo: Data de fabricação**


- **Campo: Data de vencimento**


216


- **Campo: Data de admissão**



217




## SPS-0071 - Não é permitido adicionar Pedido de Compra com a quantidade maior do planejado do contrato guarda-chuva
### ASTER - Trava 125

- **Campo: Quantidade**

Cálculo de quantidade do contrato guarda-chuva.
> OBS: Imagem da trava não documentada, pois a trava nativa do SAP está sobrepondo essa trava.

218


## SPS-00114- Não permite adicionar Lote Duplicado.

ASTER – Trava 126

- **Campo: Lote**




219


## SPS-0072 - Variação de quantidade superior à definida para o Item!

### ASTER - Trava 127

- **Campo: % Qtd. Variação Positiva Recebimento**

Cadastro de item.

220


- **Campo: Quantidade**

Pedido de compra.
- **Campo: Quantidade**


Recebimento de mercadorias.
> OBS: Trava que impede inserção do Recebimento de mercadorias advinda do pedido de compras com variação de quantidade superior à permitida para o item, com base na quantidade vinculada no pedido de compra, e quantidade informada no campo “% Qtd. Variação Positiva Recebimento” no cadastro de item.

221


## SPS-00115-	Impede	inserção	de	data	de	vencimento	menor	que fabricação/admissão.
ASTER – Trava 128

- **Campo: Data de vencimento**


222


## SPS-00117- Não permite adicionar Pedido de Compra com a Unidade de Medida divergente do Contrato Guarda Chuva.
ASTER – Trava 129

- **Campo: Código da UM**


223


## SPS-00118- Não permite adicionar PC com o campo utilização vazio.

ASTER – Trava 130

- **Campo: Utilização**


224


## SPS-0073 - Variação de quantidade superior à definida para o Item!

### ASTER - Trava 131

- **Campo: % Qtd. Variação Positiva Recebimento**

Cadastro de item.
- **Campo: Quantidade**

Pedido de compra.

225


- **Campo: Quantidade**


Nota Fiscal de Entrada.
> OBS: Trava que impede inserção da Nota Fiscal de Entrada advinda do pedido de compras com variação de quantidade superior à permitida para o item, com base na quantidade vinculada no pedido de compra, e quantidade informada no campo “% Qtd. Variação Positiva Recebimento” no cadastro de item.

226


## SPS-00120-	Impede	inserção	de	data	de	vencimento	menor	que fabricação/admissão.
ASTER – Trava 132

- **Campo: Data de fabricação**


227


## SPS-00121- Impede inserção de quantidade total de volumes distribuídos diferente da quantidade do lote.
ASTER – Trava 133

- **Campo: Distribuir Volumes**


228


- **Campo: Quantidade**





## SPS-0074 - Variação de preço superior à definida para o Item!

### ASTER - Trava 134

- **Campo: % Variação Positiva Preço**


229


Cadastro de item.
- **Campo: Preço após desconto**


Pedido de compra.
- **Campo: Preço após desconto**


Recebimento de Mercadorias.
> OBS: Trava que impede inserção de Recebimento de Mercadorias advinda do pedido de compras com variação de preço superior à permitida para o item, com base no preço

230


vinculada no pedido de compra, e quantidade informada no campo “% Variação Positiva Preço” no cadastro de item.

## SPS-00122- Não permite realizar saída de mercadorias sem entrada da NFe.

ASTER – Trava 135

- **Campo: Modelo**

> OBS: Modelo deve ser diferente de NFe (55).

231


## SPS-00123- Não permite adicionar Pedido de Venda com PN sem as qualificações do Alvará (Para Item controlado).
ASTER – Trava 136

- **Campo: Produto Controlado**


232


- **Campo: Certificado de Responsabilidade Técnica (CRT)**


- **Campo: Licença ou alvará de localização e funcionamento (Expedido por órgão Municipal)**


233


- **Campo: Autorização de funcionamento da Anvisa (AFE)**


- **Campo: Certificado de Responsabilidade Técnica (CRT)**


234


- **Campo: Licença ou alvará de localização e funcionamento (Expedido por órgão Municipal)**


235


- **Campo: Licença de funcionamento ou alvará sanitário (Expedido por órgão sanitário)**


236


## SPS-0075 - Variação de preço superior à definida para o Item!

### ASTER - Trava 137

- **Campo: % Variação Positiva Preço**

Cadastro de item.
- **Campo: Preço após desconto**

Pedido de compra.

237


- **Campo: Preço após desconto**

Nota Fiscal de Entrada.
> OBS: Trava que impede inserção de Nota Fiscal de Entrada advinda do pedido de compras com variação de preço superior à permitida para o item, com base no preço vinculada no pedido de compra, e quantidade informada no campo “% Variação Positiva Preço” no cadastro de item.

238


## SPS-0076 - Item sem preço!

### ASTER - Trava 138

- **Campo: Preço após desconto**

> OBS: Não permite adicionar NF de saída com item sem preço.

239


## SPS-0077 - Item sem preço!

### ASTER - Trava 139

- **Campo: Preço após desconto**


> OBS: Não permite adicionar NF de Entrada com item sem preço.

240


## SPS-0078 - Item sem preço!

### ASTER - Trava 140

- **Campo: Preço após desconto**


> OBS: Não permite adicionar Pedido de Compra com item sem preço.

241


## SPS-0079 - Item sem preço!

### ASTER - Trava 141

- **Campo: Preço após desconto**

> OBS: Não permite adicionar Pedido de Venda com item sem preço

242


## SPS-0080 - Item sem preço!

### ASTER - Trava 142

- **Campo: Preço após desconto**

> OBS: Não permite adicionar Cotação de Venda com item sem preço

243


## SPS-0081 - Item sem preço!

### ASTER - Trava 143

- **Campo: Preço após desconto**

> OBS: Não permite adicionar Recebimento de Mercadorias com item sem preço.

244


## SPS-0083 - Não é permitido adicionar NF de Entrada com a condição de pagamento divergente do pedido!
### ASTER - Trava 144

- **Campo: Condições de pagamento**

Pedido de Compra.
- **Campo: Copiar de / Copiar para**


Recebimento de Mercadorias

245


- **Campo: Condições de pagamento**

Nota fiscal de Entrada.
> OBS: Trava que impede inserção da Nota Fiscal de Entrada com a condição de pagamento divergente do pedido de compra de referência base, desde que, esse pedido tenha sido primeiramente copiado para o recebimento de mercadorias e depois para a NF de entrada a trava será acionada.

246


## SPS-00125- Não permite adicionar recebimento sem preencher informações do lote.
ASTER – Trava 145

- **Campo: Campo: Assinatura do usuário**



- **Campo: Atualização do usuário**


247




## SPS-1821 - Não é permitida a entrada de material sem a vida útil cadastrada.

### ASTER - Trava 146

- **Campo: Vida útil Dias**


Cadastro de item.

248


- **Campo: batch raw batch**

Cadastro de item.
- **Campo: Nº do item**

Cadastro de item.

249


- **Campo: Nº do item**


Entrada de mercadorias.
> OBS: Trava que não permite adicionar entrada de mercadorias sem vida útil cadastrada. Os “N° de item” iniciados com “P”, o campo “Vida útil Dias” precisa estar zerado e o campo ”batch raw batch” precisa estar como “N” para que a trava seja ativada.

250


## SPS-0084 - Não é permitido adicionar LCM sem centro de custo em contas dos grupos 3.01.01, 4.01, 5.01!
### ASTER - Trava 147

- **Campo: Centro de Custo**


> OBS: A trava valida lançamentos contábeis verificando se existem linhas com contas específicas (classes 3, 4 ou 5), exceto a conta 5.02.01.01.007, sem centro de custo informado. A regra se aplica apenas a lançamentos que não sejam de encerramento do exercício.

251


## SPS-00127- Não permite adicionar saída de mercadorias sem autorização no depósito .
ASTER – Trava 148

- **Campo: Status 2**



252


## SPS-00126B- Não permite adicionar solicitações de transferência de mercadorias sem autorização no depósito.
ASTER – Trava 149

- **Campo: Atualização do usuário**

- **Campo: UserId**




253




## SPS-00128- Não permite adicionar entrada de mercadorias sem autorização no depósito.
ASTER – Trava 150

- **Campo: Assinatura do Usuário**


254


> OBS: A trava é acionada quando a assinatura do usuário é diferente de 205 (Portal Aster), e o UserId na tabela SPS_DEPOSITOS_AUT é diferente da Assinatura do usuário.



255


## SPS-00129-	Não permite adicionar recebimento de mercadorias sem autorização no depósito.
ASTER – Trava 151

- **Campo: Assinatura do Usuário**



> OBS: A trava é acionada quando o UserId na tabela SPS_DEPOSITOS_AUT é diferente da Assinatura do usuário.

256






## SPS-0086 - Não é permitido alterar anexos em pedidos já provados/confirmados!

### ASTER - Trava 152 – INATIVA

- **Campo: SPS_AtcName**

Pedido de compra.

257


- **Campo: Nome do arquivo**

Pedido de compra.
> OBS: A trava verifica pedidos de compra confirmados, comparando o campo personalizado de anexos com os arquivos efetivamente vinculados ao documento. Caso haja divergência entre os nomes dos anexos registrados e os anexos reais, a operação é bloqueada. A validação considera apenas documentos com linhas abertas. O objetivo é garantir consistência entre anexos informados e anexos vinculados ao pedido. Desativada!

258


## SPS-00130- Não permite adicionar nota fiscal de saída de sem autorização no depósito.
ASTER – Trava 153

- **Campo: Assinatura do Usuário**

> OBS: A trava é acionada quando o UserId na tabela SPS_DEPOSITOS_AUT é diferente da Assinatura do usuário.

259


## SPS-00131- Não permite adicionar dev. nota fiscal de saída sem autorização no depósito.
ASTER – Trava 154

- **Campo: Assinatura do Usuário**

> OBS: A trava é acionada quando o UserId na tabela SPS_DEPOSITOS_AUT é diferente da Assinatura do usuário.

260


## SPS-00132- Impede inserção de embalagem sem revisão.

ASTER – Trava 155

- **Campo: Atributo lote 2**

- **Campo: SPS- Grupo N3**




261



262


## SPS-00133- Não permite adicionar PC sem fabricante para itens que este campo é obrigatório.
ASTER – Trava 156

- **Campo: U_SPS_Fabric**


263


- **Campo: Cód. Fabricante**


264


- **Campo: Item p/ Teste**


265



266


## SPS-0141- Impede inserção de itens sem controle de lotes conforme sub- grupo N3.
ASTER – Trava 157

- **Campo: Controle de Lotes Obrigatório**


- **Campo: Administrar item por**


267


## SPS-00125.1- Não permite adicionar transferência de mercadorias sem autorização no depósito.
ASTER – Trava 158

- **Campo: Assinatura do Usuário**


> OBS: A trava é acionada quando o UserId na tabela SPS_DEPOSITOS_AUT é diferente da Assinatura do usuário.

268


## SPS-00142- Não permite realizar transferência de MP com quantidade diferente da solicitada.
ASTER – Trava 159

- **Campo: SPS – Grupo N2**

- **Campo: SPS – Grupo N3**

> OBS: Diferente de MPD e MPD4.

269


- **Campo: Quantidade**



270


## SPS-0043- Não permite adicionar Recebimento de Mercadoria que exceda o estoque máximo do item.
ASTER – Trava 160

- **Campo: Produto Controlado**


271


- **Campo: Máximo**

- **Campo: Em estoque**


272



273


## SPS-00145- Não permite adicionar nota de venda com mais de 500 caixas frete realizado pela a Globo.
ASTER – Trava 161

- **Campo: Utilização**

- **Campo: Tipo de material**

> OBS: Tipo de material Mercadoria para Revenda e Produto Acabado.

274


- **Campo: Utiliza Transportadora Padrão?**

- **Campo: Transportadora Padrão**


275




> OBS: A trava é acionada quando a soma da quantidade/ quantidade por CX coletiva é maior que 500.

276


## SPS-0146- Impede inserção de Cotação de Vendas com Lista de Preço de Vencimento Curto se o item não possuir saldo em estoque.
ASTER – Trava 162

- **Campo: SPS - Lista de Preço**



- **Campo: SPS - Quantidade**


277




## SPS-00148- Impede inserção de nota fiscal de saída com Talão Normal empenhado com Lote em Vencimento Curto - Sem PV.
ASTER – Trava 163

- **Campo: Vencimento Curto**


278


- **Campo: SPS - Lista de Preço**



- **Campo: Preenche Vendedor?**


279


- **Campo: Utilização**

> OBS: Utilização diferente de Remessa p/teste.

280


## SPS-00149-	Impede inserção de nota fiscal de saída com Talão de Vencimento Curto empenhando com Lote Normal - Com PV.
ASTER – Trava 164

- **Campo: Vencimento Curto**


281


- **Campo: Lista de Preço**



282




## SPS-00150-	Impede inserção de nota fiscal de saída com Talão de Vencimento Curto empenhando com Lote Normal - Sem PV.
ASTER – Trava 165

- **Campo: Vencimento Curto**


283


- **Campo: Nº da lista de preços**

## SPS-151- Impede modificação de itens ativos para usuários que não estejam no grupo "CADASTROS".
ASTER – Trava 166

- **Campo: Grupos**


284


## SPS-0152- Não permite adicionar solicitações de transferência com lote vencido.
ASTER – Trava 167

- **Campo: Para depósito**


285


- **Campo: Data de vencimento**





286


## SPS-0153- Não permite adicionar transferência com lote vencido.

ASTER – Trava 168

- **Campo: Para depósito**



- **Campo: Data de vencimento**


287




## SPS-0002- Verifica CNPJ/CPF e I.E foram preenchidos.

ASTER – Trava 169 - INATIVA

- **Campo: CNPJ**


288


- **Campo: Inscrição Estadual**


- **Campo: CPF**


289


## SPS-00119- Não permite adicionar PC com o campo Código de Imposto vazio.
ASTER – Trava 170 - INATIVA

- **Campo: Código de imposto**


290


923- Não permite cancelar/fechar recebimento com Ordem CQ em aberto.

ASTER – Trava 171

- **Campo: BASEDOCENTRY**



291




## SPS-00145- Não permite adicionar nota de venda com mais de 1000 caixas frete realizado pela a Globo.
ASTER – Trava 172

- **Campo: Utilização**


292


- **Campo: Tipo de material**



- **Campo: Transportadora Padrão**


> OBS: Transportadora Padrão deve ser diferente de F17115437000173.

293


- **Campo: Quantidade/ Quantidade por CX coletiva**

> OBS: Trava é acionada quando a soma da quantidade/ quantidade por CX coletiva é maior que 1.000.

294


## SPS-00156- Não permite adicionar Pedido de Devolução sem Lista de Preço.

ASTER – Trava 173

- **Campo: SPS – Lista de Preço**

- **Campo: Utilização**


295


## SPS-00169- Não permite adicionar Pedido de Devolução sem Lista de Preço.

ASTER – Trava 174

- **Campo: Produto Controlado**


- **Campo: Alvarás Aptos**


296