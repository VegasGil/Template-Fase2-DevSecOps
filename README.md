# Template: Fase 2 - DevSecOps (SAST/SCA para Node.js)

Plantilla base para añadir análisis estático (SAST) y de dependencias (SCA) a proyectos en Node.js/React.

## ¿Qué incluye?
- **SAST (Semgrep):** Analiza el código buscando malas prácticas (ej. inyecciones).
- **SCA (Trivy):** Analiza `package.json` buscando CVEs en librerías (ej. Express).

## Cómo usar esta plantilla en tu Blog
1. Usa este repositorio como plantilla ("Use this template").
2. Borra la carpeta `sample-app/` (es solo para probar que el pipeline funciona).
3. Copia tu carpeta `frontend/` (React) y `backend/` (Node).
4. En los archivos `.github/workflows/sast-ci.yml` y `sca-ci.yml`, cambia `sample-app/` por las rutas de tu proyecto (`backend/ frontend/`).
5. Sube los cambios y verás cómo GitHub Actions bloquea el código si hay vulnerabilidades.