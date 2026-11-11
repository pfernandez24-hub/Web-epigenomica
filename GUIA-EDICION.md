# Cómo editar la web

Guía para el equipo. No hace falta saber programar ni instalar nada: todo se hace
desde el navegador.

- **Web publicada:** https://pfernandez24-hub.github.io/Web-epigenomica/
- **Dónde vive el texto:** el archivo `index.html`
- **Dónde vive el diseño:** la carpeta `css` (colores, tipografías, espacios)

---

## Antes de nada: ¿qué quieres cambiar?

| Lo que quieres hacer | Qué conviene |
|---|---|
| Corregir una palabra, una errata, una frase | Editar directamente aquí (sigue leyendo) |
| Añadir un párrafo o un punto a una lista | Editar directamente aquí |
| Reescribir una sección entera | Escríbelo en un documento aparte y pásaselo a Pascu |
| Cambiar colores, tipografías o la estructura | Díselo a Pascu |
| Tocar un diagrama | Díselo a Pascu |

---

## Editar un texto, paso a paso

1. Entra en el repositorio: https://github.com/pfernandez24-hub/Web-epigenomica
2. Haz clic en **`index.html`**.
3. Arriba a la derecha, pulsa el **lápiz ✏️**.
4. Busca el texto que quieres cambiar con **Ctrl+F** (Cmd+F en Mac).
5. Cámbialo respetando la regla de oro de abajo.
6. Arriba a la derecha, pulsa el botón verde **Commit changes...**.
7. En el recuadro, escribe en una línea qué has cambiado. Por ejemplo:
   *"Corregida errata en el apartado de metilación"*.
8. Pulsa **Commit changes**.

La web tarda **uno o dos minutos** en actualizarse. Si al abrirla la ves igual,
recarga con **Ctrl+F5** (Cmd+Shift+R en Mac): tu navegador está enseñándote la
copia guardada.

---

## La regla de oro

> **Cambia lo que hay entre las etiquetas. Nunca cambies las etiquetas.**

Las etiquetas son las palabras entre `<` y `>`. Van siempre en pareja: una abre y
otra cierra (la de cerrar lleva una barra `/`).

```html
<p>La epigenética estudia los cambios en la expresión génica.</p>
```

- `<p>` y `</p>` → **no se tocan**
- `La epigenética estudia...` → **esto sí se cambia**

### Las etiquetas que te vas a encontrar

| Etiqueta | Para qué sirve |
|---|---|
| `<p>` … `</p>` | Un párrafo |
| `<li>` … `</li>` | Un punto de una lista |
| `<strong>` … `</strong>` | Texto en **negrita** |
| `<em>` … `</em>` | Texto en *cursiva* |
| `<td>` … `</td>` | Una casilla de una tabla |
| `<summary>` … `</summary>` | El título de un desplegable |

### Ejemplos

**Cambiar una palabra.** Está bien:

```html
<p>El metiloma es específico de cada tipo celular.</p>
<p>El metiloma es característico de cada tipo celular.</p>
```

**Poner algo en negrita.** Está bien:

```html
<p>Esto es importante.</p>
<p>Esto es <strong>importante</strong>.</p>
```

**Añadir un punto a una lista.** Copia una línea entera y cambia su contenido:

```html
<li><strong>Cáncer:</strong> el patrón típico combina...</li>
<li><strong>Tu tema:</strong> tu texto aquí.</li>
```

**Lo que NO hay que hacer.** Esto rompe la página, porque falta la etiqueta de
cierre:

```html
<p>El metiloma es específico de cada tipo celular.
```

---

## Lo que es mejor no tocar

- Todo lo que esté entre `<svg>` y `</svg>`. Son los diagramas, y están dibujados
  con coordenadas: cambiar un número los descuadra.
- La parte de arriba del archivo, entre `<head>` y `</head>`.
- Los `id="..."` y `class="..."`. De ahí salen el diseño y los enlaces del menú.
- La carpeta `css`.

---

## Si algo se rompe

**No pasa nada y no se pierde nada.** GitHub guarda todas las versiones.

Para ver qué cambió: en el repositorio, pestaña **Commits**. Cada línea es un
cambio, con quién lo hizo y cuándo. Al abrirlo se ve en verde lo añadido y en
rojo lo quitado.

Para volver atrás, avisa a Pascu: se recupera en un minuto.

---

## Dos normas de convivencia

1. **No editéis el mismo apartado a la vez.** Si dos personas tocan el mismo
   trozo en paralelo, GitHub se queja. Repartíos las secciones y avisad por el
   grupo antes de poneros.
2. **Avisad a Pascu cuando hagáis un cambio.** Él también edita desde su
   ordenador, y necesita descargar lo vuestro antes de seguir para que no se
   pisen los cambios.

---

## Si prefieres no tocar GitHub

Totalmente válido. Escribe tu parte en un documento de Word o de Google Docs y
pásasela a Pascu, que la incorpora. Para eso va bien dejar claro **a qué
apartado** corresponde cada cosa, por ejemplo: *"Sección 02, apartado de
aplicaciones, sustituir el segundo punto por..."*.
