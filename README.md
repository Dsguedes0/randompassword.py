# randompassword.py

import random
import string

def generate_password(length=12):
    all_characters = string.ascii_letters + string.digits + string.punctuation
    
    senha = "".join(random.choice(all_characters) for _ in range(length))
    
    return senha
    
    length = int(input("a quantidade de caracteres da minha senha sera:"))
    
    senha = generate_password(length)
    print("Senha Gerada", senha)
