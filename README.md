# Servlet-Implementation-java
1-Telechargez et installez le serveur Web Apache Tomcat 
Téléchargement de Apache Tomcat version 9.

2-Tester le serveur Apache Tomcat à l’aide d’une page Html:
Après avoir ajouté le serveur Apache Tomcat à notre Eclipse Dynamic web Project, on crée une page html index.html dans le directoire de notre projet et on la run sur le serveur pour tester son fonctionnement




















On obtient le résultat attendu. Comme on peut le voir dans le URL, on a le nom de la machine dans ce cas « localhost » ainsi que le numéro du port que le serveur utilise « 8082 » ainsi que le nom de notre projet « DemoServlet » et le nom de la page HTML « index.html » crée. 
 

3-Creation d’une page HTML contenant un lien vers notre Servlet :
 
Dans notre page HTML, on a créé un form pour récupérer le prénom et nom de l’utilisateur. Cette form implémente la méthode « post » et a comme action le nom de notre servlet « HelloServlet ». 


4-Implementation du Servlet
 
Lors de la création de notre servlet 3 méthode son générée automatiquement : service, doGet et doPost
Dans notre exemple on va implémenter la méthode service ci-dessous
 
Cette méthode va récupérer les paramètres de la page html en utilisant un PrintWriter et la méthode getParameter()
Puis elle génère un texte en format html pour afficher les résultats. 

 
La page html ci-dessus prend le nom et prenom de l’utilisateur
 
En appuiyant sur submit les parametre son recues par notre servlet qui a son tour les affiche sur une autre page html comme on peut le voir dans l’image ci-dessous . 
 
