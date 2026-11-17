# Teoría: Componentes Modal en Astro

## 1. ¿Qué es un componente Modal?

Un modal es una ventana emergente que aparece sobre el contenido principal de una página. Se utiliza para mostrar información, formularios, confirmaciones o mensajes al usuario.

En Astro podemos crear un componente reutilizable llamado `Modal.astro`, utilizando propiedades (Props) y slots.

## 2. ¿Qué son las Props?

Las Props son propiedades que permiten enviar información desde un componente padre hacia un componente hijo.

En nuestro modal utilizaremos una prop llamada `titulo`, porque el título puede cambiar dependiendo del uso del modal.

Ejemplo:

```astro
<Modal titulo="Registro de usuario">
```

## 3. ¿Qué es un Slot?

El `<slot />` es un espacio reservado dentro de un componente donde podemos insertar contenido HTML desde otro archivo.

En nuestro modal utilizaremos un slot para insertar el contenido del formulario, ya que puede variar según la necesidad.

Ejemplo:

```astro
<Modal titulo="Registro de usuario">
  <form>
    <input type="text" placeholder="Nombre" />
    <input type="email" placeholder="Correo" />
    <button>Registrarse</button>
  </form>
</Modal>
```

## 4. ¿Qué elementos serán Props y cuáles Slots?

| Elemento | Tipo | Motivo |
|---|---|---|
| Título | Prop | Es un dato que cambia. |
| Contenido del formulario | Slot | Es contenido HTML variable. |
| Botón cerrar | Estructura fija | Se mantiene dentro del componente. |

## 5. Ventajas de utilizar Props y Slots

- Permiten reutilizar componentes.
- Evitan repetir código HTML.
- Facilitan el mantenimiento del proyecto.
- Permiten personalizar el contenido de cada componente.
- Separan la estructura del contenido.

## 6. Conclusión

Al crear un componente Modal en Astro, utilizamos Props para enviar información como el título y Slots para insertar contenido dinámico como formularios.

De esta manera, podemos utilizar un mismo componente para diferentes funcionalidades, como registro de usuarios, inicio de sesión o recuperación de contraseña.