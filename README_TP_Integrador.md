# Trabajo Integrador – Modelos y Sistemas

## Información general
- **Materia:** Modelos y Sistemas
- **Escuela:** E.E.S.T. N.º 2
- **Curso:** 7.º año
- **Alumno:** Francisco Juarez
- **Profesor:** Gain Franco Denaro
- **Sistema elegido:** Proyecto de prácticas profesionalizantes

## Descripción del sistema
El trabajo describe **Sistema Épico**, una aplicación de escritorio desarrollada en C# con Visual Studio. El sistema gestiona usuarios, políticas de seguridad y proveedores, y almacena la información en SQL Server.

La aplicación está organizada en capas:
- **Capa de presentación:** formularios y pantallas con los que interactúa el usuario.
- **Capa de negocio:** reglas del sistema, validaciones, cifrado y envío de correos.
- **Capa de datos:** comunicación con SQL Server mediante conexiones y procedimientos almacenados.
- **Capa de entidades:** clases que representan la información que circula entre las capas.
- **Base de datos:** estructura, configuración y procedimientos SQL.

## Contenido del documento
1. **Presentación del sistema:** descripción general y organización por capas.
2. **Marco conceptual y clasificación:** diferencias entre documentación de usuario y documentación técnica, con ejemplos.
3. **Instructivo paso a paso:** procedimiento para iniciar sesión con verificación en dos pasos, requisitos previos, resultado esperado y solución de errores frecuentes.
4. **Diagrama de flujo:** representación visual de las validaciones de acceso, los caminos de error y la habilitación de la pantalla según el rol.
5. **Caso de uso formal (CU-01):** actor principal y secundarios, precondiciones, postcondición, flujo principal y excepciones.
6. **Captura anotada e interfaz:** identificación de los elementos principales de la pantalla de inicio de sesión.
7. **Referencias:** explicación de los campos y controles de la pantalla.

## Proceso de inicio de sesión
El usuario ingresa su nombre de usuario y contraseña. El sistema valida las credenciales y comprueba que la cuenta esté activa. Si la política de seguridad requiere doble factor, envía un código de seis dígitos al correo registrado. Una vez validado el código, identifica el rol y abre la pantalla correspondiente.

Si las credenciales, el estado de la cuenta o el código no son válidos, el acceso no se concede y se informa el problema. También se contemplan situaciones como la falta de correo registrado, fallas en el envío, el primer ingreso y la ausencia de un rol asignado.

## Tecnologías mencionadas
- C#
- Visual Studio
- SQL Server
- SHA-256 para el tratamiento de credenciales, según lo descrito en el trabajo
- Servicio de correo para la verificación en dos pasos

## Archivos
- `TP_Integrador_Modelos_y_Sistemas_editado.docx`: documento principal actualizado, con índice, redacción ampliada y diagrama de flujo rediseñado.
- `README_TP_Integrador.md`: resumen y guía de lectura del trabajo.

---
Este README resume el contenido del documento y no reemplaza las explicaciones completas incluidas en el trabajo integrador.
