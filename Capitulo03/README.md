# Análisis de la experiencia digital de inversionistas internacionales

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 20 minutos |
| Complejidad | Media |
| Nivel de Bloom | Crear |

## Descripción general

En esta práctica ampliarás el caso de **Northstar Digital** para analizar la experiencia digital de tres tipos de inversionistas internacionales que utilizan un portal de inversión. Usarás Microsoft 365 Copilot Chat para investigar información pública, elaborar una matriz de experiencia por segmento y transformar el análisis en un backlog priorizado de mejoras.

El resultado no debe tratarse como asesoramiento financiero, legal o normativo. Las respuestas de Copilot serán borradores de trabajo: deberás distinguir los hechos sustentados por fuentes, las hipótesis de negocio y las recomendaciones propuestas antes de conservar el análisis en la Página de Microsoft 365 Copilot.

## Objetivos de aprendizaje

Al completar esta práctica, podrás:

- [ ] Investigar factores públicos que afectan a la experiencia digital de inversionistas internacionales.
- [ ] Usar una indicación orientada a roles, con objetivo, contexto, restricciones, formato y criterios de calidad explícitos.
- [ ] Diferenciar observaciones sustentadas, hipótesis de negocio y recomendaciones generadas por IA.
- [ ] Crear una matriz de experiencia para un inversionista minorista internacional, un representante institucional y un usuario de alto patrimonio.
- [ ] Elaborar un backlog priorizado de mejoras con impacto esperado, evidencia requerida y criterios de validación.

## Requisitos previos

### Conocimientos necesarios

Antes de comenzar, debes poder:

- Reconocer los componentes de una indicación eficaz: **objetivo, contexto y resultado esperado**.
- Revisar una respuesta de Copilot como borrador, no como una fuente definitiva.
- Distinguir entre información verificable, supuestos razonables y decisiones que requieren validación humana.
- Aplicar prácticas de uso responsable de IA: no compartir datos personales, información de clientes, contratos, credenciales, información financiera no pública ni contenido interno no autorizado.

### Acceso necesario

Debes contar con lo siguiente:

- Finalización del laboratorio **02-00-01**.
- Acceso a la Página de Copilot llamada exactamente **Northstar Digital - Cuaderno de análisis**.
- Acceso habilitado a **Microsoft 365 Copilot Chat** con capacidad de consulta web.
- Una cuenta profesional o educativa de Microsoft Entra ID con Copilot Chat y Páginas de Copilot habilitados.
- La indicación estructurada y los criterios de evaluación creados en el laboratorio anterior, disponibles en la Página de Copilot.

> **Importante:** utiliza únicamente información ficticia del caso Northstar Digital y fuentes públicas. No copies conversaciones reales de clientes, expedientes de inversiones, identificaciones, direcciones, documentos de cumplimiento ni datos de cuentas.

## Entorno de laboratorio

### Hardware de referencia

| Componente | Requisito de referencia |
|---|---|
| Pantalla | Resolución mínima de 1920 × 1080 |
| Conectividad | 10 Mbps de descarga y 2 Mbps de carga como mínimo |
| Memoria | 8 GB de RAM como mínimo |
| Almacenamiento disponible | 2 GB para caché del navegador y archivos de práctica |
| Audio | Auriculares y micrófono opcionales |

### Software y servicios de referencia

| Componente | Versión o configuración |
|---|---|
| Sistema operativo | Windows 11 Enterprise 23H2, compilación 22631.4169 |
| Navegador | Microsoft Edge 128.0.2739.79 |
| Aplicaciones de Microsoft 365 | Microsoft 365 Apps for enterprise 2408, compilación 17928.20156 |
| Servicio de IA | Microsoft 365 Copilot Chat |
| Espacio de trabajo | Páginas de Microsoft 365 Copilot |
| Directorio de trabajo | `C:\CopilotLabs\TransformarIdeasEnAccion\` |

Las capacidades visibles de Copilot pueden variar según licencia, región, configuración administrativa y cambios del servicio web. El instructor debe comprobar el tenant antes de la sesión.

### Preparación del directorio local

Este laboratorio se completa principalmente en Copilot Chat y Páginas de Copilot. Crea una carpeta local solo si necesitas guardar capturas de evidencia o un borrador exportado.

1. Abre **Símbolo del sistema** o **Windows PowerShell**.
2. Ejecuta el siguiente comando:

```powershell
New-Item -ItemType Directory -Force -Path "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-01"
```

3. Si deseas confirmar que la carpeta existe, ejecuta:

```powershell
Get-ChildItem "C:\CopilotLabs\TransformarIdeasEnAccion"
```

## Procedimiento paso a paso

### Paso 1. Confirmar el contexto y preparar el espacio de trabajo

**Objetivo:** Verificar que trabajarás sobre la página de continuidad correcta y que el análisis se limita a información pública y ficticia.

**Instrucciones:**

1. Abre Microsoft Edge e inicia sesión con tu cuenta profesional o educativa autorizada.
2. Accede a Microsoft 365 Copilot.
3. Abre **Páginas de Microsoft 365 Copilot**.
4. Localiza y abre la página cuyo nombre sea exactamente:

   ```text
   Northstar Digital - Cuaderno de análisis
   ```

5. Revisa que la página contenga el contenido creado en el laboratorio anterior, en especial la sección titulada:

   ```text
   L02 - Prompt refinado
   ```

6. Desplázate al final de la página y crea una nueva sección con el título obligatorio:

   ```text
   L03.1 - Experiencia de inversionistas
   ```

7. Debajo del título, añade esta nota de alcance:

   > **Alcance y uso responsable:** Este análisis utiliza un caso ficticio de Northstar Digital y fuentes públicas. No constituye asesoramiento financiero, legal ni normativo. Toda afirmación relevante debe verificarse antes de usarla para tomar decisiones o realizar comunicaciones externas.

8. Mantén la página abierta en una mitad de la pantalla y Copilot Chat en la otra mitad, si el tamaño de pantalla lo permite.

**Resultado esperado:**

La Página de Copilot contiene una nueva sección titulada **L03.1 - Experiencia de inversionistas** y una nota que delimita el uso responsable del análisis.

**Verificación:**

- Confirma que el nombre de la página es exactamente **Northstar Digital - Cuaderno de análisis**.
- Confirma que no has creado una página nueva independiente.
- Comprueba que no has incluido datos reales, personales, confidenciales o no autorizados.

---

### Paso 2. Formular una indicación de investigación orientada a roles

**Objetivo:** Solicitar a Copilot un análisis inicial estructurado de expectativas y fricciones de tres perfiles de inversionista internacional.

**Instrucciones:**

1. Abre una conversación nueva en **Copilot Chat**.
2. Comprueba que el modo de conversación permita consultas basadas en la web pública, si dicha opción aparece en tu experiencia.
3. Copia y pega la siguiente indicación. Puedes adaptar solo la redacción, pero conserva los segmentos, las restricciones y el formato de salida.

```text
Actúa como analista de experiencia digital para una empresa ficticia de servicios de inversión llamada Northstar Digital.

Objetivo:
Identificar factores que pueden afectar la experiencia digital de inversionistas internacionales que utilizan un portal de inversión, para crear un backlog inicial de mejoras.

Contexto:
Northstar Digital desea atender a clientes internacionales mediante un portal digital. El análisis debe considerar expectativas y posibles fricciones relacionadas con idiomas, zonas horarias, cumplimiento normativo, transparencia de tarifas, accesibilidad, seguridad, canales de soporte y confianza.

Analiza estos tres segmentos por separado:
1. Inversionista minorista internacional.
2. Representante institucional.
3. Usuario de alto patrimonio.

Restricciones:
- Usa solo información pública y principios generales; no inventes políticas, cifras, países atendidos ni características reales de Northstar Digital.
- No proporciones asesoramiento financiero, legal o fiscal.
- Diferencia claramente entre observaciones sustentadas, hipótesis de negocio y recomendaciones.
- Cuando menciones una afirmación verificable, proporciona una fuente pública o indica explícitamente que requiere validación.
- Señala cuando una necesidad puede variar por jurisdicción, idioma, mercado o tipo de cliente.

Formato de salida:
Crea una tabla con las columnas:
Segmento | Necesidad o expectativa | Posible punto de fricción | Causa posible | Clasificación (hecho/hipótesis/recomendación) | Evidencia o fuente necesaria | Impacto potencial de negocio | Pregunta de validación.

Criterios de calidad:
- Incluye al menos cuatro filas por segmento.
- Evita generalizaciones absolutas.
- Prioriza claridad, trazabilidad y utilidad para un equipo de producto.
- Indica límites o incertidumbres al final.
```

4. Envía la indicación.
5. Espera la respuesta completa y revisa si Copilot incluye fuentes, enlaces, citas o referencias.
6. No copies todavía toda la respuesta a la Página de Copilot. Primero evalúala críticamente en el paso siguiente.

**Resultado esperado:**

Copilot genera una tabla diferenciada por los tres segmentos, con necesidades, fricciones potenciales, evidencia requerida e impacto de negocio. La respuesta debe incluir advertencias sobre variaciones normativas o de mercado.

**Verificación:**

Comprueba que la respuesta:

- Incluye los tres segmentos solicitados.
- Separa explícitamente hechos, hipótesis y recomendaciones.
- No afirma que Northstar Digital cumple requisitos específicos ni opera en un país concreto.
- No presenta afirmaciones regulatorias sin fuente o sin indicar que requieren validación.
- Incluye fuentes o marca los elementos que deben validarse.

---

### Paso 3. Evaluar y refinar la respuesta de Copilot Chat

**Objetivo:** Aplicar el patrón solicitar, revisar y refinar para mejorar precisión, trazabilidad y utilidad del análisis inicial.

**Instrucciones:**

1. Revisa la respuesta generada en el paso anterior.
2. Identifica al menos:
   - Una afirmación que parezca sustentada por una fuente pública.
   - Una hipótesis sobre comportamiento o expectativas de usuarios.
   - Una recomendación propuesta por Copilot.
3. Verifica las fuentes disponibles abriendo, cuando sea posible, los enlaces o referencias proporcionados por Copilot.
4. Evalúa cada fuente con estas preguntas:
   - ¿La fuente existe y es accesible?
   - ¿Respaldan el enlace y el texto de la fuente la afirmación realizada?
   - ¿La fuente es actual y procede de una entidad fiable?
   - ¿La afirmación aplica de forma general o solo a una jurisdicción, mercado o tipo de organización?
5. Si encuentras enlaces poco claros, referencias ausentes o afirmaciones demasiado generales, envía esta indicación de refinamiento en la misma conversación:

```text
Revisa tu análisis anterior con enfoque de calidad y trazabilidad.

Para cada fila:
- Conserva la clasificación hecho, hipótesis o recomendación.
- Si es un hecho, indica una fuente pública verificable o cambia la clasificación a hipótesis.
- Si depende de una jurisdicción o normativa específica, indícalo claramente.
- Elimina o reformula cualquier afirmación que sugiera que Northstar Digital tiene una capacidad, licencia, política o cobertura geográfica no confirmada.
- Reduce las frases vagas y convierte cada punto de fricción en una situación observable por un usuario.
- Mantén el resultado en una tabla lista para copiar a una Página de Copilot.
```

6. Revisa la versión refinada.
7. Selecciona entre 12 y 15 filas útiles en total, procurando que haya al menos cuatro por segmento.
8. Da preferencia a filas que describan fricciones observables, por ejemplo:
   - Idioma de la interfaz o de los documentos.
   - Disponibilidad de soporte en franjas horarias distintas.
   - Claridad de tarifas, conversiones de moneda y cargos.
   - Requisitos de verificación de identidad.
   - Avisos de seguridad y autenticación.
   - Accesibilidad de formularios y documentos.
   - Trazabilidad de solicitudes y comunicaciones.
   - Necesidades de aprobación, auditoría o reportes para clientes institucionales.

**Resultado esperado:**

Dispones de una versión revisada del análisis que evita afirmaciones no verificadas, expresa incertidumbres y diferencia con claridad entre evidencia, hipótesis y recomendaciones.

**Verificación:**

Antes de continuar, confirma lo siguiente:

| Criterio | Resultado esperado |
|---|---|
| Hechos | Tienen fuente pública comprobable o una nota de validación pendiente. |
| Hipótesis | Están redactadas como posibilidades, no como certezas. |
| Recomendaciones | Describen una posible acción y no se presentan como requisito normativo confirmado. |
| Referencias normativas | Indican que pueden depender de la jurisdicción y deben ser revisadas por especialistas autorizados. |
| Caso Northstar Digital | No contiene datos inventados sobre productos, clientes, países, licencias o resultados financieros. |

---

### Paso 4. Crear la matriz de experiencia en la Página de Copilot

**Objetivo:** Conservar un análisis reutilizable y trazable en la Página de Copilot de continuidad.

**Instrucciones:**

1. Vuelve a la Página **Northstar Digital - Cuaderno de análisis**.
2. En la sección **L03.1 - Experiencia de inversionistas**, añade el subtítulo:

   ```text
   Matriz de experiencia por segmento
   ```

3. Inserta una tabla con las siguientes columnas:

| Segmento | Necesidad o expectativa | Punto de fricción | Causa posible | Tipo de hallazgo | Evidencia necesaria | Impacto de negocio | Prioridad inicial |
|---|---|---|---|---|---|---|---|

4. Copia desde Copilot Chat únicamente las filas revisadas y útiles.
5. Ajusta la columna **Tipo de hallazgo** usando exclusivamente una de estas etiquetas:
   - **Hecho sustentado**
   - **Hipótesis de negocio**
   - **Recomendación propuesta**
6. En la columna **Evidencia necesaria**, indica una fuente o método de validación. Utiliza formulaciones concretas, por ejemplo:
   - “Verificar fuente pública citada y fecha de publicación.”
   - “Revisar analítica de abandono por idioma y país.”
   - “Realizar cinco entrevistas de descubrimiento por segmento.”
   - “Solicitar revisión de cumplimiento por jurisdicción.”
   - “Ejecutar prueba de accesibilidad con lectores de pantalla y navegación por teclado.”
   - “Analizar tickets de soporte por zona horaria y canal.”
7. En la columna **Impacto de negocio**, usa uno de estos niveles:
   - Alto
   - Medio
   - Bajo
8. Asigna una **Prioridad inicial** usando este criterio:
   - **P1:** impacto alto y riesgo relevante de confianza, cumplimiento, seguridad o abandono.
   - **P2:** impacto medio o alto, pero evidencia insuficiente para priorizar definitivamente.
   - **P3:** mejora útil con impacto bajo o que depende de una necesidad todavía no validada.
9. Añade, debajo de la tabla, una nota de interpretación:

   > Las prioridades son iniciales y se basan en información pública, hipótesis y criterios de experiencia. Deben validarse con datos autorizados, investigación de usuarios, responsables de producto, seguridad, accesibilidad y cumplimiento antes de planificar cambios.

**Resultado esperado:**

La sección **L03.1 - Experiencia de inversionistas** contiene una matriz de 12 a 15 filas, organizada por segmento y con trazabilidad sobre el tipo de hallazgo y la evidencia necesaria.

**Verificación:**

La matriz debe incluir los tres segmentos:

- Inversionista minorista internacional.
- Representante institucional.
- Usuario de alto patrimonio.

Además, confirma que:

- No hay afirmaciones sin clasificación.
- Cada fila tiene un método de evidencia o una fuente que debe revisarse.
- La prioridad no se basa únicamente en la redacción persuasiva de Copilot.
- Los puntos de fricción se expresan como situaciones que un usuario podría experimentar.

---

### Paso 5. Convertir la matriz en un backlog priorizado

**Objetivo:** Crear un backlog inicial de mejoras de experiencia digital que pueda utilizarse como insumo en la práctica sobre escenarios económicos.

**Instrucciones:**

1. En Copilot Chat, usa la matriz creada como base. Si la interfaz permite adjuntar o referenciar el contenido de la Página de Copilot, úsalo únicamente si tienes autorización y el contenido sigue siendo ficticio y no confidencial.
2. Si no puedes referenciar la página, copia solo las filas no confidenciales de la matriz en una nueva indicación.
3. Envía la siguiente indicación:

```text
A partir de la siguiente matriz de experiencia de Northstar Digital, crea un backlog inicial de mejoras de experiencia digital.

