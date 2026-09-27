# OverTheWire — Bandit Writeups

Mes notes de progression sur le wargame [Bandit](https://overthewire.org/wargames/bandit/) 
d'OverTheWire, un jeu d'apprentissage Linux/sécurité orienté ligne de commande.

⚠️ **Pas de mots de passe ici** — seulement la méthode et les commandes utilisées. 
Le but est de partager le raisonnement, pas de spoiler le jeu.

## Progression

- [x] Level 0 → 1
- [x] Level 1 → 2
- [ ] Level 2 → 3
- [ ] Level 3 → 4
- [ ] ...

## Niveaux notables

### Level 0 — Connexion initiale
**Concept** : se connecter pour la première fois au serveur du jeu via SSH.  
**Commande clé** : `ssh bandit0@bandit.labs.overthewire.org -p 2220`  
**Ce que j'ai appris** : la syntaxe de base SSH (`utilisateur@serveur`) et l'utilisation 
de l'option `-p` pour préciser un port non standard.

### Level 0 → 1 — Mot de passe dans un fichier readme
**Concept** : trouver un mot de passe stocké dans un fichier texte du dossier personnel.  
**Commandes clés** : `ls` (lister les fichiers) puis `cat readme` (afficher le contenu).  
**Ce que j'ai appris** : les bases de la navigation et de la lecture de fichiers en ligne 
de commande. Aussi appris à copier-coller un mot de passe proprement plutôt que de le 
retaper à la main, pour éviter les erreurs de frappe.

### Level 1 → 2 — Fichier au nom piège
**Concept** : un fichier nommé littéralement `-` (un tiret), qui pose problème car le 
terminal l'interprète normalement comme une option de commande plutôt qu'un nom de fichier.  
**Commande clé** : `cat ./-` (le `./` force l'interprétation comme chemin de fichier local).  
**Ce que j'ai appris** : l'importance de préciser un chemin explicite (`./`) pour éviter 
les ambiguïtés avec des noms de fichiers spéciaux.

## Outils/notions rencontrés
`ssh`, `ls`, `cat`, navigation de base en ligne de commande, gestion des noms de fichiers 
spéciaux, copier-coller sécurisé dans le terminal.
