








FACULTAD DE INGENIERÍA 
INGENIERÍA EN COMPUTACIÓN E INFORMÁTICA


TÍTULO DE LA INVESTIGACIÓN
"Sistema de Gestión Automatizada de Reportes para la Toma de Decisiones Empresariales"



Proyecto de título para optar al título de Ingeniero en Computación e Informática




NOMBRE ESTUDIANTE
Cesar Villablanca Seguel
PROFESOR GUÍA:
Ángel Segundo Villalobos Molero



SANTIAGO, CHILE 2025











FACULTAD DE INGENIERÍA 
INGENIERÍA EN COMPUTACIÓN E INFORMÁTICA


DECLARACIÓN DE ORIGINALIDAD Y PROPIEDAD




Yo, declaro que este documento no incorpora material de otros autores sin identificar debidamente la fuente.






Santiago, xx de diciembre de 2025







alumno



AGRADECIMIENTOS



Al llegar al final de este importante camino académico, no puedo dejar de mirar hacia atrás y sentir una profunda gratitud por todas aquellas personas que me acompañaron y apoyaron durante este proceso. A pesar de estar lejos de mi familia mis padres y mis dos hermanas su respaldo incondicional fue clave para que pudiera costear mis estudios y mantenerme firme en cada paso, aun en la distancia. A ellos, les debo no solo el apoyo económico, sino también el emocional, ya que han sido mi principal fuente de motivación y esperanza.

También deseo agradecer profundamente a mi lugar de trabajo, donde siempre encontré comprensión y flexibilidad para poder continuar con mi formación. Cada gesto de apoyo ha significado mucho para mí y ha facilitado este gran desafío de estudiar y trabajar en paralelo.

De igual manera, extiendo un sincero agradecimiento a mis profesores y profesoras, especialmente a quienes guiaron este proyecto. Al profesor Ángel Segundo Villalobos Molero, por su acompañamiento constante durante el Seminario de licenciatura en ingeniería , por su tiempo, sus correcciones y su disposición para entregar orientaciones claras y constructivas. A la profesora Barbarita Lara Martínez, quien me apoyó en el desarrollo del Proyecto de Título, le agradezco su dedicación, su exigencia académica y su compromiso con la formación profesional de sus estudiantes.

Este proyecto no solo representa el cierre de una etapa académica, sino también el resultado del esfuerzo colectivo de muchas personas que creyeron en mí. A todos ellos, gracias por acompañarme en este camino y por ser parte de la base de lo que vendrá. 


RESUMEN EJECUTIVO


El presente proyecto, titulado “Sistema de Gestión Automatizada de Reportes para la Toma de Decisiones Empresariales”, surge como respuesta a la necesidad de contar con una herramienta centralizada y segura que facilite el acceso y la administración de reportes generados por distintas áreas de una organización, optimizando los procesos de análisis y toma de decisiones. 
La solución implementada consiste en el desarrollo de una plataforma web basada en Django, que integra reportes alojados en Power BI Report Server (PBIRS). El sistema permite la gestión avanzada de usuarios y roles, segmentando el acceso a los reportes según el perfil y área del usuario. A través de un panel de control moderno y responsivo, los administradores pueden crear, editar y asignar roles, mientras que los usuarios visualizan únicamente los reportes autorizados para su perfil. 
Entre las funcionalidades clave se incluyen: 
Autenticación y control de acceso robusto.
Gestión de roles y usuarios desde una interfaz intuitiva.
Visualización personalizada de reportes según permisos.
Integración directa con Power BI Report Server, permitiendo el acceso seguro a reportes .pbix.
Notificaciones y mensajes personalizados para mejorar la experiencia de usuario.
Diseño responsivo y compatible con múltiples dispositivos.
Para su desarrollo se utilizaron tecnologías como Django para el backend y la lógica de negocio, SQL Server como sistema gestor de base de datos, y Power BI Report Server para la gestión y visualización de reportes empresariales. El sistema reemplaza procesos manuales, reduce tiempos operativos, minimiza errores humanos y contribuye a la transformación digital de la organización mediante el uso de tecnologías robustas y de alto impacto.




















INTRODUCCIÓN






















Introducción detallada
En el contexto actual, las organizaciones requieren herramientas que no solo almacenen información, sino que la transformen en conocimiento útil, accesible y seguro. La visualización clara y oportuna de datos es fundamental para que las jefaturas y los tomadores de decisiones puedan actuar de manera informada y estratégica.
Este proyecto propone una solución integral basada en una plataforma web desarrollada con Django, que se conecta directamente con Power BI Report Server (PBIRS) como sistema centralizado de visualización de reportes empresariales. La plataforma no solo permite la consulta de reportes, sino que también ofrece un entorno de gestión donde los administradores pueden registrar, filtrar, asignar permisos y controlar el acceso a los reportes de manera eficiente y personalizada, todo desde una única interfaz.
A través de la gestión avanzada de roles y usuarios, el sistema garantiza que cada persona acceda únicamente a la información relevante para su perfil o área, fortaleciendo la seguridad y la confidencialidad de los datos. De este modo, la solución contribuye a la transformación digital de la organización, optimizando los procesos de análisis y toma de decisiones mediante el uso de tecnologías modernas y robustas.
Importancia de resolver el problema
La dificultad para acceder a reportes relevantes, la falta de centralización y la dependencia de procesos manuales representan desafíos significativos en muchas empresas. Estos problemas no solo ralentizan la toma de decisiones, sino que también aumentan el riesgo de errores y comprometen la seguridad de la información.
La solución propuesta en este proyecto permite automatizar la consulta y gestión de reportes empresariales, centralizando el acceso a través de una plataforma web robusta y segura. Mediante la integración con Power BI Report Server y la gestión de roles y permisos en Django, se garantiza que cada usuario acceda únicamente a los reportes autorizados para su perfil. Esto no solo optimiza la eficiencia operativa, sino que también fortalece la seguridad y la trazabilidad en el manejo de datos críticos para la organización.
Breve discusión bibliográfica
Herramientas como Power BI se han consolidado como soluciones líderes en el ámbito de la inteligencia de negocios, gracias a su capacidad para conectar múltiples fuentes de datos, procesar información en tiempo real y ofrecer dashboards interactivos y visualmente atractivos. Diversos estudios y experiencias empresariales destacan el impacto positivo de Power BI en la toma de decisiones, al facilitar la interpretación de grandes volúmenes de datos y democratizar el acceso a la información relevante dentro de las organizaciones.
Sin embargo, la integración de estas plataformas con sistemas de gestión propios aporta un valor añadido significativo. Al complementar las capacidades nativas de Power BI con una plataforma personalizada —como la desarrollada en este proyecto— es posible adaptar la experiencia de usuario a las necesidades específicas de la organización, implementar controles de acceso más granulares, y ampliar funcionalidades como la exportación de reportes, el historial de consultas, la gestión avanzada de roles o la generación de notificaciones automáticas. Esta combinación potencia la seguridad, la eficiencia y la flexibilidad en la gestión de la información estratégica.Contribución al trabajo

