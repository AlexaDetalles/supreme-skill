---
name: supreme
description: Resolver tareas con alcance explícito, ejecución proporcional y verificación. Usar cuando el usuario invoque Supreme o pida combinar workflows para implementar, depurar, revisar código o producir diseños, videos y documentos. Integrar selección de capacidades, simplicidad, planificación por resultados y comunicación concisa.
---

# Supreme

Elegir el proceso mínimo suficiente para entregar el resultado completo. Optimizar claridad y trabajo útil; tratar el ahorro de tokens como consecuencia, no como criterio para omitir evidencia.

## 1. Precisar el resultado

- Recuperar objetivo y restricciones de la conversación y archivos actuales. Leer instrucciones aplicables antes de modificar el proyecto.
- Definir de una a cinco condiciones observables de aceptación. Para tareas triviales, mantenerlas internas; para trabajo complejo, compartir un plan breve con su verificación.
- Distinguir hechos comprobados, hipótesis y decisiones. Investigar lo que las herramientas puedan resolver. Preguntar solo por decisiones del usuario o información imprescindible que no pueda recuperarse; avanzar en tareas independientes mientras tanto.
- Resolver elecciones reversibles y rutinarias con criterio propio. Hacer explícitas las suposiciones que cambien el resultado.

## 2. Elegir una ruta

| Situación | Acción | Criterio para avanzar |
|---|---|---|
| Cambio acotado | Inspeccionar el punto responsable y entregar una modificación coherente. | Vincular cada cambio al comportamiento solicitado. |
| Bug | Reproducir, trazar el flujo y contrastar una hipótesis por vez. | Tener reproducción o evidencia concreta suficiente para ubicar la causa. |
| Feature con varias capas | Planificar un recorrido completo e implementar por cortes verificables. | Completar el recorrido del usuario y sus estados relevantes. |
| Decisión técnica incierta | Crear un prototipo aislado para una pregunta específica. | Obtener evidencia para decidir; distinguir prototipo de implementación final. |
| Proyecto de varias sesiones | Escribir especificación breve y tareas con dependencias y aceptación. | Poder retomar cada tarea sin reconstruir toda la conversación. |
| Revisión | Inspeccionar diff y contexto; priorizar fallos por impacto. | Sustentar hallazgos en ubicación, escenario y consecuencia; distinguir sospechas. |
| Diseño, video o documento | Leer la skill especializada disponible y producir el formato solicitado. | Inspeccionar la salida renderizada o exportada, además de su estructura. |

Combinar rutas solo cuando la tarea lo necesite. Usar una entrevista cuando existan decisiones abiertas; resolver cambios claros sin una ceremonia de especificaciones y tickets.

## 3. Cargar capacidades con precisión

- Consultar solo skills y referencias pertinentes. Preferir versiones instaladas actuales frente a copias históricas.
- Si ISAAC SKIL está disponible y hace falta localizar un workflow de su colección, consultar la familia pertinente; no cargar toda la recopilación.
- Usar skills especializadas para formatos y servicios: sus procedimientos complementan este núcleo. Respetar instrucciones vigentes del usuario y entorno al resolver conflictos.
- Comprobar que herramientas, conexiones y recursos existan. Una descripción de MCP, ruta o script no demuestra capacidad operativa.
- Mantener este núcleo utilizable sin los plugins de procedencia. Si falta un recurso imprescindible, identificar el bloqueo concreto y completar el trabajo independiente posible.
- Delegar solo cuando el usuario o las instrucciones aplicables lo permitan y la tarea sea independiente. Compartir aceptación y artefactos mínimos; integrar y verificar los resultados recibidos.

## 4. Implementar con simplicidad

- Seguir el recorrido desde la entrada hasta la capa que posee la regla o estado. Corregir en el lugar responsable.
- Reutilizar interfaces existentes; crear abstracciones cuando varios usos reales o la propiedad del comportamiento lo justifiquen.
- Mantener estilo del proyecto y preservar trabajo del usuario. Limitar modificaciones al alcance acordado.
- Preferir el cambio coherente más pequeño, aunque atraviese varias capas. Refactorizar lo necesario si un parche duplica reglas o esconde la causa; justificar ampliaciones materiales.
- Añadir dependencias, configuración, servicios o migraciones solo cuando la aceptación lo requiera. Explicar costes relevantes antes de decisiones difíciles de revertir.
- Entregar funciones conectadas y utilizables. Mantener placeholders solo si fueron pedidos o si una dependencia bloqueada se identifica claramente.

## 5. Verificar con evidencia

- Mapear cada condición de aceptación a una comprobación pertinente. Empezar por la prueba focalizada; ejecutar también controles obligatorios del proyecto.
- Para bugs o lógica con consecuencias relevantes, usar una reproducción que falle antes y pase después cuando sea viable. Probar comportamiento observable y bordes relevantes.
- Para cambios reversibles de bajo impacto, elegir inspección o comprobación directa cuando sea suficiente; evitar tests que solo repitan la implementación.
- Para UI, revisar estados y tamaños afectados; comprobar interacciones y errores relevantes. Para archivos y video, abrir o renderizar la salida y revisar cortes, legibilidad y composición.
- Reutilizar resultados previos solo si corresponden al mismo estado y alcance. Distinguir aprobado, fallido, no ejecutado y bloqueado.
- Detener ampliaciones de alcance cuando toda la aceptación esté comprobada. Repetir pruebas solo ante nuevos cambios, fallos o dudas pendientes.

## 6. Entregar y cerrar

- Guardar artefactos y cambios mediante el mecanismo persistente del entorno. Para trabajo de varias sesiones, registrar decisiones, estado verificado y siguiente paso concreto.
- Completar acciones autorizadas hasta el final. Pedir aprobación solo cuando sea necesaria y presentar antes el resultado concreto revisable.
- Comunicar primero el resultado, después qué cambió, cómo se verificó y cualquier limitación material. Ajustar detalle a la tarea.
- Escribir de forma concisa y comprensible. Preservar nombres, rutas, comandos, restricciones y evidencia exactos al resumir.
- Afirmar únicamente lo respaldado por observaciones: un build exitoso no demuestra UX correcta; archivos locales no demuestran publicación; un catálogo no demuestra herramientas funcionando.

## Procedencia y límites

Sintetizar selección progresiva de ISAAC SKIL; planificación, aceptación y revisión de Matt Pocock Skills; simplicidad y cambios focalizados de Karpathy Guidelines; cortes coherentes, verificación acotada y economía de contexto de Caveman. Estas reglas son una adaptación, no una copia completa ni una dependencia obligatoria.

Tratar Supreme como workflow, no como un modelo nuevo ni garantía de mayor calidad o menor coste. Evaluar mejoras por resultados observados en tareas reales.
