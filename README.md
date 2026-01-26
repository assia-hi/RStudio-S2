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

# TD1 - Exo 3

rm(list=ls())

vec_1 = runif(n=5,min=0,max=1)
vec_1
mean(vec_1)
median(vec_1)
min(vec_1)
max(vec_1)

seq_1 = runif(10, -5, 5)
seq_1
mean(seq_1)
median(seq_1)
min(seq_1)
max(seq_1)

ech_1 = runif(100, 10, 20)
ech_1
mean(ech_1)
median(ech_1)
min(ech_1)
max(ech_1)

seq_2 = runif(15, 50, 100)
seq_2
mean(seq_2)
median(seq_2)
min(seq_2)
max(seq_2)

ech_2 = rnorm(20,-2,3)
moyenne = mean(ech_2)
ecart_type = sd(ech_2)
print(paste("moyenne : ", moyenne))
print(paste("ecart-type : ", ecart_type))
hist(ech_2)

ech_3 = rnorm(2000, 0, 1)
ech_3_moyenne = mean(ech_3)
ech_3_sd = sd(ech_3)
print(paste("moyenne : ", ech_3_moyenne))
print(paste("ecart-typde : ", ech_3_sd))
hist(ech_3)

quantile(ech_3, c(0.25))
quantile(ech_3, c(0.50))  
quantile(ech_3, c(0.75))
