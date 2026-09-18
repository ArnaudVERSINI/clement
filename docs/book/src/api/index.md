# API Reference

Bienvenue dans la documentation technique de l'API Clement.

## Endpoints principaux

- Configuration - Endpoints de configuration
- Health - Endpoints de santé
- Users - Gestion des utilisateurs
- Projects - Gestion des projets

## Schéma d'authentification

Clement utilise l'authentification par token Bearer.

### Exemple de requête authentifiée

```bash
curl -X GET \
  https://api.clement.dev/v1/users \
  -H 'Authorization: Bearer YOUR_TOKEN' \
  -H 'Content-Type: application/json'
```

## Codes de retour HTTP

| Code | Description |
|------|-------------|
| 200 | OK - Requête réussie |
| 201 | Created - Ressource créée |
| 400 | Bad Request - Requête invalide |
| 401 | Unauthorized - Non autorisé |
| 403 | Forbidden - Accès interdit |
| 404 | Not Found - Ressource non trouvée |
| 500 | Internal Server Error - Erreur serveur |

## Versioning

L'API suit le versioning sémantique. La version actuelle est v1.

- v1 - API v1 (actuelle)
- v2 - API v2 (future)

## Rate Limiting

- Limite : 100 requêtes par minute par IP
- Headers de rate limiting :
  - `X-RateLimit-Limit` : Limite maximale
  - `X-RateLimit-Remaining` : Requêtes restantes
  - `X-RateLimit-Reset` : Timestamp de réinitialisation