[PEGA AQUÍ LA MATRIZ REVISADA]

Instrucciones:
- No inventes datos, capacidades actuales ni requisitos regulatorios de Northstar Digital.
- Trata los elementos clasificados como hipótesis como oportunidades de investigación, no como problemas confirmados.
- Agrupa mejoras similares.
- Prioriza usando impacto potencial, riesgo para la confianza, dependencia de cumplimiento, seguridad, accesibilidad y evidencia disponible.
- Indica dependencias y la evidencia mínima necesaria antes de pasar a implementación.
- Distingue entre acciones de descubrimiento, diseño, contenido, soporte, seguridad y cumplimiento.

Formato de salida:
Crea una tabla con:
ID | Mejora u oportunidad | Segmento principal | Problema que aborda | Tipo de acción | Prioridad | Impacto esperado | Evidencia mínima requerida | Dependencias | Criterio de aceptación inicial.

Después de la tabla, incluye:
1. Las tres mejoras que deberían investigarse primero.
2. Las tres afirmaciones que requieren validación humana antes de una decisión.
3. Un apartado llamado "Supuestos y límites".
```

4. Revisa el backlog generado.
5. Elimina o reformula cualquier elemento que:
   - Presente una hipótesis como un hecho.
   - Indique que una obligación legal se aplica universalmente.
   - Asuma una funcionalidad existente de Northstar Digital.
   - Recomiende implementar una solución sin evidencia mínima o sin responsables de validación.
6. Vuelve a la Página de Copilot.
7. Debajo de la matriz, añade el subtítulo:

   ```text
   Backlog priorizado de mejoras
   ```

8. Copia el backlog revisado a la página.
9. Asegúrate de que el backlog incluya, como mínimo, seis elementos y que cubra al menos cuatro de estas áreas:
   - Idioma y localización.
   - Transparencia de tarifas.
   - Soporte y zonas horarias.
   - Accesibilidad.
   - Seguridad y confianza.
   - Cumplimiento y documentación.
   - Reportes o flujos para clientes institucionales.
10. Añade este texto al final del backlog:

   > **Conexión con la siguiente práctica:** Este backlog se utilizará como insumo para analizar cómo distintos acontecimientos económicos podrían afectar las prioridades de experiencia, comunicación y soporte de Northstar Digital.

**Resultado esperado:**

La Página de Copilot contiene un backlog de al menos seis mejoras u oportunidades, con prioridad, impacto esperado, evidencia requerida, dependencias y criterios de aceptación iniciales.

**Verificación:**

Comprueba que cada elemento del backlog responda a las siguientes preguntas:

| Pregunta de control | Resultado esperado |
|---|---|
| ¿Qué problema aborda? | El problema se describe de forma concreta y centrada en el usuario. |
| ¿Para quién es relevante? | Se identifica un segmento principal o varios segmentos afectados. |
| ¿Qué evidencia falta? | Se define una fuente, prueba, entrevista, métrica o revisión necesaria. |
| ¿Por qué tiene esa prioridad? | La prioridad se relaciona con impacto, confianza, riesgo o dependencia. |
| ¿Qué debe ocurrir antes de implementar? | Se indican dependencias, validaciones o responsables expertos. |

---

### Paso 6. Registrar una conclusión ejecutiva y validar la trazabilidad

**Objetivo:** Sintetizar el análisis sin presentar conclusiones no verificadas como decisiones definitivas.

**Instrucciones:**

1. En la sección **L03.1 - Experiencia de inversionistas**, añade el subtítulo:

   ```text
   Conclusión ejecutiva inicial
   ```

2. Redacta un resumen de entre 100 y 150 palabras que incluya:
   - Los segmentos analizados.
   - Dos o tres fricciones de mayor prioridad.
   - La diferencia entre hechos sustentados e hipótesis.
   - La necesidad de validar el backlog antes de implementarlo.
   - La conexión con el análisis de escenarios económicos de la siguiente práctica.
3. Puedes pedir a Copilot un borrador mediante esta indicación:

```text
Redacta una conclusión ejecutiva inicial de 100 a 150 palabras basada en esta matriz y backlog.

Requisitos:
- Tono profesional y claro para responsables de negocio.
- No presentes hipótesis como hechos.
- Indica que las prioridades requieren validación con evidencia autorizada.
- No incluyas asesoramiento financiero, legal o normativo.
- Menciona que el backlog será un insumo para analizar escenarios económicos posteriores.

[PEGA AQUÍ EL BACKLOG REVISADO]
```

4. Revisa y adapta el borrador antes de incorporarlo a la página.
5. Confirma que los títulos de la página respetan la convención establecida:
   - `L02 - Prompt refinado`
   - `L03.1 - Experiencia de inversionistas`

**Resultado esperado:**

La Página de Copilot presenta una conclusión ejecutiva breve, prudente y trazable, vinculada al backlog y a la siguiente práctica.

**Verificación:**

La conclusión es válida si:

- No contiene cifras, hechos regulatorios o promesas de negocio no verificadas.
- Distingue entre evidencia y supuestos.
- Indica que se requiere validación humana.
- Explica de forma comprensible por qué el backlog es relevante para decisiones futuras.

## Validación y pruebas

Realiza la siguiente lista de comprobación antes de dar por finalizado el laboratorio.

| Prueba | Método | Resultado esperado |
|---|---|---|
| Página de continuidad | Abrir Páginas de Copilot y verificar el nombre. | El trabajo está en **Northstar Digital - Cuaderno de análisis**. |
| Título de la práctica | Revisar encabezados de la página. | Existe el encabezado exacto **L03.1 - Experiencia de inversionistas**. |
| Cobertura de segmentos | Revisar la matriz. | Aparecen los tres perfiles solicitados. |
| Clasificación de hallazgos | Revisar la columna correspondiente. | Cada fila se clasifica como hecho sustentado, hipótesis de negocio o recomendación propuesta. |
| Trazabilidad | Revisar la columna de evidencia. | Todas las filas indican una fuente, prueba o validación necesaria. |
| Priorización | Revisar matriz y backlog. | Las prioridades P1, P2 y P3 se justifican por impacto, riesgo y evidencia disponible. |
| Uso responsable | Revisar el contenido introducido en Copilot. | No se incluyeron datos personales, confidenciales, financieros reales o información no autorizada. |
| Calidad de las fuentes | Abrir una muestra de enlaces o referencias. | Las fuentes son accesibles, pertinentes y no se usan como sustituto de revisión humana. |
| Preparación para la siguiente práctica | Revisar el cierre del backlog. | El backlog se identifica como insumo para el análisis de escenarios económicos. |

### Criterio de finalización

El laboratorio se considera completado cuando la Página de Copilot contiene:

1. La nota de alcance y uso responsable.
2. Una matriz de experiencia de 12 a 15 filas para los tres segmentos.
3. Una clasificación clara entre hechos, hipótesis y recomendaciones.
4. Un backlog priorizado de al menos seis elementos.
5. Una conclusión ejecutiva inicial.
6. La conexión explícita con la práctica posterior sobre escenarios económicos.

## Solución de problemas

### Problema 1: Copilot Chat no muestra fuentes, enlaces o resultados basados en información pública

**Síntomas:**

- La respuesta no contiene citas ni enlaces.
- Copilot responde con contenido muy general.
- No aparece una opción relacionada con búsqueda web o fuentes públicas.
- Las referencias no son suficientes para validar una afirmación importante.

**Causa probable:**

La capacidad de consulta web puede no estar disponible en la configuración actual, puede depender de la licencia o de políticas del tenant, o la indicación puede no haber solicitado fuentes y trazabilidad de forma explícita.

**Solución:**

1. Verifica que has iniciado sesión con la cuenta profesional o educativa correcta.
2. Inicia una conversación nueva y vuelve a solicitar fuentes públicas de manera explícita.
3. Añade a la indicación: “Incluye enlaces públicos verificables para cada hecho; si no puedes verificarlos, clasifícalos como hipótesis”.
4. Si la capacidad sigue sin estar disponible, utiliza Copilot para estructurar preguntas y registra en la matriz “Fuente pública pendiente de verificación”.
5. Informa al instructor o administrador del tenant si el laboratorio requiere búsqueda web y esta capacidad debería estar habilitada.

### Problema 2: La tabla contiene afirmaciones demasiado definitivas sobre normativa, seguridad o necesidades de los usuarios

**Síntomas:**

- Copilot afirma que una norma se aplica a todos los países.
- La respuesta indica que Northstar Digital debe implementar una función concreta sin evidencia.
- Los supuestos sobre idioma, accesibilidad, tarifas o canales de soporte se presentan como hechos confirmados.
- El backlog parece una lista de decisiones de implementación en lugar de oportunidades por validar.

**Causa probable:**

La indicación no limitó suficientemente las suposiciones o la respuesta inicial no fue revisada como borrador. Copilot puede generar contenido plausible que requiere comprobación contextual, normativa y profesional.

**Solución:**

1. Marca cada afirmación como hecho, hipótesis o recomendación.
2. Convierte cualquier afirmación no sustentada en una hipótesis, por ejemplo: “Puede existir abandono durante la verificación de identidad; validar con analítica y pruebas de usuario”.
3. Pide a Copilot que identifique jurisdicciones, incertidumbres y evidencia faltante.
4. Añade dependencias de revisión por equipos autorizados de cumplimiento, seguridad, accesibilidad, producto o jurídico cuando corresponda.
5. No implementes ni comuniques externamente una conclusión hasta validarla con las personas responsables y fuentes aplicables.

## Limpieza

1. Verifica que todo el trabajo final esté guardado en la Página **Northstar Digital - Cuaderno de análisis**.
2. Si guardaste evidencias locales, confirma que se encuentran únicamente en:

   ```text
   C:\CopilotLabs\TransformarIdeasEnAccion\03-00-01\
   ```

3. No guardes capturas que incluyan información de otras conversaciones, datos de cuentas o contenido no autorizado.
4. Cierra las pestañas de Copilot Chat que no necesites.
5. Mantén la Página de Copilot disponible para la siguiente práctica; no elimines las secciones `L02 - Prompt refinado` ni `L03.1 - Experiencia de inversionistas`.
6. Cierra sesión solo si el procedimiento de tu organización lo requiere y no vas a continuar inmediatamente con el siguiente laboratorio.

## Resumen

En esta práctica utilizaste Copilot Chat como apoyo para investigar y estructurar un análisis inicial de la experiencia digital de inversionistas internacionales. Aplicaste una indicación con objetivo, contexto, restricciones, formato y criterios de calidad, y revisaste la respuesta para distinguir hechos sustentados, hipótesis de negocio y recomendaciones.

También creaste una matriz de experiencia y un backlog priorizado en la Página de Copilot de continuidad. Estos entregables no son decisiones definitivas: constituyen un borrador trazable que debe validarse con fuentes públicas, datos autorizados, investigación de usuarios y revisión de especialistas antes de implementar cambios o realizar comunicaciones externas.

### Recursos opcionales

- [Microsoft Support: Bienvenido a Copilot Chat](https://support.microsoft.com/es-es/topic/bienvenido-a-copilot-chat-34c93d56-86e6-4b5b-8cc8-59cbe8e53bc3)
- [Microsoft Support: Introducción a Microsoft 365 Copilot Chat](https://support.microsoft.com/es-es/copilot-microsoft-365)
- [Microsoft Learn: Introducción a Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/)

---

# Análisis de acontecimientos económicos y escenarios what-if

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 20 minutos |
| Complejidad | Media |
| Nivel de Bloom | Crear |

## Descripción general

En esta práctica utilizarás Copilot Chat para construir un análisis económico de escenarios *what-if* para Northstar Digital y sus inversionistas internacionales. Partirás del backlog de experiencia digital creado en el laboratorio 03-00-01, definirás supuestos explícitos y compararás un escenario base, moderado y adverso.

El resultado será una tabla reutilizable que diferencie hechos verificados de proyecciones, relacione los escenarios económicos con prioridades de producto y proponga señales de alerta, decisiones y acciones. Guardarás el resultado en la página de continuidad obligatoria para utilizarlo en el laboratorio 03-00-03.

## Objetivos de aprendizaje

Al finalizar esta práctica, podrás:

- [ ] Formular una indicación de análisis económico con contexto, horizonte temporal, variables, supuestos y formato de salida definidos.
- [ ] Construir escenarios base, moderado y adverso que incluyan tipos de interés, volatilidad de divisas y comportamiento de un índice bursátil.
- [ ] Distinguir hechos públicos verificables, supuestos de trabajo y proyecciones generadas por IA.
- [ ] Relacionar los escenarios con el backlog de experiencia digital para decidir qué iniciativas acelerar, mantener o aplazar.
- [ ] Conservar una tabla de escenarios, indicadores de seguimiento y decisiones recomendadas en Páginas de Microsoft 365 Copilot.

## Requisitos previos

### Conocimientos necesarios

- Haber completado el laboratorio **03-00-01**.
- Comprender de forma básica los conceptos de tipo de interés, volatilidad de divisas, índice bursátil, supuesto y escenario.
- Saber que una respuesta de Copilot es un borrador que requiere revisión humana, especialmente si contiene cifras, fechas, fuentes o recomendaciones de negocio.
- Conocer la estructura de una indicación eficaz: objetivo, contexto y resultado esperado.

### Acceso necesario

- Cuenta profesional o educativa de Microsoft Entra ID.
- Acceso habilitado a Microsoft 365 Copilot Chat y Páginas de Microsoft 365 Copilot.
- Acceso web desde Microsoft Edge para consultar fuentes públicas.
- La página de continuidad creada o utilizada en prácticas anteriores con el nombre exacto:

  ```text
  Northstar Digital - Cuaderno de análisis
  ```

- La matriz de experiencia y el backlog priorizado de 03-00-01 disponibles en dicha página, normalmente bajo el título:

  ```text
  L03.1 - Experiencia de inversionistas
  ```

> **Uso responsable de IA:** utiliza únicamente el caso ficticio Northstar Digital, el backlog autorizado de la práctica y fuentes públicas. No introduzcas datos personales, información financiera interna, contratos, credenciales, datos de clientes ni contenido no autorizado.

## Entorno del laboratorio

### Hardware de referencia

| Componente | Requisito de referencia |
|---|---|
| Equipo | Windows 11 de 64 bits con Intel Core i5 de 10.ª generación o equivalente |
| Memoria | 8 GB de RAM como mínimo |
| Pantalla | Resolución mínima de 1920 x 1080 |
| Red | Conexión estable de al menos 10 Mbps de descarga y 2 Mbps de carga |
| Espacio libre | 2 GB para caché del navegador y archivos de práctica |

### Software y servicios de referencia

| Componente | Versión o configuración de referencia |
|---|---|
| Sistema operativo | Windows 11 Enterprise 23H2, compilación 22631.4169 |
| Navegador | Microsoft Edge 128.0.2739.79 |
| Aplicaciones | Microsoft 365 Apps for enterprise 2408, compilación 17928.20156 |
| Servicio de IA | Microsoft 365 Copilot Chat, experiencia web disponible para la sesión del 2026-09-16 |
| Espacio de trabajo | Páginas de Microsoft 365 Copilot |
| Directorio local | `C:\CopilotLabs\TransformarIdeasEnAccion\03-00-02\` |

> La interfaz, las opciones de búsqueda web y las capacidades disponibles pueden variar según licencia, región, configuración del tenant y cambios del servicio. El instructor debe comprobar el acceso funcional el día anterior.

### Preparación del directorio local

Si necesitas guardar una copia temporal de la indicación o de la tabla final, abre **Windows PowerShell** y ejecuta:

```powershell
New-Item -ItemType Directory -Force -Path "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-02" | Out-Null
```

Comprueba que se creó el directorio:

```powershell
Get-ChildItem "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-02"
```

## Procedimiento paso a paso

### Paso 1. Revisar el backlog y definir límites de análisis

**Objetivo:** identificar las iniciativas de experiencia digital que se evaluarán frente a los escenarios económicos y establecer límites para un análisis responsable.

**Instrucciones:**

1. Abre Microsoft Edge e inicia sesión con tu cuenta profesional o educativa.
2. Accede a Microsoft 365 Copilot y abre la página:

   ```text
   Northstar Digital - Cuaderno de análisis
   ```

3. Localiza la sección:

   ```text
   L03.1 - Experiencia de inversionistas
   ```

4. Revisa la matriz de experiencia y el backlog priorizado del laboratorio anterior.
5. Identifica entre tres y cinco iniciativas del backlog. Si el backlog contiene más elementos, selecciona las iniciativas que tengan mayor relación con:
   - Confianza de inversionistas.
   - Transparencia y acceso a información.
   - Experiencia digital internacional.
   - Rendimiento, disponibilidad o autoservicio.
   - Comunicaciones y soporte durante eventos relevantes.

6. Copia o anota únicamente los siguientes elementos autorizados:
   - Nombre breve de cada iniciativa.
   - Prioridad actual.
   - Problema de experiencia que resuelve.
   - Resultado esperado para el usuario o inversionista.
   - Dependencias conocidas, si existen.

7. Define el marco de análisis que utilizarás en la indicación:
   - **Horizonte temporal:** 6 meses.
   - **Público:** responsables de producto y liderazgo de Northstar Digital.
   - **Ámbito:** impacto en usuarios, operaciones, prioridades de producto e inversionistas internacionales.
   - **Variables obligatorias:** tipos de interés, volatilidad de divisas e índice bursátil global o relevante.
   - **Regla de seguridad:** no presentar proyecciones como hechos ni recomendar decisiones financieras de inversión.

8. Revisa que las iniciativas seleccionadas no contengan información confidencial. Sustituye cualquier referencia sensible por una descripción genérica autorizada.

**Resultado esperado:**

Dispones de una lista breve de iniciativas priorizadas y de un marco claro para analizar su comportamiento ante cambios económicos.

Ejemplo de formato de notas de trabajo:

| Iniciativa del backlog | Prioridad actual | Resultado de experiencia esperado |
|---|---|---|
| Panel de información para inversionistas | Alta | Facilitar acceso claro y rápido a información relevante |
| Mejoras de rendimiento en portal internacional | Alta | Reducir fricción y tiempos de carga |
| Centro de ayuda contextual | Media | Disminuir consultas repetitivas y mejorar autoservicio |
| Personalización avanzada de contenidos | Media | Mostrar información más relevante por perfil |

**Verificación:**

- Confirma que puedes identificar al menos tres iniciativas procedentes de 03-00-01.
- Confirma que ninguna nota incluye información personal, financiera interna o no autorizada.
- Confirma que el horizonte temporal de trabajo es de 6 meses.
- Confirma que las tres variables económicas obligatorias están definidas.

---

### Paso 2. Diseñar una indicación estructurada para el análisis what-if

**Objetivo:** crear una indicación que obligue a Copilot a declarar supuestos, separar hechos y proyecciones, y comparar escenarios de manera estructurada.

**Instrucciones:**

1. Abre Copilot Chat en una nueva conversación.
2. No pegues información confidencial ni datos reales no autorizados de tu organización.
3. Sustituye los elementos entre corchetes del siguiente modelo por las iniciativas reales o ficticias autorizadas de tu backlog de 03-00-01.
4. Copia la indicación completa en Copilot Chat.

```text
Actúa como analista de escenarios para Northstar Digital, una empresa ficticia con inversionistas internacionales. Necesito un análisis de escenarios what-if para apoyar decisiones de experiencia digital y producto; no necesito asesoramiento financiero ni recomendaciones de inversión.

