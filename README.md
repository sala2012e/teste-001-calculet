# teste-001-calculet
un html   de algoritme pour les math 
 Algorithme Calculatrice - Numéro 001 salah
# Ce programme effectue des opérations mathématiques de base

def calculatrice(question):
    question = question.lower().replace(" ", "")
    if "+" in question:
        a, b = question.split("+")
        return float(a) + float(b)
    elif "-" in question:
        a, b = question.split("-")
        return float(a) - float(b)
    elif "*" in question:
        a, b = question.split("*")
        return float(a) * float(b)
    elif "/" in question:
        a, b = question.split("/")
        if float(b) == 0:
            return "Division par zéro impossible"
        return float(a) / float(b)
    else:
        return "Je ne suis pas fait pour ça"

if __name__ == "__main__":
    print(calculatrice("5 + 3"))      # 8.0
    print(calculatrice("10 - 2"))     # 8.0
    print(calculatrice("4 * 2.5"))    # 10.0
    print(calculatrice("9 / 3"))      # 3.0
    print(calculatrice("il est quelle heure"))    # Je ne suis pas fait pour ça
    print(calculatrice(-12 * -7))      #+5.0