Este proyecto propone un enfoque mixto, donde se aprovechan las capacidades avanzadas de Power BI y se complementan con una plataforma personalizada de gestión. Así, se entregará una solución escalable, organizada y adaptable a distintas necesidades organizacionales, promoviendo el uso eficiente de la información.
Organización y presentación de este trabajo
Este documento se estructura en capítulos que abordan de manera progresiva el desarrollo del proyecto. En primer lugar, se presenta el problema identificado y su relevancia en el contexto organizacional, seguido de los objetivos generales y específicos que guían la solución propuesta. Posteriormente, se describe en detalle el diseño de la plataforma, incluyendo la arquitectura del sistema, la integración con Power BI Report Server y la gestión de usuarios y roles.
La metodología de desarrollo empleada se expone junto con el análisis de riesgos y las estrategias de aseguramiento de la calidad implementadas durante el ciclo de vida del proyecto. Además, se incluyen diagramas, prototipos y capturas de pantalla que ilustran la funcionalidad y la interfaz del sistema, así como una justificación de las tecnologías seleccionadas. Finalmente, se presentan las conclusiones obtenidas y las recomendaciones para futuras mejoras o ampliaciones del sistema.





































IDENTIFICACIÓN DEL PROBLEMA / OPORTUNIDAD



















PRESENTACIÓN Y FUNDAMENTACIÓN DEL PROBLEMA / OPORTUNIDAD DE MEJORA 
Factores internos 
El sistema actual de manejo y visualización de reportes en las empresas depende en gran medida de procesos manuales, como el envío de reportes por correo electrónico y el almacenamiento de archivos en carpetas locales o compartidas. Esta modalidad genera pérdida de tiempo, duplicidad de información, dificultades en la trazabilidad de los documentos y un mayor riesgo de errores humanos.
A nivel interno, los equipos carecen de una herramienta centralizada que les permita filtrar, visualizar y acceder a los reportes de manera dinámica y segura, de acuerdo con su rol o área dentro de la organización. La ausencia de controles de acceso automatizados y de una interfaz unificada limita la colaboración, dificulta la gestión eficiente de permisos y reduce la capacidad de respuesta ante necesidades de información estratégica.
Factores externos 
Desde el entorno externo, las organizaciones están migrando aceleradamente hacia sistemas centralizados y automatizados para el análisis de datos y la gestión de información. Soluciones como Power BI Report Server se han consolidado como herramientas clave para la integración de fuentes de datos en tiempo real, la visualización avanzada y el control seguro de la información estratégica.
La adopción de estas tecnologías permite a las empresas mejorar la toma de decisiones, reducir errores humanos y responder de manera ágil a los cambios del entorno. No contar con un sistema moderno y centralizado coloca a la organización en una posición de desventaja competitiva frente a aquellas que ya han incorporado soluciones digitales para el análisis de reportes y el control interno, limitando su capacidad de innovación y adaptación en un mercado cada vez más orientado a la transformación digital.sde el entorno externo, las organizaciones están migrando rápidamente a sistemas centralizados y automatizados de análisis de datos y gestión de información. Tecnologías como Power BI y Streamlit permiten la conexión a fuentes de datos en tiempo real, mejorando la toma de decisiones y reduciendo los errores humanos. No contar con un sistema moderno pone en desventaja competitiva a la organización frente a otras que ya han incorporado soluciones digitales para análisis de reportes y control interno.
Descripción de problemas / oportunidades de mejora
Descripción del problema
Actualmente, muchas organizaciones continúan gestionando sus reportes mediante procesos manuales, utilizando múltiples hojas de cálculo, correos electrónicos y herramientas desconectadas entre sí. Esta fragmentación operacional genera diversas dificultades: errores en la consolidación de información, pérdida de tiempo en la búsqueda y validación de datos, duplicación de esfuerzos y baja trazabilidad de los documentos compartidos.
Adicionalmente, el acceso a estos reportes no está adecuadamente segmentado por rol o área, lo que representa un riesgo tanto en términos de seguridad de la información como en eficiencia organizacional. La ausencia de un sistema centralizado y automatizado limita la capacidad de la empresa para responder ágilmente a las necesidades de información, dificulta la gestión de permisos y expone a la organización a posibles brechas de confidencialidad y control.
Oportunidades de mejora 
Existe una gran oportunidad de mejora mediante la implementación de un sistema que centralice la administración y visualización de reportes, permitiendo la asignación de permisos personalizados y la integración directa de visualizaciones generadas en Power BI Report Server. Esta solución automatizaría la consulta y gestión de reportes, facilitando el análisis de datos en tiempo real y desde cualquier dispositivo con conexión a internet.
Además, la centralización y segmentación de accesos por roles fortalecería la seguridad de la información y optimizaría los procesos internos, reduciendo la duplicidad de esfuerzos y mejorando la trazabilidad de los documentos. La adopción de esta plataforma permitiría a la organización avanzar hacia una gestión más eficiente, segura y alineada con las mejores prácticas de transformación digital.

