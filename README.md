# Programmation statistique - S2 - Rstudio

# TD1 - Exo 1

a <- 10
b <- 5

resultat <- a * b
print(resultat)

A = 7.2
B = 10.1
#R est sensible à la casse

resultat = A * B
print(resultat)
#resultat se met à jour et prend la dernière valeur qui lui est attribué

rm(a,b,A,B,resultat)
#possible d'utiliser rm(list = ls())

# TD1 - Exo 2

vecteur = c(1,2,3,4,5)
class(vec_1)
vec_1[3]

v1 = 1:5
v2 = 3+v1
v3 = 1:6
v4 = v3^2
v5 = v4/2

semaine = c("lundi", "mardi", "mercredi", "jeudi",
              "vendredi", "samedi", "dimanche")
class(semaine)
semaine[c(2,7)]
#pour afficher plusieurs valeurs à la fois
#mettre le c(indice, indice) dans les crochets

bool = c(TRUE, FALSE, TRUE, FALSE)
class(bool)

num = c(1.5, 2.5, 3.5, 4.5, 5.5, 6.5)
class(num)
num[-3]
#pour afficher tous les éléments 
#sauf celui d'un élément spécifique 
#-> mettre un -indice

mois = c("janvier", "février", "mars", 
         "avril", "mai", "juin", 
         "juillet", "août", "septembre", 
         "octobre", "novembre", "décembre")
class(mois)
mois[c(1,2,3)]

#faire le 10
