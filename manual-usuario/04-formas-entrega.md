# Formas de Entrega

La sección de **Formas de Entrega** (también llamada Métodos de Envío) te permite configurar las opciones de envío disponibles para tus clientes.

---

## Vista General

El listado de métodos de envío se organiza en tres pestañas:

- **Todos**: Muestra todos los métodos configurados
- **Activos**: Métodos habilitados para el checkout
- **Inactivos**: Métodos deshabilitados

### Columnas del Listado

| Columna | Descripción |
|---------|-------------|
| **Nombre** | Nombre del método de envío |
| **Descripción** | Descripción breve |
| **Costo** | Gratis, monto fijo o "A convenir" |
| **Plazo** | Tiempo de entrega estimado |
| **Estado** | Activo / Inactivo |
| **Acciones** | Botones de acción |

---

## Funciones Principales

### Barra de Herramientas

- **🔍 Buscar**: Busca métodos por nombre o descripción
- **➕ Agregar forma de entrega**: Crea un nuevo método

---

## Crear Método de Envío

Para crear un nuevo método de envío:

1. Haz clic en **➕ Agregar forma de entrega**
2. Completa la información:

### Información Básica

| Campo | Descripción | Requerido |
|-------|-------------|-----------|
| **Nombre** | Nombre que verá el cliente (ej: "Envío a domicilio") | ✅ Sí |
| **Descripción** | Información adicional sobre el envío | No |
| **Orden** | Posición en la lista del checkout | No |

### Configuración de Costo

Selecciona el tipo de costo:

| Opción | Descripción |
|--------|-------------|
| **Con costo** | Define un monto fijo en pesos |
| **Gratis** | El envío no tiene costo para el cliente |
| **A convenir** | El costo se acuerda con el cliente después de la compra |

Si seleccionas "Con costo", ingresa el monto en el campo que aparece.

### Opciones de Dirección

| Opción | Descripción |
|--------|-------------|
| **Requiere dirección** | ✅ El cliente debe ingresar dirección de envío |
| **Es empresa de envíos** | ✅ Habilita opciones adicionales para correos/transporte |

Si marcas "Es empresa de envíos", aparecen opciones adicionales:
- **Pedir dirección**: Solicitar dirección de la sucursal
- **Pedir nombre**: Solicitar nombre de quien retira
- **Pedir teléfono**: Solicitar teléfono de contacto

### Plazo de Entrega

Define el tiempo estimado de entrega en días hábiles:

| Campo | Descripción |
|-------|-------------|
| **De** | Mínimo de días hábiles |
| **A** | Máximo de días hábiles |

**Ejemplo**: De 3 a 5 días hábiles

> **💡 Tip**: Un plazo realista genera confianza. Es mejor prometer menos y entregar antes.

### Condiciones (Opcional)

Activa las condiciones para limitar cuándo está disponible este método:

#### Por Peso
| Campo | Descripción |
|-------|-------------|
| **De** | Peso mínimo del carrito (kg) |
| **A** | Peso máximo del carrito (kg) |

**Ejemplo**: Disponible solo para carritos de 0 a 20 kg.

#### Por Monto
| Campo | Descripción |
|-------|-------------|
| **De** | Monto mínimo de compra ($) |
| **A** | Monto máximo de compra ($) |

**Ejemplo**: Disponible solo para compras mayores a $10,000.

> **💡 Tip**: Las condiciones son útiles para ofrecer envío gratis a partir de cierto monto, o limitar opciones de envío pesado.

---

## Ejemplos de Configuración

### Retiro en Local
- **Nombre**: "Retiro en local"
- **Costo**: Gratis
- **Requiere dirección**: No
- **Es empresa de envíos**: No

### Envío a Domicilio
- **Nombre**: "Envío a domicilio"
- **Costo**: $2,500
- **Requiere dirección**: Sí
- **Plazo**: 3-5 días hábiles

### Envío Gratis (condicional)
- **Nombre**: "Envío gratis"
- **Costo**: Gratis
- **Condiciones**: Activadas
- **Monto mínimo**: $50,000

### Correo Argentino
- **Nombre**: "Correo Argentino"
- **Costo**: $1,800
- **Es empresa de envíos**: Sí
- **Pedir nombre**: Sí
- **Plazo**: 5-10 días hábiles

---

## Editar Método de Envío

Para editar un método existente:

1. Haz clic en el botón **✏️ Editar** en la fila del método
2. Modifica los campos necesarios
3. Haz clic en **Guardar**

---

## Activar/Desactivar Método

Los métodos inactivos no aparecen en el checkout pero se conservan para referencia.

Para cambiar el estado:
1. Edita el método de envío
2. Modifica la opción de estado
3. Guarda los cambios

---

## Eliminar Método de Envío

Para eliminar un método:

1. Haz clic en el botón **🗑️ Eliminar**
2. Confirma la acción

> **⚠️ Advertencia**: Eliminar un método de envío NO afecta a las órdenes históricas, pero el método ya no estará disponible para nuevas compras.

---

## Orden de Visualización

El campo **Orden** determina en qué posición aparece cada método en el checkout.

- Número menor = aparece primero
- Número mayor = aparece después
- Deja en 0 para ordenamiento automático

---

## Mejores Prácticas

### Nombres Claros
Usa nombres descriptivos que el cliente entienda fácilmente:
- ✅ "Retiro en local - Av. Corrientes 1234"
- ✅ "Envío express (24-48hs)"
- ❌ "Método 1"
- ❌ "ENV_DOM"

### Plazos Realistas
- Considera feriados y demoras típicas
- Es mejor superar las expectativas que decepcionar
- Actualiza los plazos según temporada alta/baja

### Costos Transparentes
- Si el costo es "A convenir", explica en la descripción cómo se calcula
- Considera incluir envío gratis a partir de cierto monto
- Revisa periódicamente los costos según tarifas de transportes

### Condiciones Estratégicas
- Usa condiciones de monto mínimo para incentivar compras mayores
- Limita métodos de envío para productos pesados o voluminosos
- Crea múltiples métodos para diferentes escenarios
