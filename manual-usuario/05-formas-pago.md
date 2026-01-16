# Formas de Pago

La sección de **Medios de Pago** te permite configurar las opciones de pago disponibles para tus clientes durante el proceso de checkout.

---

## Vista General

El listado de medios de pago se organiza en tres pestañas:

- **Todos**: Muestra todos los métodos configurados
- **Activos**: Métodos habilitados para el checkout
- **Inactivos**: Métodos deshabilitados

### Columnas del Listado

| Columna | Descripción |
|---------|-------------|
| **Nombre** | Nombre del medio de pago |
| **Descripción** | Descripción breve |
| **Recargo/Descuento** | Porcentaje de ajuste |
| **Proveedor** | Proveedor de pago (si aplica) |
| **Estado** | Activo / Inactivo |
| **Acciones** | Botones de acción |

---

## Funciones Principales

### Barra de Herramientas

- **🔍 Buscar**: Busca métodos por nombre o descripción
- **➕ Agregar medio de pago**: Crea un nuevo método

---

## Crear Medio de Pago

Para crear un nuevo medio de pago:

1. Haz clic en **➕ Agregar medio de pago**
2. Completa la información:

### Configuración Principal

| Campo | Descripción | Requerido |
|-------|-------------|-----------|
| **Nombre** | Nombre que verá el cliente | ✅ Sí |
| **Descripción** | Información adicional | No |

### Instrucciones para el Cliente

El campo **"Instrucciones para tu cliente, una vez realizada la compra"** permite agregar texto que se mostrará después del checkout.

**Usos comunes:**
- Datos bancarios para transferencia
- Número de cuenta para depósito
- Alias CBU/CVU
- Instrucciones para pago en efectivo
- Información de Mercado Pago/otros

**Ejemplo para Transferencia:**
```
Realizá la transferencia a:
Banco: Banco Nación
Titular: Mi Empresa SA
CBU: 0000003100000000000000
Alias: TIENDA.ONLINE

Una vez realizada, envianos el comprobante por WhatsApp al 11-1234-5678
```

### Recargo

Si necesitas aplicar un recargo por este medio de pago:

| Campo | Descripción |
|-------|-------------|
| **Recargo %** | Porcentaje a agregar al total |

**Ejemplo**: Un recargo del 10% en una compra de $10,000 resultará en $11,000.

> **💡 Tip**: El recargo se aplica DESPUÉS de calcular subtotal, descuentos, envío e IVA.

### Descuento

Si quieres ofrecer un descuento por usar este medio:

| Campo | Descripción |
|-------|-------------|
| **Descuento %** | Porcentaje a descontar del subtotal |

**Ejemplo**: Un descuento del 10% en una compra de $10,000 resultará en $9,000.

### Combinar con Promociones

| Opción | Descripción |
|--------|-------------|
| **Permitir combinar** | ✅ El descuento del medio de pago se suma a otras promociones |

Si está desactivado, el descuento del medio de pago NO se aplica si ya hay otra promoción activa.

### Proveedor de Pago

Selecciona un proveedor si el medio de pago está integrado con una pasarela:

| Proveedor | Descripción |
|-----------|-------------|
| **Mercado Pago** | Integración con MP |
| **Mobbex** | Integración con Mobbex |
| **PayWay** | Integración con PayWay |
| **Sin proveedor** | Pago manual/offline |

> **💡 Tip**: Los proveedores deben estar previamente configurados en la sección de Proveedores de Pago.

### Ordenamiento

| Campo | Descripción |
|-------|-------------|
| **Orden de visualización** | Posición en la lista del checkout |
| **Medio de pago activo** | ✅ Habilita el método |

---

## Ejemplos de Configuración

### Transferencia Bancaria
- **Nombre**: "Transferencia bancaria"
- **Descripción**: "10% de descuento"
- **Descuento**: 10%
- **Combinar con promociones**: No
- **Proveedor**: Sin proveedor
- **Instrucciones**: Datos de la cuenta bancaria

### Mercado Pago
- **Nombre**: "Mercado Pago"
- **Descripción**: "Tarjetas de crédito y débito"
- **Recargo**: 5% (para cubrir comisiones)
- **Proveedor**: Mercado Pago
- **Instrucciones**: (No necesario, redirect automático)

### Efectivo
- **Nombre**: "Efectivo al retirar"
- **Descripción**: "Pago al retirar en local"
- **Descuento**: 5%
- **Proveedor**: Sin proveedor
- **Instrucciones**: "Abonás cuando retirés tu pedido en nuestro local"

### Pago contra entrega
- **Nombre**: "Pago al recibir"
- **Descripción**: "Abonás cuando llega el pedido"
- **Recargo**: 3%
- **Proveedor**: Sin proveedor

---

## Editar Medio de Pago

Para editar un método existente:

1. Haz clic en el botón **✏️ Editar**
2. Modifica los campos necesarios
3. Haz clic en **Guardar**

---

## Activar/Desactivar Método

Para cambiar el estado de un medio de pago:

1. Edita el método
2. Activa o desactiva "Medio de pago activo"
3. Guarda los cambios

Los métodos inactivos NO aparecen en el checkout pero se conservan en el sistema.

---

## Eliminar Medio de Pago

Para eliminar un método:

1. Haz clic en el botón **🗑️ Eliminar**
2. Confirma la acción

> **⚠️ Advertencia**: Eliminar un medio de pago NO afecta órdenes históricas, pero el método ya no estará disponible.

---

## Proveedores de Pago

Los proveedores de pago son las pasarelas que procesan las transacciones. Se configuran en una sección separada (**Configuración > Proveedores de Pago**).

### Vincular un Proveedor

1. Primero configura el proveedor con sus credenciales
2. Al crear/editar un medio de pago, selecciónalo del dropdown
3. Los pagos se procesarán automáticamente por la pasarela

---

## Mejores Prácticas

### Variedad de Opciones
Ofrece múltiples medios de pago para maximizar conversiones:
- ✅ Tarjetas de crédito/débito
- ✅ Transferencia bancaria
- ✅ Efectivo (si hay retiro en local)
- ✅ Billeteras digitales (Mercado Pago, etc.)

### Transparencia en Costos
- Indica claramente si hay recargos
- Destaca los descuentos disponibles
- Explica bien las instrucciones post-compra

### Orden Estratégico
Ordena los medios de pago de más conveniente a menos:
1. Opciones con descuento primero
2. Opciones online/automáticas
3. Opciones manuales al final

### Seguridad
- Usa pasarelas de pago reconocidas
- No solicites datos de tarjeta directamente
- Mantén actualizadas las credenciales de los proveedores

### Instrucciones Claras
Para pagos manuales, incluye:
- Todos los datos necesarios
- Pasos a seguir
- Medio de contacto para confirmar
- Plazos para realizar el pago
