# School-Block

School-Block est un outil conçu pour surveiller, sécuriser les ordinateurs dans un environnement de formation.
En offrant un espace de travail numérique adapté aux cours, aux examens et sessions de travail encadrées.

---

## Table des matières

1. [Présentation](#présentation)  
2. [Fonctionnalités principales](#fonctionnalités-principales)  
3. [Installation](#installation)  
4. [Mise à jour](#mise-à-jour)  
5. [Configuration et utilisation](#configuration-et-utilisation)  
6. [Sécurité et permissions](#sécurité-et-permissions)  
7. [FAQ](#faq)  
8. [Dépannage](#dépannage)  
9. [Contact](#contact)

---

## Présentation

School-Block est un outil complet de gestion et de contrôle des ordinateurs utilisés dans un cadre éducatif / scolaire.

L'objectif principal est de sécuriser l’environnement numérique lors des examens théorique, offrant les fonctionnalités suivantes :

- Le **blocage d’Internet**, en forçant le mode avion à être actif. (Ordinateur fixe incompatibles.)
- La **Restriction des applications non autorisées** pour limiter l’usage aux programmes essentiels.
- **Sécurisation du copier-coller** afin d’empêcher le transfert non autorisé de données d'un fichier texte pré-écrit.
- **Surveillance en temps réel** pour informer le personnel éducatif, des applications ouvertes ou des tentatives d’accès interdit. (Bloque l'ordinateur)
- **Interface simplifiée** avec un installateur simple et des messages clairs.

L’application est conçue pour fonctionner sur Windows, (compatibilité non testée sur Mac OS et Linux), avec un minimum d’intervention de la part de l’utilisateur final. L'élève, n'a pas besoin d'intervenir sur l'application une fois configurée par le personnel éducatif.

---

## Fonctionnalités principales

1. **Restreint l'accès aux ressources provenant d'Internet**
   - Blocage des navigateurs et des applications Internet non autorisées. (Il est possible de forcé le mode avion sur ordinateur portable.)
   - Gestion des heures de travail : l’application peut être configurée pour fonctionner uniquement pendant certaines plages horaires.
   - Blocage du presse-papiers pour empêcher le copier-coller de contenu sensible.

2. **Sécurité et contrôle**
   - Vérification régulière (toutes les 10 secondes) qu'aucun programmes bloqués ne soient ouverts.
   - Gestion par clé USB administrateur pour accéder aux fonctionnalités avancées.
   - Blocage de l'ordinateur et avertissements lorsque des actions non autorisées sont détectées. (Un professeur, devra intervenir.)

3. **Interface utilisateur**
   - Fenêtre principale claire avec des couleurs et indicateurs pour chaque état de clé USB.
       - Vert : Clés configurées en tant que clés administrateur, connectée. (Aucune clés ne doit apparaitre vert sur l'application durant l'examen.)
       - Rouge : Clés configurées en tant que clés administrateur, mais déconnectée.
       - Bleu : Clés connectées à l'ordinateur disponible.
   - Accès facile aux tutoriels et guides intégrés.
   - Historique des versions et release notes directement consultables depuis l’interface.

4. **Compatibilité et administration**
   - Vérification automatique des droits administrateur et relance avec élévation si nécessaire.
   - Compatible avec Windows 10 et versions ultérieures.
   - Déploiement facile dans `C:\Program Files\School-Block`.
   - Raccourci bureau automatique après installation ou mise à jour.

---

## Installation

1. Téléchargez **School-Block** depuis le dépôt GitHub :  
   [Lien vers l’exécutable](https://github.com/Ezraaduk/school-block)

2. Exécutez l’installateur **en tant qu’administrateur**.

3. L’installateur vérifiera automatiquement :
   - Si `School-Block.exe` est ouvert (le bouton de mise à jour sera désactivé tant qu’il est détecté).
   - La présence de fichiers de configuration existants pour les sauvegarder temporairement.

4. L’installation inclut :
   - Téléchargement de l’exécutable principal.
   - Téléchargement du paquet `_internal.zip` contenant toutes les ressources.
   - Extraction et restauration des fichiers de configuration.
   - Création d’un raccourci sur le bureau.

---

## Mise à jour

- L’installateur détecte automatiquement la version plus récente sur GitHub.
- Les fichiers de configuration existants (`.json`, `.csv`) sont sauvegardés avant la mise à jour et restaurés après extraction.
- Le bouton **Mettre à jour** devient actif uniquement si `School-Block.exe` n’est pas en cours d’exécution.

---

## Configuration et utilisation

- **Fichiers de configuration**  
  Les configurations sont stockées dans le dossier `_internal` de l’application. Les fichiers `.json` et `.csv` contiennent :
  - Clés USB administrateur
  - Paramètres de blocage
  - Listes d’applications autorisées/interdites

- **Interface**
  - **Aide** : ouvre le guide interactif avec tous les thèmes disponibles.
  - **Versions** : affiche les release notes récentes pour suivre les modifications.
  - **Progression** : barre indiquant le téléchargement et l’extraction des fichiers.
  - **Avertissement** : label rouge pour indiquer si `School-Block.exe` est ouvert. (il est impossible de mettre à jour l'application si elle est ouverte.)

- **Exécution**
  - Double-cliquez sur le raccourci créé sur le bureau pour lancer l’application.
  - Seules les clés USB administrateur enregistrées permettent de modifier les paramètres avancés.

---

## Sécurité et permissions

- Nécessite les droits administrateur pour installer et mettre à jour le logiciel.
- Les mises à jour ne suppriment jamais les fichiers `.json` et `.csv` existants, nécessaires à l'enregistrement des paramètres de l'application.
- L’accès aux fonctionnalités avancées est sécurisé via clés USB.
- L’application ne collecte aucune donnée personnelle.

---

## FAQ

**Q : Puis-je installer School-Block sur plusieurs ordinateurs avec la même clé USB ?**  
R : Oui, les clés USB administrateur peuvent être utilisées sur plusieurs machines, mais chaque configuration est locale à l’ordinateur.

**Q : Que faire si l’application ne se lance pas ?**  
R : Vérifiez que vous avez les droits administrateur et que `School-Block.exe` n’est pas déjà en cours d’exécution. Consultez également le journal d’erreurs si disponible.

**Q : Puis-je modifier les fichiers `.json` directement ?**  
R : Il est possible de modifier certains fichiers de configuration, mais il est recommandé d’utiliser l’interface pour éviter toute incohérence.

---

## Dépannage

1. **Erreur de mise à jour : “School-Block est ouvert”**
   - Fermez tous les processus `School-Block.exe`.
   - Vérifiez dans le gestionnaire de tâches qu’aucun processus fantôme n’est actif.

2. **Problème de téléchargement de `_internal.zip`**
   - Vérifiez votre connexion Internet.
   - Assurez-vous que l’antivirus ne bloque pas le téléchargement.

3. **Problèmes de permissions**
   - Exécutez l’installateur en tant qu’administrateur.
   - Assurez-vous que vous avez accès au dossier `C:\Program Files\School-Block`.

4. **Raccourci bureau absent**
   - L’exécutable principal est présent dans le dossier d’installation ? Si oui, créez manuellement un raccourci.

---

## Contact

- **Auteur** : Ezraa  
- **Email** : `bruttomesso.enzo@gmail.com`  
- **GitHub** : [https://github.com/Ezraaduk](https://github.com/Ezraaduk)

---

**Remarque :**  
School-Block est conçu pour un usage éducatif et professionnel. L’administrateur, le professeur, doit informer l'élève du blocage mit en place.