Contexto autorizado:
- Horizonte de análisis: próximos 6 meses.
- Público: liderazgo de producto, operaciones y experiencia de inversionistas.
- Iniciativas priorizadas del backlog de experiencia digital:
  1. [Iniciativa 1: prioridad y resultado esperado]
  2. [Iniciativa 2: prioridad y resultado esperado]
  3. [Iniciativa 3: prioridad y resultado esperado]
  4. [Opcional: iniciativa 4]
  5. [Opcional: iniciativa 5]

Analiza estas variables económicas:
1. Aumento de tipos de interés.
2. Volatilidad de divisas que afecte a usuarios e inversionistas internacionales.
3. Caída de un índice bursátil amplio y relevante para inversionistas internacionales.

Usa estos escenarios de trabajo, que son supuestos para el ejercicio y no hechos actuales:
- Base: tipos +0 a +25 puntos básicos, volatilidad de divisas limitada y variación del índice entre 0 % y -5 %.
- Moderado: tipos +50 a +100 puntos básicos, depreciación o apreciación de una divisa relevante del 5 % al 10 %, e índice entre -5 % y -15 %.
- Adverso: tipos superiores a +100 puntos básicos, movimiento de divisas superior al 10 % e índice inferior a -15 %.

Instrucciones de calidad:
- Separa explícitamente: hechos públicos verificados, supuestos de trabajo, proyecciones e incertidumbres.
- Si no dispones de datos públicos actuales y verificables, indícalo; no inventes cifras, fechas, fuentes ni citas.
- Para cualquier hecho actual que menciones, incluye una fuente pública, URL y fecha de consulta. Si no puedes proporcionar una fuente verificable, clasifícalo como no verificado.
- Explica de forma prudente relaciones plausibles, no causalidades garantizadas.
- Evalúa el posible efecto sobre: usuarios/inversionistas, operaciones, confianza/reputación y prioridades de producto.
- Relaciona cada escenario con las iniciativas del backlog e indica si se debe acelerar, mantener, aplazar o revisar cada iniciativa.
- No uses lenguaje que presente los escenarios como predicciones.

Devuelve el resultado en español con estas secciones exactas:

1. Alcance y limitaciones.
2. Registro de hechos públicos verificados, con fuente y fecha de consulta.
3. Supuestos de trabajo.
4. Tabla comparativa de escenarios con las columnas:
   Escenario | Tipos de interés | Divisas | Índice bursátil | Efecto en usuarios/inversionistas | Efecto operativo | Riesgo para confianza | Nivel de incertidumbre.
5. Tabla de decisiones de backlog con las columnas:
   Iniciativa | Base | Moderado | Adverso | Decisión recomendada | Justificación | Dependencia o condición.
6. Indicadores de seguimiento con las columnas:
   Indicador | Señal de alerta | Frecuencia | Responsable sugerido | Acción al activarse.
7. Cinco preguntas de validación humana antes de presentar este análisis a dirección.

Mantén un tono ejecutivo, claro y prudente. Señala de manera visible cualquier limitación de información.
```

5. Antes de enviar la indicación, comprueba que:
   - Incluye las tres variables económicas requeridas.
   - Establece un horizonte de 6 meses.
   - Contiene escenarios base, moderado y adverso.
   - Exige una separación entre hechos, supuestos y proyecciones.
   - Solicita tablas y criterios de decisión.
   - Prohíbe inventar cifras, fuentes o citas.

6. Envía la indicación.

**Resultado esperado:**

Copilot genera un primer borrador de análisis económico con secciones diferenciadas, tablas comparativas, limitaciones y una propuesta de decisiones sobre el backlog.

**Verificación:**

Comprueba que la respuesta contiene:

- Tres escenarios claramente identificados.
- Las tres variables: tipos de interés, divisas e índice bursátil.
- Una distinción visible entre hechos, supuestos y proyecciones.
- Una tabla de escenarios y una tabla de decisiones de backlog.
- Indicadores de seguimiento y acciones asociadas.
- Advertencias o limitaciones cuando falten datos verificables.

> **Punto de control:** si Copilot presenta una cifra, una fecha o una fuente sin URL verificable, no la trates como un hecho. Márcala para validación o elimínala del entregable.

---

### Paso 3. Revisar, validar y refinar la respuesta de Copilot

**Objetivo:** comprobar la calidad del borrador, validar afirmaciones relevantes y pedir una mejora concreta a Copilot.

**Instrucciones:**

1. Lee la sección de hechos públicos verificados generada por Copilot.
2. Para cada hecho que pueda afectar una decisión, revisa:
   - Si existe una URL.
   - Si la URL corresponde a una fuente pública reconocida.
   - Si la fecha de consulta está indicada.
   - Si el contenido de la fuente respalda realmente la afirmación.
   - Si la fuente está actualizada para el horizonte de trabajo.

3. Prioriza fuentes públicas primarias o institucionales, por ejemplo:
   - Bancos centrales para tipos de interés.
   - Organismos estadísticos oficiales para indicadores económicos.
   - Bolsas o proveedores oficiales del índice para información del mercado.
   - Organismos internacionales para contexto económico general.

4. Clasifica cada afirmación revisada con una de estas etiquetas:
   - **Verificada:** fuente accesible y afirmación respaldada.
   - **Pendiente de verificar:** fuente incompleta, ambigua o no accesible.
   - **Supuesto:** valor usado solo para construir el ejercicio.
   - **Proyección:** posible consecuencia planteada para un escenario.

5. Comprueba que la lógica de cada escenario sea coherente:
   - El escenario base representa condiciones relativamente estables.
   - El escenario moderado aumenta la presión económica, pero no representa necesariamente una crisis.
   - El escenario adverso refleja mayor presión y mayor incertidumbre.
   - Las consecuencias no se presentan como seguras.
   - Las decisiones de producto se justifican por impacto, riesgo, costo, dependencia o necesidad de resiliencia.

6. Si detectas que la tabla es demasiado genérica, ambigua o no vincula claramente los escenarios al backlog, solicita un refinamiento. Usa esta indicación:

```text
Refina tu análisis sin introducir hechos nuevos no verificados. Conserva claramente la separación entre hechos, supuestos y proyecciones.

Mejora la tabla de decisiones del backlog con estos criterios:
- Prioriza iniciativas que reduzcan fricción, aumenten transparencia, mejoren rendimiento o permitan comunicaciones claras durante incertidumbre.
- Explica por qué una iniciativa se acelera, se mantiene, se aplaza o se revisa en cada escenario.
- Añade una condición de activación medible o verificable para cada decisión.
- Evita afirmar relaciones causales como certezas.
- Si falta evidencia para una recomendación, indícalo como incertidumbre y propone una pregunta de validación humana.

