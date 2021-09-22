# Python para iniciantes


##### Aqui aprenderemos de maneira intuitiva, objetiva, e rápida a programar em python

O que aprenderemos: 
   * [Instalção](#Instalação)
   * [Configuração](#Configuração)
   * [Primeiro Programa](#PrimeiroPrograma)
   * [Comentários](#Comentarios)
   * [Nível iniciante](#NívelINiciante)
       * [Variáveis](#Variáveis)
   * [Nível intermediário](#NívelIntermerdiário)       
       * [If e Else](#IfeElse)
   * [Nível avançado](#NívelAvançado)   
        * [Funções](#Funções)
        * [Loops](#Loops)
   * [CódigoBônus](#CódigoBônus)

## Instalação


Tutorial para instalação


https://python.org.br/instalacao-windows/


Download do Python versão 3.9.7

https://www.python.org/downloads/


### Etapas realizadas
[x] Instalação
[ ] Configuração
[ ] Primeiro programa
[ ] Comentários
[ ] Variáveis
[ ] If e Else
[ ] Loops
[ ] Código bônus
## Configuração 

Vídeo explicativo sobre a instalação do PyCharm 

https://www.youtube.com/watch?v=HNUq8X_0nlM

Configurando e instruindo como utilizar o PyCharm

https://www.jetbrains.com/help/pycharm/creating-and-running-your-first-python-project.html

### Etapas realizadas
[x] Instalação
[x] Configuração
[ ] Primeiro programa
[ ] Comentários
[ ] Variáveis
[ ] If e Else
[ ] Loops
[ ] Código bônus
# Primeiro programa

Mostraremos a seguir instruções de como realizar seu primeiro programa! 🙌

Escreva o código : 
```sh
print('Olá, mundo!')
```

Veja o código acessando também 

https://blog.betrybe.com/desenvolvimento-web/hello-world-ola-mundo/

### Etapas realizadas
[x] Instalação
[x] Configuração
[x] Primeiro programa
[ ] Comentários
[ ] Variáveis
[ ] If e Else
[ ] Loops
[ ] Código bônus
# Comentários

Aprenderemos agora algumas formas de utilizar o comentário em pyhton

Notação Inline
```sh
print(teste) #a instrução atrás da cerquilha será interpretada
```
Notação Multilines
```sh
'''
toda informações contida entre 3 aspas SIMPLES
é considerada como caracteres que devem ser ignorados.
'''
```
Para mais informações acesse
http://excript.com/python/comentarios-em-python.html

### Etapas realizadas
[x] Instalação
[x] Configuração
[x] Primeiro programa
[x] Comentários
[ x] Variáveis
[ ] If e Else
[ ] Loops
[ ] Código bônus

# Variáveis

Realizaremos agora a utilização de  variáveis em Python:
variável = expressão
```sh
'''
Exemplos:
k = 0  #k recebe o valor 0
a = 1 
A = 2
c = k + a + A   #c recebe os valores da soma de k, a e A
'''
```
Vale ressaltar que há distinção entre maiúsculo e minúsculo, como mostrado acima.

Para mais informações, acesse:
https://panda.ime.usp.br/panda/static/aulasPython/aula02.html

### Etapas realizadas
[x] Instalação
[x] Configuração
[x] Primeiro programa
[x] Comentários
[x] Variáveis
[ ] If e Else
[ ] Loops
[ ] Código bônus
# If e Else
Visualizaremos a seguir as atribuições de IF, ELIF, ELSE:
Para o IF
```sh
b = 300
A = 200
if A > b:     #Condição IF
    print("A é maior do que b") 
  ```
O ELIF (ELSE + IF) é uma condição similar ao ELSE, entretando, ele necessita que seja transcrita outra condição em sequência (IF).
```sh
b = 300
A = 200
if A > b:       #Condição IF
    print("A é maior do que b") 
  
elif A == b:      #Confição ELIF, caso não entre no primeiro IF
    print("A é igual a b")
  ```

 Para o ELSE
```sh
b = 300
A = 200
if A > a:            #Condição IF
    print("A é maior do que b") 
  
elif A == a:         #Condição ELIF
    print("A é igual a b")

else:                #Condição ELSE
    print("A é menor a b")
  ```
  
  Para mais informações, técnicas e conceitos sobre, acesse: 
  https://www.w3schools.com/python/python_conditions.asp
  
  ### Etapas realizadas
[x] Instalação
[x] Configuração
[x] Primeiro programa
[x] Comentários
[x] Variáveis
[x] If e Else
[ ] Loops
[ ] Código bônus

# Loops

Agora veremos as estruturas de repetição, for, while, e while true: 

For
```sh
for i in range(5):
    print(i)
  ```
 While
 ```sh
 count = 0
while count <= 5:
    print(count)
    count += 1
  ```
While True
 ```sh
while True:
   print('foo')
  ```
 Para mais informações sobre as estruturas de repetições estudadas, acesse: 
 http://devfuria.com.br/python/lacos-de-repeticao/
 https://realpython.com/python-while-loop/
  ### Etapas realizadas
[x] Instalação
[x] Configuração
[x] Primeiro programa
[x] Comentários
[x] Variáveis
[x] If e Else
[x] Loops
[ ] Código bônus

# Código bônus
 Nessa parte iremos mostrar um pouco do que é possivel se fazer com a linguagem python.
 ```sh
 Jogador = dict()  # criação de um dicionário
Todos = list()    # criação de uma lista
Gols = list()     # criação de uma lista

while True:         # Loop infinito
    Jogador.clear()  # Limpa tudo que está dentro do dicionário Jogador

    Jogador['Nome'] = str(input('Nome do Jogador: ')).strip()   # Adiciona à chave Nome do dicionário Jogador, um valor que o usuário fornece
    # Função strip é usada para retirar espaços tanto do inicio tanto do fim.

    part = int(input(f'Quantas partidas {Jogador["Nome"]} Jogou? ')) # A variavél part recebe um valor inteiro fornecido pelo usuário

    for c in range(part): # Loop for com um tamanho de part, que foi fornecido pelo usuário
        Gols.append(int(input(f' Quantos Gols na partida {c+1}? ')))    # Adiciona na lista Gols um valor fornecido pelo usuário
    Jogador['Gols'] = Gols[:]   # Faz uma cópia da lista Gols para o dicionário com a chave Gols

    Jogador['Total'] = sum(Gols)    # Adiciona na chave do dicionário Jogador Total o somatório da lista gols

    Todos.append(Jogador.copy())    # A lsita Todos recebe uma copia de todo dicionário Jogador

    Gols.clear() # Limpa a lista Gols
    while True:
        opção = str(input('Quer continuar? [S/N] ')).strip().upper()[0]
        if opção in 'SN':   # Condição if que verifica se S ou N está dentro da variavel opção
            break
        else:
            print('ERRO! Digite Somente S ou N')
    if opção == 'N':    # Condição de parada para o cadastramento de jogadores
        break

print('-='*30)
print('-'*40)
print('cod ', end='')
for i in Jogador.keys():    # loop nas chaves do dicionário
    print(f'{i:<15}', end='')
print()
print('-'*40)
for k, v in enumerate(Todos):   # Loop com enumeração dos valores que estão dentro da lista Todos
    print(f'{k+1:>3} ', end='')
    for d in v.values():
        print(f'{str(d):<15}', end='')
    print()
while True:
    busca = int(input('Mostrar dados de qual jogador? (999 para parar)')) - 1
    if busca == 999:
        break
    if busca >= len(Todos) or busca < 0:
        print(f'Erro! Não existe jogador com código {busca+1}!')
    else:
        print(f'-- LEVANTAMENTO DO JOGADOR {Todos[busca]["Nome"]}')
        for c, k in enumerate(Todos[busca]["Gols"]):
            print(f' No jogo {c+1} fez {k} gols.')
    print('-'*40)
print('<<Volte Sempre!>>')


 ```
 
