# Guide de Déploiement du Portfolio

Ce document explique comment déployer votre portfolio en ligne en utilisant différentes plateformes gratuites.

## Option 1: GitHub Pages (Recommandé)

GitHub Pages est un service gratuit qui permet d'héberger des sites web statiques directement depuis un dépôt GitHub.

### Prérequis

1. Avoir un compte [GitHub](https://github.com/)
2. Avoir [Git](https://git-scm.com/downloads) installé sur votre ordinateur

### Étapes de déploiement

1. **Créer un nouveau dépôt GitHub**
   - Connectez-vous à votre compte GitHub
   - Cliquez sur le bouton "New" pour créer un nouveau dépôt
   - Nommez votre dépôt `votre-nom-utilisateur.github.io` (remplacez "votre-nom-utilisateur" par votre nom d'utilisateur GitHub)
   - Choisissez l'option "Public"
   - Cliquez sur "Create repository"

2. **Initialiser Git dans votre projet local**
   - Ouvrez un terminal dans le dossier de votre portfolio
   - Exécutez les commandes suivantes :

   ```bash
   git init
   git add .
   git commit -m "Premier commit - Portfolio initial"
   git branch -M main
   git remote add origin https://github.com/votre-nom-utilisateur/votre-nom-utilisateur.github.io.git
   git push -u origin main
   ```

3. **Activer GitHub Pages**
   - Allez dans les paramètres de votre dépôt (onglet "Settings")
   - Faites défiler jusqu'à la section "GitHub Pages"
   - Dans la source, sélectionnez la branche "main" et le dossier "/ (root)"
   - Cliquez sur "Save"
   - Attendez quelques minutes que votre site soit déployé
   - Votre site sera accessible à l'adresse `https://votre-nom-utilisateur.github.io`

## Option 2: Netlify

Netlify est une plateforme qui offre l'hébergement gratuit avec des fonctionnalités avancées.

### Étapes de déploiement

1. **Créer un compte Netlify**
   - Inscrivez-vous sur [Netlify](https://www.netlify.com/)

2. **Déployer votre site**
   - Cliquez sur "New site from Git"
   - Connectez votre compte GitHub
   - Sélectionnez votre dépôt de portfolio
   - Configurez les options de build (laissez vide pour un site statique simple)
   - Cliquez sur "Deploy site"

3. **Personnaliser votre domaine**
   - Dans les paramètres du site, vous pouvez personnaliser le sous-domaine Netlify ou configurer votre propre nom de domaine

## Option 3: Vercel

Vercel est une plateforme optimisée pour les sites web modernes.

### Étapes de déploiement

1. **Créer un compte Vercel**
   - Inscrivez-vous sur [Vercel](https://vercel.com/)

2. **Déployer votre site**
   - Cliquez sur "New Project"
   - Importez votre dépôt GitHub
   - Configurez les paramètres du projet (laissez les valeurs par défaut pour un site statique)
   - Cliquez sur "Deploy"

## Préparation des fichiers pour le déploiement

Avant de déployer votre portfolio, assurez-vous que :

1. Tous les liens dans votre HTML utilisent des chemins relatifs
2. Toutes les images sont correctement référencées
3. Le site fonctionne correctement en local
4. Les fichiers sont bien organisés

## Test après déploiement

Après avoir déployé votre site, vérifiez :

1. Que toutes les pages se chargent correctement
2. Que les images s'affichent
3. Que les animations fonctionnent
4. Que le site est responsive sur différents appareils
5. Que les formulaires fonctionnent (si applicable)

## Mise à jour du site

Pour mettre à jour votre site après des modifications :

1. Effectuez vos changements en local
2. Committez et poussez les modifications vers GitHub :

```bash
git add .
git commit -m "Description des modifications"
git push
```

Le site se mettra à jour automatiquement après quelques minutes.