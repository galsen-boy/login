1. Connexion à la console en tant qu'utilisateur et superutilisateur (root) :

    Lorsque tu démarres la machine virtuelle, elle te demande de te connecter. Tu dois entrer ton nom d'utilisateur (par exemple "student") puis appuyer sur "Entrée". Ensuite, il te sera demandé d'entrer le mot de passe associé à cet utilisateur. Tape le mot de passe et appuie sur "Entrée".
    Pour te connecter en tant que superutilisateur, c'est le même processus, sauf que le nom d'utilisateur sera "root" et il faudra entrer le mot de passe associé à l'utilisateur root.

2. Effacer la console avec le raccourci clavier :

    Pour nettoyer l'écran et effacer ce qui est affiché dans la console, utilise le raccourci clavier Ctrl + L. Cela te donne un écran vide, mais les commandes exécutées précédemment sont toujours dans l'historique.

3. Changer le mot de passe :

    Pour changer le mot de passe de l'utilisateur actuel, tape la commande suivante :

    passwd

    Ensuite, le système te demandera d'entrer ton mot de passe actuel pour confirmer que c'est bien toi. Une fois cela fait, il te demandera le nouveau mot de passe (dans notre cas, "michelle"), que tu devras taper deux fois.

4. Afficher l'historique des commandes en utilisant cinq touches ou moins :

    Les commandes que tu as exécutées précédemment sont enregistrées dans ce qu'on appelle l'historique des commandes. Pour accéder rapidement à une commande que tu as utilisée auparavant, utilise le raccourci Ctrl + R, qui lance une recherche inverse dans l'historique.
    Tape ensuite une partie du nom de la commande que tu cherches, et elle apparaîtra automatiquement.

5. Se déconnecter avec le raccourci clavier :

    Pour te déconnecter de la session en cours, utilise le raccourci Ctrl + D. Cela revient à taper la commande exit, qui termine la session.

Connexion sur la troisième console Linux en tant que root :

    Les systèmes Linux permettent d'ouvrir plusieurs consoles (ou "terminaux virtuels"). Pour accéder à la troisième console, utilise le raccourci Ctrl + Alt + F3. Une fois là, connecte-toi en tant que "root".

Vérifier la connectivité Internet :

    Pour vérifier si tu es connecté à Internet, utilise la commande suivante :

    ping google.com

    Cette commande envoie des "paquets" de données à google.com et te montre combien de temps cela prend pour les recevoir en retour. Pour interrompre cette opération, utilise le raccourci Ctrl + C.

Identifier les éléments à l'aide de commandes :

    Pour obtenir l'inode d'un fichier spécifique :
        Chaque fichier sur le système de fichiers Linux possède un numéro unique appelé "inode". Pour voir ce numéro, utilise :

        bash

    ls -i /chemin/vers/le/fichier

    Par exemple, ls -i /etc/fstab affiche l'inode du fichier /etc/fstab.

Pour obtenir l'identifiant de l'utilisateur actuel :

    Tape :

    bash

    id -u

    Cela te donne un nombre qui représente ton utilisateur (par exemple, "0" pour root, "1000" pour l'utilisateur "student").

Pour obtenir le PID d'un programme, par exemple "bash" :

    Chaque programme en cours d'exécution possède un identifiant unique appelé PID (Process Identifier). Pour trouver le PID de "bash", tape :

pidof bash

ou

pgrep bash

Cela affiche le numéro de processus associé à "bash".