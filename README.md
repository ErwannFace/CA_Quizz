\title{Quizz d'entrée à la Code Académie \\ Expression de Besoin v0.1}
\author{Erwann DUCLOS}
\date{7 Septembre 2017}
\maketitle
\newpage


# Quizz Code Académie
## Sommaire
Dans le cadre de la Grande école du numérique, la fondation FACE a créé un organisme de formation : La Code Académie.

Cette mission est actuellement en cours, et le Lead Formateur du dispositif, M. Erwann DUCLOS, nous a contacté afin de réaliser une application de type QUIZZ pour la pré-sélection des apprenants avant leur admission au sein de l'école. 

## Définition globale du projet
L'application a pour but d'être accessible sur internet pour l'ensemble des futurs apprenants de la Code Académie. 
Il est attendu de pouvoir ajouter de nombreux types de contenus, divers et variés afin de pouvoir tester un ensemble relativement vaste des aptitudes des candidats. 
Un compte administrateur permettra de définir les personnes disposant d'un compte au sein du site, ainsi que pour administrer les questions du quizz.

## Définition de la cible

La cible de cette application, sont les personnes souhaitant s'inscrire à la prochaine session de la Code Académie. Il s'agit donc d'hommes et de femmes. Entre 16 et 55 ans.


## Définition du commanditaire
Le commanditaire du présent projet est l’association FACE (Fondation Agir Contre l'Exclusion) représentée par Erwann Duclos, lead formateur au sein de la Code Académie.
La Code Académie est un dispositif de formation mis en place dans le cadre du projet gouvernemental de la Grande école du numérique. Il s'agit d'une formation qui permet l'apprentissage du développement web/mobile. Cette formation proposée par la Fondation Agir Contre l'Exclusion de Rennes, suit la pédagogie basée sur la méthode du "Learning by doing". Spécialement orientée vers
les travaux pratiques, cette formation permet l'apprentissage des bases du développement web et des
langages tels que HTML5/CSS3, Javascript et PHP et vise à former les apprenants au métier de développeur web junior.

## Charte Graphique
L'application respectera la charte graphique ci-jointe.
cf. [pièce jointe](./annexes/charte_graphique).

## Arborescence du site
### Utilisateur non connecté
![Pannel de connection](./annexes/img/login.png)

Un utilisateur non connecté ne doit pas pouvoir avoir accès à l'application. Il doit être constamment redirigé vers la page de connection.

### Utilisateur connecté
![Page Structure](./annexes/img/site_structure.png)
Un utilisateur connecté doit pouvoir avoir accès à l'ensemble des quizz qui lui sont affectés. Il aura la possibilité de se connecter par le biais de son adresse email / mot de passe.

## Description d'un quizz

Un quizz est composé d'un titre, d'une durée, d'une description et de plusieurs questions.
Une première page sera affichée permettant d'afficher la description du quizz. Un emise en garde sera réalisée  afin de préciser à l'utilisateur qu'une fois qu'il aura commencé à réaliser le quizz il ne pourra plus revenir en arrière et  que son temps sera compté. 

Une fois que l'utilisateur accepte de réaliser le quizz, les questions lui seront affichées une à une. L'utilisateur n'aura pas la possibilité de revenir en arrière. 

Lorsque l'utilisateur a fini de répondre aux questions du formulaire. Ou lorsque le temps prévu aura écoulé, les résultats seront sauvegardés au niveau de la base de données, et un message sera affiché à l'utilisateur lui mentionnant que le quizz est fini. 
Il aura la possibilité de rajouter un dernier commentaire. 

## Description d'une question
Toute question du quizz sera composée d'une question et de 4 réponses.
La question ainsi que les réponses ne seront pas forcément textuelles, il doit être possible d'avoir les combinaisons suivantes : 

+ Questions : Texte / Image / Vidéo / Document / Son
+ Réponses  : Texte / Image / Son 

Si la question est un document, ce dernier devra s'ouvrir dans un autre onglet.

### Administration
Uniquement l'administrateur aura la possibilité de créer, modifier, supprimer des questions. Chaque question aura un tag (champ obligatoire). 


## Description d'un tag
Un tag consiste à catégoriser un/des questions. Un ensemble de critères d'évaluations doivent être pris en compte avant l'admission au sein de la Code Académie.  Par exemple, des tests sur la vision du candidat (bonne différenciation des couleurs) ou encore sur ses capacités de lecture sont de mise. 



## Compte utilisateur
Un compte utilisateur contiendra les informations suivantes : 

 * Nom (Texte <50 char)
 * Prénom (Texte <50 char)
 * Genre (Homme/Femme/Autre)
 * Email (Texte <50 char)
 * MotDePasse
 * QPV
 * RQTH (Oui / Non)
 * Actif (Oui / Non)
 * Requiers un tiers temps (Oui / Non)


Le champ Requiers un tiers temps, ne pourra petre actif que si le candidat a le champ RQTH à Oui.
Nulle vérification n'est attendue au niveau du mot de passe. 
Uniquement les administrateurs auront la possibilité de créer des comptes utilisateurs. Les personnes connectées auront la possibilité de modifier leurs comptes respectifs. Ils n'auront pas la possibilité de modifier leurs adresses mail.  

## Page de statistiques
L'administrateur aura pour chaque compte utilisateur du site, des statistiques de réussite du quizz. 
Il doit être possible de visualiser le taux de réussite général. Ainsi que de pouvoir voir en détail les catégories (tag) et la réussite dans chaque catégorie. 
Il doit également être possible de pouvoir visualiser le temps total mis par le candidat pour répondre aux questions. 

## Contraintes techniques

L'application sera développée en méthode agile par la Code Académie. Le commanditaire fera partie intégrante du processus de livraison. Pour chaque sprint, une version Beta sera livrée au client. 

### Délais
Ce site devra être livré d'ici le 10 Janvier 2018.

### Responsive
Cette application devra pouvoir s'adapter à différentes tailles d'écran. Allant de 320px de large à 1920px.

### Compatibilité navigateurs
Cette application se devra d'être compatible avec la majorités des navigateurs internet courants. Il est attendu d'avoir une application comptable avec les version de navigateurs suivantes : 

 * Google Chrome 59+
 * Mozilla Firefox 54+
 * IE11
 * Edge 14+
 * Safari 10+
 * Opera 46+


