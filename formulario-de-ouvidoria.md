# 12. Formulário de Ouvidoria

O SEI possui um formulário de ouvidoria padrão que pode ser acessado através do endereço:

| [http://\[servidor\_php\]/sei/controlador\_externo.php?acao=ouvidoria&id\_orgao\_acesso\_externo=0](http://\[servidor\_php\]/sei/controlador\_externo.php?acao=ouvidoria&id\_orgao\_acesso\_externo=0) |
| :--- |


O parâmetro id\_orgao\_acesso\_externo indica em qual órgão será gerado o processo \(verificar campo id\_orgao da tabela orgao\). Também é necessário configurar a chave HostWebServices/Ouvidoria do arquivo ConfiguracaoSEI.php com o endereço dos servidores habilitados para chamada do serviço.

No SEI é permitida apenas uma unidade de ouvidoria por órgão que pode ser configurada através do menu **Administração/Unidades/Listar **– ação Alterar Unidade – opção “Unidade de ouvidoria”. Os tipos de processo exibidos são aqueles marcados como de ouvidoria através do menu **Administração/Tipos de Processo/Listar **– ação Alterar Tipo de Processo – opção **“Exclusivo da Ouvidoria”**.

![](https://softwarepublico.gov.br/social/sei/manuais/manual-do-administrador/ouvidoria.jpg)

É possível criar outro formulário com a identidade visual da instituição pois os dados montados na página \(Estado, Cidade e Tipo\) bem como a geração do processo são realizados através de Web Services.



