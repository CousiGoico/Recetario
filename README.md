# Recetario personal

Recetario estático generado con MkDocs y Material for MkDocs.

## Objetivo

Mantener un recetario personal sencillo: cada receta vive en un archivo Markdown y la web se encarga de organizarla, mostrarla y publicarla.

## Requisitos

- Python 3.10+
- pip

## Instalación local

```bash
python -m venv .venv
. .venv/bin/activate  # Linux/macOS
# o .\.venv\Scripts\Activate.ps1  # Windows PowerShell
pip install -r requirements.txt
mkdocs serve
```

## Construcción

```bash
mkdocs build --strict
```

## Publicación en GitHub Pages

1. En GitHub, abre el repositorio.
2. Ve a Settings > Pages.
3. En Source, selecciona GitHub Actions.
4. Confirma que la acción de despliegue está habilitada.
5. Haz push al branch `main` para publicar.

## Estructura

- `docs/`: contenido del sitio
- `docs/recetas/`: categorías y recetas
- `docs/assets/images/`: recursos gráficos
- `mkdocs.yml`: configuración principal
- `.github/workflows/deploy.yml`: despliegue automático
