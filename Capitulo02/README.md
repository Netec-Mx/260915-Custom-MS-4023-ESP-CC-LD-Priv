# Práctica: Diseño y refinamiento de prompts para analizar una situación de negocio

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 12 minutos |
| Complejidad | Fácil |
| Nivel de Bloom | Aplicar |
| Tecnologías | Microsoft 365 Copilot Chat, Páginas de Microsoft 365 Copilot, Galería de indicaciones de Copilot, investigación web asistida por IA |
| Caso transversal | Northstar Digital, organización ficticia de inversión digital |

## Descripción general

En esta práctica transformarás una solicitud ambigua de negocio en una indicación estructurada para Copilot Chat. Aplicarás la estructura **Objetivo + Contexto + Datos + Expectativas**, revisarás críticamente la primera respuesta y realizarás refinamientos para distinguir hechos, supuestos y preguntas abiertas, además de priorizar recomendaciones en una tabla.

Guardarás el resultado final en una Página de Microsoft 365 Copilot denominada **“Northstar Digital - Cuaderno de análisis”**. Esta página será el cuaderno de trabajo obligatorio y el insumo de continuidad para las prácticas posteriores del módulo 3.

> **Uso responsable de IA:** Northstar Digital es una organización ficticia creada exclusivamente para esta práctica. No copies datos de clientes, empleados, inversiones, resultados financieros, credenciales ni información interna real en Copilot Chat o en la Página de Copilot.

## Objetivos de aprendizaje

Al completar esta práctica, podrás:

- [ ] Identificar objetivo, contexto, datos, restricciones, audiencia y formato de salida en una indicación de negocio.
- [ ] Convertir una solicitud ambigua en una indicación clara, verificable y reutilizable para Copilot Chat.
- [ ] Refinar una respuesta de IA para separar hechos proporcionados, supuestos, preguntas abiertas, riesgos y fuentes.
- [ ] Solicitar una tabla priorizada que facilite la toma de decisiones de negocio.
- [ ] Crear y mantener una Página de Copilot como registro trazable de indicaciones, criterios y resultados.

## Requisitos previos

### Conocimientos

Antes de comenzar, debes poder:

- Reconocer la estructura **Objetivo + Contexto + Datos + Expectativas**.
- Usar verbos de acción claros, como `analiza`, `compara`, `organiza`, `resume` y `propón`.
- Distinguir entre un hecho proporcionado, una hipótesis o supuesto, y una afirmación que requiere validación externa.
- Navegar por Microsoft 365 y utilizar una conversación de Copilot Chat.

### Acceso requerido

Debes disponer de:

- Una cuenta profesional o educativa de Microsoft Entra ID.
- Acceso habilitado a Microsoft 365 Copilot Chat.
- Acceso habilitado a Páginas de Microsoft 365 Copilot.
- Conexión a Internet estable.
- Permiso para crear y editar páginas en el entorno de Microsoft 365 de formación.

> No uses cuentas personales de Microsoft para esta práctica.

## Entorno de laboratorio

### Hardware de referencia

| Componente | Requisito de referencia |
|---|---|
| Pantalla | Resolución mínima de 1920 × 1080 |
| Conectividad | Mínimo 10 Mbps de descarga y 2 Mbps de carga |
| Equipo | Windows 11 de 64 bits, Intel Core i5 de 10.ª generación o equivalente |
| Memoria | 8 GB de RAM como mínimo |
| Almacenamiento | 2 GB libres para caché del navegador y archivos de práctica |

### Software y servicio de referencia

| Componente | Versión o experiencia de referencia |
|---|---|
| Sistema operativo | Windows 11 Enterprise 23H2, compilación 22631.4169 |
| Navegador | Microsoft Edge 128.0.2739.79 |
| Aplicaciones | Microsoft 365 Apps for enterprise 2408, compilación 17928.20156 |
| IA | Microsoft 365 Copilot Chat, experiencia web disponible el 2026-09-16 |
| Cuaderno | Páginas de Microsoft 365 Copilot, experiencia web disponible el 2026-09-16 |

