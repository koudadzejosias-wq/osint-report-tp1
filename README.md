# 🛡️ Rapport d'Enquête OSINT — TP 1

**Auteur :** koudadzejosias-wq  
**Date :** 04 juin 2026  
**Cible initiale :** Bakugo katsuki   
**Statut :** Finalisé (TLP:CLEAR)

---

## 📌 Résumé Exécutif
[cite_start]À partir d'un simple pseudonyme initial trouvé sur un forum, une investigation en sources ouvertes (OSINT) a été menée pour cartographier l'empreinte numérique de la cible[cite: 2, 8]. [cite_start]Grâce au pivotement d'identifiants, trois profils actifs ont été isolés[cite: 4, 16]. [cite_start]Une analyse approfondie des métadonnées (EXIF) a également été menée sur les fichiers multimédias publiés par la cible afin d'évaluer les risques de fuite géographique[cite: 5, 17, 19].

---

## 🔍 Méthodologie & Limites Techniques
1. [cite_start]**Username Hunting (Traque d'identifiants) :** Utilisation de l'outil automatisé **Sherlock** pour scanner la présence de l'alias sur plus de 400 plateformes[cite: 9].
2. [cite_start]**Analyse EXIF :** Utilisation de l'utilitaire **ExifTool** pour inspecter la structure binaire des images publiées[cite: 23, 26].

### ⚠️ Limites de l'enquête (Notes de l'Analyste)
* **Avertissement Faux Positifs :** Avec l'outil SHERLOCK, il est impossible de garantir à 100 % que tous les profils découverts appartiennent à une seule et même personne physique (homonymie ou réutilisation d'alias par des tiers).
* **Murs d'authentification :** Certains sites web exigent la création d'un compte utilisateur pour accéder aux détails du profil, limitant la collecte passive immédiate.

---

## 🕵️‍♂️ Résultats de la Traque (Sherlock)

[cite_start]Le balayage automatisé sur la cible `hacker_target2026` a retourné les vecteurs pivots suivants[cite: 15, 16]:

| Plateforme | URL du profil |
| :--- | :--- |
| **LessWrong** | https://www.lesswrong.com/users/hacker_target2026 |
| **Wikipedia** | https://en.wikipedia.org/wiki/Special:CentralAuth/hacker_target2026 |
| **omg.lol** | https://hacker_target2026.omg.lol |

---

## 🗺️ Analyse de Géolocalisation (GEOINT)
[cite_start]L'image de profil et les fichiers multimédias récupérés et analysés via ExifTool **ne contenaient pas de coordonnées GPS valides**[cite: 28, 29]. 

* [cite_start]**Constat :** Les métadonnées de localisation ont probablement été purgées automatiquement par les serveurs des plateformes lors du téléversement (mécanisme de protection standard des réseaux sociaux modernes), ou la fonction de géolocalisation était désactivée sur l'appareil de la cible lors de la prise de vue[cite: 19].

---

## 🧰 Outils Utilisés
* [cite_start]**Sherlock** – Recherche et corrélation de pseudonymes sur plus de 400 plateformes[cite: 9].
* [cite_start]**ExifTool** – Extraction et analyse des métadonnées binaires[cite: 23, 45].
* [cite_start]**Git / GitHub** – Gestion de version, traçabilité de l'enquête et livraison du rapport[cite: 31, 33].
