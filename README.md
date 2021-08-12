# emprestimo.python
Desafio 036 (Curso em vídeo) Escreva um programa para aprovar o empréstimo bancário para a compra de uma casa. Pergunte o valor da casa, o salário do comprador e em quantos anos ele vai pagar. A prestação mensal, não pode exceder 30% do salário ou então o empréstimo será negadovalor = float(input('Qual é o valor da casa? R$'))#

#Programa em Python

salario = float(input('Qual é o salário do comprador? R$'))
anos = int(input('Em quantos anos ele pretende pagar? '))
prestacao = valor / (anos * 12)
porcento = float(30 * salario / 100)
print('Para poder realizar o empréstimo o valor não pode exceder à 30% do seu salário')
print('30% do seu salário é igual à R${:.2f} reais'.format(porcento))
print('O valor das prestações são de R${:.2f} reais em {} anos'.format(prestacao, anos))
if prestacao < porcento:
    print('Empréstimo \033[4;32mAPROVADO\033[m')
else:
    print('Infelizment o empréstimo foi \033[4;31mNEGADO\033[m')
    print('Com parcelas de R${:.2f} reais, o valor ultrapassou 30% do seu salário'.format(prestacao))

