# Evidencias para Canvas — Laboratorio N°13

Completa los campos y adjunta capturas según se requiera.

## 1) Repositorio GitHub
- URL del repositorio: [https://github.com/TU_USUARIO/biblioteca-loans-java](https://github.com/TU_USUARIO/biblioteca-loans-java)

## 2) CI en GitHub Actions
- Captura (PNG) del run en verde: Adjuntar imagen aquí
- Enlace directo al run: https://github.com/TU_USUARIO/biblioteca-loans-java/actions/runs/XXXXXXXX
- Artifact surefire-reports: descargado o indicar ruta `target/surefire-reports/*.txt`

## 3) Reporte de pruebas
- Resumen de `mvn -DskipTests=false test` (copiar output relevante) o contenido de `target/surefire-reports/*.txt`.

## 4) Reflexión breve (≤150 palabras)
> Durante este laboratorio implementamos el dominio de préstamos de una biblioteca y diseñamos pruebas integrales que validan reglas críticas: disponibilidad, límite de préstamos, bloqueo por mora, plazo y cálculo de multa. Automatizamos la ejecución de pruebas mediante GitHub Actions, logrando un pipeline que compila y ejecuta mvn test en cada push. La CI detectó fallos de integración rápidamente y facilitó correcciones inmediatas en repositorios y servicio. Como mejora futura propongo agregar cobertura con JaCoCo y pruebas contra una BD en memoria (H2) para acercarnos más a un entorno real.

Puedes reemplazar este texto por tu reflexión propia manteniendo el límite de 150 palabras.

## Checklist
- [ ] Repo accesible y con estructura: `pom.xml`, `src/main/java/...`, `src/test/java/...`, `.github/workflows/ci.yml`.
- [ ] Capturas del pipeline y enlace directo.
- [ ] Reporte surefire adjunto o accesible.
- [ ] Reflexión agregada.