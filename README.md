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
Utilize o comando echo para salvar o nome da cidade em que vocˆe nasceu no
final do arquivo cliente01.txt

  `echo "jaragua do sul" >>cliente01.txt`
  `less cliente01.txt`
  
#### **4 Problema**
Crie um novo diret´orio chamado clientes com o comando mkdir. Confira o
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
Crie uma c´opia do arquivo cliente 01.txt com o comando cp chamado cliente01.txt.bkp.
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
acima, na mesma ordem de execu¸c˜ao.
  
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

  

