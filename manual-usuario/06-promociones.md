# Promociones

La sección de **Promociones** te permite crear descuentos automáticos que se aplican sin necesidad de ingresar un código. Son ideales para campañas de marketing y ofertas especiales.

---

## Vista General

El listado muestra todas las promociones configuradas con:

| Columna | Descripción |
|---------|-------------|
| **Nombre** | Nombre interno de la promoción |
| **Tipo** | Tipo de descuento |
| **Estado** | Activa / Inactiva |
| **Vigencia** | Fechas de validez |
| **Acciones** | Botones de acción |

---

## Funciones Principales

### Barra de Herramientas

- **🔍 Buscar**: Busca promociones por nombre
- **➕ Crear Promoción**: Crea una nueva promoción

---

## Tipos de Promoción

### 1. Lleva X y Paga Y (2x1, 3x2, etc.) {#promocion-2x1}

Permite crear ofertas del tipo "llevando X productos, pagás solo Y".

**Ejemplos:**
- 2x1: Llevando 2, pagás 1
- 3x2: Llevando 3, pagás 2
- 4x3: Llevando 4, pagás 3

**Configuración:**
| Campo | Descripción |
|-------|-------------|
| **Llevando** | Cantidad de productos que debe agregar el cliente |
| **Pagás** | Cantidad de productos que realmente paga |

**Opción adicional:**
- **Aplicar solo dentro del mismo producto**: Si está activo, la promo aplica por producto (ej: 3x2 del mismo artículo). Si está apagado, se combinan diferentes productos que apliquen a la promoción.

### 2. Descuento sobre Precios

Aplica un descuento fijo a los productos seleccionados.

**Opciones:**
| Tipo | Descripción |
|------|-------------|
| **Porcentaje** | Descuento del X% (ej: 20% OFF) |
| **Monto fijo** | Descuento de $X (ej: $500 de descuento) |

### 3. Descuento Progresivo por Cantidad {#descuento-progresivo}

El descuento aumenta según la cantidad de productos comprados.

**Ejemplo:**
| Cantidad | Descuento |
|----------|-----------|
| 2 o más | 10% |
| 5 o más | 15% |
| 10 o más | 20% |

**Configuración de escalas:**
Para cada escala, define:
- **Al comprar por lo menos**: Cantidad mínima de productos
- **Descuento %**: Porcentaje de descuento

Haz clic en **"+ Nuevo descuento progresivo"** para agregar más escalas.

### 4. Descuento Progresivo por Monto

Similar al anterior, pero basado en el monto total de compra.

**Ejemplo:**
| Monto | Descuento |
|-------|-----------|
| $10,000 o más | 5% |
| $25,000 o más | 10% |
| $50,000 o más | 15% |

**Configuración de escalas:**
- **Monto mínimo**: Valor en pesos
- **Descuento %**: Porcentaje de descuento

---

## Crear Promoción

Para crear una nueva promoción:

1. Haz clic en **➕ Crear Promoción**
2. Completa las secciones:

### Nombre

| Campo | Descripción |
|-------|-------------|
| **Nombre** | Nombre interno (NO visible para clientes) |

### Tipo de Descuento

Selecciona uno de los 4 tipos disponibles y configura sus parámetros específicos.

### Aplicar a

Define a qué productos aplica la promoción:

| Opción | Descripción |
|--------|-------------|
| **Toda la tienda** | Aplica a todos los productos |
| **Categorías** | Solo a productos de categorías específicas |
| **Productos** | Solo a productos específicos |

**Para Categorías:**
1. Selecciona "Categorías"
2. Haz clic en "Seleccionar categorías"
3. Marca las categorías deseadas
4. Las categorías seleccionadas aparecen como etiquetas

**Para Productos:**
1. Selecciona "Productos"
2. Haz clic en "Seleccionar productos"
3. Busca y marca los productos deseados
4. Los productos seleccionados aparecen como etiquetas

### Límites de Uso

**Combinar con otras promociones:**
| Opción | Descripción |
|--------|-------------|
| **Activado** | La promoción se puede combinar con otras (precio promocional, envío gratis, etc.) |
| **Desactivado** | No se combina con otras promociones |

**Fecha de vigencia:**
| Opción | Descripción |
|--------|-------------|
| **Ilimitada** | Sin fecha de expiración |
| **Período** | Define fecha de inicio y fin |

### Etiqueta Personalizada

Personaliza el texto que se muestra en los productos con promoción:

| Campo | Descripción |
|-------|-------------|
| **Texto de la etiqueta** | Máximo 30 caracteres |

**Ejemplos:**
- "20% OFF comprando 2 o más"
- "3x2 EN CAMISETAS"
- "LIQUIDACIÓN -30%"

> **💡 Tip**: Si dejas vacío, el sistema muestra automáticamente el descuento calculado.

---

## Ejemplos de Configuración

### 2x1 en toda la tienda
- **Tipo**: Lleva X y Paga Y
- **Llevando**: 2
- **Pagás**: 1
- **Aplicar a**: Toda la tienda
- **Etiqueta**: "2x1 EN TODO"

### 20% en categoría específica
- **Tipo**: Descuento sobre precios
- **Porcentaje**: 20%
- **Aplicar a**: Categorías → "Remeras", "Pantalones"
- **Etiqueta**: "20% OFF"

### Descuento progresivo por cantidad
- **Tipo**: Progresivo por cantidad
- **Escalas**:
  - 3 unidades → 10%
  - 6 unidades → 15%
  - 12 unidades → 25%
- **Aplicar a**: Productos específicos
- **Etiqueta**: "Hasta 25% llevando más"

### Promoción de temporada
- **Tipo**: Descuento sobre precios
- **Porcentaje**: 30%
- **Aplicar a**: Categorías → "Verano"
- **Período**: 01/12 al 28/02
- **Etiqueta**: "SALE VERANO -30%"

---

## Editar Promoción

1. Haz clic en el botón **✏️ Editar**
2. Modifica los campos necesarios
3. Haz clic en **Guardar**

---

## Activar/Desactivar Promoción

Las promociones inactivas NO se aplican pero se conservan en el sistema.

Para cambiar el estado, edita la promoción y modifica su configuración.

---

## Eliminar Promoción

1. Haz clic en **🗑️ Eliminar**
2. Confirma la acción

> **⚠️ Advertencia**: Eliminar una promoción es permanente. Si solo quieres pausarla, desactívala en lugar de eliminarla.

---

## Cómo se Aplican las Promociones

### Automáticamente
Las promociones activas se aplican automáticamente en el carrito cuando se cumplen las condiciones.

### Prioridad
Si un producto tiene múltiples promociones aplicables:
1. Se aplica la más beneficiosa para el cliente
2. O se combinan si "Combinar con otras promociones" está activo

### Visualización
- En la tienda: Productos con promoción muestran la etiqueta configurada
- En el carrito: Se muestra el descuento aplicado
- En el checkout: Resumen con todos los descuentos

---

## Mejores Prácticas

### Nombres Descriptivos
Usa nombres que te ayuden a identificar la promoción:
- ✅ "2x1 Remeras Verano 2026"
- ✅ "Progresivo Mayorista"
- ❌ "Promo 1"

### Fechas Claras
- Usa períodos para promociones temporales
- Deja ilimitada solo las promociones permanentes
- Recuerda desactivar promociones vencidas

### Etiquetas Atractivas
- Destaca el beneficio principal
- Usa mayúsculas para impacto
- Sé claro y conciso (máx. 30 caracteres)

### Testing
- Prueba la promoción antes de publicarla
- Verifica que se aplica correctamente en el carrito
- Confirma los cálculos de descuento
