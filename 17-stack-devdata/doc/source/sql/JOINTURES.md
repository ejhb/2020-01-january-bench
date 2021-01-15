# Jointure SQL

Les jointures en SQL permettent d’associer plusieurs tables dans une même requête. Cela permet d’exploiter la puissance des bases de données relationnelles pour obtenir des résultats qui combinent les données de plusieurs tables de manière efficace.

# Types de jointures

Il y a plusieurs méthodes pour associer 2 tables ensemble. Voici la liste des différentes techniques qui sont utilisées :

> INNER JOIN

	SELECT *
	FROM A
	INNER JOIN B ON A.key = B.key

Jointure interne pour retourner les enregistrements quand la condition est vrai dans les 2 tables. C’est l’une des jointures les plus communes.


> LEFT JOIN (ou LEFT OUTER JOIN) 

	SELECT *
	FROM A
	LEFT JOIN B ON A.key = B.key
	WHERE B.key IS NULL

Jointure externe pour retourner tous les enregistrements de la table de gauche (LEFT = gauche) même si la condition n’est pas vérifié dans l’autre table.

> RIGHT JOIN (ou RIGHT OUTER JOIN)

	SELECT *
	FROM A
	RIGHT JOIN B ON A.key = B.key

Jointure externe pour retourner tous les enregistrements de la table de droite (RIGHT = droite) même si la condition n’est pas vérifié dans l’autre table.

> FULL JOIN (ou FULL OUTER JOIN)

	SELECT *
	FROM A
	FULL JOIN B ON A.key = B.key



