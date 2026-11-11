# EVEA 2.0 - Laboratorio de Medios: El salto a lo digital

**Institución:** Colegio Superior Presidente Roque Sáenz Peña  
**Materia:** Residencia 2 - Profesorado del Consudec  
**Curso:** 2.° Año B - Turno Tarde  
**Co-formador:** Prof. Walter Guzmán  
**Practicante:** Emmanuel Galiotti  

---

## 📌 Descripción del Entorno

**EVEA 2.0 - Laboratorio de Medios** es un Entorno Virtual de Enseñanza y Aprendizaje interactivo desarrollado con **HTML5, CSS3 y JavaScript vanilla** sin dependencias externas, pensado con una estética inmersiva de escritorio de laboratorio y navegación por estaciones mediante un **Menú de Inicio** con iconos grandes para las 5 fases didácticas.

Todas las rutas a recursos locales son **relativas** (`./assets/...`), lo que garantiza compatibilidad inmediata tanto en local como publicado en **GitHub Pages**.

---

## 📁 Estructura del Repositorio

```text
/
├── index.html             # Aplicación principal autocontenida (EVEA 2.0)
├── README.md              # Documentación y guía de despliegue en GitHub Pages
└── assets/
    └── infografia.png     # Infografía: Muestreo y Cuantificación (colocar aquí)
```

---

## ⚙️ Preparación Antes de Publicar

Antes de subir el proyecto a GitHub Pages, completá estos dos pasos simples:

1. **Agregar la infografía:** Guardá tu archivo de imagen con el nombre exacto `infografia.png` dentro de la carpeta [`./assets/`](./assets/) para que cargue automáticamente desde la ruta relativa `./assets/infografia.png` en la Fase 2 (*Contenido*).
2. **Vincular tu Google Form:**
   - Abrí tu formulario en Google Forms y hacé clic en **Enviar → Incorporar HTML (`<>`)**.
   - Copiá la URL del atributo `src` (finaliza en `?embedded=true`).
   - Abrí [`index.html`](./index.html), buscá `URL_DE_TU_GOOGLE_FORM` y reemplazalo por esa URL.

---

## 🚀 Pasos para Subir y Publicar en GitHub Pages

### Opción A: Desde la Web de GitHub (sin usar consola)

1. Iniciá sesión en [GitHub](https://github.com/) y hacé clic en **New repository** (`+` → *New repository*).
2. Asignale un nombre al repositorio (por ejemplo: `evea-laboratorio-medios`), seleccionalo como **Public** y hacé clic en **Create repository**.
3. Hacé clic en **uploading an existing file** (o **Add file → Upload files**).
4. Arrastrá y subí manteniendo la estructura de carpetas:
   - `index.html`
   - `README.md`
   - La carpeta `assets/` con `infografia.png` adentro.
5. Hacé clic en **Commit changes** para guardar los archivos en la rama `main`.
6. Andá a la pestaña **Settings** del repositorio y, en el menú lateral izquierdo, seleccioná **Pages**.
7. En **Build and deployment → Source**, elegí **Deploy from a branch**.
8. En **Branch**, seleccioná **`main`** y la carpeta **`/ (root)`**, y presioná **Save**.
9. Esperá entre 1 y 2 minutos y recargá la página de *Pages*: aparecerá el enlace público de tu EVEA con el formato:
   `https://tu-usuario.github.io/evea-laboratorio-medios/`

### Opción B: Desde la Terminal con Git

```bash
git init
git add index.html README.md assets/
git commit -m "Publicar EVEA 2.0 - Laboratorio de Medios"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/evea-laboratorio-medios.git
git push -u origin main
```

Luego activá **Settings → Pages → Branch: `main` / `(root)`** desde GitHub.

### (Opcional) Incrustar en Google Sites

Una vez publicado en GitHub Pages, podés embeber el laboratorio en Google Sites desde **Insertar → Incorporar → Por URL** pegando la URL pública de GitHub Pages, o usando:

```html
<iframe
  src="https://tu-usuario.github.io/evea-laboratorio-medios/"
  width="100%"
  height="950px"
  style="border: none; border-radius: 12px;"
  title="EVEA 2.0 - Laboratorio de Medios">
</iframe>
```

---

## 🧩 Estructura de las 5 Estaciones del Laboratorio

1. **1. Convocar:** Pregunta disparadora, comparador en vivo de reloj analógico continuo vs. reloj digital discreto y encuesta interactiva del perfil tecnológico.
2. **2. Contenido:** Teoría multimodal, simulador interactivo de ondas y ruido en Canvas, metáfora interactiva rampa vs. escalones (muestreo y cuantificación), cuadro comparativo filtrable (Casete vs. MP3) y sección **🎥 Recursos Audiovisuales y Visuales** (video de YouTube responsivo e infografía).
3. **3. Actividad:** Consigna *Arqueología Tecnológica*, formulario guiado con ejemplo precargado, guardado local, exportación en `.txt` y copia rápida para entregar a través del formulario de evaluación adjunto.
4. **4. Evaluación:** Rúbrica formativa, quiz de autoverificación inmediata, bitácora de metacognición y bloque integrado **📝 Autoevaluación y Entrega Final** mediante Google Form.
5. **5. Consultas:** Datos institucionales y de contacto, buscador de preguntas frecuentes (FAQ en acordeón) y muro colaborativo de consultas.
