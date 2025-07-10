# ALL IN ONE APPLICATION SPRING SECURITY (PRODUCT MANAGER)
Ce projet consiste en une application web de gestion des produits, développée avec Spring MVC pour une architecture modulaire et Thymeleaf comme moteur de templates pour une intégration HTML dynamique. L'injection de dépendances via Spring permet une gestion flexible des composants, tandis que Spring Security sécurise l'accès aux fonctionnalités avec une authentification et des rôles personnalisés. L'application offre des opérations CRUD sur les produits, une interface intuitive et une gestion des utilisateurs, illustrant ainsi les bonnes pratiques de développement avec Spring.

### Ajouter les dependances et creation du projet 

<img width="975" height="736" alt="image" src="https://github.com/user-attachments/assets/53efe767-dfef-44d8-ae67-9148d942b213" />


### Architecture du projet

<img width="526" height="709" alt="image" src="https://github.com/user-attachments/assets/7bc21607-375d-49b2-8307-0ce04d4973cd" />


### Creation du classe Product qui represente le modele de notre application
##### chaque produit a un identifiant, un nom, un prix et une quantite

<img width="975" height="862" alt="image" src="https://github.com/user-attachments/assets/bc72a569-375f-400c-b2d4-3b83a83cf686" />


### L'interface ProductRepository

<img width="975" height="293" alt="image" src="https://github.com/user-attachments/assets/88bda053-010d-45bd-bc10-b034542b32dd" />


## Premier test
### Creation de trois produit utilisant un objet de type ComandLineRunner

<img width="975" height="1062" alt="image" src="https://github.com/user-attachments/assets/42344984-cde3-4934-a5f8-cf6b337c68a2" />


### Configuration du base de donnees H2

<img width="975" height="254" alt="image" src="https://github.com/user-attachments/assets/46b43568-a707-451b-9ac7-a30d64061229" />


### Premier demarage du serveur

##### affiche en console la liste des produits stocker dans la base ainsi que le mot de passe generer par spring security

<img width="975" height="477" alt="image" src="https://github.com/user-attachments/assets/18dd6b25-a39e-4d7c-82e3-e0a572a14237" />


### Affichage du table produits depuis h2-console

<img width="975" height="631" alt="image" src="https://github.com/user-attachments/assets/919f4087-325d-4eeb-ad6d-2e7f8eefe84b" />


### Desactivation du spring security

<img width="975" height="501" alt="image" src="https://github.com/user-attachments/assets/d2244be6-d58d-4cb1-b343-84778e4ce452" />


### Creation du controleur dans le package web qui retourne une page produits

<img width="975" height="559" alt="image" src="https://github.com/user-attachments/assets/a39e3ed2-017f-40a4-9dfc-7821bb3151b6" />


### la page html produits

<img width="975" height="562" alt="image" src="https://github.com/user-attachments/assets/6419913c-0d25-4599-9e9a-16d88c4ce028" />


### Resultat d'affichage du premier test

<img width="975" height="489" alt="image" src="https://github.com/user-attachments/assets/6a9701c3-6483-40bf-8c85-918b071039ac" />


## Deuxieme test avec thymleaf

### Modifier le controlleur pour qu'il passe la liste des produits au model

<img width="975" height="569" alt="image" src="https://github.com/user-attachments/assets/49664d79-b131-44cc-9b82-8bb35ab12deb" />


### Recuperer la liste des produits et l'afficher a l'aide de thymleaf

<img width="975" height="743" alt="image" src="https://github.com/user-attachments/assets/4eef0882-cb86-4e0f-8712-084df7cf9b37" />


### Resultat initiale du test 

<img width="975" height="403" alt="image" src="https://github.com/user-attachments/assets/fa32975d-6411-41a9-8301-1477a8f61214" />


### integration de bootstrap 5 au dependances

<img width="975" height="626" alt="image" src="https://github.com/user-attachments/assets/b662798a-fd06-4fc3-b9c7-83fa2e39ee4f" />


### ameliortion d'affichage avec l'ajout du bouton et l'action de suppression

