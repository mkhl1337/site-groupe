# 📝 Exercice Git & GitHub – Collaboration sur une page web simple

## 🎯 Objectif

Apprendre à utiliser Git et GitHub pour :

- créer un dépôt,
- faire des commits,
- travailler avec des branches,
- pousser son travail sur GitHub,
- collaborer et résoudre un conflit.

---

## 📌 Consignes

### 1️⃣ Récupération du projet

- Clonez ce dépôt sur vos machines : https://github.com/houssemRouabeh/site-groupe.git
  ```bash
  git clone https://github.com/houssemRouabeh/site-groupe.git
  cd site-groupe
  ```

### 2️⃣ Création de la base du site (branche `main`)

- Créez un fichier `index.html` avec un titre `<h1>` "Bienvenue sur notre site".
- Créez un fichier `style.css` pour donner une couleur au titre.
- Ajoutez et validez vos fichiers :
  ```bash
  git add .
  git commit -m "Ajout de la structure de base du site"
  git push origin main
  ```

### 3️⃣ Travail en branches personnelles

- Créez une branche à votre prénom :
  ```bash
  git checkout -b prenom
  ```
- Dans `index.html`, ajoutez un paragraphe `<p>` avec votre prénom.
- Faites un commit et poussez votre branche sur GitHub.

### 4️⃣ Pull Request et fusion

- Sur GitHub, ouvrez une **Pull Request (PR)** pour demander la fusion de votre branche dans `main`.
- Attendez la validation et fusion la PR.

### 5️⃣ Création d’un conflit

- Deux étudiants doivent modifier **la même ligne du `<h1>`** dans `index.html`.
- Exemple :
  - Étudiant A : `<h1>Bienvenue sur le site de notre groupe</h1>`
  - Étudiant B : `<h1>Page principale de notre projet</h1>`
- Poussez vos modifications et tentez de fusionner vos PR.
- Un **conflit apparaîtra**.

### 6️⃣ Résolution du conflit

- Ouvrez `index.html` et repérez les marqueurs de conflit :
  ```html
  <<<<<<< HEAD
  <h1>Bienvenue sur le site de notre groupe</h1>
  =======
  <h1>Page principale de notre projet</h1>
  >>>>>>> branche-etudiantB
  ```
- Choisissez en groupe une version finale (par exemple :
  `<h1>Bienvenue sur le site de notre projet de groupe</h1>`).
- Enregistrez, validez et poussez la résolution.

---

## ✅ Résultat attendu

À la fin de l’exercice :

- Le dépôt GitHub contient une page **HTML/CSS** collaborative.
- Chaque étudiant a appris à utiliser **clone, commit, branch, push, pull request, merge et résolution de conflits**.
