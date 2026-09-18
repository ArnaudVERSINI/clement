# Contribuer à la documentation

Merci de vouloir contribuer à la documentation Clement !

## Prérequis

- [mdBook](https://github.com/rust-lang/mdBook) installé
- Git
- Un éditeur de texte (VS Code, Vim, etc.)

## Installation de mdBook

```bash
# Installer mdBook via cargo (recommandé)
cargo install mdbook

# Ou via Homebrew (macOS)
brew install mdbook

# Ou via apt (Debian/Ubuntu)
sudo apt install mdbook
```

## Structure du projet

```text
docs/book/
+-- book.toml          # Configuration de mdBook
+-- src/
    +-- SUMMARY.md     # Table des matières
    +-- introduction.md
    +-- installation.md
    +-- configuration.md
    +-- utilisation.md
    +-- api/
        +-- index.md
+-- book-output/       # Généré par mdBook
```

## Développement local

```bash
# Se placer dans le dossier du livre
cd docs/book

# Démarrer le serveur de développement
mdbook serve

# Ou construire le livre
mdbook build

# Ouvrir dans le navigateur (après mdbook serve)
# http://localhost:3000
```

## Commandes utiles

| Commande | Description |
|----------|-------------|
| mdbook serve | Démarre un serveur web avec rechargement automatique |
| mdbook build | Construit le livre en HTML |
| mdbook watch | Surveille les changements et reconstruit |
| mdbook test | Teste les liens du livre |

## Soumettre une contribution

1. Forker le dépôt
2. Créer une branche pour votre contribution (git checkout -b docs/ma-contribution)
3. Faire vos modifications
4. Tester localement avec mdbook serve
5. Commiter vos changements (git commit -m "docs: ajouter section XYZ")
6. Pousser vers votre fork (git push origin docs/ma-contribution)
7. Ouvrir une Pull Request vers la branche main

## Guidelines

- Utiliser le français pour la documentation
- Respecter la structure existante
- Ajouter des exemples de code quand pertinent
- Garder les paragraphes courts et clairs
- Utiliser des titres hiérarchiques (#, ##, ###)
- Documenter les options et paramètres
- Inclure des sections de dépannage pour les problèmes courants

## Style Markdown

- Préférer les listes à puces pour les énumérations
- Utiliser des blocs de code avec le langage approprié
- Ajouter des tableaux pour les références
- Utiliser des liens relatifs pour les références internes

## Vérification avant PR

- Vérifier que mdbook build fonctionne sans erreur
- Vérifier que tous les liens sont valides avec mdbook test
- Relire pour les fautes d'orthographe et de grammaire
- S'assurer que le contenu est à jour avec la version du projet
