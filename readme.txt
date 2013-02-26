***********
M�dulo de integra��o PagSeguro para Magento
v.1.1
***********


= Descri��o =

Este m�dulo tem por finalidade integrar o PagSeguro como meio de pagamento dentro da plataforma Magento.


= Requisitos =

Dispon�vel para a vers�o 1.7.0.2 do Magento.


= Instala��o =

1. Certifique-se de que n�o h� instala��o de outros m�dulos para o PagSeguro em seu sistema;
2. Descompacte o conte�do do arquivo zip dentro da pasta app em sua instala��o Magento. Caso seja informado da sobrescrita de alguns arquivos, voc� pode confirmar o procedimento sem problemas. Esta instala��o n�o afetar� nenhum arquivo do seu sistema, somente adicionar� os arquivos do m�dulo PagSeguro;
3. Ap�s copiar os arquivos, no administrador do Magento v� at� a opc�o Gerenciador de Cache na aba Sistema e clique na op��o Flush Magento Cache.

Pronto, o m�dulo de integra��o PagSeguro para Magento j� est� instalado.


= Configura��o =

Ap�s instalar o m�dulo, � necess�rio que se fa�a algumas configura��es para que efetivamente seja poss�vel utilizar-se dele. Essas configura��es est�o dispon�veis na op��o M�todos de pagamento nas configura��es do m�dulo.

	- email: E-mail cadastrado no PagSeguro
	- token: Token cadastrado no PagSeguro
	- url de redirecionamento: url utilizada para se fazer redirecionamento ap�s o cliente realizar a efetiva��o da compra no ambiente do PagSeguro. Pode ser uma url do pr�prio sistema ou uma outra qualquer de interesse do vendedor.
	- charset: codifica��o do sistema (ISO-8859-1 ou UTF-8)
	- log: diret�rio a partir da ra�z do sistema, onde se deseja criar o arquivo de log . Ex.: /logs/log_pagseguro.log

= Changelog =

v1.1
Modifica��o na estrutura de pastas para facilitar a intala��o.

v1.0
Vers�o inicial. Integra��o com API de checkout do PagSeguro.


= NOTAS =
	
	- Certifique-se que o email e o token informados estejam relacionados a uma conta que possua o perfil de vendedor ou empresarial;
	- Certifique-se que tenha definido corretamente o charset de acordo com a codifica��o (ISO-8859-1 ou UTF-8) do seu sistema. Isso ir� prevenir que as transa��es gerem poss�veis erros ou quebras ou ainda que caracteres especiais possam ser apresentados de maneira diferente do habitual.	