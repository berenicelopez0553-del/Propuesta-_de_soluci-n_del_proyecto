)

🛠️ Requisitos Previos

Antes de iniciar el proyecto, asegúrate de tener instalado:

✔ Software necesario

Java JDK 17 o superior

Maven 3.8+

✔ IDE recomendado

Puedes usar cualquiera de los siguientes entornos:

IntelliJ IDEA

Spring Tools Suite (STS)

VS Code con extensiones de soporte para Java & Spring Boot

📥 Instalación del Proyecto

Sigue estos pasos para preparar el entorno local:

1️⃣ Clonar o descargar el repositorio
git clone <URL-del-repositorio>

2️⃣ Entrar al directorio del proyecto
cd recoleccion-basura

3️⃣ Verificar e instalar dependencias
mvn clean install

▶️ Ejecución del Proyecto
✅ Opción 1: Ejecutar directamente con Maven
mvn spring-boot:run

✅ Opción 2: Ejecutar usando el archivo .jar

Generar el build:

mvn clean package


Ejecutar el JAR generado:

java -jar target/recoleccion-basura-0.0.1-SNAPSHOT.jar

🌐 Acceso a la Aplicación

Una vez iniciado el backend, estará disponible en:

🔗 http://localhost:8080

La mayoría de los endpoints suelen encontrarse bajo rutas:

/api/...


(Puedo generar documentación completa de endpoints si me compartes tus controladores.)

📁 Estructura del Proyecto
recoleccion-basura/
│
├── src/
│   ├── main/
│   │   ├── java/        # Código fuente principal
│   │   └── resources/   # Configuración (application.properties / .yml)
│   │
│   └── test/            # Pruebas (si aplica)
│
├── pom.xml              # Dependencias y configuración del proyecto
└── target/              # Artefactos generados automáticamente

🧪 Ejecución de Pruebas

Si el proyecto contiene pruebas unitarias:

mvn test

⚙️ Configuración Adicional

Puedes modificar los parámetros de base de datos en:

src/main/resources/application.properties

✔ Acceso a H2 (si está habilitado)
http://localhost:8080/h2-console
