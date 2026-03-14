# [cite_start]ARQUITECTURA ATM PARA LA GESTIÓN DEL SERVICIO AL CLIENTE - BANCO FIE [cite: 5]

[cite_start]Este proyecto integrador desarrolla un sistema de Cajero Automático (ATM) enfocado en la inclusión financiera y la automatización de transacciones para el Banco FIE en Bolivia[cite: 16, 82]. [cite_start]El sistema busca reducir la saturación en ventanillas y ofrecer servicios seguros las 24 horas, especialmente en zonas con conectividad limitada[cite: 25, 60].

## [cite_start]👥 Equipo de desarrollo [cite: 6]
* [cite_start]**Juan Carlos Chavez Machaca** [cite: 7]
* [cite_start]**Kevin Jiménez Jheferson Quisbert** [cite: 8]
* [cite_start]**Erick Ivan Luna Tarqui** [cite: 9]
* [cite_start]**Fernando Castro Vargas** [cite: 10]
* [cite_start]**Juan Antonio Ramos Rojas** [cite: 11]

## [cite_start]🎯 Objetivo del Proyecto [cite: 80]
[cite_start]Desarrollar un sistema de cajero automático (ATM) para gestionar de forma eficiente y segura las transacciones bancarias del Banco FIE, empleando hardware y software con especial énfasis en la usabilidad y la inclusión financiera[cite: 28, 82].

## [cite_start]🛠️ Herramientas y Stack Tecnológico [cite: 93]

### [cite_start]**Presentación (Frontend)** [cite: 97]
* [cite_start]**HTML5 & CSS3:** Diseño de interfaces bilingües (Español/Inglés)[cite: 88, 119].
* [cite_start]**jQuery:** Implementación de una **Single Page Application (SPA)** para transiciones fluidas[cite: 108, 109].
* [cite_start]**UX Inclusiva:** Diseño orientado a usuarios con baja experiencia digital y mensajes descriptivos[cite: 122, 124].

### [cite_start]**Backend (Lógica de Negocio)** [cite: 97]
* [cite_start]**PHP:** Procesamiento de la lógica bancaria bajo el patrón **MVC**[cite: 96, 97].
* [cite_start]**API RESTful:** Endpoints seguros con formato JSON y manejo de códigos HTTP[cite: 104, 106].
* [cite_start]**Seguridad Multicapa:** [cite: 99]
    * [cite_start]Autenticación mediante **JWT** con expiración de sesión[cite: 99].
    * [cite_start]Hashing de PINs con `password_hash()` y salting[cite: 99].
    * [cite_start]Protección contra inyección SQL mediante **PDO** con consultas preparadas[cite: 99].
    * [cite_start]Encriptación de datos sensibles con **AES-256-CBC**[cite: 99].

### [cite_start]**Datos y Hardware** [cite: 97, 101]
* [cite_start]**MySQL:** Base de datos para el registro seguro de transacciones y logs de auditoría[cite: 85, 89].
* [cite_start]**Arduino UNO (IoT):** Integración de hardware mediante microcontrolador para el control físico[cite: 102].
* [cite_start]**Periféricos:** Lector RFID EM-18, sensor biométrico GT511 y módulo GSM 900[cite: 103].

## [cite_start]📂 Estructura del Sistema 
```text
APP/
[cite_start]├── api/             # Endpoints RESTful y lógica de servidor 
[cite_start]├── arduino/         # Código fuente para microcontrolador Arduino 
[cite_start]├── config/          # Archivos de configuración del sistema 
[cite_start]├── database/        # Scripts SQL y modelos de datos 
[cite_start]└── public/          # Archivos accesibles desde el navegador 
    ├── assets/      # Recursos estáticos 
    │   ├── css/     # Hojas de estilo 
    │   └── lang/    # Archivos JSON para soporte bilingüe 
    ├── consulta.html
    ├── cuenta.html
    ├── deposito.html
    ├── index.html   # Punto de entrada principal 
    ├── language.html
    ├── menu.html
    ├── movimientos.html
    ├── pin.html
    ├── resultado.html
    └── retiro.html
