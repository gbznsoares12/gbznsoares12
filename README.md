
#dasafio001:
print('ola mundo!')
#desafio002:
nome = input("Digite seu nome: ")
print(f'Olá {nome}! Seja bem-vindo!')
#desafio003:
n1 = int(input('digite um numero: '))
n2 = int(input('digite outro numero: '))
s = n1 + n2
print(f'A soma entre {n1} e {n2} é igual a: {n1 + n2}')
#desafio004:
a = input("digite algo:")
print('o tipo primitivo desse valor é',type(a))
print('so tem espaço?',a.isspace())
print('e um numero?',a.isnumeric())
print('e alfabetico?',a.isalpha())
print('e alfanumerico?',a.isalnum())
#desafio005:
a = int(input('Digite um valor: '))

print(f'Seu antecessor é {a-1} e seu sucessor é {a+1}!')
#desafio006:
n = int(input('Digite um número: '))
print(f'O dobro de {n} é {n*2}.\nO triplo é {n*3}\nA raiz quadrada é {n**(1/2):.2f}.')
#desafio007:
n1 = int(input("Primeira nota do aluno: "))
n2 = int(input("Segunda nota do aluno: "))
media = (n1 + n2)/2
print(f"A Media entre {n1} e {n2} e igual a {(n1+n2)/2}")
#desafio008:
medida = float(input('Uma distancia em metros: '))
mm = medida * 1000
cm = medida * 100
dm = medida * 10
dam = medida / 10
hm = medida / 100
km = medida / 1000
print('a media  de  {}m coresponde a \n{}km \n{}hm \n{}dam \n{:.0f}dm \n{:.0f}cm \n{:.0f}mm'.format(medida, km, hm, dam, dm, cm, mm))
#desafio009:
num = int(input('Digite um número para saber sua tabuada: '))
print('A tabuada de {} é: '.format(num))
a = 0
for i in range(1,11):
    a = a+1
    print('{} x {} = ' .format(num,a), num*i)
#desafio010:
real = float(input("Quanto de dinheiro você tem na conta? R$ "))
dolar = real / 5.07
print("Com R$ {:.2f} você pode comprar US {:.2f}".format(real, dolar))
#desafio011:
largura = float(input('Digite a largura da parede: '))
altura = float(input('Digite a altura da parede: '))
print(f'Sua parede tem a dimensão de {largura}x{altura} e sua área é de {largura*altura}m².')
print(f'Para pintar essa parede, você precisará de {largura*(altura / 2)}L de tinta.')
#desafio012:
preço = float(input("Qual é o preço do produto? "))
desconto = int(input("Qual o desconto do produto? "))
resultado = preço*desconto/100
print("O desconto será de {}".format(resultado))
#desafio013:
n1 = float(input('Digite seu salário R$'))
s = n1 + (n1 * 15 / 100)
print(f'O novo salário será: R${s:.2f}')
#desafio014:
c = float(input('informe a tempratura em °c:'))
f = ((9 * c) / 5) + 32
print('a temperatura de {}°c corresponde a {}ºf!'.  format(c, f))
#desafio015:
dias = int(input('quantos dias o carro foi alugado? '))
km = float(input('quantos km rodado? '))
pago = (dias * 60) + (km * 0.15 )
print('o total a pagar e de R$ {:.2f}'.format(pago))
#desafio016:
num = float(input('digite um valor:'))
print('o valor digitado foi {} e a sua porçao inteira e {}'.format(num, int(num)))
#desafio017:
import math
co = float(input('comprimento do cateto oposto: '))
ca = float(input('comprimento do cateto adijacente: '))
hi = math.hypot(co, ca)
print('a hipotenusa vai medir {:.2f}'.format(hi))
#desafio018:
from math import radians,sin,cos,tan
angulo = float(input('dgite o angulo que vc deseja: '))
seno = sin(radians(angulo))
print('o angulo de {} tem o seno de {:.2f}'.format(angulo, seno))
cosseno = cos(radians(angulo))
print('o angulo de {} tem o cosseno de {:.2f}'.format(angulo, cosseno))
tangente = tan(radians(angulo))
print('o angulo de {} tem o tangente de {:.2f}'.format(angulo,tangente))
#desafio019:
from random import choice
n1 = (input('primeiro aluno:'))
n2 = (input('segundo aluno:'))
n3 = (input('rerceiro aluno:'))
n4 = (input('quarto aluno:'))
lista = [n1 ,n2 ,n3 ,n4]
escolhido = choice(lista)
print('o esclhido foi {}'.format(escolhido))
#desafio020:
from random import shuffle
p = input('Digite o nome do 1° aluno: ')
s = input('Digite o nome do 2° aluno: ')
t = input('Digite o nome do 3° aluno: ')
q = input('Digite o nome do 4° aluno: ')
lista = [p, s, t, q]
emb = shuffle(lista)
print('A ordem de apresentação dos alunos é: {}'.format(lista))
#desafio022:
nome = str(input('digite seu nome completo:')).strip()
print('ananlizando seu seu nome...')
print('seu nome em maiusculas e {}'.format(nome.upper()))
print('seu nome em minusculas e {}'.format(nome.lower()))
print('seu nome tem ao todo {} letras'.format(len(nome)-nome.count(' ')))
print('seu primeiro nome tem {}letras'.format(nome.find(' ')))
#desafio023:
num = int(input('informe um numero: '))
n = str(num)
print('analizando o numero {}'.format(num))
print('unidade:{}'.format(n[3]))
print('dezena:{}'.format(n[2]))
print('centena:{}'.format(n[1]))
print('milhar:{}'.format(n[0]))
#desafio024:
nome=str(input("Introduza o nome da cidade:")).strip()
print("santo" in nome.lower())
#desafio025:
nome = str(input('Qual o seu nome? ')).strip()
print('Seu nome possui "SILVA"? {}'.format('SILVA' in nome.upper().split()))
#desafio026:
f = str(input('Digite uma frase: ')).strip().upper()
print('A letra "A" aparece {} vezes nessa frase'.format(f.count('A')))
print('A mesma letra aparece pela primeira vez na posição {}'
      ' e pela última na {}'.format(f.find('A')+1,f.rfind('A')+1))
