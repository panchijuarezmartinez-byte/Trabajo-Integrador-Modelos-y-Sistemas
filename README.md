# Sistema Practicas Profesionalizantes

Sistema de escritorio para la **gestión de usuarios** y la **gestión de proveedores**.

## Tecnologías

- C# con .NET Framework 4.0
- MySQL
- Visual Studio

## Arquitectura

El proyecto está dividido en 4 capas:

| Capa | Proyecto | Carpeta | Función |
|------|----------|---------|---------|
| Presentación | `CapaVista` | `CapaPresentacion/` | Interfaz de usuario |
| Negocio | `CapaLogica` | `CapaNegocio/` | Lógica y reglas del sistema |
| Datos | `CapaDatos` | `CapaDatos/` | Acceso a la base de datos MySQL |
| Entidades | `CapaEntidades` | `CapaEntidades/` | Clases compartidas entre capas |

## Cómo ejecutarlo

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/<tu-usuario>/<tu-repositorio>.git
   ```
2. Abrir `Sistema_Epico.sln` con Visual Studio.
3. Crear la base de datos en MySQL y configurar la cadena de conexión en `CapaDatos`.
4. Establecer `CapaVista` como proyecto de inicio y presionar `F5`.
