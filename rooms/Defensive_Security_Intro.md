# Defensive Security Intro

## 🧠 Objectifs de la room

- Comprendre la cybersécurité **défensive**
- Identifier les rôles clés : analyste SOC, threat analyst, équipe DFIR
- Découvrir les outils de surveillance : SIEM, threat intel, alerting
- Apprendre les bases de la **détection d’incidents**

---

## 🎓 Compétences acquises

- Compréhension du fonctionnement d’un **Security Operations Center (SOC)**
- Détection d’activités suspectes dans des **logs** système
- Familiarisation avec les **IOC** (Indicators of Compromise)
- Introduction au **Threat Intelligence** (veille cybercriminelle)
- Vue d’ensemble sur la **réponse aux incidents** (DFIR)

---

## ⚒️ Concepts clés

| Terme | Définition |
|------|-------------|
| **IOC** | *Indicators of Compromise* : indices techniques de compromission (adresse IP, nom de domaine, hash malveillant…) |
| **SIEM** | *Security Information and Event Management* : outil centralisant les logs pour les analyser et détecter les incidents |
| **DFIR** | *Digital Forensics and Incident Response* : réponse technique à un incident (analyse, containment, récupération) |
| **SOC** | *Security Operations Center* : centre de surveillance continue de la sécurité des systèmes d’information |

---

## 🔍 Activités pratiques simulées

- Analyse d’un fichier log système (Windows/Linux)
- Identification d’une tentative d’intrusion via les logs
- Extraction manuelle d’un IOC à partir d’une alerte

---

## 🧪 Exemple de scénario défensif

**Situation :**  
Un utilisateur signale un comportement étrange sur son poste. L’équipe SOC consulte les logs et détecte :

- Connexion à une IP étrangère non autorisée
- Exécution d’un processus inconnu
- Téléchargement d’un exécutable depuis un domaine suspect

**IOC trouvés :**
- Adresse IP : `91.193.77.154`
- Domaine : `malicious-update.com`
- SHA256 : `fd2b85a...`

**Réaction DFIR :**
- Isolement du poste
- Extraction de la mémoire vive
- Analyse de la persistence
- Remédiation + rapport d’incident

---

## ✅ Recommandations professionnelles

- Centraliser tous les logs (via un SIEM type Splunk, ELK, Wazuh…)
- Mettre en place une **veille de threat intel** (OTX, VirusTotal, MISP…)
- Créer des **alertes automatiques** basées sur les IOC connus
- Documenter chaque incident (playbooks, journaux, leçons tirées)
- Entraîner les équipes avec des simulations d’attaque (Purple Team)

---

## 🧠 Carte mentale de la sécurité défensive (résumé)

- **Prévention** : firewall, endpoint security, patch management
- **Détection** : SIEM, NIDS/HIDS, SOC monitoring
- **Réaction** : DFIR, containment, forensic, remédiation
- **Amélioration continue** : mise à jour des règles, analyse post-mortem

---

## 🔚 Conclusion personnelle

Cette room m’a permis de découvrir le versant défensif de la cybersécurité.  
On y apprend qu’il ne s’agit pas seulement de « réagir » à une attaque, mais de savoir l’**anticiper, détecter, isoler**, et en tirer des enseignements pour améliorer les défenses.

C’est une composante essentielle pour tout analyste SOC ou Blue Team débutant.

---

**Lien TryHackMe :** [Defensive Security Intro](https://tryhackme.com/room/defensivesecurityintro)
