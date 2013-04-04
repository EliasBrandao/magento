-------------------------------------------------
M�dulo de integra��o PagSeguro para Magento
v1.0
-------------------------------------------------


= Descri��o =

Com o m�dulo instalado e configurado, voc� pode pode oferecer o PagSeguro como op��o de pagamento em sua loja. O m�dulo utiliza as seguintes funcionalidades que o PagSeguro oferece na forma de APIs:

	- Integra��o com a API de Pagamentos


= Requisitos =

	- Magento Community 1.7.0.2
	- PHP 5.1.6+
	- SPL
	- cURL
	- DOM


= Instala��o =

	- Certifique-se de que n�o h� instala��o de outros m�dulos para o PagSeguro em seu sistema;
	- Baixe o reposit�rio como arquivo zip ou fa�a um clone;
	- Copie as pastas 'code' e 'etc' para dentro da pasta 'app' em sua instala��o Magento. Caso seja informado da sobrescrita de alguns arquivos, voc� pode confirmar o procedimento sem problemas. Esta instala��o n�o afetar� nenhum arquivo do seu sistema, somente adicionar� os arquivos do m�dulo PagSeguro;
	- Certifique-se de que as permiss�es das pastas e arquivos rec�m copiados sejam, respectivamente, definidas como 755 e 644;
	- Na �rea administrativa do seu sistema, acesse o menu System -> Cache Management -> Flush Magento Cache.


= Configura��o =

Para acessar e configurar o m�dulo acesse o menu System -> Configuration -> Payment methods -> PagSeguro. As op��es dispon�veis est�o descritas abaixo.

	- ativar m�dulo: ativa/desativa o m�dulo
	- nome de exibi��o: define o nome que ser� utilizado para o meio de pagamento
	- e-mail: e-mail cadastrado no PagSeguro
	- token: token gerado no PagSeguro
	- url de redirecionamento: ao final do fluxo de pagamento no PagSeguro, seu cliente ser� redirecionado automaticamente para a p�gina de confirma��o em sua loja ou ent�o para a URL que voc� informar neste campo. Para ativar o redirecionamento ao final do pagamento � preciso ativar o servi�o de Pagamentos via API em https://pagseguro.uol.com.br/integracao/pagamentos-via-api.jhtml
	- charset: codifica��o do seu sistema (ISO-8859-1 ou UTF-8)
	- log: ativa/desativa a gera��o de logs
	- diret�rio: informe o local a partir da ra�z de instala��o do Magento onde se deseja criar o arquivo de log. Ex.: /logs/ps.log. Caso n�o informe nada, o log ser� gravado dentro da pasta ../PagSeguroLibrary/PagSeguro.log


= Changelog =

	v1.0

	- Vers�o inicial. Integra��o com API de checkout do PagSeguro.


= Notas =
	
	- O PagSeguro somente aceita pagamento utilizando a moeda Real brasileiro (BRL).
	- Certifique-se que o email e o token informados estejam relacionados a uma conta que possua o perfil de vendedor ou empresarial.
	- Certifique-se que tenha definido corretamente o charset de acordo com a codifica��o (ISO-8859-1 ou UTF-8) do seu sistema. Isso ir� prevenir que as transa��es gerem poss�veis erros ou quebras ou ainda que caracteres especiais possam ser apresentados de maneira diferente do habitual.
	- Para que ocorra normalmente a gera��o de logs, certifique-se que o diret�rio e o arquivo de log tenham permiss�es de leitura e escrita.
	- D�vidas? https://pagseguro.uol.com.br/desenvolvedor/comunidade.jhtml
