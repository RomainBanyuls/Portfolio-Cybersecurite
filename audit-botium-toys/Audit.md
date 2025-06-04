# 🛡️ Audit de sécurité interne – Botium Toys

> Réalisé dans le cadre d'une mise en pratique du cadre NIST Cybersecurity Framework (CSF)

---

## 📋 Sommaire

- [📘 Présentation de l'entreprise](#-présentation-de-lentreprise)
- [🎯 Objectifs de l'audit](#-objectifs-de-laudit)
- [🛑 Périmètre et risques identifiés](#-périmètre-et-risques-identifiés)
- [🔍 Résultat de l’évaluation des contrôles (NIST CSF)](#-résultat-de-lévaluation-des-contrôles-nist-csf)
- [📃 Conformité réglementaire (PCI DSS, RGPD, SOC)](#-conformité-réglementaire-pci-dss-rgpd-soc)
- [🛠️ Recommandations stratégiques](#️-recommandations-stratégiques)
- [✅ Auto-évaluation](#-auto-évaluation)
- [📌 Résumé](#-résumé)

---

## 📘 Présentation de l'entreprise

**Botium Toys** est une entreprise de vente de jouets avec un magasin physique et une activité e-commerce. Elle gère un ensemble d’actifs informatiques, dont :

- Équipements sur site
- Appareils des employés (ordinateurs, téléphones…)
- Systèmes de gestion (comptabilité, e-commerce, sécurité, etc.)
- Réseau interne, bases de données, stockage, systèmes obsolètes

---

## 🎯 Objectifs de l'audit

- Identifier les actifs à sécuriser
- Évaluer les risques critiques
- Analyser la conformité aux bonnes pratiques de sécurité
- Appliquer le NIST CSF (5 fonctions clés)
- Proposer des recommandations concrètes

---

## 🛑 Périmètre et risques identifiés

**Périmètre :** l’ensemble du système d’information, y compris les processus humains et techniques.  
**Score de risque estimé :** 8/10  
**Risques critiques détectés :**

- Données clients accessibles à tous les employés
- Absence d’IDS, de chiffrement et de sauvegarde
- Politiques de mot de passe insuffisantes
- Manque de gestion proactive des systèmes obsolètes

---

## 🔍 Résultat de l’évaluation des contrôles (NIST CSF)

| Fonction NIST | Contrôle                               | En place | Bonne pratique | Recommandation |
|---------------|----------------------------------------|----------|----------------|----------------|
| Identifier    | Privilège minimal                      | ❌       | ❌             | Implémenter RBAC |
| Identifier    | Séparation des tâches                  | ❌       | ❌             | Clarifier les responsabilités |
| Protéger      | Politique de mot de passe              | ✅       | ❌             | Renforcer les exigences |
| Protéger      | Pare-feu                               | ✅       | ✅             | ✔️ |
| Protéger      | Antivirus                              | ✅       | ✅             | ✔️ |
| Détecter      | Système IDS                            | ❌       | ❌             | Mettre en place un IDS |
| Récupérer     | Plan de reprise                        | ❌       | ❌             | Créer un PRA + sauvegardes |
| Récupérer     | Sauvegardes                            | ❌       | ❌             | Planifier des backups chiffrés |
| Protéger      | Chiffrement des données                | ❌       | ❌             | Implémenter chiffrement AES |
| Protéger      | Gestionnaire de mots de passe          | ❌       | ❌             | Déployer une solution centralisée |
| Identifier    | Maintenance des systèmes obsolètes     | ✅       | ❌             | Mettre en place une procédure régulière |
| Physique      | Sécurité physique (serrures, CCTV…)    | ✅       | ✅             | ✔️ |

---

## 📃 Conformité réglementaire (PCI DSS, RGPD, SOC)

### 🔐 PCI DSS

| Bonnes pratiques | Respectées |
|------------------|------------|
| Accès limité aux données carte bancaire | ❌ |
| Traitement sécurisé | ❌ |
| Données chiffrées | ❌ |
| Politique de mot de passe robuste | ❌ |

### 🇪🇺 RGPD

| Bonnes pratiques | Respectées |
|------------------|------------|
| Protection des données UE | ✅ |
| Notification en cas de violation (72h) | ✅ |
| Classification des données | ❌ |
| Politique de confidentialité en place | ✅ |

### 📊 SOC 1 / SOC 2

| Bonnes pratiques | Respectées |
|------------------|------------|
| Politique d’accès définie | ❌ |
| Protection des données sensibles (PII/SPII) | ❌ |
| Intégrité des données assurée | ✅ |
| Disponibilité pour utilisateurs autorisés | ✅ |

---

## 🛠️ Recommandations stratégiques

- Mettre en place une **politique d’accès par rôle (RBAC)**
- Renforcer la **politique de mot de passe** (complexité, expiration)
- Déployer un **IDS** et une solution de **chiffrement**
- Créer un **plan de reprise d’activité (PRA)** avec sauvegardes régulières
- Centraliser la **gestion des mots de passe** pour les employés et fournisseurs
- Tenir à jour un **inventaire des actifs** classifiés selon leur criticité

---

## ✅ Auto-évaluation

| Critère | Statut |
|---------|--------|
| Analyse de la portée, objectifs et risques | ✅ |
| Prise en compte des actifs et données sensibles | ✅ |
| Application du cadre NIST CSF | ✅ |
| Contrôles évalués (oui/non) | ✅ |
| Bonnes pratiques réglementaires cochées | ✅ |

---

## 📌 Résumé

> Cet audit fictif basé sur ce qu'une entreprise réelle met en œuvre dans le cadre NIST CSF pour évaluer des risques, recommander des contrôles, et analyser la conformité PCI DSS, RGPD et SOC.
> Il démontre ma capacité à structurer une analyse de sécurité complète et à proposer des améliorations concrètes.

✍️ Auteur : [Romain Banyuls](https://github.com/RomainBanyuls)  
📅 Date : Juin 2025

---

