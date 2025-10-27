# Datos a escala humana

Un libro de código abierto

[Guía de Contribución](/project/CONTRIBUTING.md) |
[Código de Conducta](/project/CODE_OF_CONDUCT.md) |
[Hoja de Ruta](/project/ROADMAP.md)

🚧 Estado del Proyecto: este libro se encuentra actualmente en las primeras
etapas de desarrollo. Espero completar un MVP para finales de octubre de
2025. Por favor, consulta la HOJA DE RUTA para más información.

## Desarrollo

### Configuración del Entorno

Para configurar el entorno de desarrollo:

```bash
# Clonar el repositorio
git clone <repository-url>
cd datos-escala-humana

# Instalar dependencias
uv sync

# Instalar pre-commit hooks
uv run pre-commit install
```

## Contribuciones

- We use [`markdownlint-cli2` to manage Markdown formatting in .qmd files](https://github.com/DavidAnson/markdownlint-cli2). To run this before committing, use:

```bash
uv run markdownlint-cli2 "**/*.qmd"
```

## Licenciamiento

Este proyecto utiliza una licencia dual:

- **Contenido y documentación**: Licenciados bajo
  [Creative Commons Attribution 4.0 International (CC BY 4.0)](/LICENSE-CC-BY-4.0)
- **Código y software**: Licenciados bajo [MIT License](/LICENSE-MIT)

Consulta los archivos de licencia completos para más detalles sobre los
términos y condiciones.

## Patrocinadores del Proyecto

[![Centro de Investigaciones Urbanas y Territoriales](public/ciut-logo.png)](https://ciut.fau.unlp.edu.ar/)

[![Facultad de Arquitectura y Urbanismo](public/fau-logo.png)](https://www.fau.unlp.edu.ar/)
