# Ventas

La sección de **Ventas** (también conocida como Órdenes) te permite gestionar todos los pedidos realizados en tu tienda online.

---

## Vista General

El listado de ventas se divide en dos pestañas:

- **Activas**: Órdenes en proceso o completadas
- **Canceladas**: Órdenes que han sido canceladas

### Columnas del Listado

| Columna | Descripción |
|---------|-------------|
| **#** | Número de orden (ID único) |
| **Fecha** | Fecha y hora de creación |
| **Cliente** | Nombre del cliente (clickeable para ver perfil) |
| **Total** | Monto total de la orden |
| **Pago** | Estado del pago + método de pago |
| **Envío** | Estado del envío + método de entrega |
| **Acciones** | Botones de acción |

---

## Funciones Principales

### Barra de Herramientas

- **🔍 Buscar**: Busca por email, número de orden o nombre del cliente
- **⚙️ Filtrar**: Panel de filtros avanzados
- **📊 Exportar**: Descarga las ventas en Excel
- **➕ Agregar Venta**: Crea una venta manual

### Filtros Avanzados

Haz clic en **Filtrar** para acceder a:

**Por Período:**
- Hoy
- Ayer
- Esta semana
- Este mes
- Período personalizado (desde - hasta)

**Por Estado de Pago:**
- Pendiente
- Autorizado
- Recibido
- Anulado
- Reembolsado
- Abandonado

**Por Estado de Envío:**
- Por empaquetar
- En armado
- Empaquetado
- Enviada
- Devuelto
- Cancelado

---

## Estados de la Orden

### Estados de Pago {#estado-pago}

| Estado | Color | Descripción |
|--------|-------|-------------|
| **Pendiente** | 🟡 Amarillo | Esperando pago |
| **Autorizado** | 🔵 Azul | Pago autorizado pero no capturado |
| **Recibido** | 🟢 Verde | Pago completado |
| **Anulado** | 🔴 Rojo | Pago cancelado |
| **Reembolsado** | 🟣 Púrpura | Dinero devuelto |
| **Abandonado** | ⚫ Gris | Carrito abandonado |

> **💡 Tip**: Haz clic en el estado de pago para cambiarlo rápidamente al siguiente estado en el flujo: Pendiente → Recibido

### Estados de Envío {#estado-envío}

| Estado | Color | Descripción |
|--------|-------|-------------|
| **Por empaquetar** | 🟡 Amarillo | Listo para preparar |
| **En armado** | 🔵 Azul | Se está preparando |
| **Empaquetado** | 🟢 Verde | Listo para enviar |
| **Enviada** | 🟢 Verde | En camino al cliente |
| **Devuelto** | 🟣 Púrpura | Devuelto al remitente |
| **Cancelado** | 🔴 Rojo | Envío cancelado |

> **💡 Tip**: Haz clic en el estado de envío para avanzar al siguiente estado: Por empaquetar → En armado → Empaquetado → Enviada

---

## Ver Orden {#ver-orden}

Para ver el detalle de una orden, haz clic en el **número de orden** o en el botón **👁️ Ver**.

La vista de detalle incluye:

### Información del Cliente
- Nombre completo
- Email
- Teléfono
- Identificación (DNI/CUIT)

### Dirección de Envío
- Calle y número
- Piso y departamento
- Localidad y código postal
- Ciudad y provincia

### Items de la Orden
Listado de productos comprados con:
- Imagen del producto
- Nombre y variante
- Cantidad
- Precio unitario
- Subtotal

### Resumen de la Orden
| Concepto | Descripción |
|----------|-------------|
| **Subtotal** | Suma de todos los productos |
| **Descuento** | Descuentos aplicados (promociones) |
| **Cupón** | Descuento por código de cupón |
| **IVA** | Impuestos (si aplica) |
| **Envío** | Costo del envío |
| **Recargo** | Recargo por método de pago (si aplica) |
| **Total** | Monto final a pagar |

### Métodos
- Método de pago seleccionado
- Método de envío seleccionado

---

## Crear Venta Manual

Para crear una venta directamente desde el panel:

1. Haz clic en **➕ Agregar Venta**
2. Completa la información:

### Información del Cliente
1. Haz clic en "Buscar cliente" para seleccionar uno existente, o
2. Completa los datos de un nuevo cliente

### Métodos de Pago y Envío
1. Selecciona el método de pago
2. Selecciona el método de envío
3. Los costos se calcularán automáticamente

### Agregar Productos
1. Haz clic en "Agregar producto"
2. Busca y selecciona los productos
3. Ajusta cantidades si es necesario
4. Aplica descuentos por item si corresponde

### Configurar Totales
- **Envío**: Ajusta el costo de envío manualmente si es necesario
- **Descuento**: Aplica descuento porcentual o de monto fijo
- **IVA**: Selecciona 0%, 10.5% o 21%
- **Recargo**: Aplica recargo si el método de pago lo requiere

### Notas
Agrega observaciones internas sobre la orden.

---

## Acciones sobre Órdenes

### Ver (👁️)
Abre la vista de detalle de la orden.

### Imprimir (🖨️)
Genera una versión imprimible de la orden con todos los detalles.

### Cancelar (🚫)
Cancela la orden activa:
1. La orden pasa a la pestaña "Canceladas"
2. Si hay integración ERP, también se cancela en el sistema externo
3. Se envía email de notificación al cliente

### Eliminar (🗑️)
Solo disponible para órdenes canceladas. Elimina permanentemente la orden.

---

## Indicadores Especiales

### Sincronización ERP
Si la orden está sincronizada con un sistema ERP externo, verás un indicador ✓ verde junto al número de orden.

### Notificaciones Automáticas
El sistema envía emails automáticos al cliente cuando:
- Se confirma el pago
- Se cancela la orden

---

## Exportar Ventas

1. Haz clic en **📊 Exportar**
2. Selecciona el período y filtros
3. El archivo Excel incluirá:
   - Datos de la orden
   - Información del cliente
   - Detalle de productos
   - Totales y métodos

---

## Paginación

Navega entre las ventas usando los controles de paginación:
- Cambia entre páginas
- Ajusta la cantidad de registros por página (10, 25, 50, 100)
- Visualiza el total de ventas
