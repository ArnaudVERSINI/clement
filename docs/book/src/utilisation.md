# Utilisation

## Démarrage rapide

### Commande de base

```bash
# Démarrer le serveur
clement start

# Démarrer en mode développement
clement start --dev

# Démarrer avec une configuration spécifique
clement start --config custom.toml
```

### Options disponibles

| Option | Description |
|--------|-------------|
| `-v, --version` | Affiche la version |
| `-h, --help` | Affiche l'aide |
| `--dev` | Mode développement |
| `--config <file>` | Fichier de configuration |
| `--port <port>` | Port du serveur |
| `--log-level <level>` | Niveau de logging |

## Exemples d'utilisation

### Exemple 1 : Démarrage simple

```bash
clement start
```

### Exemple 2 : Démarrage avec configuration personnalisée

```bash
clement start --config production.toml --port 8080
```

### Exemple 3 : Mode développement avec logs détaillés

```bash
clement start --dev --log-level debug
```

## Intégration CI/CD

Voir la section CI/CD pour l'intégration avec GitHub Actions, GitLab CI, etc.

## Dépannage

### Problèmes courants

1. **Port déjà utilisé**
   - Message: `Error: Address already in use`
   - Solution: Changer le port avec `--port` ou libérer le port existant.

2. **Fichier de configuration manquant**
   - Message: `Error: Config file not found`
   - Solution: Vérifier le chemin du fichier ou créer un fichier par défaut.

3. **Problème de connexion à la base de données**
   - Message: `Error: Connection refused`
   - Solution: Vérifier les paramètres de connexion et que la base est démarrée.

## Bonnes pratiques

- Toujours utiliser `--dev` en développement
- Ne jamais committer de fichiers de configuration avec des secrets
- Utiliser des variables d'environnement pour les informations sensibles
- Tester la configuration avant de déployer en production
