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
