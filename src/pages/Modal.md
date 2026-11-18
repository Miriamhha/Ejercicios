## 1. ¿Qué elementos serán Props y cuáles Slots?

| Elemento | Tipo | Motivo |
|---|---|---|
| Título | Prop | Es un dato que cambia. |
| Contenido del formulario | Slot | Es contenido HTML variable. |
| Botón cerrar | Estructura fija | Se mantiene dentro del componente. |

## 2. Las Ventajas de utilizar Props y Slots

- Permiten reutilizar componentes.
- Evitan repetir código HTML.
- Facilitan el mantenimiento del proyecto.
- Permiten personalizar el contenido de cada componente.
- Separan la estructura del contenido.

## 3. Conclusión

Al crear un componente Modal en Astro, utilizamos Props para enviar información como el título y Slots para insertar contenido dinámico como formularios.

De esta manera, podemos utilizar un mismo componente para diferentes funcionalidades, como registro de usuarios, inicio de sesión o recuperación de contraseña.