Devuelve únicamente:
1. La tabla de decisiones de backlog revisada.
2. La tabla de indicadores de seguimiento revisada.
3. Una lista de limitaciones y validaciones pendientes.
```

7. Revisa la respuesta refinada y conserva solo las recomendaciones que sean comprensibles, justificadas y adecuadas para el caso.

**Resultado esperado:**

Obtienes una versión refinada en la que cada decisión de backlog está asociada a un escenario, una justificación y una condición de activación o revisión.

**Verificación:**

La tabla refinada debe cumplir todos estos criterios:

- Cada iniciativa tiene una decisión visible: acelerar, mantener, aplazar o revisar.
- Cada decisión incluye una justificación de negocio o experiencia.
- Cada decisión incluye una dependencia o condición.
- Los indicadores contienen una señal de alerta y una acción.
- Las incertidumbres permanecen visibles.
- No se presentan recomendaciones como consejos de inversión ni como predicciones garantizadas.

---

### Paso 4. Convertir el análisis en decisiones y señales de alerta

**Objetivo:** seleccionar decisiones accionables y convertir el análisis en un artefacto útil para la continuidad de las prácticas.

**Instrucciones:**

1. A partir de la respuesta revisada, identifica:
   - Una iniciativa que debería **acelerarse** en escenario moderado o adverso.
   - Una iniciativa que debería **mantenerse** porque sigue siendo necesaria en los tres escenarios.
   - Una iniciativa que podría **aplazarse** si aumenta la presión sobre costos, capacidad o prioridades operativas.
   - Una iniciativa que requiera **revisión** si faltan datos o dependencias.

2. Comprueba que la decisión no se base únicamente en el texto generado por IA. Valida que sea coherente con:
   - La prioridad original del backlog.
   - El problema de experiencia que resuelve.
   - La capacidad operativa disponible en el caso.
   - Los riesgos de confianza y reputación.
   - Las dependencias técnicas o de contenido.

3. Selecciona entre tres y cinco indicadores de seguimiento. Como referencia, puedes considerar:
   - Variación de tipos de interés de referencia.
   - Movimiento porcentual de una divisa relevante.
   - Variación de un índice bursátil seleccionado.
   - Tiempo de carga o disponibilidad del portal.
   - Volumen de contactos de soporte.
   - Tasa de abandono de tareas clave.
   - Consultas relacionadas con información para inversionistas.
   - Sentimiento o temas recurrentes en comentarios públicos, si la organización dispone de un método autorizado para medirlo.

4. Para cada indicador, especifica:
   - Señal de alerta.
   - Frecuencia de revisión.
   - Responsable sugerido.
   - Acción que se debe activar.
   - Limitación o dependencia, si existe.

5. Redacta una conclusión ejecutiva de entre 80 y 120 palabras que responda:
   - Qué escenario merece mayor preparación.
   - Qué decisiones de experiencia digital no deberían retrasarse.
   - Qué señales deben activar una revisión.
   - Qué validaciones humanas siguen pendientes.

**Resultado esperado:**

Dispones de un conjunto de decisiones y señales de alerta que traduce el análisis económico en acciones de producto, experiencia y operación.

**Verificación:**

Comprueba que:

- Hay al menos una decisión de acelerar, mantener y aplazar o revisar.
- Cada decisión está vinculada a una iniciativa del backlog.
- Existen al menos tres indicadores de seguimiento.
- Cada indicador incluye una acción concreta al activarse.
- La conclusión ejecutiva distingue entre recomendaciones y hechos verificados.

---

### Paso 5. Documentar el resultado en Páginas de Microsoft 365 Copilot

**Objetivo:** guardar el análisis en la página de continuidad obligatoria con una estructura reutilizable para el laboratorio 03-00-03.

**Instrucciones:**

1. Vuelve a la página:

   ```text
   Northstar Digital - Cuaderno de análisis
   ```

2. Desplázate al final de la página existente. No crees una nueva página de continuidad.
3. Agrega un nuevo encabezado con el título exacto:

   ```text
   L03.2 - Escenarios económicos
   ```

4. Debajo del encabezado, incorpora las siguientes subsecciones:

   ```text
   Alcance, supuestos y limitaciones
   ```

   ```text
   Tabla comparativa de escenarios
   ```

   ```text
   Decisiones sobre el backlog de experiencia
   ```

   ```text
   Indicadores y señales de alerta
   ```

   ```text
   Validaciones humanas pendientes
   ```

5. Copia o adapta la tabla comparativa de escenarios. Debe incluir como mínimo estas columnas:

| Escenario | Tipos de interés | Divisas | Índice bursátil | Efecto en usuarios/inversionistas | Efecto operativo | Riesgo para confianza | Incertidumbre |
|---|---|---|---|---|---|---|---|

6. Copia o adapta la tabla de decisiones de backlog. Debe incluir como mínimo:

| Iniciativa | Escenario base | Escenario moderado | Escenario adverso | Decisión recomendada | Justificación | Condición o dependencia |
|---|---|---|---|---|---|---|

7. Añade una tabla de indicadores similar a esta:

| Indicador | Señal de alerta | Frecuencia | Responsable sugerido | Acción al activarse |
|---|---|---|---|---|
| Tipos de interés de referencia | Cambio superior al umbral definido para el escenario | Semanal o tras anuncio relevante | Responsable de estrategia o finanzas | Revisar escenario y prioridades |
| Movimiento de divisa relevante | Variación acumulada que alcance el umbral definido | Diario o semanal | Responsable internacional o financiero | Revisar contenidos, soporte y comunicaciones |
| Índice bursátil seleccionado | Descenso que alcance el umbral moderado o adverso | Diario o semanal | Responsable de relación con inversionistas | Activar revisión de mensajes y experiencia informativa |
| Disponibilidad o rendimiento del portal | Degradación respecto al objetivo acordado | Diario | Responsable de operaciones digitales | Priorizar estabilización técnica y comunicación |

8. Añade la conclusión ejecutiva elaborada en el paso anterior.
9. Incluye una lista de validaciones humanas pendientes. Como mínimo, incorpora:
   - Confirmar actualidad y relevancia de las fuentes públicas.
   - Confirmar los umbrales económicos con las personas responsables autorizadas.
   - Confirmar la capacidad técnica y presupuestaria para acelerar iniciativas.
   - Confirmar que las comunicaciones para inversionistas cumplen políticas internas y requisitos aplicables.
   - Confirmar que no se han incluido datos confidenciales.

10. Revisa que el contenido añadido no sobrescriba las secciones `L02 - Prompt refinado` ni `L03.1 - Experiencia de inversionistas`.

**Resultado esperado:**

La página **Northstar Digital - Cuaderno de análisis** contiene una sección titulada `L03.2 - Escenarios económicos` con tablas de escenarios, decisiones de backlog, indicadores, limitaciones y validaciones pendientes.

**Verificación:**

Comprueba visualmente que:

- La página conserva los resultados previos de las prácticas anteriores.
- Existe un único encabezado exacto: `L03.2 - Escenarios económicos`.
- La tabla de escenarios contiene base, moderado y adverso.
- La tabla de decisiones incluye iniciativas procedentes del backlog de 03-00-01.
- Los indicadores contienen señales y acciones.
- Las afirmaciones no verificadas están claramente etiquetadas como supuestos, proyecciones o pendientes de validación.

## Validación y pruebas

Realiza las siguientes pruebas antes de dar por finalizado el laboratorio.

### Prueba 1. Completitud de la indicación

Revisa la indicación utilizada en Copilot Chat y confirma que incluye:

- Objetivo de análisis.
- Contexto de Northstar Digital y de sus inversionistas internacionales.
- Horizonte temporal de 6 meses.
- Restricción de no proporcionar asesoramiento financiero.
- Variables de tipos de interés, divisas e índice bursátil.
- Escenarios base, moderado y adverso.
- Requisito de separar hechos, supuestos, proyecciones e incertidumbres.
- Formato de salida mediante tablas.
- Criterios de calidad y de validación.

**Resultado correcto:** la indicación permite a otra persona comprender qué se solicita, por qué se solicita y cómo debe presentarse el resultado.

### Prueba 2. Trazabilidad de información

Selecciona dos afirmaciones presentadas como hechos actuales por Copilot y verifica manualmente sus fuentes públicas.

**Resultado correcto:** cada afirmación queda clasificada como verificada, pendiente de verificar, supuesto o proyección. No se conserva ninguna afirmación no comprobada como hecho.

### Prueba 3. Coherencia de escenarios

Comprueba que el escenario moderado y el adverso no sean simplemente versiones con números mayores, sino que reflejen efectos razonables sobre:

- Comportamiento y expectativas de usuarios e inversionistas.
- Carga operativa y necesidad de soporte.
- Riesgo de confianza, transparencia y reputación.
- Prioridades de producto y experiencia digital.

**Resultado correcto:** las consecuencias están formuladas como posibilidades condicionadas, no como resultados garantizados.

### Prueba 4. Decisiones de backlog

Verifica que todas las iniciativas seleccionadas tengan una decisión y una justificación.

**Resultado correcto:** cada iniciativa se clasifica como acelerar, mantener, aplazar o revisar, y la decisión incluye una condición o dependencia.

### Prueba 5. Preparación para el siguiente laboratorio

Comprueba que la sección `L03.2 - Escenarios económicos` permite responder rápidamente a estas preguntas:

1. ¿Qué señales económicas requieren vigilancia?
2. ¿Qué iniciativas deben protegerse o acelerarse?
3. ¿Qué mensajes o riesgos de confianza podrían requerir atención durante una interrupción?
4. ¿Qué información sigue pendiente de validación humana?

**Resultado correcto:** la información está estructurada y será reutilizable para preparar comunicaciones coherentes en el laboratorio 03-00-03.

## Resolución de problemas

### Problema 1. Copilot genera cifras, fechas o fuentes sin enlaces verificables

**Síntomas:** la respuesta incluye datos económicos aparentemente precisos, pero no muestra URL, fecha de consulta o una fuente que respalde la afirmación.

**Causa probable:** la indicación no impuso suficientemente la trazabilidad de fuentes, la función de búsqueda web no está disponible en la sesión o Copilot generó una respuesta basada en patrones generales sin evidencia recuperable.

**Solución:**

1. No uses el dato como hecho en la página de continuidad.
2. Etiquétalo como **pendiente de verificar** o elimínalo.
3. Consulta una fuente pública primaria desde Edge.
4. Pide a Copilot que reformule sin hechos no verificados:

   ```text
   Reescribe el análisis usando solo hechos que tengan URL pública y fecha de consulta. Todo lo demás debe clasificarse como supuesto, proyección o incertidumbre. No inventes fuentes ni cifras.
   ```

5. Actualiza la tabla de escenarios con la clasificación correcta.

### Problema 2. La tabla no relaciona los escenarios con las iniciativas de 03-00-01

**Síntomas:** Copilot produce una explicación económica genérica, pero no indica qué iniciativas deben acelerarse, mantenerse, aplazarse o revisarse.

**Causa probable:** el backlog no se proporcionó con suficiente detalle o la indicación no exigió decisiones concretas y condiciones de activación.

**Solución:**

1. Vuelve a la sección `L03.1 - Experiencia de inversionistas`.
2. Copia únicamente los nombres autorizados, prioridades y resultados esperados de tres a cinco iniciativas.
3. Envía una solicitud de refinamiento:

   ```text
   Usa exclusivamente estas iniciativas del backlog: [pegar lista autorizada].
   Para cada una, indica una decisión para los escenarios base, moderado y adverso: acelerar, mantener, aplazar o revisar.
   Incluye una justificación, una condición de activación y una incertidumbre si corresponde. No agregues iniciativas nuevas.
   ```

4. Sustituye la tabla genérica por la tabla revisada en `L03.2 - Escenarios económicos`.

## Limpieza

1. Confirma que todo el trabajo reutilizable se encuentra en:

   ```text
   Northstar Digital - Cuaderno de análisis
   ```

2. Comprueba que la sección tiene el título exacto:

   ```text
   L03.2 - Escenarios económicos
   ```

3. Si guardaste archivos temporales en el equipo, conserva únicamente los que estén autorizados para evidencias de formación en:

   ```text
   C:\CopilotLabs\TransformarIdeasEnAccion\03-00-02\
   ```

4. Elimina borradores locales que contengan contenido duplicado, no validado o no necesario, según las políticas de tu organización.
5. Cierra las pestañas de fuentes públicas que ya no necesites y cierra sesión si trabajas en un equipo compartido.
6. No elimines ni modifiques las secciones anteriores de la página de continuidad.

## Resumen

En esta práctica diseñaste y refinaste una indicación para analizar acontecimientos económicos mediante escenarios *what-if*. Aplicaste los principios de objetivo, contexto y resultado esperado para solicitar una comparación estructurada entre los escenarios base, moderado y adverso.

También separaste hechos verificables de supuestos y proyecciones, validaste la calidad de las respuestas de Copilot y tradujiste el análisis en decisiones sobre el backlog de experiencia digital. El resultado documentado en `L03.2 - Escenarios económicos` servirá como base para preparar comunicaciones consistentes durante una interrupción de servicio bajo presión reputacional en el laboratorio 03-00-03.

### Recursos opcionales

- [Microsoft Support: Bienvenido a Copilot Chat](https://support.microsoft.com/es-es/topic/bienvenido-a-copilot-chat-34c93d56-86e6-4b5b-8cc8-59cbe8e53bc3)
- [Microsoft Learn: Introducción a Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/)
- [Banco Central Europeo](https://www.ecb.europa.eu/)
- [Banco de España](https://www.bde.es/)
- [Fondo Monetario Internacional](https://www.imf.org/)

---

# Gestión de comunicaciones ante una interrupción temporal de un servicio digital

## Metadatos

| Elemento | Valor |
|---|---|
| Duración | 23 minutos |
| Complejidad | Media |
| Nivel de Bloom | Crear |

## Descripción general

En esta práctica continuarás el caso de Northstar Digital durante una interrupción temporal de su portal de inversionistas, ocurrida en una jornada de volatilidad de divisas. Utilizarás Copilot Chat para convertir información confirmada y contexto de negocio en un paquete de comunicaciones coherente para públicos externos e internos.

El resultado no será una comunicación lista para publicar sin revisión: será un conjunto de borradores aprobables, claramente etiquetados, que separen hechos confirmados, elementos pendientes de investigación y compromisos de actualización. Conservarás los materiales en la misma Página de Microsoft 365 Copilot utilizada en prácticas anteriores para que puedan emplearse como evidencia en el reporte ejecutivo de la práctica 03-00-04.

> **Principio de uso responsable de IA:** Copilot puede ayudar a redactar y estructurar mensajes, pero no confirma causas técnicas, horas de recuperación, requisitos regulatorios ni hechos operativos. La validación humana y la aprobación por las áreas responsables son obligatorias antes de cualquier publicación.

## Objetivos de aprendizaje

Al finalizar esta práctica, podrás:

- [ ] Diseñar comunicaciones de incidente diferenciadas para audiencias internas y externas.
- [ ] Formular una indicación para Copilot Chat que incluya objetivo, contexto, restricciones, formato y criterios de calidad.
- [ ] Separar de forma explícita la información confirmada, la información pendiente de investigación y los compromisos de próxima actualización.
- [ ] Crear un calendario de actualizaciones y una matriz audiencia-canal-mensaje basados en el riesgo reputacional.
- [ ] Revisar borradores generados por IA para eliminar supuestos, promesas no autorizadas y afirmaciones no verificadas.

## Requisitos previos

### Conocimientos necesarios

Antes de comenzar, debes poder:

- Identificar los principios de precisión, oportunidad, empatía y consistencia en una comunicación de incidentes.
- Distinguir entre un hecho confirmado, una hipótesis, una información pendiente y un compromiso operativo.
- Formular solicitudes para Copilot Chat con objetivo, contexto y resultado esperado.
- Reconocer que cifras, fechas, causas, requisitos regulatorios y tiempos de recuperación requieren validación humana antes de comunicarse.

### Acceso y materiales necesarios

Debes disponer de:

- Una cuenta profesional o educativa de Microsoft Entra ID.
- Acceso habilitado a Microsoft 365 Copilot Chat y Páginas de Microsoft 365 Copilot.
- La Página de Copilot llamada exactamente **Northstar Digital - Cuaderno de análisis**.
- Los resultados de:
  - La práctica 03-00-01, incluidos el backlog de experiencia digital y las audiencias sensibles.
  - La práctica 03-00-02, incluidos los escenarios económicos, indicadores de alerta y acciones recomendadas.
- Acceso a Microsoft Edge y a Internet.
- Permiso para crear archivos de trabajo en `C:\CopilotLabs\TransformarIdeasEnAccion\03-00-03\`.

> **Importante:** No utilices datos reales de clientes, inversionistas, empleados, incidencias internas, contratos ni información no autorizada. El caso Northstar Digital es un escenario formativo ficticio.

## Entorno de laboratorio

### Hardware de referencia

| Componente | Requisito de referencia |
|---|---|
| Equipo | Windows 11 de 64 bits con Intel Core i5 de 10.ª generación o equivalente |
| Memoria | 8 GB de RAM como mínimo |
| Pantalla | Resolución mínima de 1920 x 1080 |
| Almacenamiento | 2 GB libres para caché del navegador y archivos de práctica |
| Red | Conexión estable de al menos 10 Mbps de descarga y 2 Mbps de carga |

### Software y servicios de referencia

| Componente | Versión o configuración |
|---|---|
| Sistema operativo | Windows 11 Enterprise 23H2, compilación 22631.4169 |
| Navegador | Microsoft Edge 128.0.2739.79 |
| Aplicaciones Microsoft 365 | Microsoft 365 Apps for enterprise 2408, compilación 17928.20156 |
| Servicio de IA | Microsoft 365 Copilot Chat, experiencia web disponible el 2026-09-16 |
| Espacio de trabajo | Páginas de Microsoft 365 Copilot, experiencia web disponible el 2026-09-16 |

> Las capacidades visibles pueden variar según licencia, región, tenant y configuración administrativa. El instructor debe comprobar el acceso al tenant antes de la sesión.

### Preparación del directorio de trabajo

1. Abre **Windows PowerShell**.
2. Ejecuta el siguiente comando para crear el directorio de evidencias de esta práctica:

```powershell
New-Item -ItemType Directory -Force -Path "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-03"
```

3. Si deseas conservar una copia local del paquete final, utiliza el nombre:

```text
C:\CopilotLabs\TransformarIdeasEnAccion\03-00-03\NorthstarDigital_PaqueteComunicaciones_Incidente.md
```

## Procedimiento paso a paso

### Paso 1. Revisar el contexto y establecer los límites de información

**Objetivo:** Preparar una base de trabajo que diferencie los hechos utilizables de las afirmaciones que todavía no pueden comunicarse.

#### Instrucciones

1. Abre Microsoft 365 Copilot en Microsoft Edge e inicia sesión con tu cuenta profesional o educativa.

2. Abre la Página de Copilot existente denominada:

```text
Northstar Digital - Cuaderno de análisis
```

3. Revisa las secciones creadas en las prácticas anteriores:
   - `L03.1 - Experiencia de inversionistas`
   - `L03.2 - Escenarios económicos`

4. Identifica, sin copiar datos confidenciales, los siguientes elementos de las secciones anteriores:
   - Perfiles de usuarios sensibles o prioritarios.
   - Riesgos de experiencia digital que podrían intensificarse durante una interrupción.
   - Indicadores de alerta asociados a volatilidad de divisas.
   - Riesgos reputacionales o de confianza que requieran atención en la comunicación.
   - Canales disponibles o recomendados para usuarios e interlocutores internos.

5. Crea una nueva sección en la misma Página de Copilot con el título obligatorio:

```text
L03.3 - Comunicaciones de interrupción
```

6. Dentro de esta sección, agrega el siguiente bloque de contexto formativo. No cambies las etiquetas de estado de la información.

```markdown
### Contexto operativo del ejercicio

Northstar Digital detectó una interrupción temporal del portal de inversionistas durante una jornada de volatilidad de divisas. La situación puede afectar la capacidad de usuarios autorizados para acceder a información del portal.

### Información confirmada para este ejercicio

- Se ha detectado una interrupción temporal del portal de inversionistas.
- Algunos usuarios pueden no poder acceder al portal o completar consultas habituales.
- El equipo técnico está investigando la situación.
- La jornada presenta volatilidad de divisas, por lo que la disponibilidad del portal tiene mayor sensibilidad reputacional.
- Northstar Digital debe mantener una comunicación clara, empática y coherente con la información validada.

### Información pendiente de investigación

- La causa técnica de la interrupción.
- El alcance exacto de usuarios, regiones, funciones y transacciones afectadas.
- La hora estimada de restauración.
- La necesidad de comunicaciones o notificaciones regulatorias.
- La existencia de impactos secundarios en sistemas relacionados.

