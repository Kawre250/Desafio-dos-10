"""
_from_random_import_randint é uma instrução em Python que importa uma função chamada randint do módulo random.
A função randint é usada para gerar números aleat  órios inteiros dentro de um intervalo especificado.
Ao importar a accfunção randint usando from_random_import_randint, podemos usá-la diretamente em nosso código sem precisar usar o prefixo random antes dela, o que torna o código mais fácil de ler e digitar.
"""
from random import randint

#Imprimir nome do desafio---------------
print('⚡⚡ Iníciando o DESAFIO⚡⚡')

#Variáveis------------------------------
def acerte_o_numero():
    aleatorio = randint(0, 10)
    chute = 0
    chances = 5
    pontua_max = 100
    pontua_min = 10

#começo de jogo ------------------------
    while chute != aleatorio:
        chute = input('Chute um número entre 0 a 10: ')


        try:
            chute = int(chute)
        except ValueError: 
            print("Digite apenas números!")
            continue
        
        if int(chute) < 0 or int(chute) > 10:
            print("Digite um número entre 0 e 10!!!!!!!!!!!!!!")
            continue
        
        chances = chances - 1

        if chute == aleatorio:
            print('Parabéns, você venceu! O número era {} e você ainda tinha {} chances.'.format(aleatorio, chances))
            if chances == 5:
                pts = pontua_max
            else:
                pts = pontua_min * chances
            print("Sua pontuação foi de", pts, "pontos")
            break;
        
        else: 
            if chute > aleatorio:
                print('Você errou!!! Dica: É um número menor.')
            else:
                print('Você errou!!! Dica: É um número maior.')
                print(f'Você ainda possui {chances} chances.')

#Fim de Jogo ----------------------------------
            
            if chances == 0:
                print('Suas chances acabaram, você perdeu!')
                break;
                
#Nova Partida ----------------------------------

    nova_partida = input("Deseja jogar novamente? (s/n)")
    if nova_partida == "s":
        acerte_o_numero()
    else:
        print("Obrigado por jogar!")

acerte_o_numero()
