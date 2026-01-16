# Productos

La sección de **Productos** te permite gestionar todo el catálogo de tu tienda online, incluyendo la creación, edición y organización de tus productos.

---

## Vista General

Al acceder a la sección de Productos, verás un listado con todos los productos de tu tienda organizado en una tabla con las siguientes columnas:

| Columna | Descripción |
|---------|-------------|
| **Producto** | Imagen miniatura, nombre y código del producto |
| **Precio** | Precio de venta de la variante principal |
| **Promocional** | Precio promocional (si aplica) |
| **Publicado** | Estado de visibilidad en la tienda |
| **Acciones** | Botones para editar o eliminar |

---

## Funciones Principales

### Barra de Herramientas

En la parte superior de la pantalla encontrarás los siguientes botones:

- **🔍 Buscar**: Campo de búsqueda para encontrar productos por nombre, código o descripción
- **⚙️ Filtrar**: Abre el panel lateral con filtros avanzados
- **📊 Exportar**: Descarga un archivo Excel con los productos
- **🔄 Sincronizar con ERP**: (Si está habilitado) Sincroniza productos con tu sistema de gestión
- **↕️ Ordenar catálogo**: Permite reordenar manualmente los productos
- **➕ Agregar Producto**: Crea un nuevo producto

### Filtros Avanzados

Al hacer clic en **Filtrar**, se despliega un panel lateral con las siguientes opciones:

- **Por Categoría**: Filtra productos de una o más categorías
- **Estado de Publicación**: 
  - Publicados
  - No publicados
- **Stock**:
  - Con stock
  - Sin stock
  - Stock mínimo (define una cantidad)

Los filtros activos se muestran como etiquetas debajo del buscador y pueden eliminarse individualmente o todos a la vez con "Limpiar todos".

---

## Crear Producto {#crear-producto}

Para crear un nuevo producto:

1. Haz clic en **➕ Agregar Producto**
2. Completa la información en las siguientes secciones:

### Nombre y Descripción

| Campo | Descripción | Requerido |
|-------|-------------|-----------|
| **Nombre** | Nombre del producto que verán los clientes | ✅ Sí |
| **Código** | Código interno o SKU del producto | No |
| **Descripción** | Descripción detallada con editor de texto enriquecido | No |

> **💡 Tip**: El editor de descripción permite agregar texto con formato, listas, enlaces e imágenes.

### Categorías

Selecciona una o más categorías donde aparecerá el producto. Haz clic en "Seleccionar categorías" para ver el árbol de categorías disponibles.

### Imágenes {#imágenes}

Sube las imágenes de tu producto:

1. Arrastra y suelta las imágenes en el área indicada, o
2. Haz clic para seleccionar archivos desde tu computadora

**Características:**
- Puedes subir múltiples imágenes
- Reordena las imágenes arrastrándolas
- La primera imagen será la imagen principal
- Formatos soportados: JPG, PNG, GIF, WEBP

### Video de Producto

Puedes agregar un video de YouTube al producto:

1. Ve a YouTube y copia el ID del video (la parte después de `v=` en la URL)
2. Pega solo el ID en el campo correspondiente

**Ejemplo**: Si la URL es `https://www.youtube.com/watch?v=bVYXWVs0Prc`, pega solo `bVYXWVs0Prc`

### Precios {#precios}

Configura los precios en la sección **Pricing**:

| Campo | Descripción |
|-------|-------------|
| **Precio** | Precio de venta regular |
| **Precio Promocional** | Precio con descuento (opcional) |

### Variantes {#variantes}

Si tu producto tiene diferentes opciones (talla, color, etc.), puedes crear variantes:

1. En la sección **Variantes**, haz clic en "Agregar propiedad"
2. Selecciona un atributo (ej: Talla, Color)
3. Selecciona las opciones disponibles (ej: S, M, L, XL)
4. El sistema creará automáticamente las combinaciones

**Para cada variante puedes configurar:**
- SKU específico
- Precio
- Precio promocional
- Stock
- Peso y dimensiones
- Imagen de la variante

### Filtros de Producto

Configura los filtros que permitirán a tus clientes encontrar el producto:

1. Haz clic en "Agregar filtro"
2. Selecciona el atributo (ej: Material, Temporada)
3. Selecciona los valores aplicables

### Tabla de Talles

Si vendes ropa o calzado, puedes agregar una tabla de talles:

- **Imagen**: Sube una imagen con la guía de talles
- **HTML personalizado**: Crea una tabla personalizada con el editor

### Tags/Etiquetas

Agrega etiquetas para mejorar la búsqueda y organización:

1. Escribe la etiqueta en el campo
2. Presiona Enter o coma para agregar
3. Las etiquetas se muestran como chips que puedes eliminar

### Más Opciones

| Opción | Descripción |
|--------|-------------|
| **Mostrar en la tienda** | ✅ Publica el producto para que sea visible |
| **Nuevo** | 🆕 Muestra etiqueta de "Nuevo" |
| **Destacado** | ⭐ Aparece en secciones de destacados |
| **Oferta** | 🏷️ Muestra etiqueta de oferta |
| **Agotado** | ❌ Marca el producto como sin stock |
| **Fecha de creación** | 📅 Modifica la fecha para alterar el orden en el catálogo |

---

## Editar Producto

Para editar un producto existente:

1. En el listado, haz clic en el **nombre del producto** o en el botón **✏️ Editar**
2. Realiza los cambios necesarios
3. Haz clic en **Guardar**

---

## Eliminar Producto

Para eliminar un producto:

1. Haz clic en el botón **🗑️ Eliminar** en la fila del producto
2. Confirma la eliminación en el diálogo

> **⚠️ Advertencia**: Esta acción no se puede deshacer. El producto y todas sus variantes serán eliminados permanentemente.

---

## Exportar Productos

Para exportar tu catálogo:

1. Haz clic en **📊 Exportar**
2. Selecciona el formato y las opciones deseadas
3. El archivo se descargará automáticamente

---

## Ordenar Catálogo

Para cambiar el orden de visualización de los productos:

1. Haz clic en **↕️ Ordenar catálogo**
2. Arrastra los productos para reordenarlos
3. Guarda los cambios

---

## Paginación

En la parte inferior de la pantalla encontrarás controles de paginación:

- Navega entre páginas con los botones de flecha
- Cambia la cantidad de productos por página (10, 25, 50, 100)
- Visualiza el total de productos encontrados
