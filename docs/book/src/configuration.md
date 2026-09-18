# Configuration

## Fichier de configuration principal

Le fichier de configuration principal est généralement `config.toml`, `config.json`, ou `.env` selon le projet.

### Exemple de configuration TOML

```toml
[general]
name = "clement"
version = "1.0.0"
debug = true

[database]
url = "postgres://user:password@localhost:5432/clement"
pool_size = 10

[logging]
level = "info"
file = "/var/log/clement/app.log"
```

### Exemple de configuration JSON

```json
{
  "general": {
    "name": "clement",
    "version": "1.0.0",
    "debug": true
  },
  "database": {
    "url": "postgres://user:password@localhost:5432/clement",
    "pool_size": 10
  },
  "logging": {
    "level": "info",
    "file": "/var/log/clement/app.log"
  }
}
```

## Variables d'environnement

| Variable | Description | Valeur par défaut |
|----------|-------------|-------------------|
| `CLEMENT_ENV` | Environnement (dev, prod, test) | `dev` |
| `CLEMENT_PORT` | Port du serveur | `3000` |
| `CLEMENT_DB_URL` | URL de la base de données | `postgres://localhost/clement` |

## Configuration avancée

Pour des configurations plus avancées, voir la section [API Reference](api/config.md).
