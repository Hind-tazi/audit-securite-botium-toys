# Audit de Sécurité Interne – Botium Toys

## 1. Présentation et Contexte

**Entreprise auditée :** Botium Toys  
**Date de l’audit :** 03/05/2025  
**Auditeur :** [Ton nom ici]  
**Cadre de référence :** NIST Cybersecurity Framework (NIST CSF)

**Contexte :**  
Botium Toys est une petite entreprise américaine qui développe et vend des jouets. L'entreprise dispose d'un seul site physique (bureau principal, vitrine, entrepôt) mais sa présence en ligne s'est développée, attirant des clients aux États-Unis et à l'étranger. Le serveur d'authentification du département informatique est donc soumis à une pression croissante. La responsable informatique souhaite réaliser un audit interne pour mieux sécuriser l'infrastructure, identifier les risques, et assurer la conformité avec les réglementations (paiements en ligne, RGPD...).

---

## 2. Portée et Objectifs de l’Audit

### 2.1 Portée

L’audit couvre :
- Les équipements sur site et les appareils des employés
- Le réseau interne et l’accès Internet
- Les systèmes de gestion (comptabilité, e-commerce, gestion des stocks, sécurité)
- Les dispositifs physiques (caméras, serrures, alarmes, etc.)
- Les procédures de traitement et de stockage des données

### 2.2 Objectifs

- Évaluer la posture de sécurité actuelle de Botium Toys
- Identifier les risques, menaces et vulnérabilités affectant les actifs critiques
- Vérifier la conformité avec les réglementations (PCI DSS, RGPD, SOC)
- Proposer des recommandations pour améliorer la sécurité et la conformité

---

## 3. Actifs Gérés par le Service Informatique

- **Équipements sur site** : serveurs, postes, périphériques réseau
- **Appareils des employés** : ordinateurs, portables, smartphones, casques, etc.
- **Produits en magasin** : stockés dans l’entrepôt, disponibles à la vente
- **Systèmes de gestion** : comptabilité, télécommunications, bases de données, sécurité, e-commerce, gestion des stocks
- **Accès Internet**
- **Réseau interne**
- **Conservation et stockage des données**
- **Maintenance des systèmes existants** : systèmes en fin de vie nécessitant une surveillance humaine

---

## 4. Catégories et Types de Contrôles

### 4.1 Contrôles Administratifs / de Gestion

| Contrôle                        | Type        | Objectif |
|----------------------------------|-------------|----------|
| Moindre privilège                | Préventif   | Réduire le risque de comptes malveillants ou compromis |
| Plans de reprise après sinistre  | Correctif   | Assurer la continuité des activités |
| Politiques de mots de passe      | Préventif   | Réduire le risque de compromission de compte |
| Politiques de contrôle d'accès   | Préventif   | Renforcer la confidentialité et l'intégrité des données |
| Politiques de gestion des comptes| Préventif   | Gérer le cycle de vie des comptes |
| Séparation des tâches            | Préventif   | Réduire le risque de fraude interne |

### 4.2 Contrôles Techniques

| Contrôle                         | Type        | Objectif |
|-----------------------------------|-------------|----------|
| Pare-feu                         | Préventif   | Bloquer le trafic indésirable/malveillant |
| Détecteur IDS/IPS                | Détectif/Préventif | Détecter et prévenir les attaques réseau |
| Chiffrement                      | Dissuasif   | Assurer la confidentialité des informations sensibles |
| Sauvegardes                      | Correctif   | Restauration après incident |
| Gestion des mots de passe        | Préventif   | Réduire les risques liés aux mots de passe faibles |
| Logiciel antivirus               | Préventif   | Détecter et mettre en quarantaine les menaces |
| Surveillance & maintenance manuelle| Préventif | Identifier et gérer les menaces sur les systèmes obsolètes |

### 4.3 Contrôles Physiques / Opérationnels

| Contrôle                         | Type        | Objectif |
|-----------------------------------|-------------|----------|
| Coffre-fort temporisé             | Dissuasif   | Protéger les actifs physiques |
| Éclairage adéquat                 | Dissuasif   | Réduire les risques d’intrusion |
| Caméras de surveillance (CCTV)    | Préventif/Détectif | Dissuader et détecter les incidents |
| Armoires verrouillables           | Préventif   | Protéger les équipements réseau |
| Panneaux d’alarme                 | Dissuasif   | Dissuader les intrusions |
| Verrous                           | Dissuasif/Préventif | Limiter l’accès physique |
| Détection/prévention incendie     | Détectif/Préventif | Protéger contre les incendies |