> Las opciones visibles pueden variar según la licencia, región, idioma, configuración del tenant o actualizaciones del servicio. Si la interfaz no coincide exactamente con esta guía, utiliza la opción equivalente para abrir Copilot Chat, crear una página o insertar contenido de una respuesta.

### Preparación del directorio local

Esta práctica no exige descargas. Sin embargo, crea el directorio de evidencias para guardar borradores si el instructor lo solicita.

1. Abre **Símbolo del sistema** o **Windows Terminal**.
2. Ejecuta el siguiente comando:

```powershell
New-Item -ItemType Directory -Force -Path "C:\CopilotLabs\TransformarIdeasEnAccion\02-00-01"
```

3. Si deseas guardar una copia local de tus notas, usa únicamente contenido ficticio del caso.

## Procedimiento paso a paso

### Paso 1: Revisar la solicitud ambigua y detectar información faltante

**Objetivo:** Identificar por qué una petición genérica puede producir una respuesta poco útil o basada en suposiciones no controladas.

**Instrucciones:**

1. Abre Microsoft 365 en Microsoft Edge e inicia sesión con tu cuenta profesional o educativa.
2. Abre **Microsoft 365 Copilot Chat**.
3. Lee la siguiente solicitud ambigua del área de negocio:

   > “Ayuda a Northstar Digital a mejorar la relación con sus inversionistas internacionales.”

4. Antes de enviarla a Copilot, identifica qué información falta. Considera, como mínimo, las siguientes categorías:
   - Objetivo concreto de negocio.
   - Público o audiencia.
   - Contexto de la organización.
   - Datos disponibles.
   - Alcance temporal.
   - Restricciones.
   - Formato de salida.
   - Criterios para valorar la calidad.
5. En una nota temporal, redacta al menos cinco preguntas que necesitarías responder para convertir la solicitud en una tarea verificable.

   Puedes utilizar preguntas como estas:

   - ¿Qué tipo de experiencia desea mejorar Northstar Digital: portal, comunicaciones, soporte o informes?
   - ¿Qué se sabe realmente sobre las necesidades de los inversionistas internacionales?
   - ¿Qué países, regiones o idiomas están incluidos?
   - ¿Qué resultado de negocio se espera conseguir?
   - ¿Qué recomendaciones son viables dentro de las restricciones conocidas?
   - ¿Cómo se debe presentar el análisis para que un público ejecutivo lo use?
   - ¿Qué afirmaciones requerirían fuentes externas o validación humana?

6. Envía la solicitud ambigua original a Copilot Chat:

   ```text
   Ayuda a Northstar Digital a mejorar la relación con sus inversionistas internacionales.
   ```

7. Lee la respuesta sin asumir que sus recomendaciones son hechos comprobados. Identifica rápidamente:
   - Una recomendación que parezca genérica.
   - Una afirmación que dependa de una suposición.
   - Un dato o sugerencia que requeriría validación antes de aplicarse.

**Resultado esperado:**

Dispones de una lista de información faltante y de una respuesta inicial que demuestra el efecto de una indicación poco específica. La respuesta probablemente incluirá recomendaciones generales, pero no tendrá un alcance, una audiencia, datos de referencia ni criterios de priorización claramente definidos.

**Verificación:**

Confirma que puedes explicar verbalmente o por escrito por qué la solicitud inicial no cumple plenamente con la estructura:

| Componente | ¿Está presente en la solicitud ambigua? |
|---|---|
| Objetivo específico | No, solo indica una intención general |
| Contexto suficiente | No |
| Datos disponibles | No |
| Restricciones | No |
| Audiencia del resultado | No |
| Formato de salida | No |
| Criterios de calidad | No |

---

### Paso 2: Preparar el contexto ficticio y diseñar una indicación estructurada

**Objetivo:** Crear una primera indicación clara utilizando los componentes de una indicación eficaz.

**Instrucciones:**

