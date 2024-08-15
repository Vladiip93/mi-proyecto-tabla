# My Table Component

Vladimir Escobar

NRC: 17713

Este proyecto contiene un componente web reutilizable llamado `my-table`, desarrollado con Stencil.js. El componente toma una URL de API REST como entrada y renderiza los datos en una tabla, incluyendo la capacidad de mostrar imágenes de productos.

## Características

- Consume datos de una API REST
- Renderiza datos en una tabla responsive
- Maneja errores de carga de datos
- Muestra imágenes de productos
- Estilizado con CSS para una apariencia atractiva y consistente

## Instalación

1. Clona este repositorio:
    git clone https://github.com/tu-usuario/my-table-component.git

2. Navega al directorio del proyecto:
    cd my-table-component

3. Instala las dependencias:
    npm install

## Uso

### En un proyecto Stencil

1. Construye el componente:
    npm run build

2. Copia los archivos generados en la carpeta `dist` a tu proyecto.

3. En tu archivo HTML, importa el componente:

<script type="module" src="/path/to/my-table.esm.js"></script>

4. Usa el componente en tu HTML:

<my-table api-url="https://tu-api.com/productos"></my-table>

## Propiedades

- Propiedad: api-url
- Tipo: string
- Descripción: URL de la API REST que proporciona los datos

## Estructura de datos esperada
El componente espera que la API devuelva un array de objetos JSON. Cada objeto debe tener las siguientes propiedades:

- id: número
- nombre: string
- precio: número
- imagen: string (URL de la imagen)
- stock: número

## Personalización

### Estilos
Puedes personalizar los estilos del componente modificando el archivo my-table.css. Los estilos están encapsulados dentro del shadow DOM del componente.

### Estructura de datos
Si necesitas adaptar el componente a una estructura de datos diferente, puedes modificar el método render() en my-table.tsx.

## Desarrollo

1. Inicia el servidor de desarrollo:
    npm start

2. Abre tu navegador en http://localhost:3333

3. Realiza los cambios en los archivos src/components/my-table/

4. Los cambios se reflejarán automáticamente en el navegador

## Construcción
Para construir el componente para producción: 
    npm run build

## Contribuciones
Las contribuciones son bienvenidas. Por favor, abre un issue para discutir los cambios propuestos antes de enviar un pull request.

## Licencia
Este proyecto está licenciado bajo la licencia MIT. Consulta el archivo LICENSE para más detalles.

Este README.md proporciona una documentación completa sobre cómo instalar, usar y personalizar el componente `my-table`. Incluye información sobre la estructura de datos esperada, las propiedades del componente, cómo estilizarlo, y cómo contribuir al proyecto.

Puedes ajustar cualquier parte de este README según las necesidades específicas de tu proyecto, como agregar ejemplos más detallados, información sobre la configuración del entorno de desarrollo, o cualquier otra consideración especial para tu implementación.
