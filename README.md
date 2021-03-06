<p align="center">
  <a href="#">
  	<img src="https://github.com/WalderlanSena/jogodavelhaemc/blob/master/img/jogoDaVelha.png" width="500">
   </a>
</p>

<p align="center">
<a href="#"><img src="http://www.walderlan.xyz/assets/stable.svg"></a>
<a href="#"><img src="http://www.walderlan.xyz/assets/licenseGPL.svg" alt="License"></a>
</p>

<h3 align="center">Exemplo do funcionamento do software</h3>

<p align="center">
  <a href="#">
  	<img src="https://github.com/WalderlanSena/jogodavelhaemc/blob/master/img/exemplo.jpg">
   </a>
</p>

<h3 align="center">Exemplo do Funcionamento dos Arrays (Tabelas)</h3>

<p align="center">Quando o usuário adiciona um X ou O na posição respectiva da tabela, outra tabela em background guarda este valor para que seja impossivel sua remarcação.</p>

<p align="center">
  <a href="#">
  	<img src="https://github.com/WalderlanSena/jogodavelhaemc/blob/master/img/arrays.png" width="800">
   </a>
</p>

```
	Digite uma posição, ultilizando as teclas de 1 a 9.
```
<h3>Como compilar ?<h3>
<h4>Obs: No caso de sistemas operacionais  Windows altere a linha 3 no define para:</h2>

```c
	#define CLEAR "cls"   //No caso de Sistemas Windows
	#define CLEAR "clear" //Mantenha como está para Sistemas Gnu/Linux,Unix,Mac
```


<h3>Compilando software com a bilioteca estática</h3>

```
	g++ jogodavelha.cpp lib/velha.cpp -o jogodavelha
```

<h3>Compilando a biblioteca para geração dinâmica</h3>
<small>.so no linux e .lib no windows </small>

```
	g++ -shared -fPIC lib/velha.cpp  -o lib/libvelha.so
```

<h3>Na utilização de sistemas operacionais baseados em gnu/linux, pode-se ultilizar o Makefile como:</h3>

```
	make          - Compila o programa com a biblioteca estática
	
	make libLinux - Gerando Biblioteca Dinâmica para Sistemas Operacionais Linux
	
	make clean    - Limpando os executaveis gerados
```

<h3>Licença</h3>

O Jogo da Velha é um software de código aberto licenciado sob a licença [GPL license](https://github.com/WalderlanSena/jogodavelhaemc/blob/master/LICENSE).