1. Usa exclusivamente el siguiente contexto ficticio. No sustituyas estos datos por información real de tu organización.

   **Caso ficticio: Northstar Digital**

   | Elemento | Información proporcionada para el ejercicio |
   |---|---|
   | Organización | Northstar Digital, plataforma ficticia de inversión digital |
   | Situación | Desea mejorar la relación y experiencia digital de inversionistas internacionales |
   | Público objetivo | Equipo directivo de Northstar Digital |
   | Audiencia final de las mejoras | Inversionistas internacionales existentes y potenciales |
   | Problema inicial | La organización considera que su comunicación y experiencia digital pueden resultar poco claras para audiencias internacionales |
   | Datos disponibles | No hay métricas, estudios de usuarios, países concretos, datos financieros ni comentarios reales de clientes |
   | Restricción de datos | No inventar cifras, leyes, requisitos regulatorios, países, idiomas, métricas ni características de producto |
   | Uso esperado | Preparar un análisis inicial que ayude a decidir qué información validar y qué acciones explorar |
   | Criterio principal | Las recomendaciones deben ser concretas, prudentes, priorizables y diferenciadas de los hechos conocidos |

2. Redacta una indicación inicial que incluya:
   - Un verbo de acción concreto.
   - El objetivo del análisis.
   - El contexto de Northstar Digital.
   - Los datos disponibles y las limitaciones.
   - La audiencia: equipo directivo.
   - Restricciones contra invenciones o afirmaciones no verificadas.
   - Un formato de salida reutilizable.
   - Criterios de calidad.

3. Utiliza la siguiente plantilla y complétala o úsala como referencia:

   ```text
   Analiza la situación inicial de Northstar Digital, una plataforma ficticia de inversión digital que desea mejorar su relación con inversionistas internacionales.

   Objetivo: [indica qué debe permitir decidir este análisis].
   Contexto: [resume la situación proporcionada].
   Datos disponibles: [indica explícitamente que no existen métricas ni investigaciones reales].
   Tarea: [solicita áreas de mejora y acciones iniciales].
   Restricciones: [prohíbe inventar hechos, cifras, países, leyes o requisitos regulatorios].
   Audiencia: [equipo directivo].
   Formato: [define secciones o tabla].
   Criterios de calidad: [concreción, prudencia, trazabilidad y priorización].
   ```

4. Como referencia, puedes usar esta versión estructurada:

   ```text
   Analiza la situación inicial de Northstar Digital, una plataforma ficticia de inversión digital que desea mejorar su relación y experiencia digital para inversionistas internacionales.

   Objetivo: ayudar al equipo directivo a identificar áreas de mejora iniciales y decidir qué información debe validarse antes de invertir en cambios.

   Contexto: Northstar Digital considera que sus comunicaciones y su experiencia digital pueden no ser suficientemente claras para audiencias internacionales. No se han proporcionado métricas, investigaciones de usuarios, países, idiomas, comentarios de clientes ni requisitos regulatorios reales.

   Tarea: propone entre 4 y 6 áreas de mejora relacionadas con experiencia digital, contenido, comunicación, soporte o confianza. Para cada área, explica el problema potencial, una acción inicial de bajo riesgo y la información que debe validarse.

   Restricciones: trata el caso como ficticio. No inventes cifras, países, idiomas, requisitos legales, necesidades de clientes ni características de producto. Si una recomendación depende de información no proporcionada, márcala como supuesto o pregunta abierta. No presentes asesoramiento financiero, legal o regulatorio.

   Audiencia: equipo directivo no técnico.

   Formato de salida: usa una tabla con las columnas Área de mejora, Problema potencial, Acción inicial, Dato por validar y Riesgo de asumir sin evidencia. Añade después un resumen ejecutivo de máximo 120 palabras.

   Criterios de calidad: recomendaciones concretas, lenguaje profesional y directo, distinción clara entre información conocida e incierta, y ausencia de datos inventados.
   ```

