# Mysql console

## Se connecter
* Connectez-vous à l'aide du terminal à Mysql en tant que root 

```
mysql -u root -p

```
* Entrez votre mot de passe,
  Vous êtes, maintenant, prêt à communiquer avec le système de gestion de base de données
  
## Tester quelques commandes
* Afficher toutes les bases de données
 ```
 SHOW DATABASES;
 
 ```
 * Sélectionner une base de données pour agir dessus
  ```
  USE NomDeLaBase;
  
  ```
 
* Afficher une table de la base de données sélectionnée
 ```
 SHOW TABLE;
 
 ```
* Créer une base de données 
```
 CREATE DATABASE NomDeLaBase;
 
 ```
* Créer une table 
```
 CREATE TABLE NomDeLaTable(
 NomChamp1 type(taille),
 NomChamp2 type(taille)
 ... )
 ```
* Supprimer une base de données ou une table
```
 DROP DATABASE NomDeLaBase;
 DROP TABLE NomDeLaTable;
 
 ```
* Sélectionner tout d'une table ou un champ
```
 SELECT * FROM NomDeLaTable;
 SELECT NomDuChamp FROM NomDeLaTable;
 
 ```
* Sélectionner tout d'une table où un champ a une valeur donnée 
```
 SELECT * FROM NomDeLaTable WHERE NomDuChamp = valeur;
  
 ```
* Sélectionner tout d'une table ou un champ
```
 SELECT * FROM NomDeLaTable;
 SELECT NomDuChamp FROM NomDeLaTable;
 
 ```
*Les autres commandes sont à chercher...* 



## Exercice

* Créer la base de donnée **analyse**
* Créer la table **frequence** composée des champs suivants

 | Champ |Type|
 |---|---|
 | prenom | varchar(50) |
 | nom | varchar(50) |
 | compteurVisite | smalint |
 | derniereVisite | timestamp |
 
* Afficher la structure de la table **frequence**
* Ajouter les valeurs suivantes :
```
Pierre, Tombal, 34, NOW()
Jean, Tanrien, 128, NOW()
Agathe, Zeblouse, 25, NOW()
Eva, Pauré, 98, NOW()
Justin, Petipeu, 56, NOW()
Nordine, Ateur, 64, NOW()
Yves, Remord, 102, NOW()
Sam, Fechier, 45, NOW()

```
* 1 - Lister les données contenues dans la table **frequence**
* 2 - **Affecter** la valeur **200** au champ **compteurVisite** de **Jean Tanrien**
* 3 - **Supprimer** l'enregistrement de **Nordine Ateur**
* 4 - **Compter** le nombre d'enregistrements dans la table **frequence**
* 5 - Afficher les enregistrements par **ordre alphabétique** 
* 6 - Afficher les enregistrements dont le nombre de visite est **supérieur à 50**
