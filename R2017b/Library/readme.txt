Date : 21/07/2020
Auteur : Antoine Bruy�re
Objet : Demande de modification sur les mod�les g�n�riques 

Fichiers impact�s :
- Control_Lib.slx (Matlab version R2020a)
- GFo_Lib.slx (Matlab version R2020a)

Autres fichiers remis dans l'archive zip :
- {GFo_Dev.slx ; init.m ; LoadFlow_VSC.m} : permet de tester les mod�les modifi�s
- {Control_Lib_R2017b.slx ; GFo_Lib_R2017b.slx} : fichiers impact�s sous la version Matlab R2017b
 

Description des changements :

1. Control_Lib.slx :

a. Ajout mod�les de transformation de Park g�n�riques, permettant de choisir l'axe de r�f�rence et le gain de normalisation en per-unit

b. Ajout mod�le modifi� de PLL, qui reprend les transformations de Park g�n�riques

c. Calcul du cosinus et sinus de l'angle � l'endroit o� l'angle est produit.



2. GFo_Lib.slx : 

a. L-Filter mod�le : int�gration des modifications de la librairie Control_Lib.slx au mod�le de convertisseur VSC avec filtre L
   Tests de non r�gression : OK

b. LCL-Filter : int�gration des modifications de la librairie Control_Lib.slx au mod�le de convertisseur VSC avec filtre L
   ATTENTION : le mod�le n'a pas pu �tre etst� car les modifications ont �t� faites sur un mod�le qui ne fonctionnait pas (probl�me de masque sur filtre LC)
   

