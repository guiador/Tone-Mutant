# Trabajo en Tone-Mutant

Leer primero README (o README-ES/readme), CONTINUIDAD.md y los documentos de alcance que allí se enlazan. La última petición del usuario define el trabajo actual.

- Mantener la navegación por teclado, etiquetas accesibles y compatibilidad de formatos. No atribuir validación con lectores o dispositivos a pruebas que sólo usan simulaciones.
- Conservar las licencias y avisos de cada componente. No añadir una licencia global que abarque recursos de terceros.
- Mantener herramientas descargadas, cachés, claves, datos locales y entregas fuera de Git. Los scripts de construcción propios permanecen con las fuentes.
- No seguir enlaces de directorio durante una limpieza recursiva. Verificar el destino y preservar fuentes, claves, recursos únicos y evidencia necesaria.
- Ejecutar las comprobaciones pertinentes indicadas en CONTINUIDAD.md. Registrar los fallos y límites sin sustituirlos por una afirmación de éxito.
- Favorecer cambios pequeños y comprobables; evitar reorganizaciones que rompan las rutas de construcción por razones sólo estéticas.

Mapa de módulos: ui: controles Qt6; services: MIDI y protocolo; models/constants: parámetros; tests: pruebas sin hardware; tools: captura y empaquetado.
