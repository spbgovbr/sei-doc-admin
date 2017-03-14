# 9. Infra



Para enxergar esta opção no menu esquerdo o usuário deverá ter perfil de **Informática**.



## 9.1 Agendamentos

O SEI, através do Menu Infra, permite que o usuário agende tarefas com descrição do Comando e a sua Periodicidade e Complemento.

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/infra-agendamentos1.png)



## 9.2 Auditoria

O SEI possibilita que o usuário, com perfil de Auditoria, possa rastrear todas as ações praticadas e definidas como pontos de controle nos parâmetros do SEI nas diversas unidades por seus usuários.

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/infra-auditoria1.jpeg)



##  9.3 Log

Os erros ficarão registrados no Log do Sistema.

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/logs1.jpeg)



##  9.4 Parâmetros

O Usuário poderá criar diversos parâmetros com os seus respectivos valores.

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/parametros1.jpeg)

Segue abaixo a tabela de parâmetros do SEI e SIP

**Tabela de Parâmetros SEI**

As configurações da tabela de parâmetros podem ser realizadas através do menu Infra/Parâmetros do SEI \(necessária permissão no perfil Informática\):

| ID\_MODELO\_BASE\_CONHECIMENTO | Modelo de documento utilizado pelo eDoc para geração de Bases de Conhecimento |
| :--- | :--- |
| ID\_MODELO\_INTERNO\_BASE\_CONHECIMENTO | Modelo de documento utilizado pelo editor web para geração de Bases de Conhecimento |
| ID\_SERIE\_EMAIL | ID do tipo de documento email \(valor serie.id\_serie correspondente\) |
| ID\_UNIDADE\_TESTE | Identificador da unidade de teste do sistema \(unidade.id\_unidade\). Esta unidade deve existir pois é utilizada temporariamente em algumas chamadas de Web Services. |
| SEI\_EMAIL\_ADMINISTRADOR | Endereço para envio de emails informando erro em agendamentos de tarefas do sistema \(mais de um email pode ser informado utilizando vírgula como separador\) |
| SEI\_EMAIL\_SISTEMA | naoresponder@..... \(endereço utilizado por mensagens enviadas pelo sistema\) |
| SEI\_HABILITAR\_ASSINATURA\_DOCUMENTO\_EXTERNO | 0 - desabilitado 1 - habilitado somente para unidades de protocolo |
| SEI\_HABILITAR\_GRAU\_SIGILO | 0 – desabilitado 1 – opcional 2 – obrigatório |
| SEI\_HABILITAR\_HIPOTESE\_LEGAL | 0 – desabilitado 1 – opcional 2 – obrigatório |
| SEI\_HABILITAR\_MOVER\_DOCUMENTO | 0 - desabilitado 1 - habilitado somente para unidades de protocolo 2 - habilitado para todos os usuários |
| SEI\_HABILITAR\_NUMERO\_PROCESSO\_INFORMADO | Ao gerar um processo **exibe campo para digitação do número e da data de autuação**: 0 - desabilitado 1 - habilitado somente para unidades de protocolo 2 - habilitado para todos os usuários |
| SEI\_HABILITAR\_VALIDACAO\_CPF\_CERTIFICADO\_DIGITAL | 0 – desabilitado 1 – habilitado \(o CPF do certificado deverá ser igual ao do usuário assinante\) |
| SEI\_HABILITAR\_VALIDACAO\_EXTENSAO\_ARQUIVOS | 0 – desabilitado 1 – habilitado \(somente serão aceitos arquivos contendo as extensões cadastradas através do menu Administração/Extensões de Arquivos Permitidas\) |
| SEI\_ID\_SISTEMA | Valor do campo sistema.id\_sistema referente ao sistema SEI na base de dados do SIP |
|  | SEI\_MASCARA\_ASSUNTO |
|  | SEI\_MASCARA\_NUMERO\_PROCESSO\_INFORMADO |
| SEI\_MSG\_AVISO\_CADASTRO\_USUARIO\_EXTERNO | Permite exibir um aviso para os usuários externos antes que eles efetuem o cadastro no sistema. Se este campo estiver vazio nenhuma mensagem será apresentada e o usuário será direcionado diretamente para o formulário de cadastro. |
| SEI\_NUM\_FATOR\_DOWNLOAD\_AUTOMATICO | Opcional. Permite limitar o download automático de arquivos externos de acordo com a velocidade de transferência de dados do usuário. Se a velocidade do usuário for 150kb/s e o fator for configurado com 5 então para arquivos maiores que 750kb \(150 x 5\) será exibido um link para o usuário \(ao invés de iniciar automaticamente o download\). As velocidades de transferência dos usuários podem ser consultadas através do menu Infra/Velocidades de Transferência de Dados. OBS: A velocidade somente será atualizada quando o usuário visualizar um documento externo maior que 256kb. |
| SEI\_NUM\_MAX\_DOCS\_PASTA | 20 \(informa o número de documentos para agrupamento em pastas na árvore de processo – deixar vazio para não realizar agrupamento\) |
| SEI\_SUFIXO\_EMAIL | .jus.br - sufixo adicionado em emails enviados pelo sistema, corresponde ao valor da variável`sufixo_email` |
| SEI\_TAM\_MB\_ANEXO\_EMAIL | 10 \(valor em Mb\), deve refletir o valor configurado no servidor de email da instituição |
| SEI\_TAM\_MB\_DOC\_EXTERNO | 200 \(valor em Mb\), é necessário também configurar no php.ini as variáveis: post\_max\_size 256M upload\_max\_filesize 200M |
| SEI\_VERSAO | Indica a versão instalada do sistema |
| SEI\_WS\_NUM\_MAX\_DOCS | 5 \(número máximo de documentos que podem ser gerados simultaneamente em um processo através da API de Web Services do SEI\) |

