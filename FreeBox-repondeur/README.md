FreeBox-repondeur
=================
Plugin FreeBox-repondeur

Ce plugin permet de connaitre le nombre de message sur votre répondeur FREEBOX, de les lire et de les effacer.

Plugins et programmes requis :
- Plugin Mail
- Vlc

V1.0 :
- Comptage des messages 
- Lecture des messages .wav par VLC 
- Effacement des messages
Documentation
Préparation
Configurations nécéssaires
Fonctionnement
Commandes Vocales
1°) Configurer la réception des messages FREEBOX sur votre boite mail sur le site portail.free.fr rubrique mon compte> Téléphonie > Gestion de la messagerie vocale. Sélectionnez l'option "Fichier son envoyé en attachement"
2°) Dans votre boite mail, sur le site zimbra.free.fr par exemple, créer un dossier "speech" puis créer un filtre de déplacement des mails contenant l'objet [FREEBOX]. Ainsi tout vos mail contenant un message répondeur iront automatiquement dans ce dossier
3°) Compléter les parametres du plugin mail par l'interface web de sarah http://127.0.0.1/home. Dans la case Speechbox indiquez speech
4°) Installer le programme VLC (si ce n'est déjà fait!)
Fonctionnement du répondeur:
A interval régulier, le plugin mail analyse vos mails. Dés qu'un mail se trouve dans le dossier speech de votre boite, le plugin mail copie le message .wav dans le dossier ./plugins/mail/speech.
Vous avez donc ensuite la possibilité de connaitre le nombre de messages dans le dossier, de lire les .wav présents dans le dossier ou enfin de supprimer les messages du dossier (ATTENTION LES MESSAGES SUPPRIMES NE VONT PAS DANS LA CORBEILLE ET SONT IRRECUPERABLES !).