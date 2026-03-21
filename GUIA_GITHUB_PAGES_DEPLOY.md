# 🚀 Deploy en GitHub + GitHub Pages: Guía Completa

## 📋 Resumen Rápido

```
Objetivo: Tu landing HTML en GitHub Pages
Tiempo: 15-20 minutos
Costo: Gratis (100% GitHub Pages)
Resultado: Tu sitio en https://tu-usuario.github.io/automind-landing
```

---

## PASO 1: Preparar Tus Archivos Localmente (5 minutos)

### 1.1 Crea una carpeta en tu computadora

```bash
# En tu carpeta de proyectos
mkdir automind-landing
cd automind-landing
```

### 1.2 Descarga estos archivos y colócalos en la carpeta

Los archivos necesarios son:
```
automind-landing/
├── index.html              ← Renombra automind-landing-mejorada.html a esto
├── sitemap.xml
├── robots.txt
└── 404.html
```

**Estructura exacta que necesitas:**

```bash
automind-landing/
│
├── index.html              # El archivo HTML principal (renombrado)
├── sitemap.xml             # Para SEO
├── robots.txt              # Para buscadores
└── 404.html                # Página de error personalizada
```

### 1.3 Verificar que los archivos estén correctos

Abre `index.html` en tu navegador (drag & drop):
- ¿Se ve la landing? ✓
- ¿Funcionan los botones? ✓
- ¿Se ve en móvil? ✓

Si todo funciona, continúa.

---

## PASO 2: Crear Repositorio en GitHub (5 minutos)

### 2.1 Crea cuenta en GitHub (si no tienes)

