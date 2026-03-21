# 📥 DESCARGA Y DEPLOY: Tu Landing en GitHub Pages en 15 Minutos

## 🎯 Lo que Necesitas

### 5 Archivos para Descargar

```
Descargados arriba ↑↑↑

1. automind-landing-mejorada.html    ← PRINCIPAL (renombra a index.html)
2. sitemap.xml                        ← Para SEO
3. robots.txt                         ← Para buscadores
4. 404.html                           ← Página de error
5. GUIA_GITHUB_PAGES_DEPLOY.md        ← Instrucciones
```

---

## 📂 PASO 1: Organizar Archivos (2 minutos)

### 1.1 Crea carpeta en tu computadora

```
En tu PC:
C:\Proyectos\                    (o ~/Projects en Mac)
  └─ automind-landing/           ← CREA ESTA CARPETA
```

### 1.2 Coloca los archivos descargados

```
automind-landing/
├── automind-landing-mejorada.html   ← Renombra a: index.html
├── sitemap.xml                      ✓
├── robots.txt                       ✓
└── 404.html                         ✓
```

**⚠️ IMPORTANTE:** Renombra `automind-landing-mejorada.html` a `index.html`

### 1.3 Verificar localmente (opcional pero recomendado)

1. Abre la carpeta `automind-landing`
2. Haz doble-click en `index.html`
3. Se abre en navegador
4. ¿Se ve bien? → Continúa
5. ¿Algo roto? → Revisa errores en F12

---

## 🔑 PASO 2: Crear Repositorio en GitHub (3 minutos)

### 2.1 Entra en GitHub