5. Revisa tu indicación antes de enviarla. Comprueba que no contiene contradicciones, como pedir una respuesta “muy detallada” y “de una frase”, o exigir fuentes para hechos que no se han investigado.
6. Envía la indicación estructurada a Copilot Chat.

**Resultado esperado:**

Copilot genera un análisis inicial organizado para el equipo directivo. La respuesta debe reconocer que faltan datos y presentar recomendaciones prudentes, por ejemplo, revisar claridad de contenidos, localizar necesidades de idiomas tras investigación, mejorar rutas de soporte o validar expectativas de comunicación.

**Verificación:**

Revisa la indicación enviada y confirma que responde a estas preguntas:

| Elemento | Comprobación |
|---|---|
| Objetivo | ¿Indica qué decisión o resultado debe apoyar el análisis? |
| Contexto | ¿Explica quién es Northstar Digital y qué situación afronta? |
| Datos | ¿Declara explícitamente qué información no está disponible? |
| Tarea | ¿Pide un análisis o acciones concretas? |
| Restricciones | ¿Evita datos inventados y asesoramiento no autorizado? |
| Audiencia | ¿Identifica al equipo directivo? |
| Formato | ¿Solicita tabla y resumen ejecutivo? |
| Calidad | ¿Exige prudencia, claridad y distinción de incertidumbres? |

---

### Paso 3: Evaluar críticamente la primera respuesta

**Objetivo:** Aplicar revisión humana para detectar contenido útil, contenido incierto y oportunidades de refinamiento.

**Instrucciones:**

1. Revisa la respuesta obtenida en el paso anterior.
2. Evalúala con los siguientes criterios:
   - **Relevancia:** ¿Las áreas propuestas se relacionan con la experiencia de inversionistas internacionales?
   - **Claridad:** ¿El equipo directivo puede comprender la recomendación sin conocimientos técnicos?
   - **Trazabilidad:** ¿La respuesta indica qué se conoce y qué debe validarse?
   - **Riesgo:** ¿Evita presentar hipótesis como hechos?
   - **Utilidad:** ¿Cada recomendación incluye una acción posible?
   - **Formato:** ¿La tabla contiene todas las columnas solicitadas?
3. Identifica dos elementos de la respuesta que sean útiles para conservar.
4. Identifica dos elementos que requieran refinamiento. Algunos ejemplos posibles son:
   - Una recomendación utiliza términos generales, como “mejorar la personalización”, sin explicar qué evidencia se necesita.
   - Una sugerencia presupone que los inversionistas hablan un idioma determinado.
   - Se menciona cumplimiento normativo sin una fuente, jurisdicción o revisión especializada.
   - La prioridad no está definida.
5. No corrijas manualmente la respuesta todavía. Utiliza la conversación para solicitar una revisión controlada en el siguiente paso.

**Resultado esperado:**

Has identificado fortalezas y limitaciones de la respuesta de Copilot Chat sin aceptar automáticamente sus conclusiones. Tienes criterios concretos para pedir una versión más verificable.

**Verificación:**

Puedes completar la siguiente comprobación:

- [ ] He identificado al menos dos recomendaciones que pueden conservarse como hipótesis de trabajo.
- [ ] He identificado al menos dos afirmaciones, supuestos o recomendaciones que necesitan aclaración.
- [ ] He comprobado que no se han introducido datos internos, personales o confidenciales.
- [ ] He decidido qué información requeriría validación humana o investigación con fuentes autorizadas.

---

### Paso 4: Refinar la respuesta para separar hechos, supuestos y preguntas abiertas

**Objetivo:** Solicitar una revisión que haga visible la incertidumbre y evite que recomendaciones hipotéticas se interpreten como información comprobada.

**Instrucciones:**

