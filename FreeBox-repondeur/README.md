FreeBox-repondeur
=================
Plugin FreeBox-repondeur

Ce plugin permet de connaitre le nombre de message sur votre r�pondeur FREEBOX, de les lire et de les effacer.

Plugins et programmes requis :
- Plugin Mail
- Vlc

V1.0 :
- Comptage des messages 
- Lecture des messages .wav par VLC 
- Effacement des messages
Documentation
Pr�paration
Configurations n�c�ssaires
Fonctionnement
Commandes Vocales
1�) Configurer la r�ception des messages FREEBOX sur votre boite mail sur le site portail.free.fr rubrique mon compte> T�l�phonie > Gestion de la messagerie vocale. S�lectionnez l'option "Fichier son envoy� en attachement"
2�) Dans votre boite mail, sur le site zimbra.free.fr par exemple, cr�er un dossier "speech" puis cr�er un filtre de d�placement des mails contenant l'objet [FREEBOX]. Ainsi tout vos mail contenant un message r�pondeur iront automatiquement dans ce dossier
3�) Compl�ter les parametres du plugin mail par l'interface web de sarah http://127.0.0.1/home. Dans la case Speechbox indiquez speech
4�) Installer le programme VLC (si ce n'est d�j� fait!)
Fonctionnement du r�pondeur:
A interval r�gulier, le plugin mail analyse vos mails. D�s qu'un mail se trouve dans le dossier speech de votre boite, le plugin mail copie le message .wav dans le dossier ./plugins/mail/speech.
Vous avez donc ensuite la possibilit� de connaitre le nombre de messages dans le dossier, de lire les .wav pr�sents dans le dossier ou enfin de supprimer les messages du dossier (ATTENTION LES MESSAGES SUPPRIMES NE VONT PAS DANS LA CORBEILLE ET SONT IRRECUPERABLES !).