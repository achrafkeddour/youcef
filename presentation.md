```markdown
# Guide de Collaboration Git & GitHub

## 1. Lancer le début du code dans VS Code
- Ouvrez votre projet dans **VS Code**.

## 2. Créer un "New Repository" sur GitHub
- Créez un nouveau dépôt (**Public** ou **Privé**).

## 3. Initialiser et pousser le code local vers GitHub
```bash
git init  # Initialise un nouveau dépôt Git
git add .  # Ajoute tous les fichiers et modifications à l’index (zone de staging)
git commit -m "Premier commit"
git remote add origin https://github.com/Arselenne/NOM-DU-REPO.git
git branch -M main  # Renomme la branche actuelle en "main" (ou force son nom en "main")
git push -u origin main  # Envoie la branche "main" vers le dépôt distant et définit "origin/main" comme branche par défaut
```

## 4. Partager le répertoire avec les autres
- Partagez le lien du dépôt GitHub (en site web).

## 5. Les autres clonent le dépôt
```bash
git clone https://github.com/Arselenne/NOM-DU-REPO.git
cd NOM-DU-REPO
```

## 6. Chacun crée sa propre branche
```bash
git branch  # Résultat : main
git checkout -b nom-de-la-branche  # Exemple : achraf-branch
```

## 7. Sauvegarder ses modifications
```bash
git add .
git commit -m "modifications Achraf 09/11/2025"
git push
```

## 8. Intégrer ses modifications dans `main` via Pull Request
### Étapes locales :
```bash
git checkout nom-de-la-branche  # Vérifier la branche
git pull origin main
```

### Créer une Pull Request sur GitHub :
1. Allez sur le dépôt GitHub.
2. Cliquez sur **Pull Requests** → **New Pull Request**.
3. Choisissez :
   - **base branch** : `main`
   - **compare branch** : `nom-de-la-branche`
4. Cliquez sur **Create Pull Request**.
5. Ajoutez une description.
6. Soumettez.

### Après soumission :
- Vous pouvez **accepter le merge**.
- Ou **demander des modifications** (en cas de conflits de fusion).
```