1. Ve a [github.com](https://github.com)
2. Click **"Sign up"**
3. Completa los datos
4. Verifica tu email

### 2.2 Crea nuevo repositorio

1. Haz login en GitHub
2. Click en **"+"** (esquina arriba a la derecha)
3. **"New repository"**

### 2.3 Configura el repositorio

```
Repository name: automind-landing
Description: Landing page AUTOMIND - Soluciones Digitales
Visibility: Public (IMPORTANTE para GitHub Pages)
Initialize with README: Sí
```

4. Click **"Create repository"**

### 2.4 URL de tu repositorio

Se verá algo así:
```
https://github.com/tu-usuario/automind-landing
```

**Copia esta URL, la necesitarás.**

---

## PASO 3: Subir Archivos a GitHub (5 minutos)

### Opción A: Sin Terminal (Más Fácil)

#### 1. En tu repositorio GitHub:

1. Click en **"Add file"** → **"Upload files"**

#### 2. Sube tus archivos:

Arrastra estos 4 archivos a la zona de upload:
- `index.html`
- `sitemap.xml`
- `robots.txt`
- `404.html`

#### 3. Commit:

- Mensaje: `Initial commit - AUTOMIND landing page`
- Click **"Commit changes"**

**¡Listo! Tus archivos están en GitHub.**

---

### Opción B: Con Git/Terminal (Más profesional)

#### 1. Instala Git

Descarga desde [git-scm.com](https://git-scm.com)

#### 2. En tu terminal:

```bash
# Ve a tu carpeta
cd automind-landing

# Inicializa git
git init

# Agregar todos los archivos
git add .

# Hacer commit
git commit -m "Initial commit - AUTOMIND landing page"

# Conectar con GitHub (reemplaza con tu URL)
git remote add origin https://github.com/tu-usuario/automind-landing.git

# Rename rama a main (si es necesario)
git branch -M main

# Subir a GitHub
git push -u origin main
```

**Espera a que termine. ¡Listo!**

---

## PASO 4: Activar GitHub Pages (3 minutos)

### 4.1 En tu repositorio GitHub:

1. Click en **"Settings"** (pestañas arriba)
2. En el menú izquierdo: **"Pages"**

### 4.2 Configura GitHub Pages:

En la sección "Build and deployment":

- **Source:** Selecciona **"Deploy from a branch"**
- **Branch:** Selecciona **"main"**
- **Folder:** Selecciona **"/ (root)"**
- Click **"Save"**

### 4.3 Espera el deploy (1-2 minutos)

GitHub compilará tu sitio. Verás un mensaje:

```
✓ Your site is published at: 
  https://tu-usuario.github.io/automind-landing
```

**¡LISTO! Tu landing está en vivo!**

---

## PASO 5: Verificar que Todo Funciona (2 minutos)

### 5.1 Abre tu URL

```
https://tu-usuario.github.io/automind-landing
```

### 5.2 Verifica:

- [ ] La landing se ve correctamente
- [ ] Todos los botones funcionan
- [ ] Se ve bien en móvil (F12 → Ctrl+Shift+M)
- [ ] El formulario está presente
- [ ] Los colores se ven bien
- [ ] Sin errores en consola (F12)

### 5.3 Si algo no funciona:

```
Problema: Página en blanco
↓
Solución:
1. Asegúrate que el archivo se llama index.html (exacto)
2. Espera 5 minutos más (GitHub Pages tarda)
3. Limpia cache del navegador (Ctrl+Shift+Del)
4. Abre en navegador privado

Problema: Formulario no funciona
↓
Solución: Necesitas conectar Formspree
1. Ve a PERSONALIZACION_RAPIDA_AUTOMIND.md
2. Sección "Formulario"
3. Agrega tu Form ID de Formspree
```

---

## PASO 6: Personalización Rápida (Antes de lanzar)

### 6.1 Editar en GitHub directamente

Para cambios pequeños (sin descargar nada):

1. En tu repo, abre `index.html`
2. Click en el lápiz (edit)
3. Edita lo que necesites
4. Abajo: **"Commit changes"**
5. Message: **"Update landing content"**
6. **"Commit"**

GitHub Pages se actualiza automáticamente en 1-2 minutos.

### 6.2 Editar localmente (cambios mayores)

```bash
# En tu carpeta automind-landing/

# 1. Abre index.html con editor (VS Code, Notepad++, etc)
# 2. Haz cambios
# 3. Guarda

# 4. En terminal:
git add .
git commit -m "Update - cambios en landing"
git push

# GitHub Pages se actualiza automáticamente
```

---

## Cambios Recomendados Antes de Lanzar

### META TAGS (para SEO)

En `index.html`, línea ~9:

```html
<meta name="description" content="AUTOMIND - Soluciones digitales integrales. Bot automático, QR personalizado, sistema de citas. Transforma tu empresa.">
```

**Personaliza:** Reemplaza con tu descripción.

### WhatsApp

En `index.html`, busca:
```html
<a href="https://wa.me/5491100000000">WHATSAPP</a>
```

**Reemplaza:** Tu número de WhatsApp.

Formato: `https://wa.me/CODIGOPAIS+NUMERO`
Ejemplo: `https://wa.me/5491140202030`

### Formulario (Opcional)

Si quieres que envíe emails:

1. Ve a [formspree.io](https://formspree.io)
2. Crea formulario con tu email
3. Copia el Form ID
4. En `index.html`, busca:

```html
<form id="contactForm" onsubmit="handleFormSubmit(event)">
```

5. Reemplaza con:

```html
<form action="https://formspree.io/f/TU_FORM_ID" method="POST">
```

6. Commit y push:

```bash
git add .
git commit -m "Connect form to Formspree"
git push
```

---

## Estructura Final en GitHub

Cuando termines, tu repositorio se verá así:

```
automind-landing/
├── .git/                    (Carpeta oculta de Git)
├── index.html               ✓ Landing principal
├── sitemap.xml              ✓ Para SEO
├── robots.txt               ✓ Para buscadores  
├── 404.html                 ✓ Página de error
├── README.md                (Descripción del proyecto)
└── .gitignore               (Opcional)
```

En GitHub verás una carpeta con estos archivos.

---

## URLs Finales

```
Tu repositorio:
https://github.com/tu-usuario/automind-landing

Tu landing en vivo:
https://tu-usuario.github.io/automind-landing

Sitemap para Google:
https://tu-usuario.github.io/automind-landing/sitemap.xml

robots.txt:
https://tu-usuario.github.io/automind-landing/robots.txt
```

---

## Actualizar tu Landing (Después del Launch)

### Cambios pequeños (directamente en GitHub):

```
GitHub web → Edit archivo → Commit
↓
Auto-deploy en 1-2 minutos
```

### Cambios mayores (desde tu computadora):

```bash
cd automind-landing/

# Edita los archivos en tu editor

git add .
git commit -m "Descripción del cambio"
git push

# Auto-deploy en 1-2 minutos
```

---

## Configurar Dominio Personalizado (Opcional)

Si tienes dominio propio (ej: automind.com):

### En GitHub:

1. Settings → Pages
2. "Custom domain"
3. Ingresa: `automind.com`
4. Click "Save"

### En tu proveedor de dominio (Godaddy, Namecheap, etc):

1. Dashboard → DNS
2. Crear CNAME record:
   - Name: `www`
   - Value: `tu-usuario.github.io`

3. Crear A record (para apex domain):
   - Apunta a IPs de GitHub:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153

4. Guarda cambios (propagar: 24-48 horas)

GitHub automáticamente obtendrá SSL/HTTPS.

---

## Troubleshooting

### "Página no encontrada (404)"

```
Causa: Archivo no se llama index.html
Solución: Renombra a index.html exactamente
```

### "Sitio en blanco"

```
Causa: HTML con errores de sintaxis
Solución:
1. Abre en navegador local (valida HTML)
2. Abre Developer Tools (F12)
3. Ve Console (busca errores)
4. Arregla el error
5. Push a GitHub
```

### "Cambios no se ven"

```
Causa: Cache del navegador
Solución:
1. Ctrl+Shift+Del (limpiar cache)
2. Abre navegador privado/incógnito
3. Espera 2-3 minutos (GitHub tarda)
```

### "Formulario no envía"

```
Causa: Formspree no conectado
Solución: Lee sección "Formulario" arriba
```

---

## Buenas Prácticas

### ✅ HACES

```
✓ Commit messages claros
✓ Un cambio por commit
✓ Commits frecuentes
✓ Documentación en README.md
✓ Backup local en tu PC
```

### ❌ EVITAS

```
✗ Subir archivos basura
✗ Passwords o tokens en código
✗ Commits gigantes sin descripción
✗ Editar directamente en GitHub (para cambios grandes)
```

---

## README.md: Haz uno bonito

En tu repositorio, crea `README.md`:

```markdown
# AUTOMIND Landing Page

Soluciones digitales integrales para tu empresa.

## Características

- ✓ Bot automático 24/7
- ✓ QR personalizado
- ✓ Sistema de citas automático
- ✓ Análisis en tiempo real

## Acceso

🌐 [Ver landing en vivo](https://tu-usuario.github.io/automind-landing)

## Editar

1. Clone el repo:
   ```bash
   git clone https://github.com/tu-usuario/automind-landing.git
   ```

2. Haz cambios en `index.html`

3. Push a GitHub:
   ```bash
   git add .
   git commit -m "Tu cambio"
   git push
   ```

## Deploy

GitHub Pages auto-deploya en 1-2 minutos.

## Contacto

📧 tu-email@example.com
💬 [WhatsApp](https://wa.me/5491100000000)

---

*Última actualización: [fecha]*
```

---

## Checklist Final

### Antes de lanzar:
- [ ] Archivos descargados en carpeta local
- [ ] Repositorio GitHub creado
- [ ] Archivos subidos a GitHub
- [ ] GitHub Pages activado
- [ ] Landing abierto en navegador
- [ ] Se ve correcto en desktop y móvil
- [ ] Formulario funciona (opcional)
- [ ] WhatsApp actualizado
- [ ] Meta tags personalizados
- [ ] README.md completo

### Después de lanzar:
- [ ] Compartir URL con team
- [ ] Monitorear en Google Search Console
- [ ] Agregar Google Analytics
- [ ] Hacer backup local

---

## URLs de Referencia

| Servicio | URL |
|----------|-----|
| GitHub | https://github.com |
| Git instalable | https://git-scm.com |
| Formspree | https://formspree.io |
| Google Search Console | https://search.google.com/search-console |
| Google Analytics | https://analytics.google.com |

---

## Soporte Rápido

**P: ¿Cómo veo cambios en vivo?**
A: GitHub Pages actualiza en 1-2 minutos después de push.

**P: ¿Puedo tener dominio personalizado?**
A: Sí, ver sección "Configurar Dominio Personalizado".

**P: ¿Es gratis completamente?**
A: Sí, GitHub Pages es 100% gratis.

**P: ¿Qué pasa si me equivoco?**
A: Git tiene historial. Puedes revertir en cualquier momento.

**P: ¿Cómo colabora el team?**
A: Cada uno clona el repo, hace cambios, y push.

---

## Resumen: Tu Journey en 20 minutos

```
Minuto 0-5:   Descargar y organizar archivos locales
Minuto 5-10:  Crear repo GitHub
Minuto 10-15: Subir archivos
Minuto 15-17: Activar GitHub Pages
Minuto 17-20: Verificar que está en vivo

RESULTADO:
Tu landing AUTOMIND en vivo en:
https://tu-usuario.github.io/automind-landing
```

---

**¡Estás listo para hacer deploy! 🚀**

¿Necesitas ayuda en algún paso? Pregunta y te lo resuelvo.