1. En la misma conversación de Copilot Chat, envía el siguiente refinamiento:

   ```text
   Revisa tu respuesta anterior y separa de forma explícita la información en tres categorías: Hechos proporcionados, Supuestos o hipótesis y Preguntas abiertas para validar.

   Para cada recomendación:
   1. indica qué hecho del caso la respalda;
   2. identifica cualquier supuesto que hayas utilizado;
   3. formula la pregunta de validación correspondiente;
   4. señala el riesgo de tomar una decisión sin validar esa información.

   No inventes fuentes ni afirmes que Northstar Digital cumple requisitos legales, regulatorios o financieros. Si mencionas una práctica externa o una tendencia del sector, márcala como referencia general y recomienda comprobarla con fuentes públicas y especialistas autorizados.
   ```

2. Lee la respuesta refinada.
3. Comprueba que los únicos hechos sean los proporcionados en el caso ficticio, por ejemplo:
   - Northstar Digital es una plataforma ficticia de inversión digital.
   - Desea mejorar la relación y experiencia digital de inversionistas internacionales.
   - No se han proporcionado métricas, países, idiomas, requisitos regulatorios ni datos de clientes.
4. Si Copilot presenta una afirmación externa como si fuera cierta para Northstar Digital, solicita una corrección con esta indicación adicional:

   ```text
   Corrige cualquier afirmación que presente una hipótesis o práctica general como un hecho de Northstar Digital. Conserva únicamente los hechos proporcionados en el caso y etiqueta el resto como supuesto, ejemplo o pregunta abierta.
   ```

5. Copia o conserva el resultado refinado para incorporarlo posteriormente a la Página de Copilot.

**Resultado esperado:**

La respuesta ahora diferencia claramente entre la información proporcionada, las hipótesis de trabajo y las preguntas que requieren evidencia. Esto permite que el equipo directivo use el análisis como punto de partida sin confundir recomendaciones con hechos validados.

**Verificación:**

La respuesta debe incluir una separación visible equivalente a la siguiente:

| Categoría | Ejemplo válido |
|---|---|
| Hecho proporcionado | Northstar Digital desea mejorar la experiencia digital de inversionistas internacionales. |
| Supuesto o hipótesis | Los inversionistas podrían necesitar contenidos más claros o rutas de soporte mejor definidas. |
| Pregunta abierta | ¿Qué países, idiomas, necesidades de accesibilidad y puntos de fricción priorizan los usuarios? |
| Riesgo | Diseñar cambios sin investigación puede asignar recursos a necesidades no confirmadas. |

---

### Paso 5: Refinar la salida en una tabla priorizada

**Objetivo:** Convertir el análisis en un formato ejecutivo que permita comparar acciones sin ocultar la incertidumbre.

**Instrucciones:**

1. En la misma conversación de Copilot Chat, envía la siguiente indicación de seguimiento:

   ```text
   Convierte el análisis refinado en una tabla priorizada para el equipo directivo de Northstar Digital.

   Incluye exactamente estas columnas:
   1. Prioridad
   2. Área de mejora
   3. Acción inicial propuesta
   4. Justificación basada en el caso
   5. Hecho, supuesto o pregunta abierta
   6. Evidencia necesaria antes de decidir
   7. Riesgo si no se valida
   8. Siguiente responsable sugerido

   Usa prioridad Alta, Media o Baja. Prioriza según impacto potencial, reversibilidad de la acción y necesidad de evidencia, no según cifras inventadas. Limita la tabla a un máximo de 6 filas.

   Después de la tabla, redacta:
   - tres acciones inmediatas de bajo riesgo;
   - tres preguntas para una futura investigación pública o investigación con usuarios;
   - una nota de uso responsable que indique que la salida requiere revisión humana antes de tomar decisiones.
   ```

2. Revisa que Copilot no asigne prioridades basándose en datos inexistentes.
3. Comprueba que las acciones iniciales sean razonables y reversibles. Por ejemplo:
   - Inventariar los contenidos actuales y detectar mensajes ambiguos.
   - Preparar preguntas para entrevistas o encuestas autorizadas.
   - Definir criterios para evaluar claridad, accesibilidad y rutas de soporte.
4. Comprueba que la columna **Siguiente responsable sugerido** use roles genéricos, tales como:
   - Responsable de experiencia digital.
   - Equipo de contenido.
   - Responsable de investigación de usuarios.
   - Equipo de cumplimiento o asesoría especializada, cuando proceda.
