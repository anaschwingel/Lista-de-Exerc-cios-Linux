# Lista-de-Exercios-Linux

#### **1 Problema**
Utilize o comando echo para imprimir seu nome no terminal.

  `nome="Ana";echo $nome`

#### **2 Problema**
Utilize o comando echo para salvar seu nome em um arquivo chamado cliente01.txt.
Confira o resultado com o comando less.

   `echo "ana" > cliente01.txt`
    `less`
    `less cliente01.txt`

#### **3 Problema**
Utilize o comando echo para salvar o nome da cidade em que você nasceu no
final do arquivo cliente01.txt

  `echo "jaragua do sul" >>cliente01.txt`
  `less cliente01.txt`
  
#### **4 Problema**
Crie um novo diretório chamado clientes com o comando mkdir. Confira o
resultado com o comando ls.

   `mkdir clientes´
   `ls`
  
#### **5 Problema**
Mova o arquivo cliente 01.txt para o diret´orio clientes. Confira o resultado com
os comandos ls e cd.

  `mv cliente01.txt clientes`
  `cd clientes/`
  `ls`

#### **6 Problema**
Crie uma cópia do arquivo cliente 01.txt com o comando cp chamado cliente01.txt.bkp.
Confira o resultado.

`cp clientes01.txt clientes01.txt.bkp`
`ls`
`cliente           clientes.txt      clientes.txt.bkp`

#### **7 Problema**
Remova o arquivo cliente 01.txt com o comando rm. Confira o resultado.

  `rm clientes01.txt`
  `ls`
  `cliente           clientes01.txt.bkp`
  
#### **8 Problema**
Crie um arquivo chamado de cliente.script com todos os comandos utilizados
acima, na mesma ordem de execução.
  
    #!/usr/bash

    nome="Ana";echo $nome

    echo "ana" > cliente01.txt
    less cliente01.txt

    mkdir clientes
    ls

    mv cliente01.txt clientes
    cd clientes/
    ls

    cp clientes01.txt clientes01.txt.bkp`
    ls

    rm clientes01.txt
    ls


  
#### **9 Problema**
Modifique o arquivo cliente.script com o comando chmod para se tornar um
arquivo executável. Execute o arquivo e confira o resultado. Para executar utilize o comando ./cliente.script. Obs: exclua a pasta clientes antes de executar
o script para garantir que está funcionando corretamente.

`chmod +x clientes.script` `rm -r clientes` `./clientes.script`

#### **10 Problema**
Execute o comando cal. Observe o resultado. Execute o comando echo|cal >
hoje.txt. Utilize o comandos ls e less para conferir o resultado. O que ocorreu?
Qual a função do operador — ?

`cal`

aparece o calendário

`echo|cal > hoje.txt`
`ls`

dos       hello.c   hoje.txt

a função do operador é filtrar. 

#### **11 Problema**
Utilize o comando wget para baixar o arquivo cidades sc.txt no endere¸co https:
//gist.githubusercontent.com/leandersonandre/c8cba982f42262591be628e5397d1c3f/
raw/bd13a3e13823708e477f99f9285f845b292714c6/cidades_sc.txt.

`wget https://gist.githubusercontent.com/leandersonandre/c8cba982f42262591be628e5397d1c3f/raw/bd13a3e13823708e477f99f9285f845b292714c6/cidades_sc.txt`

#### **12 Problema**
Execute o comando grep Balneario cidades sc.txt. Qual é o resultado?

`grep Balneario cidades_sc.txt`

    Balneario Arroio do Silva
    Balneario Barra do Sul
    Balneario Camboriu
    Balneario Gaivota

#### **13 Problema**
Execute o comando grep Balneario cidades sc.txt. Qual é o resultado?

`grep balneario cidades_sc.txt`

não retorna valor nenhum, porque o arquivo está no padrão camelCase. 

#### **14 Problema**
Execute o comando grep ”do Sul”cidades sc.txt. Qual é o resultado?

`grep "do Sul" cidades_sc.txt`

    Balneario Barra do Sul
    Bocaina do Sul
    Campo Belo do Sul
    Caxambu do Sul
    Cocal do Sul
    Formosa do Sul
    Guaruja do Sul
    Jaragua do Sul
    Lindoia do Sul
    Rio do Sul
    Santa Rosa do Sul
    Santiago do Sul
    Sao Bento do Sul
    Sao Cristovao do Sul
    Sao Francisco do Sul
    Sao Joao do Sul
    Timbe do Sul
    
#### **15 Problema**
Utilize os os comandos cat e grep para filtrar as cidades que coemaçam com o nome Balneario

`cat cidades_sc.txt | grep Balneario`

    Balneario Arroio do Silva
    Balneario Barra do Sul
    Balneario Camboriu
    Balneario Gaivota

#### **16 Problema**
Crie um arquivo chamado balneario.txt com o conteúdo filtrado no problema
15.

`cat cidades_sc.txt | grep Balneario > balneario.txt`

#### **17 Problema**
Compacte o arquivo balneario.txt, nomeando de compactado.tar com o comando tar.

`tar -c balneario.txt > compactado.tar`

#### **18 Problema**
Descompacte o arquivo compactado.tar com o comando tar.

`tar -xf compactado.tar`
