# Configuration du Formulaire de Contact - Acqua Propreté

Ce projet utilise un formulaire statique sécurisé via **Formspree**. Cela permet de recevoir des emails sans exposer votre adresse Gmail dans le code source et sans avoir besoin d'un serveur (PHP).

## Étape 1 : Créer votre identifiant gratuit
1. Allez sur [https://formspree.io/](https://formspree.io/).
2. Inscrivez-vous gratuitement avec votre adresse Gmail (`acquaproprete@gmail.com`).
3. Cliquez sur **"+ New Form"**.
4. Nommez-le "Contact Site Web" et liez-le à votre email Gmail.
5. Une fois créé, Formspree vous donnera une URL de ce type : `https://formspree.io/f/mjvnpqoa`.

## Étape 2 : Mettre à jour le code HTML
1. Ouvrez votre fichier `nettoyage_site.html`.
2. Recherchez la ligne `<form action="https://formspree.io/f/VOTRE_ID_ICI"`.
3. Remplacez `VOTRE_ID_ICI` par le code à la fin de l'URL fournie par Formspree (ex: `mjvnpqoa`).
4. Enregistrez le fichier.

## Étape 3 : Tests et Sécurité
* **Premier envoi :** Faites un test réel sur le site. Formspree vous demandera de confirmer votre adresse mail la première fois.
* **RGPD :** Les messages sont stockés temporairement sur Formspree. Vous pouvez configurer la suppression automatique dans leurs options pour plus de confidentialité.
* **Anti-Spam :** Le champ caché `_gotcha` dans le code bloque automatiquement les robots qui tentent de remplir le formulaire.

## Hébergement
* **GitHub Pages :** Téléchargez simplement votre fichier `.html` sur votre dépôt GitHub. Le formulaire fonctionnera immédiatement.
* **NAS / Pro :** Aucun changement de code nécessaire, la solution est universelle.
