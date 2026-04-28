# Memoria del Proyecto: Landing Page INGEMA LAB

## 1. Contexto Inicial
El proyecto consistía en la modernización de la Landing Page de **INGEMA LAB** (Laboratorio de Ingeniería en Medio Ambiente y Riesgo Ambiental SA de CV), evolucionando su diseño hacia una experiencia *Premium* de alta fidelidad, y preparando la plataforma para futuras integraciones.

## 2. Acciones Realizadas

### 2.1. Integración de Identidad y Marca
- Se realizó la extracción del logo corporativo oficial desde el documento `CARTA DE PRESENTACIÓN OLD.pdf` proporcionado por el cliente, empleando un script de extracción PDF basado en `PyMuPDF`.
- El logo fue optimizado y guardado localmente como `logo_ingema.png`.
- Se reemplazó el logotipo tipográfico ("ib") que se encontraba originalmente tanto en el Header (barra de navegación) como en el Footer, posicionando la imagen oficial de forma responsiva.

### 2.2. Diseño "Antigravity"
Se aplicaron los principios de "Antigravity Design" para elevar el nivel estético del sitio:
- **Glassmorphism:** Se implementaron fondos translúcidos con desenfoque (`backdrop-filter`) y bordes sutiles en las tarjetas de servicios y otros contenedores destacados.
- **Micro-interacciones y Motion:** Se añadieron efectos dinámicos de elevación y escala (`transform: translateY() scale()`) y proyecciones de sombras que se activan al hacer *hover*, aportando una sensación de ligereza visual.
- **Ajustes de UI:** Mejoras generales en el renderizado de los componentes clave para alinear la estética al alto estándar de una empresa de consultoría e ingeniería ambiental, manteniendo en todo momento los servicios (Fuentes Fijas, Ambiente Laboral, Calidad del Aire, Consultoría Ambiental) y estructura originales.

### 2.3. Detalles de Marca (Versionado)
- Se integró la firma discreta "**INGEMALAB 2.0**" en la parte inferior del pie de página (footer) para marcar simbólicamente la evolución del proyecto sin romper la formalidad institucional.

### 2.4. Agente de Servicio "LABITO"
- Se estableció la infraestructura para integrar a "LABITO", un Agente de IA concebido específicamente para dar soporte al cliente y operar sobre el contexto de INGEMA LAB.
- Se documentó la parametrización de dicho agente en el archivo `AGENTS.md` bajo el framework correspondiente.
- **Widget Interactivo:** Se implementó el frontend del agente directamente en `index.html` usando JavaScript y CSS puros con diseño *Glassmorphism*. El widget ofrece tres flujos: Tour Rápido, Acceso a Clientes y Sugerencia de Servicios Cruzados. Cuenta con un temporizador de auto-despliegue tras 5 segundos y almacenamiento de sesión (`sessionStorage`) para no resultar intrusivo.
- **Acceso a Clientes:** Se incorporó el enlace en el Navbar simulando el acceso seguro al Portal del Cliente.

### 2.5. Geometría Honeycomb y Corrección de Logotipos
- **Logo Transparente:** Se reemplazaron todas las referencias al logotipo principal por `images/ingemalab_logo_transparent.png`, resolviendo defectos visuales en recortes y adaptando el isotipo dentro de los componentes del sitio.
- **Estructura Hexagonal:** Se implementó el sistema visual Honeycomb exacto para el Hero Banner utilizando 6 hexágonos entrelazados con recortes poligonales por CSS (`clip-path: polygon(50% 0%, 100% 25%, 100% 75%, 50% 100%, 0% 75%, 0% 25%)`).

### 2.6. Auditoría y Optimización Web
- **Revisión de Estilos:** Se auditaron las reglas tipográficas y accesibilidad del proyecto mediante estándares modernos (cambio de elipsis de `...` a `…` y adición de propiedades de renderizado).

## 3. Estado Actual
La landing page (`index.html`) se encuentra completamente funcional y optimizada. El widget de LABITO está integrado, y el diseño visual se mantiene premium y alineado con los manuales técnicos. 

## 4. Regla de Aislamiento Persistente
Este repositorio y su memoria están estrictamente vinculados a **INGEMA LAB**. Ningún dato, asset o lógica de este negocio debe ser cruzado con otras entidades operadas por el usuario (e.g., Farma Medic o Vértice EHS). La persistencia de este contexto se mantiene dentro de este directorio.
