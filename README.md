# MLBB API Status

Mini API estatica para GitHub Pages.

## Endpoint

```text
https://TU_USUARIO.github.io/TU_REPO/status.json
```

## Activar o desactivar el sistema

Editar `status.json`:

```json
{
  "enabled": true,
  "message": "Sistema habilitado",
  "updated_at": "2026-05-27"
}
```

Para bloquear el sistema:

```json
{
  "enabled": false,
  "message": "Sistema deshabilitado temporalmente",
  "updated_at": "2026-05-27"
}
```

## GitHub Pages

1. Crear un repositorio en GitHub, por ejemplo `mlbb-api-status`.
2. Subir estos archivos a la raiz del repositorio.
3. Ir a `Settings > Pages`.
4. En `Build and deployment`, elegir `Deploy from a branch`.
5. Seleccionar la rama `main` y carpeta `/root`.
6. Copiar la URL final de GitHub Pages.

Luego pegar esa URL en `REMOTE_SWITCH_URL` dentro de `index1.html`.
