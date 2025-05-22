# Linux Fundamentals Part 1

## 🧠 Objectifs de la room

- Comprendre le fonctionnement d’un système Linux
- Apprendre à naviguer dans l’arborescence de fichiers
- Exécuter des commandes de base en ligne de commande
- Gérer des fichiers et répertoires via le terminal

---

## 🎓 Compétences acquises

- Navigation dans l’arborescence (`pwd`, `cd`, `ls`)
- Lecture et édition de fichiers (`cat`, `nano`, `less`)
- Manipulation de fichiers (`cp`, `mv`, `rm`, `mkdir`)
- Compréhension des chemins absolus/relatifs
- Utilisation des permissions de base (`chmod`, `ls -l`)
- Compréhension des comptes utilisateurs (`whoami`, `id`)

---

## ⚒️ Commandes et outils utilisés

| Commande | Fonction |
|----------|----------|
| `pwd` | Affiche le chemin courant |
| `ls -la` | Liste les fichiers avec détails et fichiers cachés |
| `cd` | Change de répertoire |
| `cat` | Affiche le contenu d’un fichier |
| `nano` / `vi` | Éditeurs de texte en terminal |
| `cp`, `mv`, `rm` | Copier, déplacer, supprimer un fichier |
| `mkdir` | Créer un dossier |
| `chmod` | Modifier les permissions |
| `whoami`, `id` | Affiche les infos de l’utilisateur actif |

---

## 📂 Notions clés

- **FHS** : Filesystem Hierarchy Standard (structure Linux `/etc`, `/bin`, `/home`, etc.)
- **Chemin absolu vs relatif** : `/home/user/docs` vs `../docs`
- **Utilisateurs et groupes** : gestion de base des droits d’accès
- **Permissions Unix** : lecture (r), écriture (w), exécution (x)

---

## 🧪 Scénario simulé

**Mission :** Tu es connecté à une machine distante Linux.  
Tu dois :
- Te déplacer dans différents dossiers
- Lire un fichier caché (`.hidden.txt`)
- Donner des droits d’exécution à un script (`chmod +x`)
- Exécuter un script pour récupérer un flag

**Extrait de séquence réussie :**
```bash
cd /home/student/.secret/
ls -la
cat flag.txt
chmod +x runme.sh
./runme.sh
```

---

## ✅ Recommandations (vue admin débutant)

- Toujours utiliser `ls -la` pour voir tous les fichiers
- Se méfier de l’impact des commandes destructives (`rm -rf`, etc.)
- Apprendre les raccourcis : `..`, `~`, `tab` pour autocomplétion
- Éditer prudemment les fichiers système avec `sudo`
- S’exercer régulièrement sur une machine Linux (VM, WSL, TryHackMe)

---

## 🔚 Conclusion personnelle

Cette room est une excellente introduction à l’univers Linux.  
Elle m’a permis de comprendre que **la maîtrise du terminal est indispensable** en cybersécurité, aussi bien pour les attaques que pour l’analyse de logs ou la réponse à incident.

Un indispensable pour tout débutant !

---

**Lien TryHackMe :** [Linux Fundamentals Part 1](https://tryhackme.com/room/linuxfundamentals1)