Figura 1 
Árbol de oportunidad
 
Fuente: Elaboración propia 
Identificación cuantitativa de problemas
Factores concienciación
La digitalización y automatización de procesos es cada vez más valorada dentro de las organizaciones, especialmente en áreas estratégicas como finanzas, recursos humanos y operaciones. La implementación de un sistema como el propuesto fortalecerá la cultura digital en la empresa, promoviendo el uso de herramientas modernas y prácticas más eficientes para el análisis y la gestión de información clave.
Adoptar una plataforma centralizada para la administración y visualización de reportes no solo optimiza los procesos internos, sino que también impulsa la concienciación sobre la importancia de la seguridad, la trazabilidad y la accesibilidad de los datos. Este cambio cultural facilita la adaptación a nuevas tecnologías y prepara a la organización para enfrentar los desafíos de la transformación digital de manera proactiva y sostenible.
Factores económicos
La automatización del acceso y la visualización de reportes reduce significativamente el tiempo que los equipos dedican a la elaboración, revisión y distribución de documentos. Esta optimización se traduce en un ahorro directo de horas hombre y recursos operacionales, permitiendo que el personal enfoque sus esfuerzos en tareas de mayor valor estratégico.
Además, contar con información clara, centralizada y oportuna disminuye el riesgo de tomar decisiones erróneas, lo que puede representar una mejora directa en la productividad y en la reducción de costos asociados a la mala gestión de datos. La inversión en una plataforma moderna de gestión de reportes contribuye así a la eficiencia operativa y a la sostenibilidad económica de la organización.
Factores tecnología 

El proyecto se desarrolla utilizando tecnologías modernas, accesibles y de alto rendimiento, como Django para la gestión de usuarios, roles y servicios backend, Power BI Report Server para la visualización centralizada de datos empresariales, y SQL Server como sistema gestor de base de datos. Estas herramientas permiten construir un sistema robusto, seguro, escalable y fácilmente mantenible, sin necesidad de realizar grandes inversiones en infraestructura adicional.
La elección de estas tecnologías garantiza compatibilidad multiplataforma, integración con sistemas existentes y la posibilidad de ampliar funcionalidades en el futuro, asegurando así la sostenibilidad y evolución del sistema en el contexto de la transformación digital de la organización.
Factores comunidad 
El sistema propuesto es altamente replicable y adaptable a diversos contextos organizacionales, tales como municipalidades, PYMEs, universidades u ONGs. Gracias a su diseño modular y a la utilización de tecnologías ampliamente adoptadas como Django y Power BI Report Server, la solución puede ser personalizada según las necesidades y requerimientos específicos de cada institución.
Esta flexibilidad facilita la transferencia de conocimiento y la colaboración entre distintas organizaciones, promoviendo la adopción de buenas prácticas en la gestión y visualización de información estratégica, y contribuyendo al fortalecimiento de la cultura digital en la comunidad.
Factores medioambiente
Al reducir el uso de papel y optimizar el envío digital de reportes, el sistema contribuye activamente a la sostenibilidad medioambiental y promueve una cultura organizacional más ecológica. La centralización y digitalización de la gestión de reportes disminuye la necesidad de impresiones físicas y el almacenamiento de documentos en formato papel, lo que se traduce en un menor consumo de recursos y una reducción en la generación de residuos.
De esta manera, la implementación de la plataforma no solo mejora la eficiencia operativa, sino que también apoya los objetivos de responsabilidad social y medioambiental de la organización.
Análisis FODA

Fortaleza:
Automatización de la gestión y visualización de reportes.
Integración directa con Power BI Report Server para visualización avanzada.
Control granular de permisos y acceso por roles, mejorando la seguridad y la trazabilidad.
Oportunidades:
Escalabilidad del sistema para adaptarse a organizaciones de distintos tamaños y sectores.
Compatibilidad y replicabilidad en diversos contextos, como empresas, instituciones públicas, educativas y ONGs.
Potencial para incorporar nuevas funcionalidades y tecnologías en el futuro.
Debilidades:
Posible resistencia al cambio por parte de usuarios acostumbrados a procesos manuales o tradicionales.
Curva de aprendizaje inicial para la adopción de la nueva plataforma.
Amenazas:
Dependencia de la conexión a internet para el acceso y consulta de reportes.
Riesgos de seguridad si no se implementan correctamente los mecanismos de autenticación, autorización y protección de datos.
Objetivos general y específicos

Objetivo general
Diseñar e implementar un sistema de gestión automatizada de reportes que integre visualizaciones de Power BI Report Server, permitiendo el acceso segmentado por usuario y área, con control avanzado de permisos, filtros dinámicos y opciones de exportación, con el fin de optimizar y respaldar la toma de decisiones organizacional.
Objetivos específicos y métricas 

