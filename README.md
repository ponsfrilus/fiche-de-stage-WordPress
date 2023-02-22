# Stage WordPress

## Description du stage

Déployer un site WordPress sur une VM Linux sans utiliser Docker.

## Sujets couverts par le stage

   - Linux
   - SSH
   - LAMP
   - Réseau
   - Configuration Apache
   - Configuration MariaDB
   - WordPress

## Objectifs

### Pour WordPress

   - Configuration de WordPress (menu settings, par exemple URL Rewriting)
   - Authentification : réfléchir aux possibilités d'intégeration de système d'authentification tel qu'un SSO ou un LDAP. Installer les plugins d'identification et d'authentification de l'EPFL ([Tequila](https://github.com/epfl-si/wordpress.plugin.tequila) et [Accred](https://github.com/epfl-si/wordpress.plugin.accred))
   - Installation d'un certificat SSL pour que le site soit en HTTPS (par exemple avec [Let's encrypt](https://letsencrypt.org/))
   - Découverte du backoffice de WordPress et de son administration
   - Gestion des thèmes (le stagiaire doit installer un thème de son choix et le [thème EPFL](https://github.com/epfl-si/wp-theme-2018) en plus du thème par défaut de WordPress)
   - Gestion des plugins (le stagiaire doit installer un plugin de son choix et les plugins d'authentification cités plus haut)
   - Configuration de l'envois des emails (par exemple pour la récupération de son mot-de-passe)
  
### Créer un environnement de développement

Lors que le déploiement de WordPress sur la machine virtuelle a été validé, le stagiaire effectuera le travail suivant : afin de ne pas tester en "prod", un environnement de développement doit être mis en place. Les contraintes suivantes sont imposées :

   - Utiliser [Docker](https://www.docker.com) et [docker-compose](https://docs.docker.com/compose/)
   - L'environnement doit tourner sur le laptop du stagiaire
   - Les données se trouvant sur la machine virtuelle doivent être récupérée
   - L'environnement doit fournir
      - le serveur web
      - la base de donnée
      - et le site WordPress
   - Comme l'environnement est local, il n'est pas nécessaire d'avoir le certificat SSL
  

## Rendus

Tout au long de son stage le stagiaire documentera la procédure d'installation et de mise en place en [MarkDown](https://daringfireball.net/projects/markdown/syntax) ; le but est qu'un apprentis de première année puisse reproduire et comprendre les étapes de la procédure.

Le document doit également expliquer les points suivants :
  - Qu'est que WordPress ? 
     - Quelles sont ses alternatives ?
     - Est-il beaucoup utilisé ?
     - Selon vous, quels sont ses avantages et incovénients ?
     - Citez 3 sites Internet publiques qui l'utilise.
  - Expliquer ce que sont et à quoi servent les posts, pages, catégories et tags
  
En plus des différentes étapes pour attendre l'objectif, le stagiaire répondra aux questions suivantes :
   - Quelles mesures sont nécessaires pour la sécurité et protection de la machine et du site Internet ?
   - Comment assurer des backups du système mis en place ? Faire des propositions fonctionnelles de solutions de backup.
   - Expliquez de quelle manière vous avez géré les secrets (par exemple le mot-de-passe root de la base de données) ? Quels sont les avantages de votre méthode ?
   - Quelles alternatives il y a-t-il pour mettre en place un certificat SSL ?
   - Quelle est la différence en un plugin et un mu-plugin ?
   - Quels sont les avantages a avoir utilisé Docker pour l'environnement de développement ? Serait-il possible d'utiliser Docker directement sur la machine virtuelle (développez).



