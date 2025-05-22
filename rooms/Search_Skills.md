# Search Skills

## 🧠 Objectifs de la room

- Développer des compétences **OSINT** (Open Source Intelligence)
- Apprendre à faire des recherches efficaces et ciblées
- Utiliser des **Google Dorks** pour fouiller le web profond
- Découvrir des outils d’analyse de domaine, IP, certificat SSL, etc.

---

## 🎓 Compétences acquises

- Utilisation avancée de **Google** (dorking)
- Exploration d’outils publics comme `crt.sh`, `whois`, `dnsdumpster`
- Recherches sur les réseaux sociaux et dans les archives DNS
- Découverte passive d’informations exploitables (emails, services, CVEs)

---

## ⚒️ Outils et ressources utilisés

| Outil | Utilité |
|-------|--------|
| `Google Dorks` | Recherche ciblée sur le contenu web indexé |
| `crt.sh` | Recherche de certificats SSL liés à un domaine |
| `dnsdumpster` | Cartographie DNS d’un domaine |
| `whois` | Informations sur un nom de domaine ou une IP |
| `theHarvester` | Collecte d'emails, noms de domaines et sous-domaines |
| `social media` | Recherche d’identité, pseudonymes, historiques |

---

## 🔍 Google Dorks – exemples pratiques

```text
site:example.com inurl:login
filetype:pdf site:gov "password"
intitle:index.of site:edu confidential
```

💡 Ces requêtes permettent de :
- Trouver des pages de connexion non sécurisées
- Explorer des documents PDF indexés contenant des mots sensibles
- Lister des répertoires accessibles en clair

---

## 🧪 Scénario simulé

**Mission :** Un pseudonyme a été repéré sur un forum.  
Tu dois en apprendre plus sans interagir directement (renseignement passif).

**Méthodes utilisées :**
- Recherche du pseudo via Google avec `site:` et `intitle:`
- Consultation des résultats sur `crt.sh` → domaine lié
- Recherche WHOIS sur le domaine
- Résolution DNS → découverte de sous-domaines
- Recherche sur Twitter → image de profil et prénom trouvés

Résultat : en croisant les données, identité probable trouvée.

---

## ✅ Recommandations (vue analyste OSINT)

- Croiser les sources pour confirmer une information
- Ne jamais se baser sur une seule plateforme (Twitter ≠ LinkedIn ≠ Whois)
- Éviter de se connecter ou d’interagir : privilégier la **veille passive**
- Garder une trace des recherches (journal de collecte + date)
- Vérifier les informations avec des bases publiques comme HaveIBeenPwned

---

## 📘 Astuces OSINT utiles

- Utiliser des **machines virtuelles anonymes** pour vos recherches
- Rester dans la **légalité** : pas d’accès sans autorisation, même public
- Enquêter sur un **projet GitHub** peut révéler des infos (auteurs, emails…)
- Penser à chercher les **anciennes versions de sites** sur [archive.org](https://web.archive.org)

---

## 🔚 Conclusion personnelle

Cette room m’a appris à mener des recherches OSINT structurées et efficaces, sans interaction directe.  
C’est une compétence précieuse autant en **phase de reconnaissance** dans un pentest que pour un travail de **threat hunting** ou d’enquête cyber.

---

**Lien TryHackMe :** [Search Skills](https://tryhackme.com/room/searchskills)