Desarrollar una plataforma web funcional para la gestión de reportes Power BI Report Server.
Métrica: La plataforma deberá estar operativa al finalizar el tercer mes de implementación, permitiendo la visualización de al menos tres reportes cargados y visibles para distintos usuarios con permisos segmentados.
Implementar un sistema de autenticación con roles diferenciados (administrador y usuario).
Métrica: Se considerará cumplido cuando el 100% de los usuarios registrados en el sistema puedan iniciar sesión bajo el rol correspondiente, y se verifique que los permisos funcionan correctamente según su perfil.
Establecer un panel de administración para asignar permisos por área o cargo.
Métrica: Al finalizar la cuarta semana del desarrollo, el administrador deberá poder crear, editar y asignar permisos de visualización para al menos tres categorías distintas de usuarios.
Incorporar filtros dinámicos en los reportes según criterios como fecha, categoría o área.
Métrica: El sistema permitirá aplicar al menos tres tipos de filtros por cada reporte cargado, y se verificará que estos funcionen correctamente en la visualización final.
Habilitar funciones de exportación de reportes en formatos PDF y Excel (para reportes compatibles).
Métrica: Al cierre del desarrollo, los usuarios deberán poder exportar al menos un reporte en ambos formatos sin pérdida de información visual o estructural.
Garantizar el diseño responsivo del sistema para su correcta visualización en dispositivos móviles.
Métrica: Se considerará cumplido cuando el sistema sea funcional en al menos tres tipos de dispositivos móviles (teléfono, tablet, notebook), con adaptabilidad confirmada mediante pruebas de interfaz.
Alcances y limitaciones del proyecto
Alcances
El proyecto contempla el diseño e implementación de una plataforma web funcional orientada a la gestión eficiente y centralizada de reportes automatizados. Las principales funcionalidades que se abordarán en esta implementación son las siguientes:

Inicio de sesión con roles diferenciados, permitiendo separar el acceso entre usuarios administradores y usuarios estándar, asegurando la segmentación y privacidad de la información.
Panel de administración, que permitirá a los usuarios con perfil de administrador registrar y gestionar visualizaciones generadas en Power BI Report Server, así como asignar permisos personalizados de acceso según el cargo o área del usuario.
Visualización de reportes según permisos definidos, permitiendo que cada usuario acceda únicamente a los reportes que le han sido habilitados, integrando la autenticación y control de acceso con la gestión de roles en Django.
Aplicación de filtros dinámicos (por fecha, año, categoría u otros criterios), además de ofrecer opciones de descarga/exportación de los reportes en formatos como PDF y Excel (para reportes compatibles).
Diseño responsivo y multiplataforma, asegurando el acceso y la correcta visualización del sistema desde distintos dispositivos.

Limitaciones

La plataforma no incluirá edición directa de dashboards, ya que estos se gestionarán y actualizarán exclusivamente desde Power BI Report Server. El sistema solo permitirá la visualización y administración de accesos a los reportes ya publicados.
El sistema requerirá conexión a internet o a la red interna de la organización para acceder a los reportes y funcionalidades de la plataforma, dependiendo de la configuración de Power BI Report Server.
La autenticación estará limitada a credenciales básicas (usuario/contraseña) gestionadas por el sistema Django, sin integración con servicios corporativos como LDAP o Azure Active Directory en esta fase inicial.
La exportación a PDF y Excel estará disponible solo para reportes compatibles, dependiendo de las capacidades de Power BI Report Server y el tipo de reporte publicado.


















METODOLOGÍA





















METODOLOGÍA DE DESARROLLO
Para el desarrollo del presente proyecto se adoptó una metodología ágil de tipo incremental, basada en la entrega continua de funcionalidades en ciclos cortos (sprints). Esta estrategia permitió validar avances de forma temprana, incorporar retroalimentación del equipo supervisor y mitigar riesgos técnicos o de diseño durante las distintas etapas de implementación.
Las fases del proyecto se estructuraron en:
Planificación: Definición de requerimientos, alcance, objetivos y cronograma de trabajo.
Desarrollo backend: Implementación de la lógica de negocio, gestión de usuarios, roles y permisos utilizando Django y la integración con la base de datos SQL Server.
Desarrollo frontend: Construcción de la interfaz de usuario, paneles de administración y visualización de reportes, asegurando un diseño responsivo y accesible.
Integración con herramientas externas: Conexión y consumo de reportes desde Power BI Report Server, asegurando la correcta autenticación y segmentación de accesos.
Validación funcional: Pruebas de usabilidad, seguridad y funcionamiento en distintos escenarios y dispositivos, incorporando mejoras según la retroalimentación recibida.
Cierre: Documentación, capacitación a usuarios clave y entrega final del sistema.

Esta metodología permitió una evolución flexible del sistema, adaptándose a los cambios y necesidades detectadas durante el desarrollo, y asegurando la calidad y pertinencia de la solución entregada.
Materiales 
Para el desarrollo del sistema se utilizarán los siguientes recursos:
Equipos de desarrollo: Computador personal con sistema operativo Windows, equipado para el desarrollo y pruebas de aplicaciones web.
Conexión a internet y/o red interna: Para pruebas, acceso a Power BI Report Server y gestión de reportes.
Instancia de Power BI Report Server: Para la publicación y visualización centralizada de reportes empresariales.
Herramientas de desarrollo: Visual Studio Code como editor principal, navegador web moderno para pruebas de interfaz y usabilidad, y herramientas de diseño gráfico para la elaboración de prototipos y recursos visuales.
Base de datos SQL Server: Para el almacenamiento de usuarios, roles, permisos y metadatos del sistema.
Entorno de desarrollo Django: Para la implementación del backend, lógica de negocio y gestión de usuarios y roles.
Método
Se seguirá un enfoque incremental basado en entregables funcionales, con pruebas al finalizar cada sprint. Las fases serán:

