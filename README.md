# Laboratorio 13 — Pruebas integrales e Integración Continua (Maven + JUnit 5)

Este repositorio contiene el dominio de préstamos de biblioteca, repos en memoria, servicio de negocio y pruebas integrales.

## Requisitos
- Java 17
- Maven 3.8+

## Ejecutar
- Compilar (sin tests):
  ```bash
  mvn -DskipTests=true compile
  ```
- Ejecutar pruebas:
  ```bash
  mvn -DskipTests=false test
  ```
- Reportes de pruebas: se generan en `target/surefire-reports/` (si hay tests ejecutados).

Nota: La clase de prueba integral se llama `LoanFlowIT`. Con la configuración por defecto de Surefire, los patrones estándar son `**/Test*.java`, `**/*Test.java`, `**/*Tests.java`, `**/*TestCase.java`. Si no se detecta el archivo `LoanFlowIT.java`, esto se debe al patrón de nombres (IT). Para mantener el enunciado intacto, no se modifica el `pom.xml`. En CI puede no adjuntarse el artifact si no se generan reportes.

## CI
- Workflow: `.github/workflows/ci.yml`
- Ejecuta `mvn test` en cada push/PR.
- Publica artefacto `surefire-reports` (si existen archivos `.txt`).

## Estructura
```
src/
  main/java/com/tecsup/library/
    model/
    repo/
    repo/mem/
    service/
    util/
  test/java/com/tecsup/library/integration/
    LoanFlowIT.java
``` 

## Evidencias
Usa `Evidencias_Canvas.md` para completar enlaces y capturas de CI y reporte de pruebas.