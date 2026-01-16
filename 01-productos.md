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

La funcionalidad de **Ordenar Catálogo** te permite definir cómo se muestran los productos en cada categoría de tu tienda.

### Acceder al Ordenamiento

1. Ve a **Productos**
2. Haz clic en **↕️ Ordenar catálogo**
3. Se abrirá la pantalla de ordenamiento

### Seleccionar Categoría

1. En el selector **Categoría**, elige la categoría que deseas ordenar
2. Las subcategorías se muestran con formato jerárquico:
   - `Ropa`
   - `Ropa > Remeras`
   - `Ropa > Remeras > Manga Corta`
3. Los productos de esa categoría se cargarán automáticamente

### Criterios de Ordenamiento

Selecciona cómo quieres ordenar los productos en el selector **Ordenar por**:

| Criterio | Descripción |
|----------|-------------|
| **Precio: menor a mayor** | Del más barato al más caro |
| **Precio: mayor a menor** | Del más caro al más barato |
| **Nombre: A → Z** | Alfabético ascendente |
| **Nombre: Z → A** | Alfabético descendente |
| **Más nuevo** | Productos más recientes primero |
| **Más viejo** | Productos más antiguos primero |
| **Orden manual** | Arrastra para personalizar el orden |

### Orden Manual (Drag & Drop)

Cuando seleccionas **Orden manual**, puedes personalizar completamente el orden:

1. Selecciona "Orden manual" en el selector
2. Aparecerá un ícono de arrastre (⋮⋮) en cada producto
3. **Para reordenar:**
   - Haz clic y mantén presionado sobre un producto
   - Arrastra a la posición deseada
   - Suelta para confirmar
4. El número de posición (#1, #2, #3...) se actualiza automáticamente

### Reordenar Rápidamente

Cuando estás en modo "Orden manual", aparece una opción especial para **reordenar productos**:

1. Verás un panel azul con la opción "Reordenar productos"
2. Selecciona un criterio base (ej: "Precio: menor a mayor")
3. Los productos se reorganizarán según ese criterio
4. Luego puedes ajustar manualmente posiciones específicas

> **💡 Tip**: Esto es útil para empezar con un orden lógico y luego destacar productos específicos moviéndolos al principio.

### Vistas de Ordenamiento

Puedes ver los productos en dos formatos:

| Vista | Descripción |
|-------|-------------|
| **Lista** | Vista compacta en filas, ideal para muchos productos |
| **Grilla** | Vista de tarjetas con imágenes más grandes |

Cambia entre vistas usando los botones **Lista** y **Grilla**.

### Información Mostrada

Cada producto muestra:
- **#N**: Número de posición actual
- **Imagen**: Miniatura del producto
- **Nombre**: Nombre del producto (clickeable para editar)
- **Precio**: Precio de la variante principal
- **Fecha de creación**: Cuándo se creó el producto

### Guardar el Orden

**¡Importante!** Los cambios NO se guardan automáticamente.

1. Realiza todos los cambios de orden que necesites
2. Haz clic en el botón **Grabar** (arriba a la derecha)
3. Espera la confirmación "Orden guardado"

> **⚠️ Advertencia**: Si sales de la página sin guardar, perderás los cambios realizados.

### Carga Infinita

Si la categoría tiene muchos productos:
- Se cargan de a 30 productos por vez
- Al hacer scroll hacia abajo, se cargan más automáticamente
- El indicador "Cargando más productos..." aparece durante la carga
- Cuando no hay más productos, verás "No hay más productos para mostrar"

### Ejemplos de Uso

#### Destacar productos nuevos
1. Selecciona "Orden manual"
2. Usa "Reordenar" con "Más nuevo"
3. Los productos recientes quedan primero
4. Guarda

#### Mostrar ofertas primero
1. Selecciona "Precio: menor a mayor"
2. Guarda
3. Los productos más económicos aparecen primero

#### Orden personalizado para landing
1. Selecciona "Orden manual"
2. Arrastra los productos destacados a las primeras posiciones
3. Organiza visualmente para máximo impacto
4. Guarda

### Consideraciones

- El orden se guarda **por categoría**
- Cada categoría puede tener su propio criterio
- Los productos en múltiples categorías pueden tener diferente orden en cada una
- El orden afecta cómo se muestran en la tienda online

---

## Paginación

En la parte inferior de la pantalla encontrarás controles de paginación:

- Navega entre páginas con los botones de flecha
- Cambia la cantidad de productos por página (10, 25, 50, 100)
- Visualiza el total de productos encontrados
