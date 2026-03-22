# Sistema Biometrico UMG — Version Web (Spring Boot)

**Universidad Mariano Galvez de Guatemala — Sede La Florida, Zona 19**

Aplicacion web accesible desde cualquier navegador.

## Tecnologias
- Java 19 + Spring Boot 3.2
- Thymeleaf (plantillas HTML)
- Spring Security (autenticacion y roles)
- Spring Data JPA + PostgreSQL
- WebSocket (camara en tiempo real)
- CSS puro — paleta azul UMG

## Modulos
| Ruta | Descripcion |
|------|-------------|
| /login | Inicio de sesion por carnet |
| /menu | Panel principal con los 6 modulos |
| /registro | Alta de personas con foto y biometrico |
| /ingreso/puerta | Control de acceso facial puerta principal |
| /catedratico | Dashboard con arbol visual de estudiantes |
| /reportes | 4 vistas de arbol: puertas, fechas, salones, asistencia |
| /admin/restringidos | Gestion de restricciones de acceso |

## Instalacion
```bash
git clone https://github.com/Dfrancoc256/biometrico-umg-web.git
cd biometrico-umg-web
```

Editar `src/main/resources/application.properties` con los datos de la base de datos:
```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/biometrico_umg
spring.datasource.username=postgres
spring.datasource.password=TU_CONTRASENA
```

```bash
mvn spring-boot:run
# Abrir: http://localhost:8080
```

## Requisitos
- Java 19+: https://adoptium.net/es/
- Maven 3.8+: https://maven.apache.org/
- PostgreSQL 13+: https://www.postgresql.org/
- Base de datos creada con el script del repo escritorio

## Credenciales predeterminadas
| Carnet | Contrasena |
|--------|------------|
| ADMIN-001 | admin123 |

## Version Escritorio
Existe tambien la version de escritorio (JavaFX): https://github.com/Dfrancoc256/biometrico-umg

---
*Universidad Mariano Galvez — Sede La Florida, Zona 19 — 2026*