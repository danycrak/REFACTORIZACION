# Refactorización

## Problemas Identificados en la Aplicación Original

### Redundancia de Estilos
** ** Algunos estilos, como colores y tamaños, están definidos directamente en el código en lugar de utilizar constantes, lo que podría dificultar la coherencia y mantenimiento a largo plazo.

### Manejo de Eventos Duplicado
La lógica del evento `onPress` está duplicada en ambas ramas del condicional, lo que puede ser propenso a errores y dificulta la modificación en el futuro.

## Asegurando la No Afectación Negativa de la Funcionalidad Existente

- Implementa pruebas unitarias exhaustivas antes de realizar la refactorización. Las pruebas deben cubrir todas las funcionalidades críticas y escenarios de uso.
- Realiza pruebas de regresión para verificar que las características existentes sigan funcionando correctamente después de cada cambio.
- Utiliza sistemas de control de versiones para realizar rollbacks rápidos en caso de problemas.

## Mejoras Logradas con el Refactoring

- Hace que el código sea más modular y fácil de entender.
- Se han creado funciones `renderHeader` y `renderFooter` para separar las partes de la interfaz de usuario relacionadas con la cabecera y el pie de página. Esto mejora la legibilidad y permite reutilizar código si es necesario.

## Desafíos Significativos Durante el Proceso de Refactoring y Soluciones

- **Miedo a Romper Funcionalidades Existentes:** Se supera mediante la implementación de pruebas unitarias antes y después de la refactorización.
- **Falta de Tiempo:** Se supera estableciendo prioridades claras, dividiendo la refactorización en tareas manejables y realizando mejoras incrementales.

## Impacto en la Experiencia del Usuario Final

La refactorización puede proporcionar una base sólida para la introducción de nuevas características y mejoras en el futuro, enriqueciendo así la experiencia del usuario. Es crucial realizar pruebas exhaustivas después de la refactorización para garantizar que no se hayan introducido nuevos errores.

## Aplicando Lecciones Aprendidas a Futuros Proyectos

- Fomenta una comunicación efectiva dentro del equipo.
- Asegúrate de que todos los miembros del equipo estén al tanto de las decisiones de diseño y de las prácticas de codificación adoptadas para mantener la coherencia y evitar malentendidos.
- Las tecnologías y las mejores prácticas evolucionan, por lo que es importante que el equipo se mantenga actualizado y esté dispuesto a adaptarse y aprender de cada proyecto.
