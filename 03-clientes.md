# Clientes

La sección de **Clientes** te permite gestionar la base de datos de clientes de tu tienda, incluyendo sus datos personales, direcciones de facturación y historial de compras.

---

## Vista General

El listado de clientes se organiza en tres pestañas:

- **Todos**: Muestra todos los clientes registrados
- **Activos**: Clientes con cuenta activa
- **Inactivos**: Clientes con cuenta desactivada

### Columnas del Listado

| Columna | Descripción |
|---------|-------------|
| **Cliente** | Nombre completo del cliente |
| **Email** | Correo electrónico |
| **Teléfono** | Número de contacto |
| **Identificación** | DNI o CUIT |
| **Estado** | Activo / Inactivo |
| **Acciones** | Botones de acción |

---

## Funciones Principales

### Barra de Herramientas

- **🔍 Buscar**: Busca por email, nombre, teléfono o identificación
- **📊 Exportar**: Descarga la lista de clientes en Excel
- **➕ Agregar Cliente**: Crea un nuevo cliente

### Búsqueda

El buscador permite encontrar clientes por:
- Correo electrónico
- Nombre o apellido
- Número de teléfono
- DNI o CUIT

Para buscar:
1. Escribe el término de búsqueda
2. Presiona **Enter** para aplicar
3. El filtro activo se muestra como etiqueta
4. Haz clic en la **X** para quitar el filtro

---

## Crear Cliente {#crear-cliente}

Para crear un nuevo cliente:

1. Haz clic en **➕ Agregar Cliente**
2. Completa la información requerida:

### Datos Personales

| Campo | Descripción | Requerido |
|-------|-------------|-----------|
| **Nombre** | Nombre del cliente | ✅ Sí |
| **Apellido** | Apellido del cliente | ✅ Sí |
| **Correo electrónico** | Email (será el usuario de login) | ✅ Sí |
| **Contraseña** | Contraseña inicial (solo en creación) | No |
| **Teléfono** | Número de contacto | No |
| **Empresa** | Nombre de la empresa (si aplica) | No |
| **CUIT / DNI** | Documento de identificación | No |

> **💡 Tip**: El email no puede modificarse después de crear el cliente. Asegúrate de ingresarlo correctamente.

### Datos de Facturación

| Campo | Descripción | Requerido |
|-------|-------------|-----------|
| **Calle** | Nombre de la calle | No |
| **Número** | Número de puerta | No |
| **Piso** | Piso (si aplica) | No |
| **Departamento** | Departamento (si aplica) | No |
| **Código postal** | CP de la zona | No |
| **Ciudad** | Ciudad de residencia | No |
| **Provincia** | Provincia (seleccionar de lista) | No |

3. Haz clic en **Guardar** para crear el cliente

---

## Editar Cliente

Para editar un cliente existente:

1. En el listado, haz clic en el botón **✏️ Editar** o en el nombre del cliente
2. Modifica los campos necesarios
3. Haz clic en **Guardar**

**Campos que NO pueden modificarse:**
- Correo electrónico (es el identificador único)
- Contraseña (el cliente debe cambiarla desde su cuenta)

---

## Ver Cliente

Para ver el perfil completo de un cliente:

1. Haz clic en el **nombre del cliente** en el listado
2. Accederás a la vista de detalle que incluye:

### Información del Perfil
- Datos personales completos
- Dirección de facturación
- Fecha de registro
- Estado de la cuenta

### Historial de Compras
- Lista de todas las órdenes del cliente
- Total gastado acumulado
- Última compra realizada

---

## Exportar Clientes

Para exportar la base de clientes:

1. Haz clic en **📊 Exportar**
2. Se descargará un archivo Excel con:
   - ID del cliente
   - Nombre y apellido
   - Email
   - Teléfono
   - Identificación
   - Empresa
   - Estado de cuenta
   - Fecha de registro
   - Direcciones

El archivo se nombra automáticamente con la fecha: `clientes_2026-01-16.xlsx`

---

## Estados de Cliente

| Estado | Descripción |
|--------|-------------|
| **Activo** | El cliente puede iniciar sesión y realizar compras |
| **Inactivo** | La cuenta está deshabilitada |

Para cambiar el estado de un cliente, debes editar su perfil.

---

## Filtrar por Estado

Usa las pestañas para filtrar rápidamente:

1. **Todos**: Muestra clientes activos e inactivos
2. **Activos**: Solo clientes con cuenta habilitada
3. **Inactivos**: Solo clientes con cuenta deshabilitada

> **💡 Tip**: Al cambiar de pestaña, el buscador se limpia automáticamente.

---

## Eliminar Cliente

Para eliminar un cliente:

1. Haz clic en el botón **🗑️ Eliminar**
2. Confirma la acción en el diálogo

> **⚠️ Advertencia**: Eliminar un cliente es una acción permanente. El historial de compras asociado NO se elimina, pero el cliente no podrá acceder a su cuenta.

---

## Paginación

Navega entre los clientes usando los controles:
- Flechas para cambiar de página
- Selector de registros por página (10, 25, 50, 100)
- Contador del total de clientes

---

## Consejos y Mejores Prácticas

### Gestión de Datos
- Mantén los emails actualizados para comunicaciones
- Verifica la identificación para facturación
- Completa las direcciones para agilizar los envíos

### Privacidad
- Los datos de los clientes son confidenciales
- Cumple con las normativas de protección de datos
- No compartas información de clientes con terceros

### Soporte al Cliente
- Usa la vista de detalle para entender el historial
- Verifica el total gastado para atención personalizada
- Revisa las direcciones antes de confirmar envíos
