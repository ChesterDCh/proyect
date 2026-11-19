##Ragnarok Portable en Español

## Sesión 1: Título y descripción general

```markdown
# Ragnarok Portable en Español

Esta copia incluye una traducción al español del cliente, los objetos, las misiones principales, los logros,
la Caja de consejos (guía de aventura) y la guía de gremio.
Los archivos originales en inglés se conservan y se pueden restaurar en cualquier momento.
```

---

## Sesión 2: Qué se tradujo

```markdown
## Qué se tradujo

- **Interfaz y menús del cliente:** `Ragnarok/Game/data/msgstringtable.txt`
- **Nombres y descripciones de objetos:** `Ragnarok/Game/SystemES/LuaFiles514/itemInfo.lua`
- **Misiones principales:** `Ragnarok/Game/SystemES/OngoingQuests.lub`
- **Misiones recomendadas:** `Ragnarok/Game/SystemES/RecommendedQuests.lub` y `RecommendedQuests_basic.lub`
- **Categorías y filtros de misiones:** `Ragnarok/Game/SystemES/QuestClassificationInfo.lub`
- **Logros (títulos, resúmenes, detalles y progreso):** `Ragnarok/Game/SystemES/achievements.lub`
- **Caja de consejos / guía de aventura:** `Ragnarok/Game/SystemEN/tipbox.lub`
  (en la carpeta del idioma activo)
- **Guía de gremio (Alt+G):** `Ragnarok/Game/GuildTip.txt`
- **Presentación de la Guía de aventura (6 tarjetas):**
  `Ragnarok/Game/data/luafiles514/lua files/AdventureGuide/Guide_Intro.lub`
- **Ventana Hotkey Guide (etiquetas de teclas):**
  `Ragnarok/Game/data/luafiles514/lua files/msgstring_kr.lub` y `msgstring_kr_s.lub`
```

---

## Sesión 3: Cómo cambiar el idioma

```markdown
## Cómo cambiar el idioma

1. Cierra Ragnarok por completo.
2. Ejecuta `# Idioma.bat` en la carpeta principal.
   También puedes usar `# Configure-your-Ragnarok.bat` y elegir la opción **5 - Idioma / Client Language**.
3. Elige:
   - `1 - Español`
   - `2 - English`
4. Abre el cliente.

El selector intercambia las carpetas `SystemEN` y `SystemES`, copia la tabla de interfaz
correspondiente a `data/msgstringtable.txt`, cambia la guía de gremio (`GuildTip.txt`),
las etiquetas de la ventana Hotkey Guide y la presentación de la Guía de aventura.

La **Caja de consejos** se abre con `/tip`, con `Alt+D` o con el icono de la Caja de consejos.
La **guía de gremio** se abre con `Alt+G`. La **ventana Hotkey Guide** muestra las
etiquetas de las teclas de acceso rápido en español.

> **Nota:** la presentación de la Guía de aventura está traducida, pero las páginas internas
> de cada categoría (episodios, monstruos, misiones, mazmorras, armas y armaduras) siguen
> en inglés. Se pueden traducir más adelante si se desea.
```

---

## Sesión 4: Carpetas y archivos (tabla)

```markdown
## Carpetas y archivos

| Ruta | Contenido |
|---|---|
| `Ragnarok/Game/SystemEN/` | Carpeta activa que lee el cliente. Su contenido cambia según el idioma. |
| `Ragnarok/Game/SystemES/` | Copia maestra en español. Solo existe mientras el inglés está activo. |
| `Ragnarok/Game/SystemEN_EN/` | Copia maestra en inglés. Solo existe mientras el español está activo. |
| `Ragnarok/Game/data/msgstringtable.txt` | Interfaz activa. |
| `Ragnarok/Game/data/msgstringtable_es.txt` | Interfaz en español. |
| `Ragnarok/Game/data/msgstringtable_en.txt` | Interfaz en inglés (respaldo). |
| `Ragnarok/Game/GuildTip.txt` | Guía de gremio activa (Alt+G). |
| `Ragnarok/Game/GuildTip_es.txt` | Guía de gremio en español. |
| `Ragnarok/Game/GuildTip_en.txt` | Guía de gremio en inglés (respaldo). |
| `.../lua files/AdventureGuide/Guide_Intro.lub` | Presentación de la Guía de aventura activa. |
| `.../lua files/AdventureGuide/Guide_Intro_es.lub` | Presentación en español. |
| `.../lua files/AdventureGuide/Guide_Intro_en.lub` | Presentación en inglés (respaldo). |
| `.../lua files/msgstring_kr.lub` | Etiquetas de la ventana Hotkey Guide activas. |
| `.../lua files/msgstring_kr_es.lub` | Etiquetas en español. |
| `.../lua files/msgstring_kr_en.lub` | Etiquetas en inglés (respaldo). |
| `.../lua files/msgstring_kr_s.lub` | Variante activa de las etiquetas (cliente alternativo). |
| `.../lua files/msgstring_kr_s_es.lub` | Variante en español. |
| `.../lua files/msgstring_kr_s_en.lub` | Variante en inglés (respaldo). |
```

---

## Sesión 5: Notas importantes

```markdown
## Notas importantes

- La traducción se generó automáticamente y se revisó para usar terminología habitual de Ragnarok:
  **Clase** (Job), **Grupo** (Party), **Carta** (Card), **Objeto** (Item), **Puntos** (Cash),
  **Zeny**, **Mazmorra Memorial**, etc.
- Algunos nombres propios, mapas, habilidades o términos muy específicos pueden quedar en inglés.
- Los archivos originales en inglés no se borran ni se sobrescriben: al elegir **English** se restauran.
- Si el juego está abierto, el selector no podrá renombrar las carpetas. Cierra el cliente primero.
- Los archivos de texto usan codificación **CP1252/Latin-1** para que los acentos se vean correctamente
  en el cliente. No los guardes como UTF-8.
- Si algo falla, ejecuta `# Idioma.bat` y elige **English** para volver al estado original.
```

---

## Sesión 6: Herramientas de traducción (opcional)

```markdown
## Herramientas de traducción

La carpeta `OpenCode/ragnarok-es/` contiene las herramientas usadas para generar la traducción:

- `Translator.exe`: traductor reanudable con caché (`work/cache.tsv`).
- `Validator.exe`: comprobador de estructura, colores, marcadores `%s` y comillas de los archivos Lua.
- `work/`: archivos intermedios y copias de la interfaz.

No es necesario usar estas herramientas para jugar.
```
