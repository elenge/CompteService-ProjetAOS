# CompteService-ProjetAOS

Application REST permettant la gestion de comptes bancaires.

Réalisateurs : Alexandre Bodin et Kévin Cot

Objectif : l'application doit fournir des services de gestion de comptes bancaires en ligne, et notamment des opérations telles que la création de compte bancaire, de dépôt et de retrait d'un montant sur un compte précis ainsi que la consultation du solde d'un compte.

Pour atteindre cet objectif, les développements ont été séparés en deux chantiers : 
- le premier a porté sur le développement et la mise en place du WebService côté serveur, représentant les services fournis. Cela a été réalisé grâce au langage Java en respectant l'architecture REST (REpresentational State Transfer) avec l'IDE Eclipse (Dynamic Web Projet avec le framework Jersey JAX-RS) 
- le second chantier a porté sur la réalisation d'un client permettant d'accéder de manière ergonomique et transparente aux services. Ce client a été réalisé à l'aide des langages HTML, CSS (utilisation du framework d'interface Bootstrap) et Javascript (Jquery)  ainsi que de l'Ajax pour traiter les requêtes HTTP (Put,Get,Post) vers notre WebService.


Le déploiement en local :

 - Nous avons utilisé un serveur local Tomcat 7,
 - Nous avons déployé notre WebService REST dans le dossier webapps de Tomcat 7 sous la forme d'un fichier .war,
 - Nous avons également déployé le client dans le dossier webapps car Tomcat limite les accès externes,
 - Après avoir lancé Tomcat 7, on peut accéder au client via cette URL : http://localhost:8080/ClientRestBanqueService/indexClient.html,
 - Le client est maintenant prêt à être utilisé.
 - Un premier compte est automatiquement initialisé au premier démarrage de l'application afin de générer le fichier support de la sérialisation.

Mode d'emploi du client :
	
	- Pour créer un compte, il suffit de cliquer sur le bouton "Créer un compte", renseigner le nom du propriétaire, cliquer sur "Créer" puis sur "Close" et enfin sur "Actualiser".
	- Pour connaître le solde d'un compte, il faut cliquer sur le bouton "Connaître le solde", renseigner le numéro du compte, cliquer sur "OK" puis sur "Cancel".
	- Pour effectuer un dépôt sur un compte il faut cliquer sur le bouton "Dépôt", renseigner le numéro de compte et le montant souhaité, cliquer sur "OK" puis "Cancel" et enfin sur "Actualiser".
	- Pour effectuer un retrait sur un compte il faut cliquer sur le bouton "Retrait", renseigner le numéro de compte et le montant souhaité, cliquer sur "OK" puis "Cancel" et enfin sur "Actualiser".