Levantamiento de requerimientos funcionales: Identificación y documentación de las necesidades del usuario, los flujos de información y los objetivos del sistema.
Diseño del flujo del sistema: Elaboración de diagramas de arquitectura, modelado de datos y definición de la estructura de roles y permisos.
Implementación del backend utilizando Django: Desarrollo de la lógica de negocio, gestión de usuarios, roles y permisos, y conexión con la base de datos SQL Server.
Implementación del frontend y panel de administración: Construcción de la interfaz de usuario y los paneles de gestión, asegurando compatibilidad y usabilidad en distintos dispositivos.
Integración con visualizaciones generadas en Power BI Report Server: Consumo y visualización de reportes empresariales, asegurando el control de acceso y la segmentación por roles.
Pruebas funcionales, de seguridad y usabilidad: Validación del correcto funcionamiento del sistema, pruebas de acceso, visualización y experiencia de usuario.
Entrega del sistema final y documentación: Preparación de manuales de usuario y administrador, capacitación y traspaso del sistema a la organización.
Herramientas
Lenguaje de programación: Python.
Framework backend: Django (gestión de usuarios, roles, lógica de negocio y panel de administración).
Framework frontend: Django Templates y Bootstrap (interfaz web moderna y responsiva).
Base de datos: SQL Server (almacenamiento de usuarios, roles, permisos y metadatos del sistema).
Visualización: Power BI Report Server (publicación y visualización centralizada de reportes .pbix).
Exportación de reportes: Funcionalidad nativa de Power BI Report Server para exportar reportes compatibles en PDF y Excel.
Control de versiones: Git (repositorio en GitHub).
Diseño de prototipos: Canva o Figma (para wireframes y prototipos de interfaz).
Descripción general de la propuesta de solución
Propuesta de solución
El sistema propuesto permitirá a un administrador registrar y gestionar reportes publicados en Power BI Report Server, asignar permisos de acceso a usuarios según su área o cargo, y garantizar que cada usuario pueda visualizar únicamente los reportes habilitados para su perfil. La plataforma contará con una interfaz web moderna y responsiva, que incluirá filtros dinámicos por año, área u otros criterios relevantes, así como funcionalidades de descarga de reportes (para formatos compatibles), notificaciones personalizadas y una experiencia de usuario adaptada a distintos dispositivos.
La solución centraliza la administración de reportes, automatiza el control de accesos y facilita la consulta de información estratégica, contribuyendo a la eficiencia operativa y a la seguridad de los datos dentro de la organización.
Flujo del proceso
El administrador inicia sesión en la plataforma y registra el enlace o referencia del reporte publicado en Power BI Report Server.
Asigna permisos de acceso a los reportes, segmentando por usuario, área o cargo, mediante el panel de administración.
El usuario inicia sesión en la plataforma y visualiza únicamente los reportes que le han sido habilitados según su perfil y permisos asignados.
El usuario puede aplicar filtros dinámicos (por año, área u otros criterios) y, si el reporte lo permite, descargarlo en formato PDF o Excel.
El sistema registra las visualizaciones y accesos realizados por cada usuario, permitiendo la trazabilidad y el monitoreo de la consulta de reportes.

Propuesta de controles
Factores de calidad 
Seguridad de acceso por roles:
El sistema garantiza que cada usuario acceda únicamente a los reportes autorizados para su perfil, mediante un control robusto de roles y permisos gestionados desde la plataforma.
Visualización clara y rápida:
La integración con Power BI Report Server y el diseño responsivo de la interfaz aseguran una visualización de reportes ágil, intuitiva y adaptada a distintos dispositivos.
Compatibilidad multiplataforma:
La plataforma es accesible desde navegadores modernos en computadoras, tablets y teléfonos móviles, permitiendo la consulta de reportes desde cualquier lugar y dispositivo.
Correcto funcionamiento de los filtros y exportación:
El sistema permite aplicar filtros dinámicos sobre los reportes y, para aquellos compatibles, exportar la información en formatos PDF y Excel, asegurando la integridad y claridad de los datos exportados.

Actividades de calidad
Pruebas unitarias y funcionales por módulo:
Se realizan pruebas sistemáticas sobre cada componente del sistema (gestión de usuarios, roles, reportes, etc.) para asegurar su correcto funcionamiento de manera aislada y en conjunto.
Validación de accesos por rol:
Se verifica que los usuarios solo puedan acceder a los reportes y funcionalidades permitidas según su perfil, garantizando la seguridad y segmentación de la información.
Revisión de carga y visibilidad de reportes:
Se comprueba que los reportes registrados sean correctamente visibles y accesibles para los usuarios autorizados, y que la visualización sea clara y eficiente.

Actividades de calidad en desarrollo
Validaciones automáticas en backend:
El sistema implementa validaciones automáticas para asegurar la integridad de los datos, la correcta asignación de permisos y la prevención de errores comunes durante la operación.
Interfaz con retroalimentación visual:
La plataforma proporciona feedback inmediato al usuario ante acciones como inicio de sesión, asignación de roles, carga de reportes o aplicación de filtros, mejorando la experiencia y usabilidad.
Documentación del código y de la arquitectura:
Se mantiene documentación actualizada del código fuente, la arquitectura del sistema y los flujos principales, facilitando el mantenimiento, la escalabilidad y la transferencia de conocimiento.

Análisis de probabilidades de riesgo y nivel de impacto
Evaluación y pesaje del riesgo




Tabla 1.
Análisis de probabilidades de riesgo y nivel de impacto.
Fuente: Elaboración propia.
Plan de riesgos y estrategias de mitigación

