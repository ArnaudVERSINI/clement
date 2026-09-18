# Installation

## Prérequis

- Système d'exploitation : Linux, macOS, ou Windows
- [Rust](https://www.rust-lang.org/) (si le projet est en Rust)
- [Node.js](https://nodejs.org/) (si nécessaire)
- [Python](https://www.python.org/) (si nécessaire)

## Installation depuis les sources

```bash
# Cloner le dépôt
git clone https://github.com/ArnaudVERSINI/clement.git
cd clement

# Installer les dépendances (exemple pour un projet Rust)
cargo build --release

# Ou pour un projet Node.js
npm install
npm run build
```

## Installation via package manager

Si disponible :

```bash
# Exemple pour npm
npm install -g @arnaudversini/clement

# Exemple pour cargo
cargo install clement
```

## Vérification de l'installation

```bash
clement --version
# ou
clement -v
```
