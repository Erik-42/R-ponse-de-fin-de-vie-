J'ai utilisé ça et Claude pour documenter trois phases. 
1. Documentation du homelab et de la maison intelligente - où est quoi, ce que ça fait, dépendances
2. Aider le ChatBot IA - mettre en place un bot de chat interne qui peut répondre aux questions, tant techniques que pratiques, sur la maison. Si les films ne jouent pas, il se réfère à la documentation, vérifie Docker, vérifie la connexion Internet, et revient avec une description en anglais simple de ce qu'il faut faire et vérifier, ou le corrige si possible 
3. Documentation de mes responsabilités du point de vue de la maison. Factures, entretien, rappels. J'ai déjà vaultwarden avec tous les mots de passe et j'ai mis des choses dans un dossier "si je pars".

Maintenant, il s'agit juste de s'assurer qu'elle retient bien les informations de base et sait par où commencer.

Toutes mes affaires importantes doivent tenir sur un seul disque dur externe branché à l'arrière de mon NAS. Si je meurs, j'ai dit à ma femme de le débrancher et de le brancher sur son PC. 

Ce sont juste des fichiers et des photos. C'est l'une de mes exigences pour héberger mes fichiers, ça ne peut pas mettre des choses dans une base de données inaccessible (pour ma femme) si c'est important.

J'ai quelques SSD connectés à l'un de mes serveurs. Deux fois par jour, un script s'exécute et sauvegarde des données. Chaque disque est destiné à un utilisateur spécifique. Donc le disque contient toutes les photos immich, les exports de vaultwarden pour les mots de passe en texte clair. L'idée est que ma femme et moi avons accès aux données, et tout ce que quelqu'un a à faire, c'est de débrancher le disque du serveur et de l'utiliser sur n'importe quel ordinateur. J'ai le script qui envoie un retour via mqtt à home assistant pour confirmer que ça s'est bien terminé et ensuite une automatisation nodered me dit si les sauvegardes échouent.

