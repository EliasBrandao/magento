***********
M�dulo PagSeguro para o Magento
Este m�dulo tem por finalidade realizar transa��es de pagamentos entre sistema Magento e o PagSeguro
Dispon�vel para as vers�es 1.7.0.2 do Magento.
***********

- Instala��o
	
	
Para instalar o m�dulo Magento do PagSeguro abra a pasta app localizada na raiz do magento.

Ap�s entrar na pasta app, v� para a pasta etc e localize a pasta modules.

Ap�s localizar a pasta modules, copie o arquivo PagSeguro_PagSeguro.xml dentro dela.

Ap�s copiar o arquivo, volte para a pasta app e entre na pasta code.

Dentro de code, copie a pasta PagSeguro (m�dulo) dentro da pasta local.

Caso a pasta local n�o exista, basta criar.

Ap�s copiar os arquivos, no administrador do Magento v� at� a opc�o Gerenciador de Cache na aba Sistema e clique na op��o Flush Magento Cache.

Pronto, o magento j� est� instalado. 	

- Configura��es

Ap�s instalado o m�dulo, � necess�rio que se fa�a algumas configura��es para que efetivamente seja poss�vel utilizar-se dele. Essas configura��es est�o dispon�veis na op��o M�todos de pagamento nas configura��es do m�dulo.

	- email: E-mail cadastrado no PagSeguro
	- token: Token cadastrado no PagSeguro
	- url de redirecionamento: url utilizada para se fazer redirecionamento ap�s o cliente realizar a efetiva��o da compra no ambiente do PagSeguro. Pode ser uma url do pr�prio sistema ou uma outra qualquer de interesse do vendedor.
	- charset: codifica��o do sistema (ISO-8859-1 ou UTF-8)
	- log: diret�rio a partir da ra�z do sistema, onde se deseja criar o arquivo de log . Ex.: /logs/log_pagseguro.log
			
* NOTAS:
	
	- Certifique-se que o email e o token informados estejam relacionados a uma conta que possua o perfil de vendedor ou empresarial;
	- Certifique-se que tenha definido corretamente o charset de acordo com a codifica��o (ISO8859-1 ou UTF8) do seu sistema. Isso ir� prevenir que as transa��es gerem poss�veis erros ou quebras ou ainda que caracteres especiais possam ser apresentados de maneira diferente do habitual.
	