5. Si la tabla incluye un rol, requisito o hecho que no se conoce, pide a Copilot que lo cambie por una formulación condicional.

**Resultado esperado:**

Obtienes una tabla ejecutiva de hasta seis filas que diferencia acciones, evidencia pendiente, riesgos y responsables sugeridos. La prioridad representa una hipótesis razonada para iniciar la conversación, no una decisión definitiva.

**Verificación:**

Comprueba que la tabla cumple todos los requisitos:

- [ ] Tiene exactamente las ocho columnas solicitadas.
- [ ] Tiene seis filas o menos.
- [ ] Usa prioridades Alta, Media o Baja.
- [ ] Identifica evidencia necesaria antes de decidir.
- [ ] No contiene cifras, países, normativas o métricas inventadas.
- [ ] Incluye una nota explícita de revisión humana.
- [ ] Propone responsables por función, no personas reales.

---

### Paso 6: Crear el cuaderno de análisis y conservar la trazabilidad

**Objetivo:** Crear la Página de Copilot obligatoria y registrar el caso, la indicación final y los criterios de calidad para reutilizarlos en prácticas posteriores.

**Instrucciones:**

1. Abre **Páginas de Microsoft 365 Copilot** desde Microsoft 365 o desde la opción disponible en Copilot Chat para crear una página a partir de contenido de la conversación.
2. Crea una página nueva.
3. Asigna exactamente el siguiente nombre a la página:

   ```text
   Northstar Digital - Cuaderno de análisis
   ```

4. En la página, crea una sección con el siguiente título obligatorio:

   ```text
   L02 - Prompt refinado
   ```

5. Dentro de la sección, agrega los siguientes apartados:

   ```markdown
   ## L02 - Prompt refinado

   ### Resumen del caso

   ### Solicitud ambigua inicial

   ### Información faltante identificada

   ### Prompt final estructurado

   ### Criterios de calidad

   ### Resultado refinado: hechos, supuestos y preguntas abiertas

   ### Tabla priorizada y próximos pasos

   ### Nota de uso responsable
   ```

6. Completa **Resumen del caso** con un texto breve como el siguiente:

   > Northstar Digital es una plataforma ficticia de inversión digital que desea mejorar su relación y experiencia digital para inversionistas internacionales. El caso no proporciona métricas, datos de usuarios, países, idiomas, información financiera ni requisitos regulatorios. El análisis se utiliza para identificar hipótesis y necesidades de validación antes de proponer decisiones o inversiones.

7. En **Solicitud ambigua inicial**, pega la solicitud del paso 1.
8. En **Información faltante identificada**, pega o resume las preguntas que preparaste en el paso 1.
9. En **Prompt final estructurado**, pega la indicación final del paso 2, incluyendo objetivo, contexto, datos, tarea, restricciones, audiencia, formato y criterios de calidad.
10. En **Criterios de calidad**, agrega al menos los siguientes criterios:

    - El análisis debe usar solo los hechos proporcionados en el caso.
    - Los supuestos deben etiquetarse explícitamente.
    - Las preguntas abiertas deben indicar qué evidencia falta.
    - Las recomendaciones deben ser concretas y comprensibles para un público ejecutivo.
    - No se deben inventar cifras, países, idiomas, leyes, requisitos regulatorios ni características de producto.
    - El resultado requiere validación humana antes de emplearse en decisiones o comunicaciones oficiales.
    - Cualquier investigación pública futura debe citar fuentes verificables y respetar las políticas internas.

11. En **Resultado refinado: hechos, supuestos y preguntas abiertas**, pega la respuesta del paso 4.
12. En **Tabla priorizada y próximos pasos**, pega la tabla y las acciones inmediatas obtenidas en el paso 5.
13. En **Nota de uso responsable**, agrega el siguiente texto:

    > Este cuaderno contiene un caso ficticio y resultados asistidos por IA. Las recomendaciones son hipótesis de trabajo y no sustituyen investigación con usuarios, revisión de fuentes públicas, asesoramiento legal, regulatorio o financiero, ni aprobación de las funciones responsables. No incorporar información confidencial, personal o no autorizada.

