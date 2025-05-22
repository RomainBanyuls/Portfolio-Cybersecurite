# Offensive Security Intro

## 🧠 Objectifs de la room

- Découvrir le métier de hacker éthique
- Apprendre à réaliser un scan de site web
- Utiliser des outils comme **Gobuster**, **Hydra**, **Burp Suite**
- Comprendre la méthodologie d’un test d’intrusion basique

---

## 🎓 Compétences acquises

- Scan de répertoires web avec Gobuster
- Brute force de mot de passe avec Hydra
- Interception de requêtes avec Burp Suite
- Compréhension des statuts HTTP et des erreurs associées
- Identification d’une page d’administration ou d’un fichier vulnérable

---

## ⚒️ Outils utilisés

- `gobuster` : énumération de répertoires/fichiers sur un site web
- `hydra` : force brute de mots de passe
- `burpsuite` : proxy HTTP pour capturer et manipuler les requêtes

---

## ⚙️ Commandes pratiques

### Scan de répertoires avec Gobuster
```bash
gobuster dir -u http://[IP] -w /usr/share/wordlists/dirb/common.txt
```

### Brute force formulaire web avec Hydra
```bash
hydra -l admin -P /usr/share/wordlists/rockyou.txt [IP] http-post-form "/login:username=^USER^&password=^PASS^:Invalid credentials"
```

---

## 🔎 Étapes de l’attaque (MITRE ATT&CK simplifié)

1. **Reconnaissance** : scan des répertoires pour identifier les points d'entrée (Gobuster)
2. **Accès initial** : tentative de login avec credentials faibles (Hydra)
3. **Exploitation** : utilisation de Burp Suite pour contourner des protections ou manipuler les paramètres

---

## 🧪 Scénario simulé

**Cible** : un serveur web fictif accessible à l’adresse IP donnée par TryHackMe.

**Étapes réalisées :**
- Énumération des dossiers → découverte de `/admin`
- Tentative de connexion → mot de passe faible
- Interception de la requête → modification des headers avec Burp

**Résultat attendu** : accès au panneau admin et lecture d’un flag final prouvant l'accès non autorisé.

---

## ✅ Recommandations (vue consultant sécurité)

- Restreindre l’accès aux répertoires sensibles (authentification, firewall)
- Ne jamais utiliser de mots de passe par défaut (admin/admin)
- Éviter les messages d’erreur explicites (ex: "Invalid credentials")
- Monitorer les tentatives de brute force
- Filtrer les entrées utilisateur côté **serveur**, pas uniquement dans le navigateur

---

## 🔚 Conclusion personnelle

Cette room m’a permis de comprendre la logique d’un test de pénétration simple :
- découverte de surface d’attaque,
- exploitation des vulnérabilités d’accès,
- contournement de protections simples via des outils standards.

Une très bonne initiation à la cybersécurité offensive et au raisonnement méthodique.

---

**Lien TryHackMe :** [Offensive Security Intro](https://tryhackme.com/room/offensivesecurityintro)
