# Pedra-Papel-e-Tesoura---Python
from time import sleep
import random

lista = ('PEDRA', 'PAPEL', 'TESOURA')
print('PEDRA, PAPEL, TESOURA')
print('*'*40)
sleep(1)
valor = int(input('Digite o número correspondente ao que deseja \n [1] PEDRA \n [2] PAPEL \n [3] TESOURA \n DIGITE AQUI SUA PREFERÊNCIA: '))

pc = random.choice(lista)
sleep(1)

if valor == 1:
    print('Você escolheu PEDRA!')
    sleep(1)
    print('Eu escolho {}!'.format(pc))
    sleep(1)
    val = 'PEDRA'
    if val == pc:
        print('Empate!')
    elif val == 'PEDRA' and pc == 'TESOURA' or val == 'TESOURA' and pc == 'PAPEL' or val == 'PAPEL' and pc == 'PEDRA':
        print('Você venceu!')
    else:
        print('Você perdeu!')
elif valor == 2:
    print('Você escolheu PAPEL!')
    sleep(1)
    print('Eu escolho {}!'.format(pc))
    sleep(1)
    val = 'PAPEL'
    if val == pc:
        print('Empate!')
    elif val == 'PEDRA' and pc == 'TESOURA' or val == 'TESOURA' and pc == 'PAPEL' or val == 'PAPEL' and pc == 'PEDRA':
        print('Você venceu!')
    else:
        print('Você perdeu!')
elif valor == 3:
    print('Você escolheu TESOURA!')
    sleep(1)
    print('Eu escolho {}!'.format(pc))
    sleep(1)
    val = 'TESOURA'
    if val == pc:
        print('Empate!')
    elif val == 'PEDRA' and pc == 'TESOURA' or val == 'TESOURA' and pc == 'PAPEL' or val == 'PAPEL' and pc == 'PEDRA':
        print('Você venceu!')
    else:
        print('Você perdeu!')
else:
    print('Valor inválido.')

