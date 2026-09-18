# Clement

> Projet Clement par Arnaud VERSINI

## 📖 Documentation

La documentation complète est disponible sur [GitHub Pages](https://arnaudversini.github.io/clement/).

### Lire la documentation localement

```bash
# Installer mdBook
cargo install mdbook

# Se déplacer dans le dossier de documentation
cd docs/book

# Démarrer le serveur de documentation
mdbook serve

# Ouvrir http://localhost:3000 dans votre navigateur
```

## 🚀 Démarrage rapide

### Installation

```bash
git clone https://github.com/ArnaudVERSINI/clement.git
cd clement
# ... (voir la documentation pour les détails)
```

## 📁 Structure du projet

```
.
├── docs/
│   └── book/                 # Documentation mdBook
│       ├── src/              # Sources Markdown
│       │   ├── introduction.md
│       │   ├── installation.md
│       │   ├── configuration.md
│       │   ├── utilisation.md
│       │   ├── api/
│       │   │   └── index.md
│       │   ├── SUMMARY.md
│       │   └── CONTRIBUTING.md
│       ├── book.toml         # Configuration mdBook
│       └── book-output/      # Généré par mdBook (ignoré)
├── .github/
│   └── workflows/
│       ├── docs.yml         # CI/CD pour la documentation
│       └── test-docs.yml    # Tests de la documentation
├── .gitignore
└── README.md
```

## 🤝 Contribuer

Voir [CONTRIBUTING.md](docs/book/src/CONTRIBUTING.md) pour les guidelines de contribution.

## 📄 Licence

Ce projet est sous licence MIT.
