# 📱 App de Comunicación para Personas con Autismo

## 🧩 Introducción

En este proyecto, voy a desarrollar una aplicación móvil diseñada para mejorar la comunicación de personas con autismo a través de una interfaz intuitiva basada en pictogramas. Mi objetivo es facilitar la interacción social y la expresión verbal de los usuarios de la aplicación, proporcionando una herramienta personalizable para entornos escolares.

---

## 🎯 Objetivos

- 🏗 **Crear una interfaz accesible** basada en pictogramas con texto asociado.
- 🎤 **Mejorar la comunicación** y la expresión verbal de los usuarios.
- 📊 **Proporcionar herramientas para maestros**, permitiéndoles gestionar contenido y monitorear el progreso de los estudiantes.

---

## 📌 Características Principales

✅ Interfaz sencilla e intuitiva basada en pictogramas.<br>
✅ Base de datos sincronizada para almacenar progreso y personalización.<br>
✅ Módulo administrativo exclusivo para maestros.<br>
✅ Informes y estadísticas de progreso.

---

## 📊 Tecnologías Utilizadas

| Tecnología | Uso |
|------------|-----|
| ![Android Studio](https://img.shields.io/badge/Android-3DDC84?style=flat&logo=android&logoColor=white) | Desarrollo móvil |
| ![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=flat&logo=kotlin&logoColor=white) | Lenguaje principal |
| ![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white) | Base de datos |
| ![Arasaac](arasaac2.png) | Creación Pictogramas |
| ![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat&logo=figma&logoColor=white) | Desarrollo Interfaz |

---

## 🔄 Flujo de la Aplicación

```mermaid
flowchart TD
    A[Inicio] --> B[Iniciar Sesión]
    B --> C{Seleccionar tipo de usuario}
    C -->|Profesor| D[Ingresar nombre y contraseña]
    C -->|Alumno| E[Ingresar nombre y contraseña]
    D --> F[Gestión de pictogramas]
    F --> G[Añadir pictogramas]
    F --> H[Crear pictogramas]
    F --> I[Eliminar pictogramas de alumnos]
    F --> J[Acceder a palabras aprendidas]
    E --> K[Interacción con pictogramas]
    K --> L[Reproducir sonido al pulsar]
    K --> M[Solicitar más palabras al profesor]
```

---

## 📆 Planificación (Diagrama Gantt)

```mermaid
gantt
    title Desarrollo de la App
    dateFormat  YYYY-MM-DD
    section Investigación
    Estudio de necesidades :done, 02-01, 02-15
    Consulta con expertos  :active, 02-16, 02-28
    section Diseño y Desarrollo
    Creación de interfaz   :active, 03-01, 03-15
    Implementación base de datos :active, 03-16, 04-01
    Desarrollo de funcionalidades :active, 04-02, 05-01
    Pruebas de usuario     : 05-02, 05-15
    Documentación         : 05-16, 05-30
```

---
## 🐙 Planificación (Diagrama Git)

```mermaid
gitGraph
    commit id: "Configuración inicial"
    branch dev
    commit id: "Desarrollo de Interfaz"
    checkout main
    commit id: "Commit en main"
    merge dev
    commit id: "Merge de dev a main"
    branch bugfix
    commit id: "Error RecicleView"
    checkout dev
    commit id: "Implementación BBDD" tag: "v1.0.0"
    merge bugfix
    checkout dev
    commit id: "Desarrollar Funcionalidades" tag: "v1.2.0"
    checkout main
    merge dev
    commit id: "Merge de dev a main"
    commit id: "Versión 2.0.0" tag: "v2.0.0"


```
---
# 📊 Gráficos de Estudio realizado
```mermaid
pie showData  
    title Personas con TEA en España  
    "Castilla y León": 27  
    "País Vasco": 25  
    "Madrid": 9  
    "Andalucía": 9  
    "Galicia": 9  
    "Cataluña": 8  
```

```mermaid
pie showData  
    title Servicios utilizados personas con TEA  
    "Información, orientación y asesoramiento": 83.69  
    "Ocio y tiempo libre": 54  
    "Diagnóstico y evaluación": 51.44  
    "Intervenciones especializadas y/o apoyo en contextos naturales": 48.42  
    "Apoyo de educación y servicios de apoyos educativos": 47  
    "Apoyo psicológico y emocional": 44  
    "Apoyos especializados para la promoción de la salud": 42.7  

```

### Realidad, mitos y retos del autismo
Melisa Tuya, autora del libro ‘Tener un hijo con autismo’ y la psicóloga especialista en personas con 
Asperger, Diana Bohórquez analizan las realidades y los retos a los que se enfrentan diariamente las 
familias y personas con Trastorno de Espectro Autista (TEA). Como madre de un niño con autismo, 
Melisa Tuya insiste en la necesidad de acabar con los falsos mitos sobre este trastorno. “El autismo no es 
una enfermedad. Es una característica de la persona. Tenemos que trabajar para que las personas con 
autismo tengan un potencial máximo y sean felices.”

<br>

[![Video entrevista a Melisa](https://i.ytimg.com/vi/0JcUmM63rPI/hq720.jpg?sqp=-oaymwEXCNAFEJQDSFryq4qpAwkIARUAAIhCGAE=&rs=AOn4CLDRnQd_MMJBUwS_DaMHbOE5qcilYA)](https://www.youtube.com/watch?v=0JcUmM63rPI)

<p align="right">
    <a href="https://www.youtube.com/watch?v=0JcUmM63rPI" title="Aprendemos Juntos 2030">Video entrevista a Melisa</a>
</p>


##### Fuente
Gestión. (2019, 8 julio). *El estudio sociodemográfico desarrollado por Autismo España cuenta ya con 2.116 registros de personas con TEA*. Autismo España. [https://autismo.org.es/actualidad/noticias/el-estudio-sociodemografico-desarrollado-por-autismo-espana-cuenta-ya-con-2116/?utm_source=chatgpt.com](https://autismo.org.es/actualidad/noticias/el-estudio-sociodemografico-desarrollado-por-autismo-espana-cuenta-ya-con-2116/?utm_source=chatgpt.com)



---
## 📊 Diagrama de Entidad-Relación Provisional

```mermaid
erDiagram
    USUARIO {
        string id_usuario
        string nombre
        string rol
    }
    PICTOGRAMA {
        string id_pictograma
        string nombre
        string categoria
    }
    PALABRA {
        string id_palabra
        string texto
    }
    INTERACCION {
        string id_interaccion
        string id_usuario
        string id_pictograma
        datetime fecha_hora
    }
    SOLICITUD {
        string id_solicitud
        string id_usuario
        string id_palabra
        datetime fecha_hora
    }
    USUARIO ||--o{ INTERACCION : "realiza"
    USUARIO ||--o{ SOLICITUD : "solicita"
    INTERACCION }o--|| PICTOGRAMA : "incluye"
    SOLICITUD }o--|| PALABRA : "contiene"
```

---

## 📜 Diagrama de Secuencia Provisional

```mermaid
sequenceDiagram
    participant Usuario
    participant Sistema
    participant Profesor
    Usuario->>Sistema: Iniciar sesión
    Sistema-->>Usuario: Solicitar credenciales
    Usuario->>Sistema: Enviar credenciales
    Sistema-->>Usuario: Confirmar acceso
    Usuario->>Sistema: Seleccionar pictograma
    Sistema-->>Usuario: Mostrar texto asociado
    Usuario->>Sistema: Reproducir audio
    Usuario->>Profesor: Solicitar nueva palabra
    Profesor->>Sistema: Agregar nueva palabra
    Sistema-->>Usuario: Confirmación de palabra agregada
```

---

## 📜 Diagrama de Requerimientos

```mermaid
requirementDiagram
    requirement R1 {
        id: 1
        text: "La aplicación debe permitir a los usuarios iniciar sesión."
    }
    requirement R2 {
        id: 2
        text: "Los profesores deben poder añadir y gestionar pictogramas."
    }
    requirement R3 {
        id: 3
        text: "Los alumnos deben poder interactuar con los pictogramas."
    }
    requirement R4 {
        id: 4
        text: "El sistema debe registrar las interacciones de los alumnos."
    }
    requirement R5 {
        id: 5
        text: "Los alumnos pueden solicitar nuevas palabras a los profesores."
    }
```

---
## 📜 Diagrama de Journey

```mermaid
journey
    title Uso de la Aplicación
    section Inicio
        Abrir la aplicación: 5: Usuario
        Iniciar sesión: 4: Usuario
    section Interacción
        Seleccionar pictograma: 5: Usuario
        Escuchar el audio del pictograma: 4: Sistema
        Solicitar nueva palabra: 3: Usuario
    section Administración (Profesor)
        Agregar pictogramas: 5: Profesor
        Revisar progreso de alumnos: 4: Profesor
```

---

## 🤝 Contribuciones

¡Las contribuciones son bienvenidas! Para colaborar:

1. **Escribe tu propuesta** con aquello que has pensado.
2. **Envíalo por correo** al <sehoul@correo.com>.
3. **Nos pondremos en contacto** contigo si nos interesa tu propuesta.

---