14. Comprueba que el contenido se ha guardado. Si la interfaz permite copiar un vínculo de la página, cópialo únicamente si el instructor solicita entregar la evidencia.

**Resultado esperado:**

Existe una Página de Copilot llamada **“Northstar Digital - Cuaderno de análisis”** con una sección titulada **“L02 - Prompt refinado”**. La página contiene el resumen del caso, la indicación final, los criterios de calidad y los resultados refinados.

**Verificación:**

Valida todos los elementos siguientes:

| Elemento obligatorio | Estado esperado |
|---|---|
| Nombre de la página | `Northstar Digital - Cuaderno de análisis` |
| Título de sección | `L02 - Prompt refinado` |
| Resumen del caso ficticio | Incluido |
| Solicitud ambigua | Incluida |
| Información faltante | Incluida |
| Prompt final estructurado | Incluido |
| Criterios de calidad | Incluidos |
| Hechos, supuestos y preguntas abiertas | Incluidos |
| Tabla priorizada | Incluida |
| Nota de uso responsable | Incluida |

> No crees una página distinta para las siguientes prácticas. Las prácticas posteriores deben añadir sus resultados a esta misma página mediante los títulos establecidos: `L03.1 - Experiencia de inversionistas`, `L03.2 - Escenarios económicos`, `L03.3 - Comunicaciones de interrupción` y `L03.4 - Reporte ejecutivo`.

## Validación y pruebas

Realiza esta validación final antes de marcar la práctica como completada.

### Prueba 1: Comprobación de estructura de la indicación

Relee tu prompt final y comprueba que contiene los ocho componentes siguientes:

| Componente | Resultado esperado |
|---|---|
| Objetivo | Indica qué decisión o análisis debe apoyar Copilot |
| Contexto | Describe la situación ficticia de Northstar Digital |
| Datos | Delimita la información disponible y la no disponible |
| Tarea | Solicita áreas de mejora y acciones concretas |
| Restricciones | Prohíbe inventar datos y evita asesoramiento no autorizado |
| Audiencia | Identifica al equipo directivo |
| Formato | Solicita una tabla y un resumen ejecutivo |
| Criterios de calidad | Exige claridad, prudencia, trazabilidad y revisión humana |

**Criterio de aprobación:** los ocho componentes están presentes y no se contradicen entre sí.

### Prueba 2: Comprobación de uso responsable

Examina la salida refinada y verifica:

- [ ] Los hechos provienen únicamente del caso ficticio proporcionado.
- [ ] Los supuestos están claramente etiquetados.
- [ ] Las preguntas abiertas indican qué información debe obtenerse o validarse.
- [ ] No existen nombres de personas reales, datos personales, credenciales ni datos internos.
- [ ] No se presentan recomendaciones como asesoramiento financiero, legal o regulatorio.
- [ ] Cualquier referencia externa se trata como información que debe verificarse con fuentes confiables.

**Criterio de aprobación:** no hay afirmaciones no sustentadas presentadas como hechos de Northstar Digital.

### Prueba 3: Comprobación de utilidad ejecutiva

Revisa la tabla priorizada.

**Criterio de aprobación:** la tabla tiene ocho columnas, hasta seis filas, prioridades claras, evidencia requerida, riesgos y responsables sugeridos por función. Un directivo debe poder identificar qué acción explorar primero y qué evidencia falta antes de aprobar cambios.

### Prueba 4: Comprobación de continuidad

Abre Páginas de Microsoft 365 Copilot y verifica el nombre y contenido del cuaderno.

**Criterio de aprobación:** la página se llama exactamente **“Northstar Digital - Cuaderno de análisis”** y contiene la sección **“L02 - Prompt refinado”** con todos los apartados requeridos.