Para minimizar el impacto de los riesgos identificados en el desarrollo y operación del sistema, se implementarán las siguientes estrategias de mitigación:
Realizar pruebas con distintos perfiles de usuario:
Se llevarán a cabo pruebas funcionales y de acceso utilizando cuentas con diferentes roles y permisos, asegurando que la segmentación y la seguridad funcionen correctamente en todos los escenarios.
Implementar validación automática de enlaces Power BI al registrarlos:
El sistema verificará que los enlaces o referencias a reportes de Power BI Report Server sean válidos y accesibles antes de permitir su registro, reduciendo la probabilidad de errores en la visualización.
Utilizar diseño responsivo y realizar pruebas en distintos navegadores y dispositivos:
Se adoptará un enfoque de diseño responsivo y se realizarán pruebas de compatibilidad en los principales navegadores y dispositivos móviles, garantizando una experiencia de usuario consistente y sin errores de visualización.
Guardar logs de errores para depuración rápida:
El sistema almacenará registros detallados de errores y eventos relevantes, facilitando la detección, análisis y resolución de problemas técnicos de manera oportuna.Estas acciones permitirán anticipar y mitigar los principales riesgos, asegurando la calidad, seguridad y continuidad operativa del sistema.

Cronograma del proyecto 

Duración estimada: 8 semanas, desde el diseño hasta la entrega.
El cronograma se divide en etapas:



Gráfico 1.
Cronograma del proyecto.

Fuente: Elaboración propia.
Prototipo
El prototipo inicial desarrollado para el sistema incluye las siguientes funcionalidades clave:

Página de inicio de sesión diferenciada por rol:
Permite el acceso seguro de usuarios y administradores, mostrando opciones y paneles personalizados según el perfil de cada usuario.
Panel de administración:
Ofrece la posibilidad de registrar y gestionar reportes publicados en Power BI Report Server, así como asignar permisos de acceso a usuarios según área o cargo, facilitando la administración centralizada de la información.
Panel de usuario:
Presenta la visualización de reportes habilitados para cada usuario, con la posibilidad de aplicar filtros dinámicos y, para reportes compatibles, exportar la información en formatos PDF o Excel.
Integración visual básica:
El prototipo cuenta con una interfaz moderna y responsiva que simula la experiencia final del sistema, permitiendo validar flujos de navegación, usabilidad y la correcta segmentación de accesos antes de la implementación definitiva.
.




















DESARROLLO DEL PROYECTO






















DESARROLLO DEL PROYECTO
Gestión de proyecto 
El desarrollo del sistema de gestión automatizada de reportes empresariales se organizó bajo un enfoque metodológico ágil de tipo incremental, con el objetivo de construir un sistema funcional mínimo viable (MVP) en un plazo de ocho semanas. Esta estrategia permitió mantener la flexibilidad necesaria para responder ante cambios, priorizar funcionalidades clave y asegurar avances continuos en la implementación técnica.
El proyecto se dividió en etapas semanales, donde cada una correspondía a una entrega funcional: desde el diseño inicial de la arquitectura del sistema y la base de datos, hasta la integración con Power BI Report Server, la creación de vistas y endpoints para la gestión de usuarios, roles y reportes, y el diseño de las interfaces de usuario y administrador. Cada etapa fue abordada con objetivos concretos, permitiendo validar avances de forma constante y ajustar prioridades según la retroalimentación recibida.
Las herramientas empleadas durante la ejecución fueron seleccionadas por su compatibilidad y robustez en el entorno de desarrollo propuesto:
Visual Studio Code como entorno de desarrollo principal.
Django y SQL Server como base tecnológica del backend y almacenamiento de datos.
SQL Server Management Studio (SSMS) para la administración de la base de datos.
PlantUML y draw.io para la creación de diagramas técnicos y de arquitectura.
Bootstrap y Django Templates para el desarrollo de la interfaz gráfica y pruebas del MVP.
Power BI Report Server para la publicación y visualización centralizada de reportes analíticos.
La planificación y control del proyecto se realizaron utilizando listas de tareas y sprints semanales autoorganizados. No se utilizó un software de gestión formal como Trello o Jira, dado que el equipo de trabajo fue individual. Sin embargo, se mantuvo un registro claro de los avances por semana, lo que permitió cumplir con el cronograma establecido.
A continuación, se presenta el cronograma general del proyecto representado en una carta Gantt, donde se visualizan las actividades desarrolladas durante las ocho semanas del periodo asignado.
Gráfico 1.
Cronograma del proyecto.
Fuente: Elaboración propia.
Diseño de los componentes funcionales de la propuesta solución 
La propuesta de solución se estructuró considerando una arquitectura modular y escalable, que integra componentes frontend, backend, base de datos y sistemas externos de visualización (Power BI Report Server). Cada componente funcional fue diseñado para interactuar de forma segura y eficiente, optimizando el acceso y la gestión de reportes empresariales.
Frontend: Desarrollado con Django Templates y Bootstrap, proporciona una interfaz web moderna, responsiva y fácil de usar, permitiendo a los usuarios y administradores interactuar con el sistema desde cualquier dispositivo.
Backend: Implementado en Django, gestiona la lógica de negocio, la autenticación, la asignación de roles y permisos, y la integración con la base de datos SQL Server.
Base de datos: Utiliza SQL Server para almacenar de manera segura la información de usuarios, roles, permisos y metadatos de los reportes.
Sistema de visualización externa: Power BI Report Server se encarga de la publicación y visualización centralizada de los reportes .pbix, integrándose con la plataforma para ofrecer acceso seguro y segmentado según los permisos definidos en el sistema.
Seguridad y control de acceso: El sistema implementa controles robustos de autenticación y autorización, asegurando que cada usuario acceda únicamente a los reportes y funcionalidades permitidas según su perfil.
Arquitectura General del Sistema
El sistema sigue una arquitectura en capas que define claramente los roles de cada módulo:
Usuarios y Administradores interactúan con el Frontend Django.
El Frontend Django muestra paneles, filtros, reportes y exportaciones, y comunica con el Backend Django.
El Backend Django gestiona autenticación, permisos, CRUD y logs, y se conecta a la Base de Datos SQL Server.
Los reportes se visualizan en Power BI Report Server (PBIRS), al cual se redirige desde el frontend solo a los reportes permitidos.
Toda la gestión de usuarios, roles y permisos se hace en Django, y la base de datos almacena usuarios, reportes, roles, permisos y logs.












