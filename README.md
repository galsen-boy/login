# Login
### Étapes

1. Démarrer la VM pour booter sur le système Debian précédemment installé.

2. Pour l'utilisateur et le superutilisateur (root) :
    - Se connecter dans la console :
        - Utilisez votre nom d'utilisateur pour vous connecter.
    - Effacer la console en utilisant le raccourci clavier :
        - Appuyez sur ``Ctrl + L``.
    - Changer le mot de passe en michelle :
        - Tapez la commande : ``passwd`` et suivez les instructions.
    - Afficher l'historique des commandes en utilisant cinq frappes au maximum (en utilisant l'auto-complétion) :
        - Tapez ``history`` et appuyez sur Enter.
    - Se déconnecter en utilisant le raccourci clavier :
            Appuyez sur ``Ctrl + D`` ou tapez ``exit``.

    - Se connecter en tant que root sur la troisième console Linux :
        - Appuyez sur ``Ctrl + Alt + F3`` pour accéder à la troisième console.
    - Connectez-vous avec le nom d'utilisateur ``root`` et le mot de passe correspondant.

    - Vérifier la connectivité Internet avec la commande :
        - Tapez : ``ping google.com`` et interrompez le programme avec ``Ctrl + C`` après quelques sauts.

###  Trouver les informations demandées

- Trouver l'inode d'un fichier spécifique :
    - Utilisez la commande : ``ls -i`` <nom_du_fichier> pour obtenir l'inode. Par exemple, pour obtenir l'inode de ``/etc/fstab`` :
```
ls -i /etc/fstab

```
- Trouver l'ID utilisateur actuel :
    - Utilisez la commande : ``id -u``.

- Trouver le PID d'un programme, par exemple ``bash`` :
    - Utilisez la commande : ``pgrep bash`` pour obtenir le PID du programme ``bash``.

## Résumé des commandes

- Changer le mot de passe :
```
passwd
```

- Afficher l'historique :
```
history
```

- Vérifier l'inode d'un fichier :
```
ls -i /etc/fstab
```

- Obtenir l'ID utilisateur :
```
id -u
```

- Trouver le PID de bash :
```
pgrep bash
```
