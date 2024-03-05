# UNIFOR
**Disciplina** Raciocinio Logico Algoritmo
**Orientador:** Querido Prof. Ricardo Carubbi

## Lista de exercicios
 
### Exercicio 03
Represente, em fluxograma e pseudocódigo, um algoritmo para determinar se um ==numero inteiro e positivo e par ou impar==

#### Fluxograma
```mermaid 
flowchart TD
A([INICIO]) --> B{{Digite um numero:}}
B --> C[numero]
C --> D{numero >= 0}
D --NAO--> E{{O numero deve ser positivo!}}
E --> Z([FIM])
D --SIM--> F[resto = numero % 2]
F --> G{resto == 0}
G --NAO--> H{{O numero é impar!}}
G --SIM--> I{{O numero e par!}}
H --> Z
I --> Z
```
### Pseudocodigo 
```
1  	ALGORITMO verificar_par_impar
2  	DECLARE numero, resto NUMERICO
3  	ESCREVA "Digite um numero: "
4  	LEIA numero
5  	SE numero >= 0 ENTAO
6		resto <-  numero % 2
7		SE resto == 0 ENTAO 
8			ESCREVA "O numero é par!"
9		SENAO
10			ESCREVA "O numero é impar!"
11	SENAO
12		ESCREVA " O numero deve ser positivo"
13	FIM_ALGORITMO	
```
