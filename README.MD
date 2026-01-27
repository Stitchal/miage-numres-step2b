

# Proposition
Ce repo contient une proposition d'amélioration du repo `miage-numres-step2a`

# Fork du projet
L'objectif est de créer une copie du projet 'miage-numres-step2b' sur votre compte github.

1. Se rendre sur le projet github [miage-numres-step2b] (https://github.com/aepsilon-tek/miage-numres-step2b)

# lancement de CodeSpaces

1. Rendez-vous sur la page principale de votre projet forké
1. En haut de cette page, cliquez sur le bouton vert <> Code
1. Sélectionnez l'onglet Codespaces
1. Cliquez sur Create codespace on main
1. Attendez environ 1 à 2 minutes que l'environnement se construise (le système installe Java et les extensions nécessaires automatiquement).

Sinon vous pouvez clicquer ici  [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=main&repo=${github.repository_id})

> [!TIP]
> Fermez la fenêtre de Copilot, vous n'en avez pas besoin.

> [!WARNING]
> Assurez-vous d'avoir forké ce projet sur votre compte personnel avant de cliquer sur le bouton ci-dessus, sinon vous ne pourrez pas enregistrer (pusher) vos modifications.

> [!WARNING]
> Vous disposez de 60 heures gratuites par mois. Quand vous avez terminé votre travail, cliquez sur le nom du Codespace en bas à gauche et choisissez Stop Current Codespace.



# Evaluer la proposition
## En mode JVM
1. Construire l'application en mode JVM
1. Lancer l'applicatif construit : `java -jar target/quarkus-app/quarkus-run.jar`
1. Répondre aux questions Q1 à Q4 du fichier **_Questions.md_**
1. Commiter  & Pusher le fichier **_Questions.md_**


## En mode Natif
1. Installer GraalVM dans un terminal : sdk install java 21.0.2-graalce
1. Construire l'application en mode Natif
1. Lancer l'applicatif construit : `./target/api-quarkus-1.0.0-SNAPSHOT-runner`
1. Répondre aux questions Q5 à Q8 du fichier **_Questions.md_**
1. Commiter  & Pusher le fichier **_Questions.md_**


# Bilan
1. Répondre aux questions Q9 et Q10   **_Questions.md_**
1. Commiter  & Pusher le fichier **_Questions.md_**


# Pull Request
Une fois tous vos commits & Push réalisés sur votre repo, il est nécessaire de faire la **Pull Request** sur le repo **parent**.
Pour cela, il suffit de :
1. Se rendre sur votre compte personnel sur `GitHub`.
1. Sur la page principale, se rendre sur `Contribute` > `Open pull Request`
1. Remplir le titre de la pull request en précisant votre nom (vos noms) et `Create pull request`

# Commandes Utiles
* ```./mvnw clean compile ``` : Compilation du projet
* ```./mvnw clean package``` : Construction du projet en mode JVM
* ```./mvnw clean package -P native -Dquarkus.native.container-build=false``` : Construction du projet en mode Natif
