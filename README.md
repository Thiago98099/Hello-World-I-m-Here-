# Hello-World-I-m-Here-
This is my first step



algoritmo  "Desafio 1"

Var
Ano : Inteiro
Salario : real
Aumento : real


Inicio

Ano <- 2005
Salario <- 1000
Aumento <- 15

Enquanto Ano < 2018 faca
Ano <- Ano + 1
Salario <- Salario + Aumento
Aumento <- Aumento * 2
fimenquanto

escreval ("Ano: ",Ano)
escreval ("Salario atual: R$",Salario,",00")


fimalgoritmo



----------------------------------------------------------------------------------------------




algoritmo    "Desafio 2"

Var
num1, num2 : inteiro
a, b, c : inteiro

Inicio

escreval ("Digite o primeiro número primo")
leia(num1)

    enquanto (num1 <=0) faca
             escreval("O primeiro número deve ser maio que zero")
             escreval("Digite novamente")
             leia(num1)
    fimenquanto
    
escreval ("Digite o segundo número primo")
leia(num2)

 enquanto num1 > num2 faca
          limpatela
          escreval("O primeiro numero deve ser menor que o segundo numero")
          escreval("Digite novamente o segundo numero")
          leia(num2)
 fimenquanto

  para a de num1 ate num2 faca
      c <- 0

       para b de 1 ate a faca
            se (a mod b=0) entao
            c <- c + 1
            fimse
       fimpara

       se (c=2) entao
          escreva (a)
       fimse
  fimpara
Fimalgoritmo



----------------------------------------------------------------------------------------------



algoritmo   "Desafio 3"

Var
sal, hr : real
salt, liqui : real

Inicio

escreval ("Informe as horas trabalhadas")
leia(hr)
escreval ("informe o salario minimo")
leia(sal)

salt <- (sal*0.1)+sal
liqui <- salt-(salt*0.03)

limpatela
escreval ("O salario liquido a receber e: R$",liqui:1:2)
Fimalgoritmo



------------------------------------------------------------------------------




Algoritmo "Desafio 4"

Var

mtsQ, lataL : real
tintaM, valor, lata : real
a : inteiro

Inicio

valor <- 80

escreval ("Me informe a area em metros quadrados")
leia (mtsQ)


lataL <- mtsQ / 3
lata <- lataL / 18

lata <- int(lata)

   se (lata < 1) entao
   lata <- 1
   escreval(lata," Lata. No valor total de R$", valor)
   senão
   valor <- lata * valor
escreval(lata:1:0," Latas. No valor total de R$", valor:2:2)
   fimse



Fimalgoritmo



---------------------------------------------------------------------------------------------------




algoritmo "Desafio 5"

var

nome, conta : caracter
verificar : inteiro
saldo : real
retornar : inteiro
opcao : inteiro
retorno : logico
depositoV, saqueV : real
flag : inteiro
saida : inteiro


inicio

saldo <- 0


procedimento laco
inicio

  se (retorno = verdadeiro) entao
  menuP
  fimse
fimprocedimento

procedimento menu
  inicio

limpatela
escreval ("Informe seu nome")
leia (nome)
escreval ("Informe seu numero de conta")
leia (conta)
limpatela
menuP
fimprocedimento

procedimento verificarsaldo
  inicio

limpatela
escreval ("Saldo disponível: R$", Saldo)
escreval ("digite 1 para voltar para o menu")
leia(retornar)
    se (retornar = 1) entao
     retorno <- verdadeiro
    fimse
    laco
fimprocedimento

procedimento realizarDep
  inicio

limpatela
escreval("Informe o valor a ser depositado")
leia(depositoV)
  se (depositoV > 0) entao
     saldo <- saldo + depositoV
  senao
    escreval("Informe um valor maior que 0")
    leia(flag)
     realizarDep
  fimse
escreval("Deposito realizado com sucesso")
escreval("Novo saldo: R$", saldo:1:2)
escreval(" ")
escreval("Digite 1 para voltar ao menu")
leia(retornar)
 se (retornar = 1) entao
      retorno <- verdadeiro
     fimse
     laco
fimprocedimento

procedimento saque
inicio

limpatela
  escreval("Informe o valor desejado para saque")
  leia (saqueV)
       se (saqueV > saldo) entao
       escreval("O saque nao deve ultrapassar o valor do saldo")
       leia(flag)
       saque
       fimse
  saldo <- saldo - saqueV
  escreval("Saque realizado com sucesso!")
  escreval(" ")
  escreval("Novo saldo R$", saldo)
  escreval(" ")
  escreval("Digite 1 para voltar ao menu")
      leia(retornar)
      se (retornar = 1) entao
          retorno <- verdadeiro
      fimse
     laco
  
fimprocedimento

procedimento alterarNome
inicio

limpatela
   escreval("Qual seria o nome novo?")
   leia(nome)
    escreval("Digite 1 para voltar ao menu")
      leia(retornar)
      se (retornar = 1) entao
          retorno <- verdadeiro
      fimse
     laco
fimprocedimento

procedimento encerrar
inicio

limpatela
escreval("Gostaria de sair?")
escreval("1-Sim 2-Nao")
leia(saida)
    se (saida = 2) entao
    menuP
    senao
    fimalgoritmo
    fimse

fimprocedimento


procedimento menuP
inicio

retornar <- 0
limpatela
escreval("Bem vindo ", nome,"  C/C: ", conta)
escreval("Este é o menu, o que gostaria de fazer?")
escreval("1-Verificar saldo")
escreval("2-Deposito")
escreval("3-Saque")
escreval("4-Alterar nome")
escreval("5-Sair")
leia(opcao)
opcaoescolha
fimprocedimento

procedimento opcaoescolha
inicio
escolha opcao

caso 1
verificarsaldo

caso 2
realizarDep

caso 3
saque

caso 4
alterarnome

caso 5
encerrar

outrocaso
escreval("opcao invalida")
fimprocedimento

menu


fimalgoritmo



--------------------------------------------------------------------------------------------------------




algoritmo "Desafio 6"


var

x, y, Px, Py : real
PmetrosQ, metrosQ : real
perimetro : real
pisos : real
validar, validarP : inteiro
quantPisos : real
retorno : real


inicio

procedimento medida
inicio

limpatela
escreval("Informe a medida do local desejado")
leia(x)
leia(y)
limpatela

escreval("Confirma dados? Digite 1 para redigitar as medidas")
escreval(x," X ",y)
leia(validar)

   se (validar = 1) entao
   medida
   fimse
   calculopiso
fimprocedimento

procedimento calculopiso
inicio

limpatela
escreval("Me informe a medida do piso para te informar a quantidade do mesmo")
leia(Px)
leia(Py)
escreval("Confirma dados? Digite 1 para redigitar as medidas")
escreval(Px," X ",Py)
leia(validarP)

   se (validarP = 1) entao
   calculopiso
   fimse
   resultado
fimprocedimento

procedimento resultado
inicio

limpatela
perimetro <- x + y
metrosQ <- x * y
PmetrosQ <- Px * Py
QuantPisos <- metrosQ / PmetrosQ

escreval("Quantidade necessaria de metro de rodape:", perimetro)
escreval("Quantidade de pisos necessaria conforme a medida informada:")
escreval(QuantPisos," Pisos")
escreval(" ")
escreval ("Gostaria de refazer? Digite 1 para refazer")
leia(retorno)

se (retorno = 1) entao
   medida
senao
fimalgoritmo
fimse
fimprocedimento
medida