### Restricciones obligatorias

- No afirmar una causa técnica no confirmada.
- No indicar una hora de recuperación ni una duración estimada no autorizada.
- No garantizar que no existe impacto financiero, regulatorio, contractual o de seguridad.
- No prometer compensaciones, exenciones, reembolsos ni acciones regulatorias.
- No atribuir responsabilidades a personas, proveedores o equipos.
- No incluir datos personales, datos de clientes, datos de cuentas ni información interna no autorizada.
```

7. Añade debajo una lista titulada `Audiencias sensibles identificadas` y registra los perfiles procedentes de tus resultados anteriores. Si no existe una clasificación previa utilizable, emplea únicamente estos perfiles ficticios de referencia:
   - Inversionistas que consultan información durante períodos de volatilidad.
   - Equipos de relación con inversionistas y atención al cliente.
   - Soporte técnico y operaciones.
   - Liderazgo ejecutivo y comunicaciones corporativas.
   - Público externo que pueda consultar canales oficiales.

8. Lee el bloque completo antes de continuar. Comprueba que ninguna frase convierte una situación pendiente en un hecho.

#### Resultado esperado

La Página de Copilot contiene una sección titulada `L03.3 - Comunicaciones de interrupción` con:

- El contexto de la interrupción.
- Una separación visible entre información confirmada y pendiente.
- Restricciones explícitas para evitar afirmaciones inventadas.
- Una lista de audiencias sensibles basada en prácticas anteriores.

#### Verificación

Confirma lo siguiente:

- [ ] El nombre de la página sigue siendo **Northstar Digital - Cuaderno de análisis**.
- [ ] El encabezado de la nueva sección es exactamente `L03.3 - Comunicaciones de interrupción`.
- [ ] La causa, el alcance completo, la duración y las obligaciones regulatorias aparecen como pendientes.
- [ ] No se han introducido nombres reales, números de cuenta, datos personales ni información confidencial.

---

### Paso 2. Diseñar una indicación controlada para el paquete de comunicaciones

**Objetivo:** Solicitar a Copilot Chat un primer borrador estructurado sin permitir que invente hechos operativos o compromisos.

#### Instrucciones

1. Abre Copilot Chat en una nueva conversación.

2. Antes de pegar la indicación, recuerda que Copilot Chat puede no acceder automáticamente al contenido de tu Página de Copilot o a todos los archivos de Microsoft 365. Proporciona solo el contexto ficticio y aprobado que sea necesario para esta práctica.

3. Copia y pega la siguiente indicación. Sustituye los elementos entre corchetes únicamente por información ficticia o por conclusiones aprobadas de las prácticas anteriores.

```text
Actúa como asistente de redacción para comunicaciones de incidente de Northstar Digital. Necesito un paquete de borradores para una interrupción temporal de un portal de inversionistas durante una jornada de volatilidad de divisas.

Objetivo:
Crear comunicaciones claras, empáticas, transparentes y coherentes para varias audiencias, listas para revisión humana y aprobación antes de su uso.

Contexto confirmado:
- Se ha detectado una interrupción temporal del portal de inversionistas.
- Algunos usuarios pueden no poder acceder al portal o completar consultas habituales.
- El equipo técnico está investigando.
- La volatilidad de divisas incrementa la sensibilidad reputacional de la situación.
- Audiencias sensibles identificadas: [pegar perfiles ficticios o aprobados].

Información pendiente:
- Causa técnica.
- Alcance exacto de usuarios, regiones y funcionalidades.
- Hora estimada de restauración.
- Impacto financiero, contractual, de seguridad o regulatorio.
- Necesidad de comunicaciones regulatorias.

Restricciones obligatorias:
- No inventes causas, plazos de recuperación, cifras, impactos, compromisos regulatorios, compensaciones ni responsabilidades.
- No afirmes que los datos están seguros ni que no existe impacto financiero o regulatorio.
- No uses datos personales, nombres de clientes ni información confidencial.
- Si falta información, usa expresiones como “estamos investigando”, “la información se confirmará tras la validación correspondiente” o marcadores [POR CONFIRMAR].
- Trata todos los textos como borradores sujetos a aprobación humana.
- Distingue visualmente entre hechos confirmados, información pendiente y próximo compromiso de actualización.

Genera el resultado en español y con las siguientes secciones:
1. Matriz audiencia-canal-mensaje-riesgo.
2. Aviso inicial de estado del servicio para usuarios externos, máximo 120 palabras.
3. Actualización de progreso para usuarios externos, máximo 140 palabras.
4. Preguntas frecuentes para soporte, con respuestas que no especulen.
5. Mensaje para equipo interno, máximo 180 palabras.
6. Comunicado de resolución con marcadores [POR CONFIRMAR] donde sea necesaria validación.
7. Calendario escalonado de actualizaciones.
8. Lista final de validaciones humanas requeridas antes de publicar.

Criterios de calidad:
- Tono profesional, directo y empático.
- Lenguaje comprensible para público no técnico.
- Coherencia entre todos los mensajes.
- Cada mensaje debe indicar qué se sabe, qué sigue pendiente y cuándo o bajo qué condición se comunicará una nueva actualización.
```

4. Envía la indicación.

5. Lee la respuesta sin asumir que es correcta. Busca especialmente:
   - Causas técnicas no proporcionadas.
   - Horas o fechas concretas no autorizadas.
   - Expresiones absolutas, por ejemplo: “no hay impacto”, “los datos están seguros” o “el servicio se restaurará a las 14:00”.
   - Promesas de compensación o avisos regulatorios.
   - Incoherencias entre el aviso inicial, la actualización y el comunicado de resolución.
   - Mensajes que no indiquen el siguiente punto de actualización.

6. Si Copilot inventa información, utiliza una solicitud de refinamiento como la siguiente:

```text
Revisa el paquete anterior aplicando un control estricto de supuestos. Elimina o reemplaza cualquier causa, plazo, garantía, cifra, compromiso regulatorio o conclusión sobre impacto que no esté explícitamente en el contexto confirmado. Usa [POR CONFIRMAR] cuando sea necesario. Mantén el formato solicitado y añade una columna “Validación necesaria” a la matriz.
```

7. Conserva la versión más segura y coherente para el siguiente paso.

#### Resultado esperado

Copilot Chat genera un paquete inicial que contiene los cinco tipos de comunicación requeridos, una matriz de audiencias y un calendario de actualizaciones. Los contenidos no afirman causas ni plazos no confirmados.

#### Verificación

Revisa la respuesta y confirma:

- [ ] El aviso inicial comunica la indisponibilidad sin especular sobre la causa.
- [ ] La actualización de progreso informa que la investigación continúa, sin prometer una hora de recuperación.
- [ ] Las preguntas frecuentes orientan a soporte sin proporcionar respuestas técnicas inventadas.
- [ ] El mensaje interno incluye una instrucción de coordinación y evita divulgar información no aprobada.
- [ ] El comunicado de resolución contiene marcadores `[POR CONFIRMAR]` para elementos que solo pueden completarse tras validación.
- [ ] Todos los mensajes incluyen o remiten a un compromiso de próxima actualización.

---

### Paso 3. Refinar los mensajes para cada audiencia y construir la matriz de comunicaciones

**Objetivo:** Transformar el borrador inicial en una matriz que conecte audiencia, canal, propósito, mensaje y control de aprobación.

#### Instrucciones

1. En Copilot Chat, solicita una revisión específica de la matriz. Copia esta indicación:

```text
A partir del paquete anterior, crea una matriz de comunicaciones de incidente para Northstar Digital.

Incluye estas columnas:
- Audiencia
- Necesidad o riesgo principal
- Canal recomendado
- Propósito del mensaje
- Mensaje clave permitido
- Información que no se debe afirmar
- Responsable de validación
- Momento o condición de envío
- Validación necesaria antes de publicar

Incluye al menos estas audiencias:
- Usuarios del portal de inversionistas.
- Equipo de relación con inversionistas y atención al cliente.
- Soporte técnico y operaciones.
- Liderazgo ejecutivo.
- Comunicaciones corporativas o canal público oficial.

No inventes nombres de herramientas, cargos concretos, obligaciones regulatorias, horarios ni responsables individuales. Si un responsable no se conoce, usa un rol genérico como “responsable de comunicaciones”, “equipo técnico” o “[POR ASIGNAR]”.
```

2. Revisa la tabla generada. Ajusta los canales a los que estén disponibles o aprobados en el caso formativo. Puedes emplear categorías generales como:
   - Página o banner de estado del servicio.
   - Centro de ayuda o mensaje de soporte.
   - Correo interno.
   - Canal interno de colaboración.
   - Reunión de coordinación.
   - Canal corporativo externo aprobado.

3. Evita asumir que todos los canales son apropiados para todas las audiencias. Por ejemplo:
   - Un aviso público puede informar de indisponibilidad, pero no debe incluir detalles técnicos no confirmados.
   - El equipo técnico puede requerir más contexto operativo, pero sigue necesitando respetar el principio de necesidad de conocer.
   - El liderazgo ejecutivo necesita una síntesis de riesgo, decisiones pendientes y próxima actualización, no una narración técnica extensa.

4. En la Página de Copilot, dentro de `L03.3 - Comunicaciones de interrupción`, agrega el subtítulo:

```text
### Matriz audiencia-canal-mensaje
```

5. Copia la matriz revisada desde Copilot Chat y pégala debajo del subtítulo.

6. Revisa manualmente cada fila y añade, si no existe, una columna o nota con la marca:

```text
Estado: Borrador para validación humana
```

7. Comprueba que la matriz incluye una audiencia externa, una audiencia de soporte, una audiencia técnica y una audiencia ejecutiva.

#### Resultado esperado

La Página de Copilot contiene una matriz que muestra cómo varían el canal, el mensaje, el riesgo y la validación necesaria según la audiencia.

#### Verificación

Valida que:

- [ ] Cada audiencia tiene un canal razonable y un propósito específico.
- [ ] La matriz diferencia entre mensaje permitido e información que no debe afirmarse.
- [ ] El responsable se expresa como función o rol, no como nombre real de una persona.
- [ ] Ningún canal externo incluye detalles técnicos, causas o compromisos no autorizados.
- [ ] Todas las filas están marcadas como borradores sujetos a validación humana.

---

### Paso 4. Crear y revisar los cinco borradores de comunicación

**Objetivo:** Producir textos consistentes que puedan entregarse al proceso de aprobación sin presentar hipótesis como hechos.

#### Instrucciones

1. En Copilot Chat, utiliza esta indicación para obtener una versión final de trabajo de los cinco mensajes:

```text
Genera una versión revisada y consistente de los siguientes cinco borradores para Northstar Digital. Usa solo la información confirmada indicada anteriormente.

Requisitos comunes:
- Idioma: español.
- Tono: profesional, empático, transparente y no especulativo.
- Estado: borrador para revisión humana.
- Incluir claramente: lo confirmado, lo pendiente y el compromiso de próxima actualización.
- No inventar causas, tiempos de resolución, alcance total, impactos, obligaciones regulatorias ni compensaciones.
- Usar [POR CONFIRMAR] cuando una frase necesite aprobación o evidencia adicional.

Borradores requeridos:
A. Aviso inicial de estado del servicio para usuarios externos, máximo 120 palabras.
B. Actualización de progreso para usuarios externos, máximo 140 palabras.
C. Preguntas frecuentes para soporte: al menos 5 preguntas y respuestas.
D. Mensaje interno para equipos de soporte, operaciones, relación con inversionistas y comunicaciones, máximo 180 palabras.
E. Comunicado de resolución, máximo 160 palabras, con una lista separada de datos que deben validarse antes de enviarlo.

Después de los cinco borradores, incluye una tabla de consistencia que compare:
- Hecho confirmado comunicado.
- Información pendiente.
- Próxima actualización.
- Riesgo si se publica sin validación.
```

2. Revisa cada borrador con los siguientes criterios:

| Borrador | Aspectos que debes revisar |
|---|---|
| Aviso inicial | Indica que existe una interrupción, reconoce el inconveniente y no atribuye una causa. |
| Actualización de progreso | Explica que la investigación continúa, no ofrece una estimación inventada y remite al siguiente canal o actualización. |
| Preguntas frecuentes | Ofrece respuestas útiles para soporte sin afirmar seguridad, impacto o recuperación no validados. |
| Mensaje interno | Coordina a los equipos, define una fuente única de información y evita mensajes contradictorios. |
| Comunicado de resolución | No debe usarse hasta que se confirmen restauración, alcance, causa aprobada y próximos pasos autorizados. |

3. Si alguno de los borradores no cumple los límites o contiene afirmaciones no validadas, solicita una corrección puntual. Ejemplo:

```text
Reescribe únicamente el comunicado de resolución. No afirmes la causa, la duración, el alcance total ni que no hubo impacto. Mantén [POR CONFIRMAR] para esos elementos y añade una nota visible: “No publicar hasta completar validación técnica, jurídica y de comunicaciones”.
```

4. En la Página de Copilot, agrega el siguiente subtítulo:

```text
### Borradores de comunicación
```

5. Copia los cinco borradores revisados. Etiqueta cada uno con el formato siguiente:

```markdown
#### A. Aviso inicial de estado del servicio
Estado: Borrador para validación humana

#### B. Actualización de progreso
Estado: Borrador para validación humana

#### C. Preguntas frecuentes para soporte
Estado: Borrador para validación humana

#### D. Mensaje para equipo interno
Estado: Borrador para validación humana

#### E. Comunicado de resolución
Estado: No publicar hasta completar validación técnica, jurídica y de comunicaciones
```

6. Debajo del comunicado de resolución, incluye una lista titulada `Validaciones previas a la resolución` con, como mínimo:
   - Confirmación técnica de la restauración.
   - Confirmación del alcance afectado.
   - Aprobación de la descripción de causa, si se autoriza comunicarla.
   - Revisión jurídica, regulatoria y de comunicaciones según las políticas aplicables.
   - Aprobación del responsable designado.

#### Resultado esperado

La Página de Copilot conserva cinco borradores diferenciados, con restricciones visibles y una lista de validaciones antes del comunicado de resolución.

#### Verificación

Comprueba que:

- [ ] Existen exactamente los cinco tipos de borrador solicitados.
- [ ] El comunicado de resolución no se presenta como listo para publicar.
- [ ] Todos los textos emplean un tono empático sin exagerar ni minimizar el incidente.
- [ ] Los mensajes externos no contradicen el mensaje interno.
- [ ] Las preguntas frecuentes no responden con certezas sobre elementos que siguen en investigación.

---

### Paso 5. Elaborar un calendario escalonado de actualizaciones

**Objetivo:** Definir una secuencia de comunicación que mantenga la oportunidad sin prometer plazos técnicos no confirmados.

#### Instrucciones

1. En Copilot Chat, escribe la siguiente indicación:

```text
Crea un calendario escalonado de actualizaciones para una interrupción temporal del portal de inversionistas de Northstar Digital.

Usa condiciones y frecuencias relativas, no horas concretas ni tiempos de recuperación inventados.

Incluye estas fases:
1. Detección y confirmación inicial.
2. Investigación en curso.
3. Cambio material en el estado o alcance.
4. Restauración confirmada.
5. Cierre posterior y revisión.

Para cada fase, muestra:
- Activador o condición.
- Audiencias.
- Canal.
- Mensaje o propósito.
- Responsable por rol.
- Aprobaciones requeridas.
- Riesgo de no comunicar.
- Riesgo de comunicar información no validada.