#desafio027:
nome = input('Qual o seu nome completo? ')
m = nome.split()
print(f'Seu primeiro nome é {m[0]} e seu último nome é {m[-1]}')
#desafio028:
import random
pc = random.randint(0, 5)
vc = int(input('Digite um número de 0 a 5:'))
if pc==vc:
    print('Você ganhou!!!')
else:
    print('O PC ganhou!!!')
#desafio029:
vel = float(input('Qual a velocidade atual do carro?'))
if vel <= 80:
    print('Tenha um bom dia!Dirija com segurança!')
else:
    print('MULTADO! Você excedeu o limite permetido que é de 80km/h')
    print('Você deve pagar uma multa de R${:.2f}!'.format((vel - 80) * 7))
#desafio030:
número = int(input('me diga um número qualquer: '))
if número % 2 == 0:
    print(número,'é par.')
else:
    print(número,'é impar.')
#desafio031:
km = float(input('Qual a distância em (Km) você deseja percorrer? '))
if km <= 200:
    print('Sua passagem vai custar {} reais. '.format(km * 0.5))
else:
    print('Sua passagem vai custar {} reais. '.format(km * 0.45))
#desafio032:
import calendar
ano = int(input('Digite o ano: '))
ano6 = calendar.isleap(ano)
if ano6 is True:
    print(f'O ano de {ano} é bissexto')
else:
    print(f'O ano de {ano} não é bissexto')
#desafio033:
n1 = int(input('Primeiro valor: '))
n2 = int(input('Segundo valor: '))
n3 = int(input('Terceiro valor: '))

print(f'O menor valor digitado foi {min(n1,n2,n3)}')
print(f'O maior valor digitado foi {max(n1,n2,n3)}')
#desafio034:
salario = float(input('Digite o seu salário: '))
aumentom = (salario * (10/100)) + salario
aumentoM = (salario * (15/100)) + salario

if(salario > 1250):
    print(' Seu salário era R${:.2f} \n Com o aumento, seu salário passa a ser R${:.2f}'.format(salario, aumentom))
else:
    print(' Seu salário era R${:.2f} \n Com o aumento, seu salário passa a ser R${:.2f}'.format(salario, aumentoM))
#desafio035:
l1 = float(input("Digite a medida do lado 1 do triângulo: "))
l2 = float(input("Digite a medida do lado 2 do triângulo: "))
l3 = float(input("Digite a medida do lado 3 do triângulo: "))

if (l1 + l2 > l3) and (l2 + l3 > l1) and (l1 + l3 > l2):
    print("Com esses lados, é possivel formar um triângulo.")
else:
    print("Não é possível formar um triângulo.")