---

## 5. Liste de Contrôle des Contrôles de Sécurité

Réponds "Oui" ou "Non" selon l’état actuel chez Botium Toys :

| Contrôle                                                  | Oui | Non |
|-----------------------------------------------------------|:---:|:---:|
| Moindre privilège                                         |  X  |     |
| Plans de reprise après sinistre                           |     |  X  |
| Politiques de gestion des mots de passe                   |  X  |     |
| Séparation des tâches                                     |  X  |     |
| Pare-feu                                                  |  X  |     |
| Système de détection d'intrusion (IDS)                    |     |  X  |
| Sauvegardes régulières                                    |  X  |     |
| Logiciel antivirus                                        |  X  |     |
| Surveillance/maintenance manuelle (systèmes existants)    |  X  |     |
| Chiffrement                                               |     |  X  |
| Système de gestion des mots de passe                      |     |  X  |
| Serrures (bureaux, vitrine, entrepôt)                     |  X  |     |
| Système de vidéosurveillance (CCTV)                       |  X  |     |
| Détection/prévention incendie (alarme, gicleurs, etc.)    |  X  |     |

---

## 6. Liste de Contrôle de Conformité

### 6.1 PCI DSS (Paiements par carte)

| Bonne pratique                                                                | Oui | Non |
|-------------------------------------------------------------------------------|:---:|:---:|
| Seuls les utilisateurs autorisés ont accès aux infos de carte de crédit       |  X  |     |
| Infos de carte stockées, acceptées, traitées et transmises de façon sécurisée |  X  |     |
| Chiffrement des données de transaction                                        |     |  X  |
| Politiques de gestion des mots de passe sécurisées                            |  X  |     |

### 6.2 RGPD (Clients UE)

| Bonne pratique                                                                | Oui | Non |
|-------------------------------------------------------------------------------|:---:|:---:|
| Données clients UE confidentielles et sécurisées                              |  X  |     |
| Plan de notification en cas de violation sous 72h                             |     |  X  |
| Données correctement classées et inventoriées                                 |  X  |     |
| Politiques/processus de confidentialité documentés                            |     |  X  |

### 6.3 SOC 1 / SOC 2

| Bonne pratique                                                                | Oui | Non |
|-------------------------------------------------------------------------------|:---:|:---:|
| Politiques d’accès utilisateur établies                                       |  X  |     |
| Données sensibles (PII/SPII) confidentielles                                  |  X  |     |
| Intégrité des données (cohérence, exactitude, validation)                     |  X  |     |
| Accès aux données réservé aux personnes autorisées                            |  X  |     |

---

## 7. Recommandations

1. **Mettre à jour et tester les plans de reprise après sinistre**  
   - Documenter les procédures de sauvegarde/restauration, faire des tests réguliers.

2. **Déployer un système de détection d’intrusion (IDS)**  
   - Installer et configurer un IDS pour surveiller le réseau et détecter les attaques.

3. **Mettre en place le chiffrement des données sensibles**  
   - Chiffrer les bases de données clients et les transactions de paiement.

4. **Mettre en place un système de gestion des mots de passe**  
   - Utiliser un gestionnaire de mots de passe sécurisé pour tous les employés.

5. **Documenter un plan de notification RGPD**  
   - Préparer une procédure pour informer les clients UE en cas de fuite de données.

6. **Former le personnel à la sécurité et à la confidentialité**  
   - Organiser des sessions de sensibilisation régulières.

---

## 8. Conclusion

Cet audit a permis d’identifier les points forts et les axes d’amélioration de la sécurité chez Botium Toys.  
La mise en œuvre des recommandations ci-dessus permettra de renforcer la posture de sécurité, de réduire les risques et d’assurer la conformité réglementaire.

**Prochaine étape :** Suivi de la mise en œuvre des recommandations et réévaluation dans 12 mois.

---
l'audit de sécurité Botium Toys)
