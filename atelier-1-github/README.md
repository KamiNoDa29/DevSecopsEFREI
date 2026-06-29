# Atelier 1 — GitHub

Reprend l'atelier "Atelier sur GitHub" (EFREI Paris).

## Contenu déjà prêt dans ce dossier

Un projet Spring Boot minimal généré comme si vous l'aviez téléchargé depuis https://start.spring.io/ (équivalent du point "Télécharger un code springboot-maven").

- `pom.xml`
- `src/main/java/com/example/demo/DemoApplication.java`
- `src/test/java/com/example/demo/DemoApplicationTests.java`
- `.gitignore`

## Ce qu'il vous reste à faire vous-même

### 1. Créer un compte GitHub
Allez sur https://github.com/login et créez votre compte si ce n'est pas déjà fait.

### 2. Créer un repository
1. Cliquez sur votre photo de profil (en haut à droite) → **Your repositories**.
2. Cliquez sur **Create repository** (ou **New**).
3. Renseignez :
   - le **nom** de votre projet (ex : `demo`)
   - une **description**
4. Cliquez sur **Create repository**.

### 3. Lier votre code local au repository
GitHub affiche des commandes après la création. Placez-vous dans ce dossier (`atelier-1-github`) puis exécutez :

```bash
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/<votre-utilisateur>/<votre-repo>.git
git push -u origin main
```

> **NB 1** : pas besoin d'exécuter la commande `echo ... >> README.md` proposée par GitHub.
> **NB 2** : au lieu de `git add README.md`, utilisez bien `git add .` pour ajouter tout le projet.

### 4. Vérifier la structure
Une fois le push effectué, vérifiez sur GitHub que vous avez bien cette structure à la racine du repository :
```
demo/
├── pom.xml
├── .gitignore
└── src/
    ├── main/java/com/example/demo/DemoApplication.java
    └── test/java/com/example/demo/DemoApplicationTests.java
```

## Défis

### Défi 01 — Créer une organisation GitHub
1. Cliquez sur votre photo de profil → **Your organizations**.
2. Cliquez sur **New organization**.
3. Choisissez un plan (gratuit ou payant selon vos besoins).
4. Donnez un nom à votre organisation + une adresse email.
5. Suivez les instructions pour finaliser la création.

### Défi 02 — Ajouter des utilisateurs à votre organisation
1. Allez sur la page de votre organisation.
2. Cliquez sur **People** dans le menu latéral gauche.
3. Cliquez sur **Invite member**.
4. Entrez le nom d'utilisateur GitHub ou l'email de la personne à inviter.
5. Cliquez sur **Send Invitation**.

### Défi 03 — Créer une équipe (Teams)
1. Allez sur la page de votre organisation.
2. Cliquez sur **Teams** dans le menu latéral gauche.
3. Cliquez sur **New team**.
4. Donnez un nom à l'équipe (ex : "Développeurs", "Admins").
5. Ajoutez une description si besoin.
6. Cliquez sur **Create team**.
