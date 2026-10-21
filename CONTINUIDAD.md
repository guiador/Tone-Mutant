# Continuidad — Tone-Mutant

Actualizado el 20 de octubre de 2026. Editor MIDI Casio CT-X con interfaz española Qt 6 y soporte experimental CT-X800.

## Punto de partida

Repositorio de trabajo: https://github.com/guiador/Tone-Mutant (public). Se conserva el historial y la procedencia; esta organización no convierte los componentes de terceros en código propio.

ui: controles Qt6; services: MIDI y protocolo; models/constants: parámetros; tests: pruebas sin hardware; tools: captura y empaquetado.

## Construcción y comprobación

Usar requirements-desktop.txt y requirements-build.txt. El entorno actual es .runtime/python312/Scripts/python.exe; Iniciar Tone Mutant.cmd lo selecciona. tools/build_portable.py genera el portable.

python -m unittest discover -s tests -v con QT_QPA_PLATFORM=offscreen. No se requiere escribir en el teclado real.

Comprobaciones ejecutadas durante la preparación de continuidad:

- APROBADA: `python.exe -m unittest discover -s tests -v` (14.27 s).
  Resultado: Ran 52 tests in 8.505s; OK

Las comprobaciones automáticas describen sólo lo ejecutado. No certifican accesibilidad humana, funcionamiento de todos los dispositivos ni equivalencia entre un paquete anterior y el código actual. La evidencia histórica conserva su fecha y versión.

## Entrega y entorno local

En el equipo de trabajo, el índice único es `Codex/Entregas/Tone Mutant`. `Codex/Entregas/LEEME.md` y sus manifiestos identifican los paquetes conservados y sus SHA-256. Las entregas anteriores a esta revisión no deben presentarse como compilaciones de este commit. Los paquetes y entornos no forman parte del código fuente.

Las herramientas locales se reúnen en `Codex/Soporte/Herramientas`; los enlaces de compatibilidad conservan las rutas de los scripts. En otro equipo se deben preparar las dependencias indicadas por este proyecto. No copiar ciegamente rutas de Guillermo ni tratar un entorno virtual Windows como un instalador portable.

Las claves de firma y configuraciones privadas se conservan localmente y se excluyen de Git. No se sustituyen para crear una actualización; usar las claves existentes o documentar una nueva identidad de paquete. No incorporar cuentas, bases, fotos ni documentos de usuarios a las pruebas.

## Próximo trabajo útil

Probar NVDA y el CT-X800 físico. Mantener las escrituras experimentales deshabilitadas por defecto y distinguir las lecturas capturadas de una consulta actual. Publicar en guiador/Tone-Mutant mediante contribution; origin pertenece al autor original.

Antes de editar, leer el alcance vigente y revisar `git status`. Mantener separados cambios de producto, construcción y limpieza. Conservar las APIs, formatos y licencias salvo que la tarea requiera cambiarlos y se pueda verificar la migración. Las instrucciones posteriores del usuario prevalecen sobre esta nota.

## Referencias

- [README.md](README.md)
- [ACCESIBILIDAD.md](ACCESIBILIDAD.md)
- [docs](docs)
