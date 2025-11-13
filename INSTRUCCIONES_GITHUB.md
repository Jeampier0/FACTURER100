# 📚 Guía para Publicar tu HTML en GitHub

## Paso 1: Crear un Repositorio en GitHub

1. Ve a [GitHub.com](https://github.com) e inicia sesión
2. Haz clic en el botón **"+"** (arriba a la derecha) y selecciona **"New repository"**
3. Completa los datos:
   - **Repository name**: `generador-facturas` (o el nombre que prefieras)
   - **Description**: "Generador de facturas electrónicas"
   - **Visibilidad**: Elige **Public** (necesario para GitHub Pages gratuito)
   - **NO marques** "Initialize this repository with a README"
4. Haz clic en **"Create repository"**

## Paso 2: Inicializar Git en tu Carpeta Local

Abre PowerShell o Terminal en la carpeta del proyecto y ejecuta estos comandos:

```powershell
# Inicializar git
git init

# Agregar todos los archivos
git add .

# Hacer el primer commit
git commit -m "Primera versión del generador de facturas"

# Conectar con tu repositorio de GitHub (reemplaza TU_USUARIO con tu nombre de usuario)
git remote add origin https://github.com/TU_USUARIO/generador-facturas.git

# Cambiar a la rama main (si es necesario)
git branch -M main

# Subir los archivos a GitHub
git push -u origin main
```

**Nota**: La primera vez que hagas `git push`, GitHub te pedirá autenticarte. Puedes usar:
- Tu token de acceso personal (recomendado)
- O GitHub CLI

## Paso 3: Activar GitHub Pages

1. Ve a tu repositorio en GitHub
2. Haz clic en **"Settings"** (Configuración)
3. En el menú lateral, busca **"Pages"**
4. En **"Source"**, selecciona:
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Haz clic en **"Save"**

## Paso 4: Acceder a tu Sitio Web

Después de unos minutos, tu sitio estará disponible en:
```
https://TU_USUARIO.github.io/generador-facturas/
```

## 🔄 Actualizar tu Sitio

Cada vez que hagas cambios, ejecuta:

```powershell
git add .
git commit -m "Descripción de los cambios"
git push
```

Los cambios aparecerán en tu sitio en unos minutos.

## 📝 Notas Importantes

- El archivo `index.html` es el que GitHub Pages mostrará automáticamente
- Si cambias algo, espera 1-2 minutos para que se actualice
- Puedes verificar el estado del despliegue en la pestaña **"Actions"** de tu repositorio

