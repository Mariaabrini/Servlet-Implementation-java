# Servlet-Implementation-java
1-Telechargez et installez le serveur Web Apache Tomcat 
![image](https://user-images.githubusercontent.com/82711846/216997376-f7a167cd-6e12-4eee-abb0-411df6fae46a.png)

Téléchargement de Apache Tomcat version 9.

2-Tester le serveur Apache Tomcat à l’aide d’une page Html:
Après avoir ajouté le serveur Apache Tomcat à notre Eclipse Dynamic web Project, on crée une page html index.html dans le directoire de notre projet et on la run sur le serveur pour tester son fonctionnement

![image](https://user-images.githubusercontent.com/82711846/216997478-b85531ec-7d75-4e64-b045-a69be6edcbed.png)



















On obtient le résultat attendu. Comme on peut le voir dans le URL, on a le nom de la machine dans ce cas « localhost » ainsi que le numéro du port que le serveur utilise « 8082 » ainsi que le nom de notre projet « DemoServlet » et le nom de la page HTML « index.html » crée. 
 ![image](https://user-images.githubusercontent.com/82711846/216997575-aced93a4-b3c2-4f15-bf8e-aa053b799eaf.png)


3-Creation d’une page HTML contenant un lien vers notre Servlet :
 ![image](https://user-images.githubusercontent.com/82711846/216997615-a4318f99-8a0c-45fa-8797-53da722e72f9.png)

Dans notre page HTML, on a créé un form pour récupérer le prénom et nom de l’utilisateur. Cette form implémente la méthode « post » et a comme action le nom de notre servlet « HelloServlet ». 


4-Implementation du Servlet
 ![image](https://user-images.githubusercontent.com/82711846/216997686-88b0925f-ce0d-4045-9754-f8f8cbd61e05.png)

Lors de la création de notre servlet 3 méthode son générée automatiquement : service, doGet et doPost
Dans notre exemple on va implémenter la méthode service ci-dessous
 ![image](https://user-images.githubusercontent.com/82711846/216997741-5a4d93b1-02c7-4822-9819-c0c5401ab853.png)

Cette méthode va récupérer les paramètres de la page html en utilisant un PrintWriter et la méthode getParameter()
Puis elle génère un texte en format html pour afficher les résultats. 
![image](https://user-images.githubusercontent.com/82711846/216997798-d9e1c330-4adf-4cea-a6b3-3a84baad5dc0.png)

 
La page html ci-dessus prend le nom et prenom de l’utilisateur
 ![image](https://user-images.githubusercontent.com/82711846/216997845-e0c33e20-b51e-4d72-bbb9-20423c829f09.png)

En appuiyant sur submit les parametres son recues par notre servlet qui a son tour les affiche sur une autre page html comme on peut le voir dans l’image ci-dessous . 
 ![image](https://user-images.githubusercontent.com/82711846/216997893-f828a2e9-f943-4d09-824b-b5667ada4393.png)