## Solución de problemas

### Problema 1: Copilot Chat no está disponible o muestra que la cuenta no tiene acceso

**Síntomas:**

- No aparece Copilot Chat en Microsoft 365.
- Se muestra un mensaje de licencia, acceso restringido o cuenta no compatible.
- La interfaz indica que se ha iniciado sesión con una cuenta personal.

**Causa probable:**

La cuenta no es una cuenta profesional o educativa de Microsoft Entra ID, Copilot Chat no está habilitado para el usuario o la configuración del tenant restringe el acceso.

**Solución:**

1. Cierra sesión en Microsoft 365.
2. Inicia sesión con la cuenta profesional o educativa asignada para la formación.
3. Confirma que el dominio y el perfil corresponden a la organización educativa o de trabajo.
4. Actualiza Microsoft Edge y vuelve a abrir Microsoft 365.
5. Si el problema continúa, informa al instructor para que valide la licencia, la asignación de Copilot Chat y la configuración del tenant. No sustituyas la cuenta por una cuenta personal.

### Problema 2: No se puede crear, guardar o encontrar la Página de Copilot

**Síntomas:**

- No aparece la opción para crear una página.
- La página no se guarda o no aparece después de actualizar el navegador.
- Se creó una página, pero tiene un nombre distinto del requerido.

**Causa probable:**

La capacidad de Páginas de Microsoft 365 Copilot puede estar deshabilitada, la sincronización puede estar pendiente o se ha creado contenido en una conversación sin convertirlo en página.

**Solución:**

1. Verifica que estás en la experiencia de Microsoft 365 Copilot con la cuenta de formación correcta.
2. Busca la opción equivalente a **Páginas**, **Crear página**, **Nueva página** o **Agregar a página**; los nombres pueden variar según la experiencia disponible.
3. Crea manualmente una página nueva si no puedes convertir directamente la respuesta de chat.
4. Asigna el nombre exacto: `Northstar Digital - Cuaderno de análisis`.
5. Espera unos segundos, actualiza la lista de páginas y confirma que la página aparece.
6. Si la función sigue sin estar disponible, guarda temporalmente el contenido ficticio en `C:\CopilotLabs\TransformarIdeasEnAccion\02-00-01\` y comunica la incidencia al instructor para que valide la habilitación de Páginas de Copilot.

## Limpieza

1. Conserva la Página de Copilot **“Northstar Digital - Cuaderno de análisis”**. No la elimines, porque se utilizará en las prácticas posteriores.
2. Conserva la conversación de Copilot Chat si tu entorno la mantiene disponible; puede servir para revisar las iteraciones realizadas.
3. Si creaste archivos temporales locales y el instructor no requiere entregarlos, elimínalos de:

   ```text
   C:\CopilotLabs\TransformarIdeasEnAccion\02-00-01\
   ```

4. Cierra las pestañas de Microsoft 365 si has terminado la sesión.
5. No conserves localmente ni compartas información real, confidencial, personal o no autorizada.

## Resumen

En esta práctica aplicaste una estructura de indicación eficaz para transformar una necesidad de negocio ambigua en un análisis inicial reutilizable. Definiste el objetivo, el contexto, los datos disponibles, las restricciones, la audiencia, el formato y los criterios de calidad.

También utilizaste Copilot Chat de forma iterativa: primero generaste una respuesta inicial, después solicitaste separar hechos, supuestos y preguntas abiertas, y finalmente pediste una tabla priorizada para facilitar el análisis ejecutivo. El resultado se guardó en la Página de Copilot **“Northstar Digital - Cuaderno de análisis”**, que servirá como registro trazable y base de continuidad para las siguientes prácticas.

### Recursos opcionales

- [Microsoft Support: Introducción a Microsoft 365 Copilot Chat](https://support.microsoft.com/es-es/copilot)
- [Microsoft Learn: Crear indicaciones eficaces para Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/prompt-engineering)
- [Microsoft Learn: Información general sobre Microsoft 365 Copilot Chat](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-chat)
