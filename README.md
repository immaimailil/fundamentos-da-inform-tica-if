DESAFIO 1: A Calculadora (Revisão)
Objetivo: Calcular a expressão (100 + 50 - 30) * 2 / 10.
Arquivo: Salve como desafio1_calculadora.sbl.
Calculadora Aritmética
LOAD 100
ADD 50
SUB 30
STORE BX
LOAD 2
MUL BX
DIV 10
STORE CX
MUL 2
STORE CX
HLT

DESAFIO 2: O Porteiro Digital (Lógica Condicional)
Objetivo: Criar um programa que verifica se um número é igual a 18. Se for, ele deve parar com o valor 1 no registrador AX (indicando "permitido"). Se não for, deve parar com o valor 0 (indicando "negado").
Arquivo: Salve como desafio2_porteiro.sbl.
Novos Comandos:
CMP valor: Compara o valor em AX com valor. Se forem iguais, o Zero Flag (Z) é ativado (vai para 1).
JZ linha: Jump if Zero. Pula para a linha especificada SE o Zero Flag estiver ativado.
Verificador de Idade (18 anos)
LOAD 18
CMP 18

JZ 8

LOAD 0
HLT

LOAD 1
HLT

DESAFIO 3: A Contagem Regressiva (Loop Simples)
Objetivo: Criar um programa que começa em 5 e conta para trás até chegar a 0.
Arquivo: Salve como desafio3_contagem.sbl.
Novos Comandos:
DEC registrador: DECrementa (subtrai 1) do valor no registrador.
JMP linha: JuMP. Pula incondicionalmente para a linha especificada.
Contagem Regressiva de 5 a 0
LOAD 5 

DEC AX 
CMP 0
JZ 7
JMP 2

HLT
