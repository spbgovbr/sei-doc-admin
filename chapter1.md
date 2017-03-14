# 2. Cadastro do Órgão



Os órgãos deverão ser cadastrados em duas etapas.

Primeiramente, o órgão deve ser incluído no sistema SIP. Para fazer essa operação, entre no SIP com perfil de Administrador e clique em **Órgãos&gt;Novo**, conforme abaixo:

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/menu-incluir-orgao.png "menu-incluir-orgao")

Em seguida, na tela **Novo Órgão**, preencha os campos Sigla do Órgão e Descrição do Órgão e clique em **Salvar **no canto superior direito da tela.

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/tela-novo-orgao.png "tela novo órgão")



Realizado o cadastro no SIP, os dados cadastrais do órgão devem ser complementados no SEI. Entre no sistema SEI com perfil **Administrador **e selecione **Administração&gt;Órgãos**:

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/menu-orgao-sei.png "menu orgão sei")



Em seguida, na tela **Órgãos**, selecione o ícone de edição:

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/tela-orgaos.png "tela órgãos")



Preencha os dados cadastrais do Órgão na tela **Alterar Órgão**:

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/tela-alterar-orgao.png "tela alterar órgãos")



Ainda na tela **Alterar Órgão**, se for o caso, marque os **Check Boxes **referentes ao recebimento de processos e publicação de documentos, bem como anexe o arquivo correspondente ao timbre do órgão. Ao finalizar, clique no botão **Salvar **no canto superior direito da tela. O Campo **Formato da Numeração **é utilizado para criar a fórmula de numeração do protocolo. Veja instruções especificas de como configurar esse campo na página [**Fórmula de Protocolo**](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/2.-cadastro-do-orgao/#01).

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/tela-timbre.png "tela timbre")



## **2.1 Fórmula de Protocolo**

Com a publicação da Portaria Interministerial MJ/MP n° 2.321, de 30 de dezembro de 2014, os órgãos e entidades terão até 180 dias da data de sua publicação para se organizarem, a fim de iniciarem, todos simultaneamente, a implantação da nova sistemática de utilização do Número Único de Protocolo \(NUP\), em substituição à sistemática definida na Portaria SLTI/MP n° 03, de 16 de maio 2003.

[Página sobre o novo NUP](http://comprasgovernamentais.gov.br/paginas/comunicacoes-administrativas/numero-unico-de-protocolo-nup)

| **Importante!**A fórmula para o novo NUP \(21 dígitos\) no SEI: cod\_unidade\_sei\_07d.seq\_anual\_cod\_unidade\_sei\_08d/ano\_4d-dv\_mod97\_base10\_executivo\_federal\_2d **Onde:** **cod\_unidade\_sei\_07d:**Código SIP da unidade em que deverá estar atribuído o código do SIORG da unidade protocolizadora **seq\_anual\_cod\_unidade\_sei\_08d:**Código seguencial por ano relacionado à unidade do SEI **ano\_4d:**Ano, com quatro dígitos **dv\_mod97\_base10\_executivo\_federal\_2d:**Máscara para o novo dígito verificador conforme definido nos normativos.[\#132](https://processoeletronico.gov.br/issues/132) |
| :--- |


Quando a Portaria Interministerial MJ/MP n° 2.321, de 2014 entrar em vigor, esta será a nova composição do NUP a ser atribuído aos documentos \(avulsos ou processos\):

**0000000.00000000/0000-00  
\(21 dígitos\)**

Primeiro grupo \(7 dígitos\): código SIORG da unidade administrativa que atua como unidade protocolizadora

Segundo grupo \(8 dígitos\): sequencial numérico

Terceiro grupo \(4 dígitos\): ano de formação do documento \(avulso ou processo\)

Quarto grupo \(2 dígitos\): dígitos de verificação

O SEI permite criar algorítimo para a geração automática do número do Protocolo. No âmbito da Administração Federal, é adotado o Número Único de Protocolo - NUP, cuja geração é realizada de acordo com a seguinte formulação:

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/formula-imagem-0.png "fórmula protocolo")

**Observação:**para cadastrar o código da unidade protocolizadora, que corresponde ao código**uuuuu**na figura acima, preencha o campo **Código SEI **da tela **Alterar Unidade **seguindo as instruções da pagina [**Unidades no SEI**](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/3.-cadastro-de-unidades/#02).

O SEI pode ser programado para a geração do NUP, segundo a fórmula utilizada no âmbito da Administração Federal, ou ainda, segundo outras fórmulas utilizadas nos protocolos nos âmbitos estadual, municipal ou das autarquias e empresas públicas das três esferas dos três poderes. Para tal, o SEI oferece uma linguagem simples de programação e variáveis pré estabelecidas que podem ser utilizadas na codificação da fórmula.

A codificação da fórmula é introduzida no SEI através do campo **Formato da Numeração **da tela **Alterar Órgão**. A codificação utilizada para a geração do NUP, no âmbito da Administração Federal, é a seguinte:

.

**`@cod_unidade_sei_05d`@seq\_anual\_cod\_unidade\_sei\_06d@/`@ano_4d`@-`@dv_mod11_executivo_federal_2d`@**, onde as seguintes variáveis foram utilizadas na formulação:

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/formula-imagem-1.png)

A quantidade de dígitos de cada variável é parametrizável, por meio da numeração que aparece ao final de cada variável, conforme mostrado abaixo:



![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/formula-imagem-2.png)



Outro elemento utilizado na fórmula do NUP, são os caracteres utilizados na separação das variáveis. Esses caracteres são introduzidos diretamente na fórmula sem nenhum tratamento especial, conforme podemos constatar na figura abaixo. No caso da fórmula do NUP, foram utilizados os caracteres**"."**,**"/"**e**"-"**, porém outros caracteres podem ser utilizados.

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/formula-imagem-3.png)

As variáveis pré formatadas no SEI, que podem ser utilizadas na programação do código gerador do número do protocolo, são as seguintes:



![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-adminisrador/formula-imagem-4.png)

  