Ten en cuenta que la volatilidad de divisas incrementa la necesidad de comunicaciones oportunas para usuarios sensibles, sin convertir la velocidad en una justificación para especular.
```

2. Revisa que el calendario use condiciones como:
   - “Tras la confirmación inicial de indisponibilidad”.
   - “Mientras la investigación continúe”.
   - “Ante un cambio material validado”.
   - “Después de confirmar la restauración”.
   - “Tras la revisión interna autorizada”.

3. Rechaza y corrige cualquier fila que incluya:
   - Una hora fija de recuperación.
   - Una obligación regulatoria no confirmada.
   - Una promesa de actualización en una frecuencia que no pueda cumplirse.
   - Un canal no autorizado.
   - Un responsable individual no proporcionado.

4. Agrega en la Página de Copilot el subtítulo:

```text
### Calendario escalonado de actualizaciones
```

5. Copia el calendario revisado debajo del subtítulo.

6. Añade al final del calendario esta nota de control:

```markdown
**Regla operativa:** una actualización debe publicarse cuando exista información validada que cambie materialmente el mensaje o cuando se alcance el punto de actualización comprometido. Si no hay cambios confirmados, la actualización debe indicar que la investigación continúa sin especular sobre causas ni plazos.
```

#### Resultado esperado

La Página de Copilot contiene un calendario que conecta cada fase del incidente con una audiencia, un canal, una condición de activación y una aprobación requerida.

#### Verificación

Confirma lo siguiente:

- [ ] El calendario contiene las cinco fases solicitadas.
- [ ] No usa tiempos de recuperación inventados.
- [ ] Distingue claramente entre actualización por cambio material y actualización de continuidad.
- [ ] Considera a las audiencias sensibles identificadas en prácticas anteriores.
- [ ] Incluye riesgos tanto de silencio prolongado como de comunicación no validada.

---

### Paso 6. Consolidar la evidencia y preparar la transición al reporte ejecutivo

**Objetivo:** Dejar una línea de tiempo reutilizable para la práctica 03-00-04 y verificar la calidad del paquete completo.

#### Instrucciones

1. En la Página de Copilot, agrega el último subtítulo de la sección:

```text
### Registro de decisiones y validaciones
```

2. Crea una tabla con el siguiente formato y complétala con decisiones del ejercicio:

| Elemento | Decisión de trabajo | Estado de validación | Riesgo controlado |
|---|---|---|---|
| Aviso inicial | Comunicar indisponibilidad confirmada sin causa | Pendiente de aprobación | Especulación técnica |
| Actualización de progreso | Informar investigación en curso y próximo punto de comunicación | Pendiente de aprobación | Promesa de recuperación no autorizada |
| Preguntas frecuentes | Guiar a soporte con respuestas no especulativas | Pendiente de aprobación | Respuestas inconsistentes |
| Mensaje interno | Establecer coordinación y fuente única de información | Pendiente de aprobación | Mensajes contradictorios |
| Comunicado de resolución | Usar solo tras validaciones formales | No publicar aún | Información incompleta o no aprobada |

3. Ajusta la tabla si tus decisiones reales de trabajo son distintas, pero no elimines la separación entre borrador, aprobación pendiente y publicación.

4. Revisa toda la sección `L03.3 - Comunicaciones de interrupción` y confirma que incluye:
   - Contexto y restricciones.
   - Matriz audiencia-canal-mensaje.
   - Cinco borradores.
   - Calendario escalonado.
   - Registro de decisiones y validaciones.

5. Si la experiencia de Páginas de Copilot permite exportar o copiar el contenido, guarda una copia local opcional en:

```text
C:\CopilotLabs\TransformarIdeasEnAccion\03-00-03\NorthstarDigital_PaqueteComunicaciones_Incidente.md
```

6. No elimines la sección de la Página de Copilot. Será una fuente de trabajo para el reporte ejecutivo de la práctica 03-00-04.

#### Resultado esperado

La Página de Copilot contiene una evidencia completa, organizada y reutilizable del proceso de diseño de comunicaciones de incidente.

#### Verificación

Confirma que:

- [ ] La sección se titula exactamente `L03.3 - Comunicaciones de interrupción`.
- [ ] La matriz, los borradores, el calendario y el registro de decisiones están presentes.
- [ ] Todos los artefactos muestran que son borradores sujetos a validación humana.
- [ ] No hay causas, plazos, impactos o compromisos presentados como confirmados sin evidencia.
- [ ] El contenido puede utilizarse como línea de tiempo y evidencia para `L03.4 - Reporte ejecutivo`.

## Validación y pruebas

Realiza las siguientes pruebas antes de dar por finalizada la práctica.

### Prueba 1. Control de hechos y supuestos

Lee cada borrador y clasifica las afirmaciones en tres grupos:

| Clasificación | Ejemplo aceptable |
|---|---|
| Confirmado | “Hemos detectado una interrupción temporal del portal de inversionistas.” |
| Pendiente | “El equipo técnico está investigando el alcance de la situación.” |
| Requiere validación | “[POR CONFIRMAR: hora de restauración y alcance final].” |

**Criterio de aprobación:** no debe existir ninguna afirmación sobre causa, duración, impacto financiero, seguridad de datos, alcance completo o requisitos regulatorios sin una fuente validada.

### Prueba 2. Consistencia entre mensajes

Compara el aviso inicial, la actualización de progreso, las preguntas frecuentes, el mensaje interno y el comunicado de resolución.

**Criterio de aprobación:**

- Todos describen la situación como una interrupción temporal.
- Ninguno contradice el estado de investigación.
- El mensaje interno no promete información que los mensajes externos no puedan sostener.
- El comunicado de resolución permanece bloqueado hasta completar sus validaciones.

### Prueba 3. Adecuación por audiencia

Selecciona una fila de la matriz para cada audiencia y responde:

1. ¿El canal permite llegar a esa audiencia de manera razonable?
2. ¿El tono responde a su necesidad principal?
3. ¿El mensaje evita detalles no necesarios?
4. ¿El responsable y la aprobación son suficientes para el riesgo?

**Criterio de aprobación:** cada audiencia debe tener un mensaje útil, proporcional al riesgo y sujeto a una validación definida.

### Prueba 4. Calidad de la indicación utilizada

Revisa la indicación principal enviada a Copilot Chat. Debe incluir:

- Objetivo.
- Contexto confirmado.
- Información pendiente.
- Restricciones.
- Formato de salida.
- Criterios de calidad.
- Instrucciones para no inventar información.

**Criterio de aprobación:** la indicación proporciona suficiente contexto para reducir supuestos y permite identificar claramente lo que Copilot no debe afirmar.

### Lista final de comprobación

- [ ] Se utilizó únicamente información ficticia o autorizada.
- [ ] Se mantuvo la misma Página de Copilot para preservar la trazabilidad.
- [ ] Los riesgos reputacionales de volatilidad y acceso al portal se reflejan en el calendario y la matriz.
- [ ] Se definieron comunicaciones iniciales, de progreso, de soporte, internas y de resolución.
- [ ] Se separaron hechos confirmados, asuntos pendientes y validaciones requeridas.
- [ ] Los borradores están preparados para revisión humana, no para publicación automática.
- [ ] La evidencia está disponible para el reporte ejecutivo de la práctica 03-00-04.

## Resolución de problemas

### Problema 1. Copilot Chat añade una causa técnica, una hora de recuperación o una garantía no proporcionada

**Síntomas:** La respuesta afirma que el problema fue causado por un proveedor, un fallo de infraestructura, un ciberataque o una actualización. También puede indicar una hora estimada de resolución, asegurar que los datos están protegidos o declarar que no existe impacto regulatorio.

**Causa:** La solicitud no estableció suficientes restricciones, o Copilot completó información ausente con una suposición plausible.

**Solución:**

1. No copies ni publiques la afirmación no validada.
2. Envía una solicitud de corrección como esta:

```text
Elimina todas las causas, estimaciones, garantías y conclusiones de impacto no incluidas explícitamente en la información confirmada. Sustitúyelas por “estamos investigando”, “[POR CONFIRMAR]” o una pregunta para el responsable de validación.
```

3. Revisa manualmente el resultado antes de incorporarlo a la Página de Copilot.
4. Registra la validación pendiente en la matriz o en el registro de decisiones.

### Problema 2. No puedes encontrar la Página de Copilot anterior o no aparece contenido de las prácticas 03-00-01 y 03-00-02

**Síntomas:** La página **Northstar Digital - Cuaderno de análisis** no aparece en la lista, se abre una página nueva vacía o no se visualizan las secciones `L03.1` y `L03.2`.

**Causa:** Puede haberse iniciado sesión con otra cuenta, la página no se guardó correctamente, el contenido está en otro espacio de trabajo o las capacidades de Páginas de Copilot varían en el tenant.

**Solución:**

1. Verifica que has iniciado sesión con la cuenta profesional o educativa asignada al curso.
2. Busca la página por el nombre exacto: `Northstar Digital - Cuaderno de análisis`.
3. Actualiza Microsoft Edge e intenta abrir de nuevo Microsoft 365 Copilot.
4. Si no puedes recuperar el contenido, informa al instructor antes de crear una página sustituta.
5. Como contingencia autorizada por el instructor, crea una nueva página con el mismo nombre y documenta que las audiencias y escenarios usados son los perfiles ficticios de referencia de esta guía.

## Limpieza

1. Conserva la Página de Copilot **Northstar Digital - Cuaderno de análisis** y la sección `L03.3 - Comunicaciones de interrupción`.
2. Conserva, si la creaste, la copia local en:

```text
C:\CopilotLabs\TransformarIdeasEnAccion\03-00-03\
```

3. Cierra las pestañas de Copilot Chat que contengan borradores duplicados o versiones descartadas, si no necesitas conservarlas como evidencia.
4. No elimines los resultados de las prácticas `L03.1`, `L03.2` o `L03.3`; se utilizarán en la práctica `L03.4 - Reporte ejecutivo`.
5. Cierra sesión solo si el procedimiento de tu organización o del aula lo requiere.

## Resumen

En esta práctica diseñaste un paquete de comunicaciones para una interrupción temporal del portal de inversionistas de Northstar Digital durante un período de volatilidad de divisas. Utilizaste Copilot Chat para acelerar la creación de borradores, pero aplicaste controles para que la IA no inventara causas, tiempos de recuperación, impactos ni compromisos regulatorios.

También organizaste el trabajo en una matriz audiencia-canal-mensaje, un calendario escalonado de actualizaciones, cinco borradores de comunicación y un registro de decisiones y validaciones. Estos materiales constituyen una línea de tiempo reutilizable para la siguiente práctica, donde transformarás el análisis acumulado en un reporte ejecutivo.

### Recursos opcionales

- [Microsoft Support: Bienvenido a Copilot Chat](https://support.microsoft.com/es-es/topic/bienvenido-a-copilot-chat-34c93d56-86e6-4b5b-8cc8-59cbe8e53bc3)
- [Microsoft Support: Introducción a Microsoft 365 Copilot](https://support.microsoft.com/es-es/copilot-microsoft-365)
- [Microsoft Learn: Introducción a Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/)

---

# Análisis de incidencias operativas y generación de un reporte ejecutivo

## Metadatos

| Campo | Valor |
|---|---|
| Duración | 22 minutos |
| Complejidad | Difícil |
| Nivel de Bloom | Crear |

## Descripción general

En esta práctica cerrarás el caso transversal de **Northstar Digital** mediante la consolidación de los análisis elaborados en laboratorios anteriores. Utilizarás Copilot Chat para analizar una incidencia operativa simulada que produjo una interrupción temporal del portal de inversionistas y distinguirás explícitamente entre hechos confirmados, hipótesis, impactos estimados y datos pendientes de validación.

A continuación, transformarás el análisis en un reporte ejecutivo conciso dirigido al comité directivo. El producto final incluirá un resumen ejecutivo, una línea de tiempo, el impacto para clientes y negocio, riesgos, decisiones requeridas, acciones correctivas, responsables y próximos pasos. Guardarás el reporte y la lista de validación final en la Página de Microsoft 365 Copilot compartida con las prácticas anteriores.

> **Principio de uso responsable de IA:** todos los datos de esta práctica son ficticios y están autorizados para formación. No introduzcas datos reales de clientes, empleados, contratos, incidentes, credenciales, direcciones IP internas, registros de producción ni información confidencial de tu organización.

## Objetivos de aprendizaje

Al finalizar esta práctica, podrás:

- [ ] Sintetizar información operativa, de experiencia de cliente, económica y de comunicaciones en un reporte ejecutivo para dirección.
- [ ] Solicitar a Copilot Chat un análisis que separe hechos conocidos, hipótesis, impacto estimado y datos pendientes.
- [ ] Identificar patrones, riesgos, posibles causas y acciones correctivas sin presentar hipótesis como hechos confirmados.
- [ ] Crear un reporte ejecutivo de una página o equivalente con estructura, trazabilidad y criterios de calidad explícitos.
- [ ] Aplicar una revisión humana final para validar exactitud, tono, consistencia, seguridad y adecuación para el comité directivo.

## Requisitos previos

### Conocimientos requeridos

Antes de comenzar, debes poder:

- Formular indicaciones con objetivo, contexto, restricciones, formato de salida y criterios de calidad.
- Distinguir hechos comprobados de suposiciones, interpretaciones, estimaciones e hipótesis.
- Revisar críticamente resultados generados por IA antes de utilizarlos como base para una comunicación o decisión.
- Reconocer que Copilot Chat genera borradores de trabajo y no sustituye la aprobación humana ni la investigación técnica.
- Aplicar buenas prácticas de protección de datos: usar solo contenido público, simulado o expresamente autorizado.

### Acceso y materiales requeridos

Debes contar con lo siguiente:

- Finalización de los laboratorios:
  - `02-00-01`
  - `03-00-01`
  - `03-00-02`
  - `03-00-03`
- Acceso con una cuenta profesional o educativa de Microsoft Entra ID.
- Microsoft 365 Copilot Chat habilitado en el tenant de formación.
- Acceso a Páginas de Microsoft 365 Copilot.
- La página existente con el nombre exacto:

  ```text
  Northstar Digital - Cuaderno de análisis
  ```

- Resultados anteriores disponibles en esa misma página, con los títulos:
  - `L02 - Prompt refinado`
  - `L03.1 - Experiencia de inversionistas`
  - `L03.2 - Escenarios económicos`
  - `L03.3 - Comunicaciones de interrupción`

> **Importante:** si no encuentras alguno de los resultados previos, no inventes su contenido. Continúa con los datos simulados incluidos en esta guía y señala en el reporte que el análisis previo correspondiente no estaba disponible para su verificación.

## Entorno de laboratorio

### Hardware de referencia

| Componente | Requisito de referencia |
|---|---|
| Equipo | Windows 11 de 64 bits |
| Procesador | Intel Core i5 de 10.ª generación o equivalente |
| Memoria | 8 GB de RAM como mínimo |
| Pantalla | Resolución mínima de 1920 x 1080 |
| Conectividad | 10 Mbps de descarga y 2 Mbps de carga como mínimo |
| Espacio local | 2 GB libres para caché del navegador y archivos de práctica |

### Software y servicios de referencia

| Componente | Versión o configuración |
|---|---|
| Sistema operativo | Windows 11 Enterprise 23H2, compilación 22631.4169 |
| Navegador | Microsoft Edge 128.0.2739.79 |
| Aplicaciones de Microsoft 365 | Microsoft 365 Apps for enterprise 2408, compilación 17928.20156 |
| Servicio de IA | Microsoft 365 Copilot Chat |
| Espacio de trabajo | Páginas de Microsoft 365 Copilot |
| Fecha de referencia del servicio | 2026-09-16 |

> Las opciones visibles de Copilot pueden variar según la licencia, región, idioma, directivas de la organización y configuración del tenant. El instructor debe comprobar el funcionamiento de Copilot Chat y Páginas de Copilot el día anterior a la sesión.

### Preparación del directorio local

Aunque el producto principal se guardará en Páginas de Copilot, crea las carpetas de trabajo estándar para conservar evidencias o borradores descargados si el instructor lo solicita.

1. Abre **Windows PowerShell**.
2. Ejecuta el siguiente comando:

```powershell
New-Item -ItemType Directory -Force -Path `
  "C:\CopilotLabs\TransformarIdeasEnAccion\02-00-01", `
  "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-01", `
  "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-02", `
  "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-03", `
  "C:\CopilotLabs\TransformarIdeasEnAccion\03-00-04"
```

