# Cómo cambiar las fechas del programa

Las fechas del sitio (la fecha de inicio y todo el cronograma de encuentros) están
en un solo archivo llamado **`datos.json`**. Cambiás las fechas ahí y el sitio se
actualiza solo. No hace falta tocar nada más.

---

## Paso a paso

### 1. Entrar a GitHub

- Andá a **https://github.com** e iniciá sesión con tu usuario.

### 2. Ir al repositorio del sitio

- Abrí este enlace: **https://github.com/Evesujo/page**
- (Es el repositorio donde vive tu página.)

### 3. Abrir el archivo `datos.json`

- En la lista de archivos, hacé clic en **`datos.json`**.
- Enlace directo: **https://github.com/Evesujo/page/blob/main/datos.json**

### 4. Editar

- Arriba a la derecha del archivo, hacé clic en el **lápiz** ✏️ ("Edit this file").
- Cambiá solo el texto que está **entre comillas**. Por ejemplo:

  ```
  "inicio": "25 de julio",
  ```

  lo cambiás por:

  ```
  "inicio": "1 de agosto",
  ```

- Para el cronograma, cada encuentro tiene su `"fecha"`. Cambiás solo lo que está
  entre comillas:

  ```
  "fecha": "Sábado 8/8 · 10.30 a 12.30hs",
  ```

### 5. Guardar

- Bajá hasta el final y hacé clic en el botón verde **"Commit changes"**.
- Volvé a hacer clic en **"Commit changes"** en la ventanita que aparece.

¡Listo! En 1 o 2 minutos el sitio muestra las fechas nuevas.
(Puede que tengas que refrescar la página con `Ctrl + F5`.)

---

## Reglas importantes para no romper el archivo

- ✅ Cambiá **solo el texto entre comillas**.
- ✅ Cada línea con texto termina en **coma** `,` (salvo la última de cada bloque).
  Si ya venía con coma, dejala.
- ❌ **No borres** las comillas `"`, las llaves `{ }` ni los corchetes `[ ]`.
- ❌ No cambies los nombres de la izquierda (`"inicio"`, `"fecha"`, `"titulo"`, etc.).

Si algo se ve raro después de un cambio, avisame y lo reviso.

---

## Qué es cada cosa en `datos.json`

- **`inicio`** → el texto que aparece en la etiqueta **"Inicia el …"** del inicio.
- **`encuentros`** → la lista de los 8 encuentros. Cada uno tiene:
  - `fecha` → la fecha y horario del encuentro.
  - `titulo` → el nombre del encuentro.
  - `invitado` → el nombre de quien acompaña (si no hay, se deja `""` vacío).
  - `descripcion` → el texto que explica el encuentro.
