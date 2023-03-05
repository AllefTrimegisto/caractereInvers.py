# caractereInvers.py
 Escreva um programa que inverta os caracteres de um string.



IMPORTANTE:

a) Essa string pode ser informada através de qualquer entrada de sua preferência ou pode ser previamente definida no código;

b) Evite usar funções prontas, como, por exemplo, reverse;
# Recebe a string a ser invertida
string = input("Digite uma string: ")

# Converte a string em uma lista de caracteres
lista_caracteres = list(string)

# Inverte a ordem dos caracteres na lista
for i in range(len(lista_caracteres) // 2):
    lista_caracteres[i], lista_caracteres[len(lista_caracteres) - i - 1] = lista_caracteres[len(lista_caracteres) - i - 1], lista_caracteres[i]

# Converte a lista de volta para uma string
string_invertida = ''.join(lista_caracteres)

# Imprime a string invertida
print("String invertida:", string_invertida)
