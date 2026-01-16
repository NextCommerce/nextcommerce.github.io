# Cupones

La sección de **Cupones** te permite crear códigos de descuento que los clientes pueden ingresar durante el checkout para obtener beneficios especiales.

---

## Vista General

El listado muestra todos los cupones configurados:

| Columna | Descripción |
|---------|-------------|
| **Código** | Código que ingresa el cliente |
| **Tipo** | Porcentaje o monto fijo |
| **Valor** | Cantidad del descuento |
| **Usos** | Cantidad de veces usado |
| **Estado** | Válido / Expirado |
| **Acciones** | Botones de acción |

---

## Funciones Principales

### Barra de Herramientas

- **🔍 Buscar**: Busca cupones por código
- **➕ Agregar Cupón**: Crea un nuevo cupón

---

## Crear Cupón {#crear-cupon}

Para crear un nuevo cupón:

1. Haz clic en **➕ Agregar Cupón**
2. Completa las secciones:

### Código del Cupón

| Campo | Descripción | Requerido |
|-------|-------------|-----------|
| **Código** | Texto que ingresa el cliente | ✅ Sí |

**Recomendaciones para códigos:**
- Usa mayúsculas
- Sin espacios ni caracteres especiales
- Fácil de recordar y comunicar

**Ejemplos:**
- `BIENVENIDO10` - 10% para nuevos clientes
- `VERANO2026` - Promoción de temporada
- `ENVIOGRATIS` - Envío sin cargo
- `BLACKFRIDAY` - Evento especial

### Tipo de Descuento

| Tipo | Descripción |
|------|-------------|
| **Porcentaje** | Descuento del X% del subtotal |
| **Monto fijo** | Descuento de $X del total |
| **Envío gratis** | Elimina el costo de envío (próximamente) |

**Para Porcentaje:**
- Ingresa el porcentaje (ej: 15 para 15%)
- Máximo 100%

**Para Monto fijo:**
- Ingresa el monto en pesos (ej: 2000 para $2,000)

### Límites de Uso

#### Combinar con otras promociones
| Opción | Descripción |
|--------|-------------|
| **Activado** | El cupón se suma a promociones existentes |
| **Desactivado** | El cupón NO aplica si hay otras promociones |

#### Por Cupón (límite global)
| Opción | Descripción |
|--------|-------------|
| **Ilimitado** | Sin límite de usos |
| **Limitado** | Define cantidad máxima de usos totales |

**Ejemplo**: Si configuras "Limitado" con 100, el cupón podrá usarse 100 veces en total (entre todos los clientes).

#### Por Cliente
| Opción | Descripción |
|--------|-------------|
| **Ilimitado** | Cada cliente puede usarlo sin límite |
| **Limitado** | Define cuántas veces puede usarlo cada cliente |
| **Primera compra** | Solo en la primera compra del cliente |

**Primera compra**: El cupón solo funciona si el cliente nunca ha realizado una compra previa.

#### Fecha de Vigencia
| Opción | Descripción |
|--------|-------------|
| **Ilimitado** | Sin fecha de expiración |
| **Período** | Define fecha de inicio y fin |

Para período, selecciona:
- **Desde**: Fecha a partir de la cual es válido
- **Hasta**: Fecha hasta la cual es válido (inclusive)

#### Monto del Carrito
| Campo | Descripción |
|-------|-------------|
| **Mayor de $** | Monto mínimo de compra para que aplique |

**Ejemplo**: Si configuras "Mayor de $5,000", el cupón solo funciona si el subtotal del carrito es mayor a $5,000.

> **💡 Tip**: No aplica al costo de envío, solo al subtotal de productos.

### Aplicar a

Define a qué productos aplica el cupón:

| Opción | Descripción |
|--------|-------------|
| **Toda la tienda** | Aplica a cualquier producto |
| **Categorías** | Solo a productos de categorías específicas |
| **Productos** | Solo a productos específicos |

**Para Categorías:**
1. Selecciona "Categorías"
2. Haz clic en "Seleccionar categorías"
3. Marca las categorías
4. Las seleccionadas aparecen como etiquetas

**Para Productos:**
1. Selecciona "Productos"
2. Haz clic en "Seleccionar productos"
3. Busca y selecciona productos
4. Los seleccionados aparecen como etiquetas

---

## Ejemplos de Configuración

### Cupón de Bienvenida
- **Código**: `BIENVENIDO15`
- **Tipo**: Porcentaje
- **Valor**: 15%
- **Por cliente**: Primera compra
- **Aplicar a**: Toda la tienda
- **Combinar**: Sí

### Cupón para Mailing
- **Código**: `NEWSLETTER10`
- **Tipo**: Porcentaje
- **Valor**: 10%
- **Por cupón**: Limitado a 500 usos
- **Por cliente**: 1 uso
- **Aplicar a**: Toda la tienda

### Cupón de Temporada
- **Código**: `VERANO30`
- **Tipo**: Porcentaje
- **Valor**: 30%
- **Período**: 01/12/2025 al 28/02/2026
- **Aplicar a**: Categorías → "Verano", "Playa"

### Cupón con Mínimo
- **Código**: `DESCUENTO2000`
- **Tipo**: Monto fijo
- **Valor**: $2,000
- **Monto mínimo**: $15,000
- **Aplicar a**: Toda la tienda

### Cupón VIP
- **Código**: `VIP25`
- **Tipo**: Porcentaje
- **Valor**: 25%
- **Por cupón**: Limitado a 50 usos
- **Combinar**: Sí

### Cupón Influencer
- **Código**: `INFLUENCER20`
- **Tipo**: Porcentaje
- **Valor**: 20%
- **Por cliente**: Ilimitado
- **Combinar**: No

---

## Editar Cupón

1. Haz clic en el botón **✏️ Editar**
2. Modifica los campos necesarios
3. Haz clic en **Guardar**

> **💡 Tip**: No cambies el código de un cupón que ya se ha compartido. Mejor crea uno nuevo.

---

## Eliminar Cupón

1. Haz clic en **🗑️ Eliminar**
2. Confirma la acción

> **⚠️ Advertencia**: Eliminar un cupón es permanente. Si solo quieres deshabilitarlo, edítalo y desactiva la opción "Válido".

---

## Diferencia entre Cupones y Promociones

| Aspecto | Cupones | Promociones |
|---------|---------|-------------|
| **Requiere código** | ✅ Sí | ❌ No |
| **Aplicación** | Manual por cliente | Automática |
| **Control de usos** | Por cupón y cliente | No |
| **Ideal para** | Campañas específicas, influencers, fidelización | Ofertas generales, liquidaciones |

---

## Mejores Prácticas

### Códigos Memorables
- ✅ `VERANO2026`, `BIENVENIDO`, `VIP50`
- ❌ `XJ7K2M`, `PROMO123`, `DESC_01`

### Comunicación Clara
Al compartir un cupón, incluye:
- El código exacto
- El beneficio (% o monto)
- Condiciones (mínimo de compra, categorías)
- Fecha de vencimiento

### Tracking
- Usa códigos únicos para cada canal (INSTA20, EMAIL15)
- Monitorea los usos para evaluar efectividad
- Analiza qué cupones generan más conversiones

### Límites Inteligentes
- **Primera compra**: Para captar nuevos clientes
- **Límite por cliente**: Evita abuso
- **Límite global**: Controla el impacto financiero
- **Monto mínimo**: Aumenta el ticket promedio

### Fechas Estratégicas
- Configura períodos para eventos específicos
- No olvides desactivar cupones vencidos
- Crea urgencia con fechas de expiración cortas
