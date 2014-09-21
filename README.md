OS Deployment on OpenShift
======
Creation de l'application :
- Executer le fichier create.sh
- Se connecter a PhpMyAdmin depuis OpenShift pour importer les donnees depuis move_in.sql
      Connection Openshift
      user : theophile.ravillion@gmail.com
      mdp  : Isep2014
      Connection phpMyAdmin
      -user : admin4sZ9TwT
      -mdp  : kXRiM7GgxQky

- Executer deployOpenshift.sh en passant en argument l'url du projet, l'adresse du server, le nom de la bdd, le user de la bdd, le mdp de la bdd soit : 
ssh://541e21a3e0b8cd42fa00044f@projectos-ostheorav.rhcloud.com/~/git/projectos.git/ 127.5.123.2:3306 projectos admin4sZ9TwT  kXRiM7GgxQky

Quelques remarques sur l'elaboration de ce projet :

- Mon site web d'A1 etant introuvable, y compris apres de longues recherches, je me suis permis d'en emprunter un a des camarades consentants non concernes par ce rattrapage.

- Le site web n'etant pas idealement construit, le parametrage pour l'acces a la base de donnees a en fait du etre fait a la main. Il n'existe pas de fichiers bddparam.php comme le sous entends le code.

- La nouvelle version de linux m'a oblige a revoir le code d'installation de ruby. mon code n'est donc valide que pour Ubuntu 14.4

- Ma principale erreur, qui m'a coutee beaucoup de temps, fut de ne pas me mettre dans le bon dossier une fois l'application cree. Je diagnostiquais d'autres erreurs ce qui m'a permis de decouvrir beaucoup de choses sur openshift que je n'ai pas eu besoin d'utiliser ici.

- J'ai conscience qu'il existe des moyens plus adaptees pour le parametrage de la bdd. Des fonctions permettent de retourner l'user, le mdp, &cie mais je n'ai pas reussi a les utiliser.

- Mes scripts sont assez sommaires, on pourrait imaginer un script multifonction prenant en parametre different arguments. 
