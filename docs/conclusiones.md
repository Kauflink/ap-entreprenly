# Conclusiones y recomendaciones

## Conclusiones

1. **La investigación preliminar validó la existencia de una brecha tecnológica real en el comercio minorista peruano.** A través de la aplicación de la técnica 5W's y 2H's, el análisis competitivo y las entrevistas con comerciantes y consumidores del segmento objetivo, el equipo confirmó que la mayoría de los pequeños negocios de retail —bodegas, minimarkets y puestos de mercado— opera sin herramientas digitales de gestión, lo que genera pérdidas directas por productos vencidos, desabastecimiento no detectado y ventas sin trazabilidad. Este hallazgo fundamenta con solidez la propuesta de valor de Entreprenly como solución viable y necesaria para ese segmento.

2. **El proceso Lean UX permitió definir un alcance de producto acotado y orientado a resultados medibles.** La formulación de Hypothesis Statements con criterios de éxito cuantificables —como la reducción del 60% en descuadres de inventario o la disminución del 50% en el tiempo de cierre de caja— estableció una hoja de ruta clara para las iteraciones futuras. Este enfoque garantiza que el desarrollo del producto se mantenga alineado con las necesidades reales del usuario y no se desvíe hacia funcionalidades sin sustento en la problemática identificada.

3. **La arquitectura de software definida mediante Domain-Driven Design y el modelo C4 proporcionó una base técnica robusta y escalable para el desarrollo de Entreprenly.** La identificación de siete Bounded Contexts independientes —Autenticación, Perfil, Suscripción, Inventario, Ventas, Chatbot y Pagos— y su documentación a nivel de Contexto, Contenedor y Componente permitió al equipo establecer responsabilidades claras entre capas, facilitando el desarrollo paralelo y la futura incorporación de nuevas funcionalidades sin comprometer la integridad de la arquitectura base.

4. **El Sprint 1 demostró la capacidad del equipo para entregar un producto funcional y desplegado en producción dentro de un ciclo corto.** La implementación y publicación del Landing Page de Entreprenly en `entreprenly.online` mediante un pipeline de CI/CD automatizado con GitHub Actions validó el entorno de trabajo colaborativo del equipo y estableció la base de infraestructura de despliegue para los sprints siguientes. El Landing Page cumplió su objetivo al comunicar la propuesta de valor del producto a los dos segmentos objetivo con secciones diferenciadas, selector de idioma y soporte de tema claro/oscuro.

5. **La adopción de GitFlow, Conventional Commits y Semantic Versioning como estándares de gestión del código fuente fortaleció la trazabilidad y la calidad del proceso de desarrollo colaborativo.** Los 20 commits distribuidos en 5 Pull Requests durante el Sprint 1, con mensajes descriptivos y revisión entre pares, evidencian que el equipo internalizó las buenas prácticas de ingeniería de software desde la primera iteración, sentando un precedente de disciplina técnica que deberá mantenerse en los sprints subsiguientes.

6. **La elaboración del Product Backlog con User Stories estructuradas bajo el formato Connextra y criterios de aceptación en formato Given-When-Then provee al equipo una base de requisitos suficientemente detallada para planificar los sprints 2 y 3 con alta precisión.** La gestión de estas historias en Jira Software bajo el proyecto ENT permite administrar el trabajo de forma ágil, trazable y visible para todos los integrantes, integrando directamente la herramienta de gestión con el flujo de desarrollo documentado en el informe.

---

## Recomendaciones

1. En los sprints siguientes, se recomienda iniciar la implementación del Frontend Web Application con Vue Framework priorizando los Bounded Contexts de Autenticación e Inventario, dado que son las funcionalidades de mayor valor para el usuario principal y constituyen el núcleo operativo del producto.

2. Se recomienda realizar al menos una sesión de validación del Landing Page con usuarios reales del segmento objetivo antes del Sprint 2, con el fin de incorporar retroalimentación temprana sobre la claridad de la propuesta de valor y la efectividad de los CTAs diferenciados por segmento.

3. Para mantener la coherencia del sistema de diseño a lo largo del desarrollo, se recomienda que el equipo documente los tokens de diseño definidos en el Style Guidelines (colores, tipografías, espaciados) como variables CSS globales en el repositorio del Frontend, garantizando consistencia visual entre el Landing Page y la Web Application.