Figura 2.
Diagrama arquitectura General del Sistema.

Fuente: Elaboración propia.
Modelo de Datos
El modelo de datos fue diseñado bajo principios de normalización y eficiencia relacional, asegurando integridad, escalabilidad y facilidad de mantenimiento. Las principales entidades del sistema son:
Usuario: Registra la información de los usuarios del sistema, incluyendo nombre, correo electrónico, contraseña cifrada, fecha de registro, estado de actividad, último acceso y la relación con su rol correspondiente. Permite gestionar la autenticación y la asignación de permisos de manera centralizada.
Rol: Define los distintos tipos de acceso dentro del sistema, como administrador y usuario estándar. Cada usuario está asociado a un único rol, lo que facilita la gestión de permisos y la administración de privilegios.
Reporte: Almacena información relevante sobre los reportes disponibles, incluyendo título, descripción, URL de acceso en Power BI Report Server, área temática, fecha de subida, usuario que lo subió y estado. Esta entidad permite organizar y categorizar los reportes para su fácil acceso y gestión.
Permiso: Controla el acceso de los roles a los distintos reportes. Relaciona roles, reportes y tipos de permiso (por ejemplo, visualización, edición), permitiendo una administración granular de los privilegios sobre los reportes.
Log de Acceso: Registra el historial de accesos de los usuarios a los reportes, almacenando información como el usuario, el reporte accedido y la fecha/hora de acceso. Esta entidad es fundamental para auditoría, trazabilidad y análisis de uso del sistema.








Figura 3
Diagrama modelo de datos

Fuente: elaborado con cursor y Plantuml.
Casos de Uso
Se definieron los siguientes casos de uso para cubrir las funcionalidades principales:
Inicio de sesión con autenticación segura.
Visualización de reportes permitidos por el rol.
Aplicación de filtros por fecha, área o categoría.
Exportación de reportes en formatos PDF o Excel.
Administración de usuarios, roles y permisos.

Figura 4.
Diagrama caso de uso.

Fuente: Elaboración propia.
Flujo de MVP
Se diagramó el flujo de navegación mínimo viable (MVP), considerando:
Inicio de sesión:
El usuario (humano) ingresa sus credenciales en la plataforma Django.
El sistema valida las credenciales contra la base de datos SQL Server.
Si las credenciales no son válidas, se muestra un mensaje de error.
Si son válidas, el sistema determina el rol del usuario (usuario o administrador).
Panel de usuario:
Si es usuario estándar, se muestra el panel de usuario.
El usuario puede visualizar los reportes permitidos (redirigido a PBIRS).
Puede aplicar filtros (si el reporte lo permite en PBIRS).
Puede exportar el reporte (si PBIRS lo permite).
Cada acceso a reporte queda registrado en la tabla de logs de acceso.
Panel de administrador:
Si es administrador, se muestra el panel de administración.
El administrador puede:
Registrar (cargar) un nuevo reporte en el sistema (no en PBIRS, solo en Django).
Asignar roles/permisos a los reportes.
Gestionar usuarios (crear, editar, desactivar).
Las actividades administrativas relevantes quedan registradas en logs.










Figura 5.
Diagrama BPMN.

Fuente: elaborado con cursor y Plantuml.
Mapa de Navegación de Pantallas

Se diseñó un mapa que muestra la navegación entre pantallas principales del sistema:
Login → Panel Usuario → Visualización de Reportes
Login → Panel Administrador → Gestión de Usuarios/Reportes






Figura 6 
Mapa de navegación

Fuente: Elaboración propia 
Matriz de Trazabilidad de Requerimientos
A continuación se presenta la matriz de trazabilidad, la cual vincula cada requerimiento funcional del sistema con los artefactos de análisis y diseño desarrollados, facilitando el seguimiento y validación durante todo el ciclo de vida del proyecto.
Tabla 2
Matriz de Trazabilidad de Requerimientos

Fuente: Elaboración propia

CONCLUCIONES
INTRODUCCIÓN 
El desarrollo del sistema de gestión automatizada de reportes para la toma de decisiones empresariales tuvo como propósito principal optimizar y asegurar el acceso a información relevante mediante la integración de tecnologías robustas como Django, SQL Server y Power BI Report Server. A lo largo del proyecto, se abordaron diversos desafíos técnicos y organizacionales, adaptando la solución a las restricciones y necesidades reales de la organización. A continuación, se presenta el análisis del cumplimiento de los objetivos específicos y general definidos al inicio del proyecto.
OBJETIVOS ESPECÍFICOS
Diseñar e implementar una plataforma web segura para la gestión de usuarios, roles y permisos.
Este objetivo fue plenamente alcanzado. Se desarrolló una plataforma basada en Django que permite la gestión avanzada de usuarios y roles, con autenticación segura, validaciones personalizadas y control de acceso granular. Solo los administradores pueden gestionar usuarios y roles, lo que garantiza la integridad y seguridad del sistema.
 Integrar la visualización de reportes empresariales utilizando Power BI Report Server.