1. Ve a [github.com](https://github.com)
2. Haz login (o crea cuenta si no tienes)

### 2.2 Crear nuevo repo

1. Click en **"+"** (arriba a la derecha)
2. **"New repository"**

### 2.3 Llena el formulario

```
Repository name:     automind-landing
Description:         Landing page AUTOMIND - Soluciones Digitales
Visibility:          PUBLIC (⭐ IMPORTANTE)
README:              ☑ Initialize with README
```

### 2.4 Click "Create repository"

```
✓ Tu repo está creado!
URL: https://github.com/tu-usuario/automind-landing
```

**Copia esta URL, la necesitas.**

---

## 📤 PASO 3: Subir Archivos a GitHub (5 minutos)

### OPCIÓN A: Sin Terminal (Super Fácil) ← RECOMENDADO

#### 1. En tu repo GitHub:

Click en **"Add file"** → **"Upload files"**

#### 2. Sube tus 4 archivos:

```
Arrastra a la zona de upload:
✓ index.html           (renombrado)
✓ sitemap.xml
✓ robots.txt
✓ 404.html
```

#### 3. Completa el commit:

```
Commit message:  Initial commit - AUTOMIND landing page
              
Click: "Commit changes"
```

**¡Listo! Archivos subidos.**

---

### OPCIÓN B: Con Terminal (Si prefieres profesional)

#### 1. Abre terminal/CMD en tu carpeta

```bash
# Windows: Abre PowerShell o CMD
# Mac/Linux: Abre Terminal

# Ve a tu carpeta
cd automind-landing
```

#### 2. Copia y ejecuta estos comandos

```bash
# Inicializar git
git init

# Agregar todos los archivos
git add .

# Primer commit
git commit -m "Initial commit - AUTOMIND landing page"

# Conectar con tu repo (cambia tu-usuario)
git remote add origin https://github.com/tu-usuario/automind-landing.git

# Cambiar rama a main
git branch -M main

# Subir a GitHub
git push -u origin main
```

**Espera a que termine. ✓**

---

## ⚙️ PASO 4: Activar GitHub Pages (3 minutos)

### 4.1 En tu repo GitHub:

1. Click en **"Settings"** (pestaña arriba)
2. En el menú izquierdo: **"Pages"**

### 4.2 Configura:

```
Build and deployment:
  Source: "Deploy from a branch"
  Branch: "main"
  Folder: "/ (root)"
  
Click: "Save"
```

### 4.3 Espera a que se compile (1-2 minutos)

GitHub procesará tu sitio. Verás el mensaje:

```
✓ Your site is published at:
  https://tu-usuario.github.io/automind-landing
```

**Copia esta URL.**

---

## ✅ PASO 5: Verificar en Navegador (2 minutos)

### 5.1 Abre tu URL

```
https://tu-usuario.github.io/automind-landing
```

### 5.2 Checklist Visual

- [ ] Se ve el hero con "Automatiza tu negocio"
- [ ] Aparece la barra de features
- [ ] Se ven los 3 planes de pricing
- [ ] Están los botones (Ver planes, Consultar, WhatsApp)
- [ ] Se ve en móvil bien (F12 → Ctrl+Shift+M)
- [ ] Sin errores de CSS/JS

**Si todo OK → ¡LANZADO! 🎉**

---

## 🎨 PERSONALIZACIÓN ANTES DE LANZAR (5 minutos)

### A. Cambiar WhatsApp

En GitHub, abre `index.html`:

1. Click en el archivo `index.html`
2. Click en el ✏️ (edit button)
3. Busca: `https://wa.me/5491100000000`
4. Reemplaza con tu número:
   - Formato: `https://wa.me/CODIGOPAIS+NUMERO`
   - Ejemplo: `https://wa.me/5491140202030`
5. Commit changes

```
Mensaje: Update WhatsApp number
```

### B. Cambiar Meta Tags (SEO)

En el editor, busca (línea ~9):

```html
<meta name="description" content="AUTOMIND - ...">
```

Personaliza con tu descripción.

### C. Conectar Formulario (Para recibir leads)

1. Ve a [formspree.io](https://formspree.io)
2. Sign up con Gmail
3. "New Form"
4. Email: tu-email@gmail.com
5. Copia el **Form ID** que te da

6. En GitHub, abre `index.html`, busca:

```html
<form id="contactForm" onsubmit="handleFormSubmit(event)">
```

7. Reemplaza con:

```html
<form action="https://formspree.io/f/TU_FORM_ID" method="POST">
```

8. Commit changes

---

## 🌐 Tu Landing está VIVA

```
Tu repositorio:
https://github.com/tu-usuario/automind-landing

Tu landing en producción:
https://tu-usuario.github.io/automind-landing

SEO:
- sitemap.xml: https://tu-usuario.github.io/automind-landing/sitemap.xml
- robots.txt: https://tu-usuario.github.io/automind-landing/robots.txt
```

---

## 🔄 Cómo Actualizar Después (Muy Fácil)

### Para cambios pequeños:

```
1. En GitHub, abre el archivo
2. Click ✏️ (edit)
3. Haz cambios
4. "Commit changes"
↓
Auto-actualizado en 1-2 minutos ✓
```

### Para cambios grandes (desde tu PC):

```bash
# En tu carpeta
cd automind-landing

# Edita los archivos en tu editor

# Sube cambios
git add .
git commit -m "Descripción del cambio"
git push

↓
Auto-actualizado en 1-2 minutos ✓
```

---

## ✨ Comparativa: Donde Está Tu Landing

```
ANTES:
- En tu computadora
- No accesible públicamente
- No indexada en Google

DESPUÉS (ahora):
- En GitHub (gratis, versionado)
- Accesible en: https://tu-usuario.github.io/automind-landing
- Indexada en Google
- Auto-despliega con cada cambio
- Dominio personalizado disponible
- HTTPS automático
- Performance excelente
```

---

## 🎁 Bonus: Si Quieres Dominio Personalizado

Si tienes dominio propio (ej: automind.com):

### En GitHub:

1. Settings → Pages
2. "Custom domain"
3. Ingresa: `automind.com`
4. Save

### En tu proveedor de dominio:

Busca DNS y crea estos records:

**Para CNAME:**
```
Name: www
Value: tu-usuario.github.io
```

**Para A records (apex domain):**
```
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153
```

Espera 24-48 horas a que propague.

---

## 🆘 Si Algo Falla

### "Página en blanco o 404"

```
Causa: Probablemente archivo no se llama index.html
✓ Verifica que sea exactamente "index.html"
✓ Espera 2 minutos más
✓ Limpia cache (Ctrl+Shift+Del)
```

### "El HTML se ve pero sin estilos"

```
Causa: Muy raro en este archivo
✓ Abre Developer Tools (F12)
✓ Ve Console por errores
✓ Comparte el error en issue en GitHub
```

### "Formulario no envía"

```
Causa: No configuraste Formspree
✓ Lee sección "Conectar Formulario"
✓ Agrega tu Form ID
✓ Vuelve a hacer push
```

---

## 📋 Checklist Final

### ✅ Antes de decir "LANZADO"

```
Descarga:
☑ automind-landing-mejorada.html descargado
☑ sitemap.xml descargado
☑ robots.txt descargado
☑ 404.html descargado

Setup Local:
☑ Carpeta automind-landing creada
☑ Archivos colocados en carpeta
☑ index.html renombrado (de automind-landing-mejorada.html)
☑ Abierto en navegador local - ¿Funciona?

GitHub:
☑ Repositorio creado
☑ Visibility: PUBLIC
☑ Archivos subidos

GitHub Pages:
☑ Settings → Pages
☑ Source: "Deploy from a branch"
☑ Branch: main
☑ Folder: / (root)
☑ Saved

Verificación:
☑ Landing abierta en https://tu-usuario.github.io/automind-landing
☑ Se ve bien en desktop
☑ Se ve bien en móvil
☑ Botones funcionan
☑ Sin errores en console (F12)

Personalización:
☑ WhatsApp actualizado
☑ Meta tags personalizados
☑ Formulario conectado (opcional)

RESULTADO: ✅ LANDING VIVA Y FUNCIONANDO
```

---

## 🎯 Resumen de Tiempos

```
Paso 1: Descargar y organizar        2 min  ✓
Paso 2: Crear repo GitHub             3 min  ✓
Paso 3: Subir archivos                5 min  ✓
Paso 4: Activar GitHub Pages          3 min  ✓
Paso 5: Verificar en navegador        2 min  ✓

TOTAL: 15 minutos para estar VIVO
```

---

## 🚀 PRÓXIMO PASO

**Ahora mismo:**

1. ✅ Descarga los 4 archivos HTML (arriba)
2. ✅ Crea la carpeta `automind-landing` en tu PC
3. ✅ Coloca los archivos
4. ✅ Renombra `automind-landing-mejorada.html` → `index.html`
5. ✅ Sigue PASO 2 en adelante (GitHub)

**¡Tu landing estará en vivo en 15 minutos!**

---

## 📞 Si Necesitas Ayuda

```
Pregunta                          Respuesta
─────────────────────────────────────────────
"¿Dónde descargo?"                Arriba ↑
"¿Cómo renombro?"                 Click derecho → Rename
"¿Git qué?"                       Usa Opción A (sin terminal)
"¿URL que escribo?"               https://tu-usuario.github.io/automind-landing
"¿Cómo edito después?"            En GitHub directo o clone local
"¿Es seguro en GitHub?"           100% seguro, código HTML es público
"¿Cuánto cuesta?"                 GRATIS completamente
```

---

## 🎉 FELICIDADES

**Tu landing AUTOMIND estará:**
- ✅ En vivo en internet
- ✅ En GitHub (versionado y respaldado)
- ✅ Gratis de hosting
- ✅ Con HTTPS automático
- ✅ SEO optimizado
- ✅ Performance excelente
- ✅ Fácil de actualizar
- ✅ Listo para generar leads

**¡Tiempo de lanzar! 🚀**
