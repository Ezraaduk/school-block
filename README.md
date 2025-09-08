# School-Block

**School-Block** est une application de contrôle et de sécurisation des ordinateurs en environnement scolaire ou professionnel. Conçue pour offrir un espace de travail numérique adapté aux cours, examens et sessions de travail encadrées, elle permet de restreindre l’accès aux applications, à Internet et au copier-coller, tout en garantissant la sécurité des données utilisateur et la simplicité de déploiement.

---

## Table des matières

1. [Présentation](#présentation)  
2. [Fonctionnalités principales](#fonctionnalités-principales)  
3. [Installation](#installation)  
4. [Mise à jour](#mise-à-jour)  
5. [Configuration et utilisation](#configuration-et-utilisation)  
6. [Sécurité et permissions](#sécurité-et-permissions)  
7. [Dépendances](#dépendances)  
8. [Contact](#contact)

---

## Présentation

School-Block est un outil complet de gestion et de contrôle des ordinateurs utilisés dans un cadre éducatif ou professionnel. Son objectif principal est de sécuriser l’environnement numérique des utilisateurs en offrant les fonctionnalités suivantes :

- **Blocage d’Internet** pour éviter les distractions ou les triches pendant les examens.
- **Restriction des applications non autorisées** pour limiter l’usage aux programmes essentiels.
- **Sécurisation du copier-coller** afin d’empêcher le transfert non autorisé de données.
- **Surveillance en temps réel** pour informer les administrateurs des applications ouvertes ou des tentatives d’accès interdit.
- **Interface conviviale** avec un installateur simple et des messages clairs.

L’application est conçue pour fonctionner sur Windows, avec un minimum d’intervention de la part de l’utilisateur final.

---

## Fonctionnalités principales

1. **Restreint l'accès aux ressources provenant d'Internet**
   - Force l'activation du mode avion. (Sur ordinateur portable uniquement)
   - Heures de travail configurable (L'application est bloquée en dehors des heures de travail définie.)
   - Blocage du presse-papiers.

3. **Sécurité et contrôle**
   - Vérification régulière (toutes les 10 secondes) qu'aucun programmes bloqué soit ouvert lors d'un examen.
   - Blocage de l’accès à Internet via fermeture des navigateurs autorisés ou interdits.
   - Gestion par clé USB administrateur pour accéder aux fonctionnalités avancées, paramètres sensible de l'application.

4. **Interface utilisateur**
   - Fenêtre principale claire avec couleurs définie pour chaque état des clés USB.
   - Paramètres de configuration réuni en une seule fenêtre.
   - Boutons pour accéder aux tutoriels, depuis l'application.

5. **Compatibilité et administration**
   - Vérification automatique des droits administrateur et relance avec élévation si nécessaire.
   - Compatible avec Windows 10 et versions ultérieures.
   - Déploiement facile dans `C:\Program Files\School-Block`.

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
- Les mises à jour ne suppriment jamais les fichiers `.json` et `.csv` existants, nécessaire à l'enregistrement des paramètres de l'application.
- L’accès aux fonctionnalités avancées est sécurisé via clés USB.

---

## Dépendances

- Python 3.10+
- Modules Python requis :
  - `requests`
  - `psutil`
  - `natsort`
  - `pywin32`
- Windows 10 ou supérieur recommandé.

---

## Contact

- **Auteur** : Ezraa  
- **Email** : `bruttomesso.enzo@gmail.com`
- **GitHub** : [https://github.com/Ezraaduk](https://github.com/Ezraaduk)

---

**Remarque :**  
School-Block est conçu pour un usage éducatif et professionnel. L’administrateur doit informer les utilisateurs des