El objetivo se logró satisfactoriamente. Se instaló y configuró Power BI Report Server, y se implementó la visualización de reportes a través de redirecciones seguras desde la plataforma web, asegurando que los usuarios solo accedan a los reportes permitidos según su rol y permisos asignados.
 Automatizar y registrar el acceso a los reportes, permitiendo la trazabilidad y auditoría de uso.
Este objetivo fue cumplido. Se diseñó un modelo de datos que incluye una entidad de logs de acceso, donde se registra cada visualización de reporte por parte de los usuarios. Esto permite realizar auditorías y análisis de uso, contribuyendo a la transparencia y seguridad del sistema.
 Facilitar la administración y asignación de permisos sobre los reportes publicados.
El sistema permite a los administradores registrar manualmente los reportes, asignar permisos a roles y usuarios, y gestionar el acceso de manera flexible y eficiente. Aunque la automatización total de la carga de reportes desde PBIRS no fue posible por limitaciones de la API, la solución implementada cumple con los requerimientos funcionales y de seguridad.
OBJETIVO GENERAL
Desarrollar un sistema integral para la gestión y visualización segura de reportes empresariales, que permita la administración eficiente de usuarios, roles y permisos, y garantice la trazabilidad de accesos.
El objetivo general fue alcanzado en su totalidad. El sistema desarrollado integra de manera efectiva la gestión de usuarios y permisos, la visualización segura de reportes mediante Power BI Report Server, y el registro detallado de accesos. La solución es robusta, escalable y adaptable a futuras necesidades, evidenciando el cumplimiento de los requerimientos planteados y aportando valor a la toma de decisiones empresariales.



RECOMENDACIONES
INTRODUCCIÓN 
Si bien el sistema desarrollado cumple con los objetivos propuestos y responde a las necesidades actuales de la organización, siempre existen oportunidades de mejora y expansión. A continuación, se presentan recomendaciones específicas para cada uno de los objetivos abordados, con el fin de orientar futuras investigaciones o desarrollos que busquen perfeccionar o ampliar la solución implementada.
OBJETIVO 1: Plataforma web segura para la gestión de usuarios, roles y permisos
RECOMENDACIÓN:
Se sugiere explorar la integración de autenticación multifactor (MFA) y la adopción de protocolos de autenticación federada (como SAML o OAuth2) para fortalecer aún más la seguridad. Además, sería beneficioso implementar auditorías automáticas y alertas ante actividades sospechosas, así como mejorar la experiencia de usuario en la gestión de roles y permisos mediante interfaces más intuitivas.
OBJETIVO 2: Integración de la visualización de reportes empresariales utilizando Power BI Report Server
RECOMENDACIÓN:
Para futuras versiones, se recomienda investigar la posibilidad de una integración más profunda con Power BI Report Server, por ejemplo, mediante el uso de APIs avanzadas o conectores personalizados que permitan automatizar la carga y actualización de reportes desde la plataforma web. También sería valioso evaluar la integración con otros sistemas de visualización o BI para ampliar la flexibilidad y cobertura del sistema.
OBJETIVO 3: Automatización y registro del acceso a los reportes
RECOMENDACIÓN:
Se aconseja enriquecer el módulo de logs de acceso con funcionalidades de análisis avanzado, como reportes automáticos de uso, detección de patrones anómalos y visualización gráfica de la actividad. Además, podría considerarse la integración con herramientas de SIEM (Security Information and Event Management) para una gestión centralizada de la seguridad y auditoría.
OBJETIVO 4: Administración y asignación de permisos sobre los reportes publicados
RECOMENDACIÓN:
Se recomienda continuar explorando alternativas para automatizar la gestión de permisos y la carga de reportes, superando las limitaciones actuales de la API de Power BI Report Server. El desarrollo de scripts personalizados o la colaboración con el área de TI para habilitar integraciones más profundas podría facilitar la administración y reducir la carga operativa de los administradores.
Estas recomendaciones buscan no solo mantener la robustez y seguridad del sistema, sino también anticipar las necesidades futuras de la organización, promoviendo la innovación y la mejora continua en la gestión de reportes empresariales.
REFERENCIAS
Django Software Foundation. (2024). Django documentation. Recuperado de 
Microsoft. (2024a). Power BI Report Server documentation. Recuperado de 
Microsoft. (2024b). SQL Server documentation. Recuperado de 
Bootstrap. (2024). Bootstrap documentation. Recuperado de 
Python Software Foundation. (2024). Python documentation. Recuperado de 
PlantUML. (2024). PlantUML documentation. Recuperado de 
Instituto Nacional de Ciberseguridad de España. (2023). Guía de buenas prácticas en la gestión de usuarios y contraseñas. Recuperado de 
OpenAI. (2024). ChatGPT (GPT-4), modelo de lenguaje grande. Recuperado el [19 de mayo de 2025] de 
Sommerville, I. (2016). Ingeniería de software (10a ed.). Pearson Educación.
Pressman, R. S., & Maxim, B. R. (2021). Ingeniería de software: Un enfoque práctico (9a ed.). McGraw-Hill.
Rodríguez, F. (2019). Gestión de proyectos con metodologías ágiles: Scrum y Kanban. Alfaomega.
Project Management Institute. (2017). Guía del PMBOK®: Guía de los fundamentos para la dirección de proyectos (6a ed.). Project Management Institute.
ISO/IEC. (2018). ISO/IEC 27001:2013 – Information technology — Security techniques — Information security management systems — Requirements. International Organization for Standardization.

