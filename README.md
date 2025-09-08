# 📦 Sistema de Facturación e Inventario – RRM Dev v1.0 

Este proyecto es un **sistema modular de facturación e inventario**, desarrollado en **C# WinForms** con base de datos **MySQL**, pensado para ser extensible, mantenible y adaptable a diferentes negocios.  

El sistema busca ofrecer una solución integral para la gestión de ventas, inventarios, usuarios y reportes, con especial enfoque en **seguridad, trazabilidad e historial de datos**.  

---

## 🚀 Funcionalidades actuales  
- ⚙️ **Gestión de conexión a base de datos**  
  - Configuración segura de conexión (con archivo encriptado en carpeta `Configuracion`).  
  - Selección de base de datos disponible en el servidor.  
  - Pruebas de conexión y logs automáticos.  

- 🖥️ **Consola integrada en el sistema**  
  - Mensajes en tiempo real (información, advertencias, errores).  
  - Generación de archivos de logs diarios en carpeta `Logs`.  
  - Visor de logs con exploración en árbol, filtros y conteo de registros.  

- 📂 **Gestión de carpetas internas**  
  - Creación automática de carpetas del sistema: `Modulos`, `Reportes`, `Configuracion`, `Backup`, `Logs`.  

- 🔧 **Configuración del sistema**  
  - Timeout de sesión.  
  - Notificaciones activas/desactivas.  
  - Restauración de valores predeterminados.  

- 🗄️ **Manejo de base de datos**  
  - Creación de nuevas bases de datos desde el sistema.  
  - Creación automática de tablas base (`usuarios`, `inventario`, `terceros`, `facturas`, `logs`).  
  - Scripts centralizados en `DbSchema.cs`.  
  - Verificación de integridad de tablas.  
  - Limpieza de registros antiguos (ej. logs).  

---

## 🛠️ Funcionalidades en desarrollo / próximas a implementar  
- 👤 **Gestión de usuarios y roles**  
  - Acceso restringido por permisos.  
  - Roles configurables para limitar módulos y acciones.  

- 🧩 **Módulos dinámicos**  
  - Arquitectura modular con carga de plugins (MEF).  
  - Panel de módulos en el formulario principal.  

- 🛡️ **Mantenimiento de base de datos**  
  - Verificación de integridad desde interfaz.  
  - Optimización de tablas.  
  - Respaldo automático en carpeta `Backup`.  

- 📦 **Inventario y facturación**  
  - Registro de productos y terceros.  
  - Manejo de facturación con cálculo de impuestos.  
  - Kardex automático para movimientos de inventario.  

- 📊 **Reportes**  
  - Generación y almacenamiento en carpeta `Reportes`.  
  - Exportación a PDF, Excel y otros formatos.  

- 🎨 **Interfaz moderna**  
  - Barra de estado con información en tiempo real (usuario, hora, conexión).  
  - Tooltips explicativos en todos los formularios.  
  - Atajos de teclado para acciones rápidas.  

---

## 📂 Estructura principal del sistema  
- Configuracion/ -> Configuración de conexión y sistema
- Logs/ -> Archivos de logs diarios
- Modulos/ -> Plugins o módulos cargables
- Reportes/ -> Archivos de reportes generados
- Backup/ -> Respaldo de base de datos

---

## 📌 Notas  
👉 Este sistema está en constante evolución, integrando buenas prácticas de desarrollo, arquitectura modular y control de errores centralizado.  
