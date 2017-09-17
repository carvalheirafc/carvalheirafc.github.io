# GDB --help
## Don't Panic !
> [Documentação do GDB](https://www.gnu.org/software/gdb/)

_______________________

## Quick Guide

> help or h : ativa a ajuda do gdb

> run or r : executa o programa do início

> quit or q : sai do gdb

> kill or k : interrompe a execução do programa

> list linha or l linha : lista partes do código fonte

> show listsize & set listsize N : mostra & configura a qtde de linhas mostradas no comando list

> break linha or b linha : adiciona um ponto de parada na linha especificada do arquivo principal

> break funcaoX or b funcaoX : adiciona um ponto de parada no inicio da funcaoX do arquivo corrente

> break arq.cpp:linha or b arq.cpp:linha : adiciona um ponto de parada na linha especificada do arquivo
fonte de nome arq.cpp

> info break or i b : lista informações sobre os pontos de parada definidos

> delete N or d N : remove o ponto de parada N (visualize o valor de N com o comando info break) – o
comando delete sem a indicação do ponto de parada permite remover todos os pontos de parada de
uma só vez

> disable N or não remove, mas desativa o ponto de parada N

> enable N or reativa o ponto de parada N



## Setando as opções para compilação

> -g: Para poder habilitar a opção de depuração do GDB.

> -O#: Para modificar o quão otimizado o g++ vai deixar o seu código. 0 Nenhuma otimização. 3 Otimização Máxima. 

![flag](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/flag.png)



## Executando o Programa.

> gdb ./$PROG : Para poder executar o programa em função do executável criado com as flags de depuração.

![execution](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/executing.png)




## Caso não saiba o que fazer ainda.

> quit ou q : Faz com que o programa termine e conclua a execução do GDB.

![quit](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/quit.png)

## Executando Normalmente o programa.

> Neste exemplo estou usando um código que sei que não há nenhum tipo de erros ou problemas, tanto na compilação quanto na execução.
> Digitando **run** no prompt do GDB vai fazer o programa ser executado todo de uma unica vez, e como o mesmo não tem nenhum ponto de parada, será executado até o fim.

![run](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/run.png)  
![Exit Normaly](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/exit_normal.png)

## Executando com BrakPoints
> Uma das melhores funções do GDB, é poder monitorar a execução do programa, sem que o código fonte seja alterado, por meio de contadores ou uso de alguma saida para o terminal, como **printf** ou **std::cout**.

> Para isso pode-se adicionar brakpoints. Para isso, basta digitar **breakpoints** e o nome da função.<sub>(Pode se ao digitar o nome da mesma, usar o **tab** para completar o nome da função)</sub>

> Ao finalizar de colocar os breakpoints no GDB, execute o programa normalmente com o comando **run**

![break Points](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/b_main.png) 

> Para continuar pode-se digitar **continue** para pular a execução de um breakpoint para outro  ou **next** para executar o programa, passo a passo, podendo assim ver cada execução de cada linha do código.

![continue or next](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/num_loop.png)

> E para saber o quanto vale alguma variável, basta digitar **print** mais o nome da variavel.

![print](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/print_i%20.png)
