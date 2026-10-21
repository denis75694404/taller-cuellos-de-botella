# Taller: cuellos de botella

Taller participativo en vivo: cada persona responde desde su celular, todos ven las respuestas como en un chat, votan (2 votos por persona, a propuestas distintas) y se obtiene un podio con las 3 prioridades.

- `index.html` — versión en vivo con Firebase (varios celulares, sala con código y QR).
- `pantalla-unica.html` — versión sin internet para una sola laptop + proyector.
- `firestore.rules` — reglas de seguridad para pegar en Firestore.

## Configurar Firebase (una vez)

1. Crea un proyecto en https://console.firebase.google.com
2. **Build → Authentication → Comenzar → Método de acceso → Anónimo → Habilitar.**
3. **Build → Firestore Database → Crear base de datos** (modo producción, ubicación cercana, p. ej. `southamerica-east1`).
4. En **Firestore → Reglas**, pega el contenido de `firestore.rules` y publica.
5. **Configuración del proyecto → Tus apps → Web (</>)**, registra la app y copia `firebaseConfig`.
6. Abre la página y pega esa configuración cuando la pida (o ponla en `FIREBASE_CONFIG` dentro de `index.html`).
