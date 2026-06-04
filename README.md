\# 🛡️ Rapport d'Enquête Cyber-Renseignement (OSINT) — TP 1



\*\*Date du rapport :\*\* 04 juin 2026  

\*\*Statut :\*\* Finalisé  

\*\*Classification :\*\* TLP:CLEAR (Public)  

\*\*Auteur :\*\* Analyste Cyber



\---



\## 📑 1. Résumé Exécutif

Ce rapport documente les opérations de collecte de renseignement d'origine source ouverte (OSINT) menées à l'encontre de l'identifiant cible `hacker\_target2026`. L'investigation a permis de cartographier l'empreinte numérique de la cible à travers plusieurs plateformes tierces et de définir la méthodologie requise pour son identification géographique.



\---



\## 🔍 2. Phase 1 : Pivotement d'Identifiants (Username Hunting)



\### 2.1 Méthodologie et Outillage

Une campagne de corrélation d'identifiants a été exécutée à l'aide de l'outil de balayage open-source \*\*Sherlock\*\*. Cet outil automatise la détection de profils sur plus de 400 plateformes en mesurant les codes de réponse HTTP.



```cmd

python -m sherlock\_project hacker\_target2026 --timeout 5

