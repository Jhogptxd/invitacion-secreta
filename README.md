 Invitación Sorpresa (Web App Interactiva)

Una pequeña aplicación web de una sola página (SPA) diseñada para invitar a salir a esa persona especial de una forma interactiva y original. Cuenta con una temática de "hacker romántico" y una animación fluida en el fondo estilo Matrix con código y corazones cayendo.

La aplicación tiene un flujo de 4 pasos:
1. **Login falso:** Se desbloquea ingresando el nombre correcto.
2. **Selección de plan:** Una cuadrícula interactiva para elegir la actividad (cine, algo random, almuerzo).
3. **Selección de horario:** Para escoger a qué hora sincronizar la salida.
4. **Confirmación:** Un botón dinámico que envía la confirmación final directamente por WhatsApp.



 Cómo usar este código (Plantilla)

Si quieres usar este proyecto para invitar a alguien más, el código está listo para usarse de forma segura. Solo copia el código del archivo `index.html` y modifica estas dos líneas:

### 1. Cambia el nombre para desbloquear
Busca en la configuración principal (al inicio de la etiqueta `<script>`) la siguiente variable:

```javascript
const NOMBRE_VALIDO = "sofia";
```

Reemplaza `"sofia"` por el nombre de la persona a la que vas a invitar. **Nota:** Escríbelo siempre en minúsculas y sin tildes (el sistema lo reconocerá automáticamente aunque la persona lo escriba con mayúsculas en la pantalla).

### 2. Cambia el número de WhatsApp
Para que el mensaje de confirmación te llegue a tu propio teléfono, busca esta variable:

```javascript
const NUMERO_WHATSAPP = "XXXXXXXXXX";
```

Reemplaza las `X` por tu número real. Recuerda poner el código de tu país al inicio (por ejemplo `593` para Ecuador) sin el símbolo `+` y seguido de tu número celular.

---

  Tecnologías utilizadas y Arquitectura

Este proyecto está construido con un enfoque en código limpio y rendimiento nativo en el navegador:
* **HTML5 & CSS3:** Uso de Variables CSS (`:root`), Flexbox, CSS Grid para las cuadrículas de selección y funciones modernas como `clamp()` para un diseño 100% responsivo.
* **Vanilla JavaScript:** Lógica de estado sin frameworks externos.
* **Optimización de Rendimiento:** La animación del fondo (`<canvas>`) utiliza `requestAnimationFrame` en lugar de temporizadores estáticos para garantizar fluidez a 60fps sin consumir recursos excesivos ni batería en dispositivos móviles.
* **Estructuras Seguras:** El código evita por completo el uso de estructuras `do-while` para prevenir ciclos infinitos accidentales, priorizando métodos de iteración modernos y limpios como `forEach`.

---

 👨‍💻 Autor

Juan  Estudiante de Ingeniería de Software
