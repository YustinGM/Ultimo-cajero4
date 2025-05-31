Banco Smith - Cajero Virtual (Colombia)
Banco Smith es una aplicación web desarrollada con Spring Boot, que simula el funcionamiento de un cajero automático. El diseño visual está inspirado en la estética del Pacífico colombiano, y su estructura técnica sigue los principios modernos de desarrollo de software empresarial. Este sistema permite a clientes y administradores realizar operaciones bancarias esenciales a través de una interfaz intuitiva y segura.

🛠️ Tecnologías utilizadas
Java 17

Spring Boot (Spring MVC + Spring Data JPA)

Thymeleaf

MySQL (con script SQL incluido)

HTML5, CSS3, Bootstrap 5

FontAwesome

🚀 Funcionalidades destacadas
Registro, gestión y desbloqueo de clientes

Creación de cuentas bancarias de tipo Ahorros o Corriente

Inicio de sesión seguro con número de cuenta y PIN

Operaciones disponibles para el cliente:

Retiros

Consignaciones

Transferencias entre cuentas

Cambio de clave personal

Consulta de movimientos y saldos

Control de acceso basado en roles (cliente y administrador)

Diseño responsive con identidad visual institucional

📁 Estructura del Proyecto
bash
 
BancoSmith/
├── src/
│   ├── main/
│   │   ├── java/com/fortbank/BancoSmith/
│   │   │   ├── controller/         # Controladores de rutas y flujo de vistas
│   │   │   ├── dto/                # Objetos de transferencia de datos (DTOs)
│   │   │   ├── entity/             # Entidades JPA que modelan la base de datos
│   │   │   ├── repository/         # Interfaces de persistencia con Spring Data
│   │   │   └── services/           # Lógica de negocio y reglas del dominio
│   │   └── resources/
│   │       ├── static/styles/      # Archivos de estilos CSS
│   │       └── templates/          # Plantillas Thymeleaf (.html)
│   └── test/                       # Pruebas unitarias e integradas
├── banco_smith.sql                 # Script SQL para creación de base de datos
├── pom.xml                         # Archivo de configuración del proyecto (Maven)
└── README.md                       # Documento de presentación del proyecto
📌 Requisitos previos
Java 17 o superior

Maven 3.6 o posterior

MySQL o XAMPP con phpMyAdmin

⚙️ Instalación y ejecución
Clonar el repositorio:

bash
 
git clone https://github.com/tuusuario/banco-smith.git
cd banco-smith
Importar el archivo banco_smith.sql en phpMyAdmin.

Configurar las credenciales de conexión en application.properties.

Ejecutar el proyecto:

bash

./mvnw spring-boot:run
# O con Maven global
mvn spring-boot:run
Acceder a la aplicación en el navegador:

http://localhost:8080/admin → Panel de administración

http://localhost:8080/cajero/login → Interfaz de cajero

👨‍💻 Autor
Desarrollado por Yustin Guerrero, como proyecto final para el curso de Construcción de Software, bajo la tutoría del docente Daniel.

📄 Licencia
Este software se encuentra disponible bajo la Licencia MIT. Consulta el archivo LICENSE para más información.