3. Comprueba que las carpetas se crearon:

```powershell
Get-ChildItem "C:\CopilotLabs\TransformarIdeasEnAccion"
```

> No guardes capturas ni exportaciones que contengan información real, confidencial o personal. En este laboratorio solo se permite conservar contenido simulado.

## Procedimiento paso a paso

### Paso 1. Confirmar el contexto acumulado y preparar la página de continuidad

**Objetivo:** Verificar que la Página de Copilot contiene los resultados previos y preparar una sección para el reporte ejecutivo final.

**Instrucciones:**

1. Abre Microsoft Edge e inicia sesión con tu cuenta profesional o educativa autorizada.
2. Abre Microsoft 365 Copilot y accede a **Páginas de Copilot**.
3. Busca y abre la página cuyo nombre exacto es:

   ```text
   Northstar Digital - Cuaderno de análisis
   ```

4. Revisa que existan las secciones o encabezados de las prácticas anteriores:
   - `L02 - Prompt refinado`
   - `L03.1 - Experiencia de inversionistas`
   - `L03.2 - Escenarios económicos`
   - `L03.3 - Comunicaciones de interrupción`
5. Lee de forma selectiva los resultados previos y toma nota de elementos reutilizables, sin copiar información no autorizada. Busca especialmente:
   - Expectativas de los inversionistas o usuarios del portal.
   - Riesgos de experiencia digital identificados.
   - Escenarios económicos y supuestos usados.
   - Tono y mensajes utilizados para comunicar la interrupción.
   - Acciones pendientes, responsables o dependencias mencionadas.
6. Al final de la página, agrega un nuevo encabezado de nivel equivalente a las secciones anteriores:

   ```text
   L03.4 - Reporte ejecutivo
   ```

7. Debajo del encabezado, agrega una nota temporal:

   ```text
   Borrador generado a partir de datos simulados del laboratorio. Requiere validación humana antes de cualquier uso operativo o externo.
   ```

**Resultado esperado:**

La página `Northstar Digital - Cuaderno de análisis` contiene los resultados de las prácticas anteriores y una nueva sección titulada `L03.4 - Reporte ejecutivo`.

**Verificación:**

- Confirma que estás trabajando en la página correcta y no en una página nueva con un nombre similar.
- Confirma que el nuevo título utiliza exactamente la convención requerida: `L03.4 - Reporte ejecutivo`.
- Confirma que no has añadido datos reales de tu organización.
- Si falta una sección anterior, anota la ausencia para mencionarla después como una limitación de trazabilidad.

---

### Paso 2. Analizar los datos autorizados de la incidencia operativa simulada

**Objetivo:** Usar Copilot Chat para estructurar la información de la incidencia y separar claramente hechos, hipótesis, estimaciones y datos pendientes.

**Instrucciones:**

1. Abre **Copilot Chat** en una pestaña nueva del navegador.
2. Verifica que utilizas la experiencia de trabajo asociada a tu cuenta profesional o educativa.
3. Copia la siguiente indicación completa en Copilot Chat. Los datos incluidos son ficticios y autorizados exclusivamente para esta práctica.

```text
Actúa como analista de operaciones y experiencia de cliente para un caso simulado de formación llamado Northstar Digital.

Objetivo:
Analizar una interrupción temporal del portal de inversionistas y preparar una base verificable para un reporte ejecutivo. No presentes hipótesis, inferencias ni estimaciones como hechos confirmados.

Contexto autorizado y simulado:
- El portal de inversionistas de Northstar Digital presentó errores de acceso y carga de información el martes 15 de septiembre de 2026.
- A las 08:42, el sistema de monitorización detectó un aumento de errores HTTP 503 en el portal.
- A las 08:47, el equipo de soporte recibió los primeros contactos de usuarios que no podían iniciar sesión o consultar documentos.
- A las 08:55, el equipo de operaciones declaró una incidencia de prioridad alta y abrió un puente de coordinación.
- A las 09:10, se publicó un mensaje temporal de mantenimiento en el portal.
- A las 09:25, se publicó una comunicación breve en el canal de atención autorizado indicando que el equipo investigaba el problema y que no existía información confirmada sobre pérdida de datos.
- A las 10:05, el equipo técnico aplicó una reversión de una configuración desplegada a las 08:30.
- A las 10:18, la tasa de errores volvió a niveles normales.
- A las 10:32, se realizaron comprobaciones funcionales básicas de inicio de sesión, consulta de documentos y descarga de informes.
- A las 10:45, se restauró el acceso general al portal.
- La duración total estimada de afectación para usuarios fue de 123 minutos, desde 08:42 hasta 10:45.
- Durante ese intervalo se registraron 1.860 intentos de acceso; 1.116 terminaron con error o abandono antes de completar la tarea.
- El centro de atención recibió 74 contactos relacionados con la incidencia.
- No hay evidencia confirmada de acceso no autorizado, pérdida de datos ni modificación de documentos. La investigación de seguridad continúa abierta.
- La reversión de configuración coincidió temporalmente con la recuperación del servicio, pero aún no existe análisis de causa raíz aprobado.
- El equipo de producto tenía previsto publicar una actualización de resultados trimestrales a las 11:00.
- El escenario económico base de una práctica anterior estimó que una interrupción de menos de cuatro horas tendría impacto financiero directo limitado, pero podría aumentar el riesgo reputacional y generar costes de atención y seguimiento. Este es un supuesto de trabajo, no un dato financiero confirmado.
- En una práctica anterior de experiencia digital se identificó que la facilidad de acceso a documentos, la disponibilidad del portal y la claridad de las comunicaciones son factores relevantes para la confianza de los inversionistas.
- En una práctica anterior de comunicaciones se preparó un mensaje de interrupción con tono transparente, prudente y sin atribuir una causa antes de confirmar la investigación.

Restricciones:
- Usa únicamente los datos proporcionados.
- No inventes cifras económicas, causas técnicas específicas, nombres de sistemas, responsables reales, fechas adicionales ni compromisos regulatorios.
- Etiqueta expresamente cada elemento como hecho conocido, hipótesis, impacto estimado o dato pendiente.
- Si hay una relación temporal, descríbela como correlación y no como causalidad.
- Señala los riesgos de comunicación, experiencia de cliente, operación, seguridad y reputación.
- Redacta en español profesional para un equipo interno.

Formato de salida:
1. Hechos conocidos.
2. Hipótesis o interpretaciones que requieren validación.
3. Impacto estimado en clientes, operación y negocio.
4. Datos pendientes y preguntas para la investigación.
5. Riesgos priorizados con nivel Alto, Medio o Bajo y justificación breve.
6. Acciones correctivas iniciales separadas en: inmediatas, corto plazo y seguimiento de causa raíz.
7. Lista de afirmaciones que no deben incluirse como hechos en una comunicación ejecutiva hasta ser verificadas.

Criterios de calidad:
- Máximo 800 palabras.
- Lenguaje claro y ejecutivo.
- Trazabilidad explícita a los datos proporcionados.
- Diferencia inequívoca entre confirmación, estimación e hipótesis.
```

4. Revisa la respuesta de Copilot antes de reutilizarla.
5. Comprueba particularmente que Copilot:
   - No afirme que la configuración fue la causa raíz.
   - No afirme que no hubo pérdida de datos como una certeza absoluta; el dato disponible indica que no existe evidencia confirmada y que la investigación sigue abierta.
   - No convierta la estimación económica previa en una cifra financiera confirmada.
   - No invente sistemas, equipos, responsables personales o consecuencias regulatorias.
6. Si la separación entre categorías no es suficientemente clara, solicita un refinamiento con esta indicación:

```text
Revisa tu respuesta. Reescribe únicamente las secciones 1 a 4 en una tabla con las columnas: Categoría, afirmación, evidencia disponible, nivel de certeza y validación necesaria. Mantén la distinción entre hecho, hipótesis, impacto estimado y dato pendiente. No añadas datos.
```

**Resultado esperado:**

Dispones de un análisis inicial estructurado de la incidencia que distingue los elementos confirmados de los elementos que requieren validación.

**Verificación:**

Comprueba que la respuesta incluya, como mínimo:

- La detección de errores a las 08:42.
- La reversión de configuración a las 10:05.
- La recuperación de la tasa de errores a las 10:18.
- La restauración del acceso a las 10:45.
- La cifra de 1.860 intentos de acceso y 1.116 intentos con error o abandono.
- Los 74 contactos recibidos por el centro de atención.
- La ausencia de evidencia confirmada de pérdida de datos, indicando que la investigación sigue abierta.
- La aclaración de que la reversión coincidió con la recuperación, pero no constituye una causa raíz confirmada.

---

### Paso 3. Validar el análisis y calcular indicadores con transparencia

**Objetivo:** Revisar la coherencia del análisis generado y obtener indicadores útiles para dirección sin ocultar sus limitaciones.

**Instrucciones:**

1. En Copilot Chat, utiliza la siguiente indicación para solicitar cálculos y validación de consistencia:

```text
Usa exclusivamente los datos simulados proporcionados anteriormente.

Calcula y presenta:
- Porcentaje de intentos de acceso que terminaron con error o abandono.
- Porcentaje de intentos que no terminaron con error o abandono, si procede.
- Promedio aproximado de contactos al centro de atención por hora de afectación.
- Duración de la afectación expresada en horas y minutos.

Después, indica:
1. Qué cálculos son aritméticos y verificables con los datos proporcionados.
2. Qué conclusiones no se pueden extraer de esos cálculos.
3. Cómo redactar cada indicador para un comité directivo sin exagerar certeza ni impacto.

Formato:
Una tabla con Indicador, Cálculo, Resultado, Interpretación prudente y Limitación.
No inventes ingresos perdidos, número de clientes únicos afectados, incumplimientos regulatorios ni causa raíz.
```

2. Revisa los cálculos sugeridos. Como referencia, verifica manualmente los siguientes valores:

   - Porcentaje de intentos con error o abandono:

   ```text
   1.116 / 1.860 × 100 = 60 %
   ```

   - Porcentaje de intentos sin error o abandono:

   ```text
   744 / 1.860 × 100 = 40 %
   ```

   - Duración de la afectación:

   ```text
   123 minutos = 2 horas y 3 minutos
   ```

   - Promedio aproximado de contactos por hora:

   ```text
   74 / 2,05 horas ≈ 36 contactos por hora
   ```

3. Considera las limitaciones de estos indicadores:
   - Los intentos no equivalen necesariamente a usuarios únicos.
   - Un abandono no demuestra que un usuario no pudiera completar la tarea por otros medios.
   - El número de contactos no representa la totalidad de personas afectadas.
   - Los cálculos no permiten estimar pérdidas financieras reales.
   - La duración se refiere a la ventana estimada de afectación, no necesariamente a la experiencia individual de cada usuario.
4. Si Copilot utiliza un lenguaje excesivamente concluyente, solicita este ajuste:

```text
Reformula las interpretaciones con lenguaje prudente. Usa expresiones como “se registró”, “se estima”, “podría indicar”, “requiere confirmación” y “no permite concluir”. Conserva los cálculos, pero elimina cualquier afirmación causal o financiera no sustentada.
```

5. Copia en tus notas los indicadores y limitaciones que consideres adecuados para el reporte final.

**Resultado esperado:**

Cuentas con métricas verificadas, interpretaciones prudentes y limitaciones explícitas que pueden incluirse en un reporte para dirección.

**Verificación:**

- El porcentaje de intentos con error o abandono es **60 %**.
- La duración indicada es **2 horas y 3 minutos**.
- El reporte no equipara intentos con usuarios únicos.
- El reporte no contiene cifras de ingresos perdidos, sanciones, daños reputacionales cuantificados ni costes de recuperación no proporcionados.
- La relación entre la reversión y la recuperación está descrita como coincidencia temporal, no como causa confirmada.

---

### Paso 4. Generar el borrador del reporte ejecutivo

**Objetivo:** Pedir a Copilot Chat un reporte ejecutivo de una página o equivalente, dirigido al comité directivo y basado exclusivamente en datos autorizados.

**Instrucciones:**

1. En Copilot Chat, envía la siguiente indicación. Si tu experiencia permite referenciar contenido de la página, úsalo solo después de comprobar que los materiales citados son los resultados simulados de las prácticas previas.

```text
Genera un borrador de reporte ejecutivo de una página o equivalente para el comité directivo de Northstar Digital sobre la incidencia simulada del portal de inversionistas del 15 de septiembre de 2026.

Usa exclusivamente los datos simulados proporcionados en esta conversación y los siguientes hallazgos resumidos de prácticas anteriores:
- La disponibilidad del portal, el acceso a documentos y la claridad de las comunicaciones influyen en la confianza de los inversionistas.
- El escenario económico base indica que una interrupción inferior a cuatro horas podría tener impacto financiero directo limitado, pero puede elevar riesgos reputacionales, de atención y de seguimiento. Es un supuesto de trabajo, no una confirmación financiera.
- La comunicación durante una interrupción debe ser transparente, prudente, coherente y no atribuir causas antes de que se confirme la investigación.

Audiencia:
Comité directivo.

Propósito:
Informar, facilitar decisiones y establecer seguimiento, sin presentar hipótesis como hechos.

Estructura obligatoria:
1. Título y fecha del reporte.
2. Resumen ejecutivo de máximo 90 palabras.
3. Línea de tiempo con los hitos 08:42, 08:55, 09:10, 09:25, 10:05, 10:18, 10:32 y 10:45.
4. Impacto en clientes y negocio:
   - 1.860 intentos de acceso.
   - 1.116 intentos con error o abandono.
   - 74 contactos al centro de atención.
   - Afectación estimada de 123 minutos.
   - Explica las limitaciones de los datos sin saturar el reporte.
5. Estado de investigación:
   - Hechos confirmados.
   - Hipótesis o elementos por validar.
6. Riesgos principales:
   - Experiencia de cliente.
   - Reputación y confianza.
   - Operación.
   - Seguridad.
   - Comunicación.
7. Decisiones requeridas del comité directivo.
8. Acciones correctivas y plan de seguimiento con responsable por función, no por nombre personal:
   - Operaciones.
   - Ingeniería o plataforma.
   - Seguridad.
   - Atención al cliente.
   - Comunicaciones.
   - Dirección de producto.
9. Próximos pasos y fecha objetivo relativa, por ejemplo “en 24 horas”, “en 5 días laborables” o “tras la aprobación del análisis de causa raíz”.

Restricciones:
- Máximo 700 palabras.
- Tono ejecutivo, sobrio, claro y no defensivo.
- No inventes causa raíz, pérdidas económicas, usuarios únicos afectados, obligaciones regulatorias, responsables individuales, sistemas internos ni información de seguridad.
- Distingue visualmente hechos confirmados, estimaciones, hipótesis y datos pendientes.
- Señala que no existe evidencia confirmada de acceso no autorizado, pérdida de datos o modificación de documentos, y que la investigación de seguridad sigue abierta.
- Describe la reversión de configuración como una acción que coincidió temporalmente con la recuperación, no como causa raíz confirmada.
- Incluye una nota final: “Borrador sujeto a validación técnica, de seguridad, financiera y de comunicaciones antes de distribución.”

Criterios de calidad:
- Debe poder leerse en aproximadamente tres minutos.
- Debe permitir al comité identificar qué ocurrió, cuál fue el impacto conocido, qué sigue siendo incierto, qué decisiones debe tomar y cómo se medirá el seguimiento.
- Debe conservar trazabilidad a los datos proporcionados.
```

