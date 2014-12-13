def saisi() :
    global y
    global x
    global plateau
    y = eval(input("Saisissez un nombre de lignes : "))
    x = eval(input("Saisissez un nombre de colonnes : "))
    plateau = [[True]*x for i in range(y)] 
    
def setplateau() :
       
    for ligne in plateau:
        for elements in ligne:
            if elements == True:
                print("O",end="   ")
            else:
                print("X", end="   ")
        print("\n")



def choixcase():
        
    n = eval(input("Saisissez le numero de la ligne : "))
    m = eval(input("Saisissez le numero de la colonne : "))

    if n > x :
        return choixcase()
    elif m > m :
        return choixcase()

    else :
        for a in range(3):
            for b in range(3):
                c = n-1+a
                d = m-1+b
                
                if c == n and d == m :
                    plateau[c][d] = plateau[c][d]

                elif c >= 0 and c < x and d >= 0 and d < y :
                    plateau[c][d] = not(plateau[c][d])

             
def checkvic():
    w = 0
    for ligne in plateau:
        for elements in ligne:
            if elements is True:
                w += 1

    if w == 0 :
        return False
    else :
        return True
                
            
def continu():
    z = eval(input("Voulez vous continuer ? 1 pour oui, 0 pour non : "))
    if z == 0 :
        print("Vous êtes faible ...")

    elif z == 1 :
        return True

    else :
        print("What the fuck ?")
        return continu()


def main() :
    
    
    
    choixcase()
    setplateau()
    if checkvic() is False :
        print("C'est gagné !")
    else :
        if continu() is True :
            return main()

saisi()
setplateau()
main()
