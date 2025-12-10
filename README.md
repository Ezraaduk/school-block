# School-Block

School-Block est un outil conçu pour surveiller, sécuriser les ordinateurs dans un environnement de formation.
En offrant un espace de travail numérique adapté aux cours, aux examens et sessions de travail encadrées.

---

## Table des matières

1. [Présentation](#présentation)  
2. [Installation](#installation)  
3. [Première utilisation](#Première-utilisation)
4. [Fonctionnalités principales](#fonctionnalités-principales)
5. [Fonctionnalités principales](#fonctionnalités-principales)
6. [Mise à jour](#mise-à-jour)  
7. [Sécurité et permissions](#sécurité-et-permissions)  
8. [Dépannage](#dépannage)
9. [FAQ](#faq)
10. [Contact](#contact)

---

## Présentation

School-Block est un outil complet de gestion et de contrôle des ordinateurs utilisés dans un cadre scolaire ou formatif.

L'objectif principal est de sécuriser l’environnement numérique lors des examens théorique, cours informatique, offrant les fonctionnalités suivantes :

- Le **blocage d’Internet**, en forçant le mode avion à être actif. (Ordinateur fixe incompatibles.)
- La **Restriction des applications non autorisées** pour limiter l’usage aux programmes essentiels.
- **Sécurisation du copier-coller** afin d’empêcher le transfert non autorisé de données d'un fichier texte pré-écrit.
- **Surveillance en temps réel** pour informer le personnel éducatif, des applications ouvertes ou des tentatives d’accès interdit. (Bloque l'ordinateur)
- **Interface simplifiée** avec un installateur simple et des messages clairs.

L’application est conçue pour fonctionner sur Windows, avec un minimum d’intervention de l'équipe éducative. L'élève, n'a pas besoin d'intervenir sur l'application une fois configurée.

---

## Installation

1. L'installation comprend : 
   - Le téléchargement de l'application principale et de ses dépendances.
   - Création d'un raccourci sur le bureau.

2. Le programme d'installation vérifie :
   - Que le programme `School-Block.exe` ne soit pas ouvert, pour permettre la mise à jour.
   - La présence de fichiers de configuration existants pour les sauvegarder temporairement en cas de mise à jour, pour conserver la configuration.
  
3. **Guide d'installation** :
Pour installer ou mettre à jour l'application, vous devez simplement cliquer sur "Installer" ou "Mettre à jour". 
Pensez également à vérifier une connexion internet stable, et n'ouvrez pas l'application pendant la mise à jour.

4. Options complémentaires :
Le programme d'installation permet également de consulter le journal d'édition et le guide d'usage de l'application.

---

## Première utilisation

- **Configurer l'application**  
  Lors du premier lancement de l'application, celle-ci vous demandera de la configurer, pour cela :
  - Insérez une clé USB dans l'un des ports prévus pour et sélectionnez-la, pour définir la clé en tant que clé administrateur. (Vous devrez insérer la clé USB pour ouvrir l'application et configurer le mode examen de l'application.
 
---

## Fonctionnalités principales

1. **Restreint l'accès aux ressources provenant d'Internet** :
   - Blocage des navigateurs et des applications Internet non autorisées. (Il est possible de forcé le mode avion sur ordinateur portable.)
   - Gestion des heures de travail : l’application peut être configurée pour fonctionner uniquement pendant certaines plages horaires.
   - Blocage du presse-papiers pour empêcher le copier-coller de contenu sensible.

2. **Sécurité et contrôle**
   - Vérification régulière (toutes les 10 secondes) qu'aucun programmes bloqués ne soit ouverts.
   - Gestion par clé USB administrateur pour accéder aux fonctionnalités avancées.
   - Blocage de l'ordinateur et avertissements lorsque des actions non autorisées sont détectées. (L'équipe éducative devra intervenir sur l'ordinateur)
     
3. **Interface utilisateur**
   - Fenêtre principale claire avec des couleurs et indicateurs pour chaque état de clé USB.
       - Vert : Clés configurées en tant que clés administrateur, connectée. (Aucune clés ne doit apparaitre vert sur l'application durant l'examen.)
       - Rouge : Clés configurées en tant que clés administrateur, mais déconnectée.
       - Bleu : Clés connectées à l'ordinateur disponible.

4. **Compatibilité et administration**
   - Vérification automatique des droits administrateur et relance avec élévation si nécessaire.
   - Compatible avec Windows 10 et versions ultérieures.

---

## Mise à jour

- L’installateur détecte automatiquement la version plus récente sur GitHub.
- Les fichiers de sauvegarde existants sont sauvegardés avant la mise à jour et sont ensuite restaurés une fois la mise à jour terminée.
- Le bouton **Mettre à jour** devient actif uniquement si `School-Block.exe` n’est pas en cours d’exécution.

---

## Sécurité et permissions

- Nécessite les droits administrateur pour utiliser convenablement l'application.
- Les mises à jour ne suppriment jamais les fichiers `.json` et `.csv` existants, nécessaires à l'enregistrement des paramètres de l'application.
- L’accès aux fonctionnalités avancées est sécurisé via clés USB.
- L’application ne collecte aucune donnée personnelle.

---

## Dépannage

1. **Erreur de mise à jour : “School-Block est ouvert”**
   - Fermez tous les processus `School-Block.exe` depuis les gestionnaire de tâches si l'erreur persiste.

2. **Problème de téléchargement de `_internal.zip`**
   - Vérifiez votre connexion Internet.
   - Assurez-vous que l’antivirus ne bloque pas le téléchargement.

3. **Problèmes de permissions**
   - Exécutez l’installateur en tant qu’administrateur.
   - Assurez-vous que vous avez accès au dossier `C:\Program Files\School-Block`.

---

## FAQ

**Q : Puis-je installer School-Block sur plusieurs ordinateurs avec la même clé USB ?**  
R : Oui, les clés USB administrateur peuvent être utilisées sur plusieurs machines, mais chaque configuration est locale à l’ordinateur.

**Q : Que faire si l’application ne se lance pas ?**  
R : Vérifiez que vous avez les droits administrateur et que `School-Block.exe` n’est pas déjà en cours d’exécution.

**Q : Puis-je modifier les fichiers `.json` directement ?**  
R : Il est possible de modifier certains fichiers de configuration, mais il est recommandé d’utiliser l’interface pour éviter toute incohérence.

---

## Contact

- **Auteur** : Ezraa  
- **Email** : `bruttomesso.enzo@gmail.com`  
- **GitHub** : [https://github.com/Ezraaduk](https://github.com/Ezraaduk)

---

**Remarque :**  
School-Block est conçu pour un usage éducatif et professionnel. L’administrateur, le professeur, doit informer l'élève du blocage mit en place.
