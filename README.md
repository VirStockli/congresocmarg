# 🕊️ 1º Congreso Nacional 2026 - Comunità Magnificat

**Lema:** *"No lleven dos túnicas"* **Aplicación Web:** Cronograma y Sistema de Adoración Eucarística.

Esta es una aplicación web ligera de un solo archivo (`index.html`), diseñada específicamente para el 1º Congreso Nacional de la Comunità Magnificat. Su propósito es facilitar el acceso al programa del evento y coordinar de manera comunitaria y en tiempo real los turnos de adoración nocturna.

La paleta de colores refleja la espiritualidad del lema: los tonos marrones del pájaro hornero (que evocan la providencia y el hábito monacal) entrelazados con los colores del sol y el cielo de la bandera argentina.

---

## ✨ Características Principales

* **Cero Fricción:** No requiere instalación ni creación de cuentas. Los hermanos ingresan escaneando un código QR.
* **Cronograma Integrado:** Visualización clara de las actividades de los tres días (Viernes, Sábado y Domingo).
* **Adoración en Tiempo Real:** * Coordinación de guardias nocturnas (22:00 a 08:00 hs).
  * Cupos automáticos: Se bloquea al llegar a 6 personas para asegurar la distribución.
  * Alertas visuales: Indica en rojo los turnos que no han alcanzado el mínimo sugerido (2 personas).
  * Sincronización instantánea en todos los dispositivos conectados.

---

## 🛠️ Aspectos Técnicos

El proyecto está construido con tecnologías web estándar y no requiere servidores complejos para funcionar.

* **Estructura visual:** HTML5 y CSS3 (Estilos integrados en el mismo archivo).
* **Lógica y dinamismo:** JavaScript (Vanilla).
* **Base de Datos:** Firebase Realtime Database (v8 CDN).

### Configuración de Firebase

Las credenciales de conexión están incrustadas en la sección `<script>` del archivo `index.html`. Si en el futuro es necesario cambiar el proyecto de Firebase o actualizar las llaves de seguridad, se deben modificar los valores dentro del objeto `firebaseConfig`:

```javascript
const firebaseConfig = {
    apiKey: "TU_API_KEY",
    authDomain: "tu-proyecto.firebaseapp.com",
    databaseURL: "[https://tu-proyecto.firebaseio.com](https://tu-proyecto.firebaseio.com)",
    projectId: "tu-proyecto",
    // ...
};