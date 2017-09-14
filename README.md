# GDB --help
## Don't Panic !
> [Documentação do GDB](https://www.gnu.org/software/gdb/)

_______________________
> Quick Guide

* help or h || ativa a ajuda do gdb

* run or r | executa o programa do início

* quit || q: sai do gdb

* kill || k : interrompe a execução do programa

* list linha || l linha : lista partes do código fonte

* show listsize & set listsize N : mostra & configura a qtde de linhas mostradas no comando list

* break linha || b linha : adiciona um ponto de parada na linha especificada do arquivo principal

* break funcaoX || b funcaoX : adiciona um ponto de parada no inicio da funcaoX do arquivo corrente

* break arq.cpp:linha || b arq.cpp:linha : adiciona um ponto de parada na linha especificada do arquivo
fonte de nome arq.cpp

* info break || i b : lista informações sobre os pontos de parada definidos

* delete N || d N : remove o ponto de parada N (visualize o valor de N com o comando info break) – o
comando delete sem a indicação do ponto de parada permite remover todos os pontos de parada de
uma só vez

* disable N : não remove, mas desativa o ponto de parada N

* enable N : reativa o ponto de parada N

______________________________
> Setando as opções para compilação

**-g:** Para poder habilitar a opção de depuração do GDB.

**-O#:** Para modificar o quão otimizado o g++ vai deixar o seu código. 0 Nenhuma otimização. 3 Otimização Máxima. 
![flag](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/flag.png)

______________________

> Executando o Programa.

**gdb ./$PROG** Para poder executar o programa em função do executável criado com as flags de depuração.
![execution](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/executing.png)


_____________________

> Caso não saiba o que fazer ainda.

**quit ou q** Faz com que o programa termine e conclua a execução do GDB.
![quit](https://raw.githubusercontent.com/carvalheirafc/carvalheirafc.github.io/master/screen-shots/quit.png)
