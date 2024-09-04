#Lien Planification : https://anouarab95.atlassian.net/jira/software/projects/GDBA/boards/3/backlog
   #################################################jar : java -jar Gestion_Bibliotheque.jar #####################

   
- Gestion du Projet
Git : Utilisé pour le contrôle de version.
JIRA : Utilisé pour la gestion des tâches et le suivi des progrès.
Daily Stand-ups : Simulations de réunions quotidiennes pour coordonner le travail et résoudre les obstacles.
---------------------------------------------------------------------------------------------------------------------
Contexte du projet
Une bibliothèque municipale souhaite automatiser ses tâches via un système de gestion informatisé. Votre mission est de développer une application console en Java 8 pour gérer efficacement l'inventaire des livres et magazines, ainsi que les emprunts et retours.
----------------------------------------------------------------------------------------
 ​Fonctionnalités
 
- L'application offre les fonctionnalités suivantes :

Ajouter un document : Permet d'ajouter un livre ou un magazine à la bibliothèque.
Emprunter un document : Permet d'emprunter un document en le marquant comme indisponible.
Retourner un document : Permet de retourner un document emprunté, le rendant à nouveau disponible.
Afficher tous les documents : Affiche la liste de tous les livres et magazines disponibles dans la bibliothèque.
Rechercher un document : Recherche un document par son titre et affiche ses détails.
Quitter : Quitte l'application.
-----------------------------------------------------------------------------
Votre responsabilité consiste à :

• Concevoir une architecture en couches (présentation, métier, utilitaire)

• Implémenter les classes principales et leurs fonctionnalités

• Utiliser les concepts de base de Java (héritage)

​
----------------------------------------------------------------------------------
Structure de l'application :

Couche de présentation :

Classe ConsoleUI pour l'interface utilisateur
Couche métier :
Classe abstraite Document
Classes Livre et Magazine (héritant de Document)
Classe Bibliotheque pour la gestion des documents
Couche utilitaire :
Classe DateUtils pour la manipulation des dates
​
Contenu des classes :

Classe abstraite Document :

• Attributs : id, titre, auteur, datePublication, nombreDePages

• Méthodes abstraites : emprunter(), retourner(), afficherDetails()

Classe Livre (hérite de Document) :

• Attribut supplémentaire : isbn

• Implémente les méthodes abstraites

Classe Magazine (hérite de Document) :

• Attribut supplémentaire : numero

• Implémente les méthodes abstraites

​
---------------------------------------------------------------
Utilisation: 

- Une fois l'application démarrée, vous serez accueilli par un menu interactif vous permettant de naviguer entre les différentes fonctionnalités. Suivez les instructions à l'écran pour ajouter, emprunter, retourner, afficher ou rechercher des documents dans la bibliothèque.
​
----------------------------------------------------------------------------
Spécifications techniques :

• Utiliser ArrayList pour stocker les documents

• Implémenter une recherche rapide avec HashMap<String, Document>

• Intégrer Java Time API pour la gestion des dates

• Appliquer les expressions lambda

​----------------------------------------------------------------------

Interface utilisateur : Créer un menu interactif dans la console avec les options suivantes :

Ajouter un document
Emprunter un document
Retourner un document
Afficher tous les documents
Rechercher un document
Quitter
​

Veuillez entrer votre choix (1-6) :

​-------------------------------------------------------------------------------

Contraintes :

• Les données persistent en mémoire jusqu'à la fermeture de l'application

• Implémenter une validation des entrées utilisateur pour la gestion des erreurs possibles

​