> **OBS**: o sistema poderá alterar/adicionar automaticamente parâmetros nesta tabela.



As configurações da tabela de parâmetros podem ser realizadas através do menu Infra/Parâmetros do SEI \(necessária permissão no perfil Informática\).

O usuário com o perfil Informática poderá alterar os parâmetros no SEI. Neste caso, o usuário deverá encontrar na lista o parâmetro**SEI\_HABILITAR\_NUMERO\_PROCESSO\_INFORMADO **e depois alterar para a opção 2. Sendo assim, ao gerar um processo o SEI exibirá o campo para digitação do número e da data de autuação como na imagem abaixo.

0 - desabilitado  
1 - habilitado somente para unidades de protocolo  
**2 - habilitado para todos os usuários**

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/iniciar-processo.jpeg)

**Tabela de Parâmetros SIP**

As configurações da tabela de parâmetros podem ser realizadas através do menu Infra/Parâmetros \(o usuário deve ser administrador do sistema SIP – menu Sistemas/Administradores\):

| EMAIL\_SISTEMA | naoresponder@..... \(endereço utilizado por mensagens enviadas pelo sistema\) |
| :--- | :--- |
| EMAIL\_ADMINISTRADOR | Endereço para envio de emails informando erro em agendamentos de tarefas do sistema \(mais de um email pode ser informado utilizando ponto e vírgula como separador\) |
| ID\_SISTEMA\_SIP | Valor do campo sistema.id\_sistema referente ao sistema SIP |
| ID\_USUARIO\_SIP | Valor do campo usuario.id\_usuario referente ao usuário SIP |
| ID\_PERFIL\_SIP\_ADMINISTRADOR\_SIP ID\_PERFIL\_SIP\_ADMINISTRADOR\_SISTEMA ID\_PERFIL\_SIP\_BASICO ID\_PERFIL\_SIP\_COORDENADOR\_PERFIL ID\_PERFIL\_SIP\_COORDENADOR\_UNIDADE | Apontamentos para os perfis reservados do SIP |
| SIP\_VERSAO | Indica a versão instalada |

> **OBS:**o sistema poderá alterar/adicionar automaticamente parâmetros nesta tabela.