<img width="975" height="531" alt="image" src="https://github.com/user-attachments/assets/35f81058-2e7c-4ecc-9ead-0ed6e46e46ce" />


### Suivi de l'action de suppression

#### status code 302 siginifie que la page existe et localisatio represente la destination de redirction

<img width="975" height="579" alt="image" src="https://github.com/user-attachments/assets/43e31cb9-9caa-4aae-b3cf-ddf19b468b8a" />


### Ajoute l'action de comfirmation avant de la suppression

<img width="975" height="588" alt="image" src="https://github.com/user-attachments/assets/d64775a7-be38-4f4e-9f74-6c66c2a804c2" />


### Creation d'une template avec un header et footer fixe et contenu variable

#### integration d'une bare de navigation

<img width="975" height="766" alt="image" src="https://github.com/user-attachments/assets/12c92280-7da7-49f0-9dda-057f1dc714b2" />


<img width="975" height="320" alt="image" src="https://github.com/user-attachments/assets/71d41a68-d7bb-4b96-a7da-62a8158e9e3d" />


## Ajouter l'action d'ajout d'un produit

### modifier le controlleur avec les contraintes de saisies 

<img width="975" height="328" alt="image" src="https://github.com/user-attachments/assets/d1e8d6f4-7ccf-4ee1-a2ea-96dbd2a6289f" />


### les contraintes de saisies

<img width="975" height="359" alt="image" src="https://github.com/user-attachments/assets/6e871bd3-94c6-43bc-8de6-6f23eb5962ab" />


### Test de l'action ajouter

<img width="975" height="664" alt="image" src="https://github.com/user-attachments/assets/febff3fc-fe3a-4fad-8d83-8f27748e17b5" />


<img width="975" height="710" alt="image" src="https://github.com/user-attachments/assets/7c4ee11a-b856-454c-8b59-082c62656207" />


## Le systeme d'authenfication Spring

<img width="975" height="617" alt="image" src="https://github.com/user-attachments/assets/5f9476ef-6edc-489d-9bbb-df891d87d141" />


### Classe de configuration pour creer des utilisateurs et specification du roles

##### la strategie in memory user details manager

<img width="975" height="406" alt="image" src="https://github.com/user-attachments/assets/023fce32-8f85-4728-84fe-d0ce294b20a0" />


### Erreur 403 d'autorisation

<img width="975" height="323" alt="image" src="https://github.com/user-attachments/assets/b11706e4-82b4-43a9-8695-7ead932d2c3a" />


### Page de deconnexion

<img width="975" height="507" alt="image" src="https://github.com/user-attachments/assets/f4727d42-2f1e-4bbc-bef7-0fcf2479ced7" />


### Creation d'une page d'acces interdite

<img width="975" height="537" alt="image" src="https://github.com/user-attachments/assets/ecc76475-4e50-4d6f-9926-079879feddee" />


<img width="975" height="396" alt="image" src="https://github.com/user-attachments/assets/859c6b53-bdc9-4e86-b607-810f7ae88d45" />


### Modifier l'affichage des boutons selon les roles

##### Cacher les boutons pour les utilisateurs

<img width="975" height="650" alt="image" src="https://github.com/user-attachments/assets/4a69a4c6-8676-49c5-83eb-5a7708d0613e" />


<img width="975" height="218" alt="image" src="https://github.com/user-attachments/assets/929f9380-f0aa-4fc7-9367-24a36eac172b" />


## Affichage du token CSRF

<img width="975" height="488" alt="image" src="https://github.com/user-attachments/assets/66416b57-1921-4a6e-9fb0-e041a85974da" />

## Personnaliser la page d'authentification du spring security

<img width="975" height="750" alt="image" src="https://github.com/user-attachments/assets/1d7c89fc-9b6b-4ea7-98dd-fc7a9e573e35" />


<img width="975" height="283" alt="image" src="https://github.com/user-attachments/assets/e35037c2-a8fb-48d0-82fb-6ef496d060ef" />


## Ajouter le bouton de deconnexion

<img width="975" height="909" alt="image" src="https://github.com/user-attachments/assets/bed34b31-dc57-48e8-9b1b-48066c53e028" />