2. Lee el borrador completo antes de copiarlo a la Página de Copilot.
3. Comprueba que el resumen ejecutivo:
   - Sea breve y comprensible sin conocer todos los detalles técnicos.
   - Distinga entre la interrupción confirmada y la causa todavía en investigación.
   - No contenga lenguaje culpabilizador o especulativo.
4. Comprueba que las decisiones requeridas sean realistas y estén formuladas como decisiones para dirección. Ejemplos adecuados:
   - Priorizar y patrocinar el análisis de causa raíz.
   - Aprobar un plan de mejora de monitorización y reversión.
   - Acordar el enfoque de comunicación de seguimiento.
   - Solicitar una revisión de riesgos y controles antes de cerrar el incidente.
5. Si el reporte es demasiado extenso, solicita esta mejora:

```text
Reduce el reporte a un máximo de 550 palabras sin eliminar la línea de tiempo, la separación entre hechos e hipótesis, los riesgos, las decisiones requeridas ni los próximos pasos. Elimina repeticiones y conserva todas las cifras proporcionadas.
```

6. Si el reporte no muestra con claridad los elementos inciertos, solicita este refinamiento:

```text
Reorganiza el reporte para que use estas etiquetas visibles: “Confirmado”, “Estimado”, “Pendiente de validar” y “Hipótesis de trabajo”. No cambies los datos ni añadas información.
```

**Resultado esperado:**

Obtienes un borrador ejecutivo conciso, estructurado y apto para revisión humana antes de cualquier distribución.

**Verificación:**

El borrador debe incluir todos estos componentes:

- Resumen ejecutivo.
- Línea de tiempo.
- Impacto en clientes y negocio.
- Estado de investigación.
- Riesgos.
- Decisiones requeridas.
- Acciones correctivas con responsables por función.
- Próximos pasos.
- Nota de validación final.

Además, confirma que:

- La causa raíz no aparece como confirmada.
- Los escenarios económicos se presentan como supuestos de trabajo.
- No se incluyen datos sensibles o reales.
- No se atribuye responsabilidad a personas concretas.
- La investigación de seguridad se mantiene abierta.

---

### Paso 5. Aplicar revisión humana y crear la lista de validación final

**Objetivo:** Evaluar el borrador con criterios de exactitud, trazabilidad, tono y adecuación ejecutiva antes de guardarlo como producto final.

**Instrucciones:**

1. Revisa manualmente el borrador generado por Copilot.
2. Usa la siguiente lista de validación. Marca cada punto como `Sí`, `No` o `Requiere revisión`.

| Criterio de validación | Estado |
|---|---|
| El reporte se basa únicamente en datos simulados y autorizados. |  |
| El reporte identifica la interrupción, la ventana de afectación y los hitos principales de forma correcta. |  |
| Las cifras de 1.860 intentos, 1.116 intentos con error o abandono y 74 contactos son correctas. |  |
| La duración de 123 minutos se expresa correctamente como 2 horas y 3 minutos, si se incluye la conversión. |  |
| Se diferencia claramente entre hechos confirmados, estimaciones, hipótesis y datos pendientes. |  |
| La reversión de configuración no se presenta como causa raíz confirmada. |  |
| La ausencia de evidencia de pérdida de datos o acceso no autorizado se expresa con cautela y se indica que la investigación sigue abierta. |  |
| No se inventan impactos financieros, obligaciones regulatorias, sistemas, personas, causas ni compromisos no proporcionados. |  |
| Los riesgos incluyen experiencia de cliente, reputación, operación, seguridad y comunicación. |  |
| Las decisiones requeridas pueden ser tomadas o patrocinadas por el comité directivo. |  |
| Las acciones tienen responsables por función y plazos relativos realistas. |  |
| El tono es ejecutivo, claro, profesional y no defensivo. |  |
| El reporte puede leerse aproximadamente en tres minutos. |  |
| El reporte incluye una nota que indique que requiere validación humana antes de su distribución. |  |

3. Corrige manualmente cualquier dato incorrecto o formulación ambigua.
4. Si necesitas apoyo para identificar lenguaje de riesgo, utiliza Copilot Chat con esta indicación:

```text
Revisa el siguiente borrador únicamente para detectar riesgos de redacción. No reescribas ni añadas datos.

Identifica:
- afirmaciones que parezcan hechos pero sean hipótesis;
- lenguaje demasiado concluyente;
- cifras o promesas no sustentadas;
- ausencia de limitaciones relevantes;
- tono inadecuado para un comité directivo;
- frases que puedan interpretarse como atribución prematura de causa o responsabilidad.

Devuelve una lista con: texto problemático, motivo y propuesta de redacción prudente.
```

5. Pega el borrador revisado en la sección `L03.4 - Reporte ejecutivo` de la Página de Copilot.
6. Debajo del reporte, agrega el siguiente subtítulo:

   ```text
   Validación final y aprobación humana
   ```

7. Copia la lista de validación completada. Incluye una conclusión breve, por ejemplo:

   ```text
   Conclusión de revisión: el reporte es apto como borrador interno para revisión del comité directivo. La causa raíz, el alcance de seguridad y cualquier impacto financiero requieren validación adicional antes de una distribución final.
   ```

8. Si el instructor solicita conservar una evidencia local, guarda una copia de texto sin información real en:

```text
C:\CopilotLabs\TransformarIdeasEnAccion\03-00-04\
```

**Resultado esperado:**

La Página de Copilot contiene un reporte ejecutivo revisado y una lista de validación que demuestra la aplicación de juicio humano.

**Verificación:**

- La sección se titula exactamente `L03.4 - Reporte ejecutivo`.
- El reporte está pegado en la misma Página de Copilot que los resultados de prácticas anteriores.
- La lista de validación está completada.
- Las observaciones pendientes se documentan claramente.
- El contenido no declara que la IA haya aprobado, confirmado o investigado técnicamente el incidente.
- La conclusión establece que la aprobación final corresponde a responsables humanos.

---

### Paso 6. Consolidar la trazabilidad y preparar el cierre del caso

**Objetivo:** Confirmar que el producto final conecta los hallazgos de las cuatro prácticas sin confundir análisis previos con hechos operativos confirmados.

**Instrucciones:**

1. En la sección `L03.4 - Reporte ejecutivo`, agrega un subtítulo final:

   ```text
   Trazabilidad del caso transversal
   ```

2. Añade una lista breve que vincule el reporte con los productos anteriores:

```text
- L02 - Prompt refinado: estructura de indicación con objetivo, contexto, restricciones, formato y criterios de calidad.
- L03.1 - Experiencia de inversionistas: relevancia de disponibilidad, acceso a documentos y comunicaciones claras para la confianza.
- L03.2 - Escenarios económicos: supuesto de impacto financiero directo limitado para una interrupción inferior a cuatro horas; requiere validación financiera.
- L03.3 - Comunicaciones de interrupción: necesidad de un mensaje transparente, prudente y sin atribución de causa no confirmada.
- L03.4 - Reporte ejecutivo: consolidación del incidente simulado, riesgos, decisiones requeridas y plan de seguimiento.
```

3. Revisa que el reporte no presente los resultados de `L03.1`, `L03.2` o `L03.3` como evidencia técnica de la incidencia.
4. Asegúrate de que esos resultados se usen como contexto de decisión:
   - Experiencia digital: para interpretar el riesgo de confianza.
   - Escenarios económicos: para identificar supuestos y necesidades de validación financiera.
   - Comunicaciones: para definir el tono y los límites de los mensajes.
5. Guarda la página o espera a que se sincronice automáticamente, según la experiencia disponible.
6. Actualiza la página o vuelve a abrirla para confirmar que los cambios persisten.

**Resultado esperado:**

El cuaderno contiene una trazabilidad clara entre las cuatro prácticas y el reporte final diferencia datos operativos confirmados de análisis de contexto y supuestos de trabajo.

**Verificación:**

- La página conserva los cinco títulos requeridos.
- La trazabilidad menciona correctamente las prácticas anteriores.
- No se mezclan supuestos financieros con resultados financieros confirmados.
- No se presentan recomendaciones de comunicación como evidencia de la causa técnica.
- El reporte final sigue siendo comprensible sin abrir los materiales anteriores.

## Validación y pruebas

Completa las siguientes pruebas antes de dar por finalizada la práctica.

### Prueba 1. Exactitud de los hechos operativos

Comprueba que el reporte refleje estos datos sin modificación:

| Dato | Valor esperado |
|---|---:|
| Detección inicial de errores | 08:42 |
| Declaración de incidencia prioritaria | 08:55 |
| Mensaje temporal de mantenimiento | 09:10 |
| Comunicación inicial de atención | 09:25 |
| Reversión de configuración | 10:05 |
| Normalización de la tasa de errores | 10:18 |
| Comprobaciones funcionales básicas | 10:32 |
| Restauración general del acceso | 10:45 |
| Ventana estimada de afectación | 123 minutos |
| Intentos de acceso | 1.860 |
| Intentos con error o abandono | 1.116 |
| Contactos al centro de atención | 74 |

**Criterio de aceptación:** todos los datos coinciden con la tabla y no se añaden detalles técnicos no proporcionados.

### Prueba 2. Separación de certeza y suposición

Busca en el reporte términos como:

- `Confirmado`
- `Estimado`
- `Pendiente de validar`
- `Hipótesis de trabajo`
- `No existe evidencia confirmada`
- `Coincidió temporalmente`
- `Requiere investigación`

**Criterio de aceptación:** la causa raíz, el alcance de seguridad y el impacto financiero no se presentan como hechos confirmados.

### Prueba 3. Calidad ejecutiva

Lee el reporte como si fueras una persona miembro del comité directivo. Debes poder responder en menos de tres minutos:

1. ¿Qué ocurrió?
2. ¿Durante cuánto tiempo?
3. ¿Qué impacto se conoce?
4. ¿Qué información sigue siendo incierta?
5. ¿Cuáles son los riesgos principales?
6. ¿Qué decisiones se solicitan al comité?
7. ¿Quién debe realizar las acciones y cuándo?

**Criterio de aceptación:** el reporte permite responder estas preguntas sin consultar la conversación completa de Copilot Chat.

### Prueba 4. Seguridad y gobernanza

Confirma que el contenido:

- Usa únicamente el escenario simulado de Northstar Digital.
- No contiene nombres reales de personas.
- No contiene datos de clientes reales.
- No contiene credenciales, configuraciones internas reales ni detalles de seguridad sensibles.
- Incluye la necesidad de validación técnica, de seguridad, financiera y de comunicaciones.
- Mantiene la responsabilidad de aprobación en personas autorizadas.

**Criterio de aceptación:** no existe información confidencial, personal o no autorizada en la conversación, la página ni los archivos locales.

## Resolución de problemas

### Problema 1: Copilot Chat presenta la reversión de configuración como causa raíz confirmada

**Síntomas:**

- El borrador afirma que “la causa del incidente fue una configuración incorrecta”.
- El reporte indica que “la reversión solucionó definitivamente el problema”.
- La sección de riesgos omite la investigación técnica o de seguridad pendiente.

**Causa probable:**

Copilot ha interpretado una correlación temporal como causalidad. Los datos autorizados indican que la reversión de las 10:05 coincidió con la recuperación observada a las 10:18, pero no existe un análisis de causa raíz aprobado.

**Solución:**

1. No uses el texto como está.
2. Solicita un refinamiento en Copilot Chat:

```text
Corrige el borrador para eliminar toda afirmación de causa raíz confirmada. Indica que la reversión de configuración coincidió temporalmente con la recuperación del servicio y que la causa raíz sigue pendiente de análisis técnico aprobado. No añadas causas alternativas.
```

3. Revisa manualmente que el texto corregido utilice expresiones como:
   - “hipótesis de trabajo”
   - “elemento pendiente de validación”
   - “correlación temporal observada”
   - “análisis de causa raíz en curso”
4. Actualiza el reporte y marca en la lista de validación que la atribución causal fue revisada.

### Problema 2: No puedes encontrar, editar o guardar la página `Northstar Digital - Cuaderno de análisis`

**Síntomas:**

- La página no aparece en los resultados de búsqueda.
- Puedes verla, pero no editarla.
- Los cambios no se conservan al actualizar el navegador.
- Se muestra una solicitud de permisos o una experiencia diferente a la utilizada en prácticas anteriores.

**Causa probable:**

La cuenta activa no es la cuenta profesional o educativa correcta, no tienes permisos de edición, la página se creó en otro contexto de Microsoft 365 o existe un problema temporal de sincronización o conectividad.

**Solución:**

1. Comprueba la cuenta activa en Microsoft 365 y confirma que corresponde al tenant de formación.
2. Cierra sesión de cuentas personales o no autorizadas en el navegador.
3. Abre una ventana de InPrivate, inicia sesión solo con la cuenta profesional o educativa y vuelve a buscar la página.
4. Comprueba la conexión a Internet y actualiza la página.
5. Si puedes ver la página pero no editarla, solicita al instructor o propietario de la página permiso de edición.
6. Si el problema persiste, guarda temporalmente el borrador simulado en:

```text
C:\CopilotLabs\TransformarIdeasEnAccion\03-00-04\
```

7. Informa al instructor antes de crear una página nueva. No crees una página de sustitución con un nombre diferente sin autorización, porque se perdería la trazabilidad requerida.

## Limpieza

1. Cierra las pestañas de Copilot Chat que contengan borradores de la práctica cuando el instructor confirme que no necesitas seguir consultándolos.
2. Comprueba que el producto final esté guardado en la Página de Copilot:

   ```text
   Northstar Digital - Cuaderno de análisis
   ```

3. Si descargaste borradores o evidencias, confirma que solo contienen datos simulados.
4. Conserva únicamente los archivos que el instructor haya solicitado en:

```text
C:\CopilotLabs\TransformarIdeasEnAccion\03-00-04\
```

5. Elimina copias temporales, duplicados o borradores no necesarios que puedan causar confusión.
6. No elimines la Página de Copilot ni las secciones de las prácticas anteriores, ya que forman parte de la trazabilidad del caso transversal.
7. Cierra sesión de Microsoft 365 si utilizas un equipo compartido.

## Resumen

En esta práctica consolidaste el caso de Northstar Digital en un reporte ejecutivo de incidencia operativa. Utilizaste Copilot Chat como apoyo para estructurar hechos, hipótesis, impactos estimados, riesgos y acciones, pero aplicaste validación humana para evitar que una respuesta plausible se convirtiera en una afirmación no verificada.

El producto final conserva la trazabilidad entre la indicación refinada, el análisis de experiencia de inversionistas, los escenarios económicos, las comunicaciones de interrupción y el reporte ejecutivo. La principal práctica profesional aplicada es la distinción explícita entre:

- **Hechos conocidos:** información respaldada por los datos proporcionados.
- **Estimaciones:** cálculos o interpretaciones limitadas por los datos disponibles.
- **Hipótesis de trabajo:** explicaciones posibles que requieren investigación.
- **Datos pendientes:** información necesaria antes de cerrar el incidente o distribuir comunicaciones definitivas.

Antes de utilizar un reporte generado con apoyo de IA en un contexto real, deben revisarlo y aprobarlo las funciones responsables de operación, seguridad, finanzas, comunicaciones y dirección.

### Recursos opcionales

- [Microsoft Support: Bienvenido a Copilot Chat](https://support.microsoft.com/es-es/topic/bienvenido-a-copilot-chat-34c93d56-86e6-4b5b-8cc8-59cbe8e53bc3)
- [Microsoft Support: Introducción a Microsoft 365 Copilot Chat](https://support.microsoft.com/es-es/copilot-microsoft-365)
- [Microsoft Learn: Introducción a Microsoft 365 Copilot](https://learn.microsoft.com/es-es/copilot/microsoft-365/)
