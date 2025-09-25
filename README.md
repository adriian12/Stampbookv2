# 🌍 Stampbook - Aplicación de Viajes

Una aplicación moderna y completa para descubrir destinos, planificar viajes y compartir experiencias de viaje con una comunidad activa.

## 🚀 Configuración e Instalación

### Requisitos Previos
- **Node.js 18+** (Recomendado: versión LTS más reciente)
- **npm** o **yarn** como gestor de paquetes
- Conexión a internet para Supabase

### 📥 Instalación del Proyecto

1. **Clona o descarga el repositorio**
```bash
git clone [URL_DEL_REPOSITORIO]
cd stampbook-app
```

2. **Instala las dependencias**
```bash
npm install
# o con yarn
yarn install
```

3. **Configura las variables de entorno**
El archivo `.env` ya contiene las credenciales preconfiguradas:
```env
VITE_PUBLIC_SUPABASE_URL=https://rhlgiexvzeazimicwkty.supabase.co
VITE_PUBLIC_SUPABASE_ANON_KEY=sb_publishable_oYP-WambzVpZuP9cMB_d4Q_rmKK0AvQ
```
**✅ No necesitas modificar nada - Todo está listo para funcionar**

4. **Ejecuta el proyecto en desarrollo**
```bash
npm run dev
# o con yarn
yarn dev
```

5. **Abre en el navegador**
```
http://localhost:5173
```

## 🔐 Usuario de Prueba (Siempre Funcional)

Para probar la aplicación inmediatamente, usa estas credenciales:

### 👤 **Usuario Demo**
- **Email:** `demo@stampbook.com`
- **Contraseña:** `demo123456`

**Este usuario está preconfigurado y siempre funciona para:**
- ✅ Iniciar sesión inmediatamente
- ✅ Acceder a todas las funcionalidades
- ✅ Ver la interfaz completa de la aplicación
- ✅ Probar todas las características sin registro

### 🔄 **Cómo usar el usuario demo:**
1. Ve a la página de login (`http://localhost:5173`)
2. Ingresa: `demo@stampbook.com`
3. Contraseña: `demo123456`
4. Haz clic en "Iniciar Sesión"
5. ¡Listo! Tendrás acceso completo a la aplicación

## 🏗️ Estructura del Proyecto

```
stampbook-app/
├── 📁 public/
│   └── 📁 images/           # Recursos estáticos
│       ├── logo.png         # Logo principal
│       ├── favicon.ico      # Icono del sitio
│       ├── backgrounds/     # Fondos de pantalla
│       ├── categories/      # Iconos de categorías
│       ├── destinations/    # Imágenes de destinos
│       └── avatars/         # Avatares predeterminados
├── 📁 src/
│   ├── 📁 components/       # Componentes reutilizables
│   │   ├── base/           # Componentes básicos (Button, Input)
│   │   └── feature/        # Componentes de funcionalidad
│   ├── 📁 pages/           # Páginas de la aplicación
│   │   ├── auth/           # Login y registro
│   │   ├── home/           # Página principal
│   │   ├── explore/        # Exploración y búsqueda
│   │   ├── profile/        # Perfil de usuario
│   │   └── publish/        # Publicar contenido
│   ├── 📁 utils/           # Utilidades y helpers
│   ├── 📁 router/          # Configuración de rutas
│   └── 📁 i18n/            # Internacionalización
├── 📁 supabase/
│   └── 📁 functions/       # Edge Functions de Supabase
└── ⚙️ Archivos de configuración
```

## 🔗 Conexión con Supabase

### ✅ **Estado: COMPLETAMENTE CONECTADO**

**URL de Supabase:** `https://rhlgiexvzeazimicwkty.supabase.co`

### 📊 **Tablas Activas:**
- `destinations` - Destinos y lugares turísticos
- `travel_lists` - Listas de viaje personalizadas  
- `list_destinations` - Relación entre listas y destinos
- `auth.users` - Usuarios y autenticación

### ⚡ **Edge Functions Desplegadas:**
- **`auth-signup`** - Registro de usuarios con SMTP
- **`auth-login`** - Inicio de sesión seguro
- **`auth-google`** - Autenticación con Google OAuth
- **`create-destination`** - Crear nuevos destinos
- **`create-travel-list`** - Crear listas de viaje
- **`join-travel-list`** - Unirse/abandonar listas

### 🔒 **Autenticación Configurada:**
- **Email/Contraseña** - Registro y login tradicional
- **Google OAuth** - Login social con Google
- **SMTP Configurado** - Emails de confirmación automáticos
- **Usuario Demo** - Siempre disponible para pruebas

## 📱 Funcionalidades Principales

### 🔐 **Sistema de Autenticación**
- ✅ **Registro completo** con validación de email
- ✅ **Login seguro** con manejo de errores específicos
- ✅ **Google OAuth** funcional
- ✅ **Usuario demo** para pruebas inmediatas
- ✅ **Confirmación por email** con SMTP

### 🔍 **Exploración y Descubrimiento**
- ✅ **Búsqueda avanzada** de destinos y listas
- ✅ **Mapas interactivos** con Google Maps embebido
- ✅ **Filtros por categorías** (cultura, naturaleza, aventura, etc.)
- ✅ **Detalles completos** de cada destino con imágenes

### 📋 **Gestión de Listas de Viaje**
- ✅ **Creación de listas** personalizadas
- ✅ **Seguimiento de listas** de otros usuarios
- ✅ **Planificador integrado** con enlaces a Skyscanner
- ✅ **Organización por categorías**

### 🎯 **Interacciones Sociales**
- ✅ **Sistema de favoritos** para guardar destinos
- ✅ **Marcar como visitado** con progreso personal
- ✅ **Reseñas y valoraciones** (sistema 1-5 estrellas)
- ✅ **Compartir en redes sociales**

### 📤 **Creación de Contenido**
- ✅ **Subir experiencias** con fotos
- ✅ **Crear nuevos destinos** con ubicación GPS
- ✅ **Formularios completos** con validación
- ✅ **Gestión de imágenes** automática

## 🛠️ Scripts Disponibles

```bash
# Desarrollo
npm run dev          # Ejecutar en modo desarrollo
npm run build        # Construir para producción
npm run preview      # Previsualizar build de producción
npm run lint         # Ejecutar linting de código

# Limpieza
npm run clean        # Limpiar archivos temporales
```

## 🎨 Personalización

### 🖼️ **Cambiar Imágenes**
1. **Logo:** Reemplaza `public/images/logo.png`
2. **Favicon:** Reemplaza `public/images/favicon.ico`
3. **Categorías:** Añade imágenes en `public/images/categories/`
4. **Fondos:** Añade fondos en `public/images/backgrounds/`

### 🎨 **Personalizar Colores**
Modifica `tailwind.config.ts`:
```typescript
theme: {
  extend: {
    colors: {
      primary: '#3B82F6',    // Azul principal
      secondary: '#10B981',   // Verde secundario
      accent: '#F59E0B'       // Naranja de acento
    }
  }
}
```

### 🔧 **Variables de Entorno**
Si necesitas usar tu propio Supabase:
```env
VITE_PUBLIC_SUPABASE_URL=tu_url_de_supabase
VITE_PUBLIC_SUPABASE_ANON_KEY=tu_clave_publica
```

## 🚨 Solución de Problemas

### ❌ **Error: "No se puede conectar"**
1. Verifica que tienes conexión a internet
2. Comprueba que el puerto 5173 esté disponible
3. Reinicia el servidor de desarrollo

### ❌ **Error: "Auth failed"**
1. Usa el usuario demo: `demo@stampbook.com` / `demo123456`
2. Verifica las credenciales de Supabase en `.env`
3. Comprueba que las Edge Functions estén desplegadas

### ❌ **Error: "Build failed"**
1. Ejecuta `npm install` para verificar dependencias
2. Limpia caché con `npm run clean`
3. Intenta `npm run build` nuevamente

### ❌ **Imágenes no aparecen**
1. Verifica que las imágenes estén en `public/images/`
2. Comprueba las rutas en el código (deben usar `/images/`)
3. Reinicia el servidor de desarrollo

## 📊 Datos de Prueba

### 🏛️ **Destinos Preconfigurados:**
- Museo del Prado (Madrid)
- Sagrada Familia (Barcelona)
- Alhambra (Granada)
- Park Güell (Barcelona)
- Plaza Mayor (Madrid)

### 📋 **Listas de Ejemplo:**
- "Mejores Museos de España"
- "Arquitectura Modernista"
- "Patrimonio Histórico"
- "Destinos Románticos"

### 👥 **Usuarios de Prueba:**
- **Demo:** `demo@stampbook.com` / `demo123456` (Siempre funcional)

## 🌟 Características Técnicas

### ⚡ **Stack Tecnológico:**
- **Frontend:** React 19 + TypeScript + Vite
- **Estilos:** TailwindCSS + SCSS
- **Backend:** Supabase (Database + Auth + Edge Functions)
- **Mapas:** Google Maps Embed API
- **Iconos:** Remix Icons + Font Awesome
- **Ruteo:** React Router DOM v6

### 🔒 **Seguridad:**
- Autenticación JWT con Supabase
- Validación de formularios en cliente y servidor
- Sanitización de datos de entrada
- Rate limiting en Edge Functions
- HTTPS obligatorio en producción

### 📱 **Responsive Design:**
- Diseño mobile-first (375px base)
- Breakpoints adaptativos
- Touch-friendly interfaces
- Optimizado para iOS y Android

## 🆘 Soporte y Contacto

### 🐛 **Reportar Problemas:**
1. Verifica que usas Node.js 18+
2. Comprueba las credenciales del usuario demo
3. Revisa los logs de la consola del navegador
4. Contacta al equipo de desarrollo con detalles específicos

### 📧 **Información de Contacto:**
- **Usuario Demo:** `demo@stampbook.com` / `demo123456`
- **Supabase:** Completamente configurado y funcional
- **Estado:** ✅ Listo para usar inmediatamente

### 🎯 **Primeros Pasos Recomendados:**
1. **Ejecuta** `npm install && npm run dev`
2. **Inicia sesión** con `demo@stampbook.com` / `demo123456`
3. **Explora** las funcionalidades principales
4. **Crea** tu primer destino o lista
5. **Personaliza** colores y logo según tu marca

---

## 🎉 ¡Listo para Explorar!

**Tu aplicación Stampbook está completamente configurada y lista para usar. El usuario demo te dará acceso inmediato a todas las funcionalidades sin necesidad de registro.**

### 🚀 **Comando de Inicio Rápido:**
```bash
npm install && npm run dev
```

### 🔑 **Credenciales de Acceso Inmediato:**
- **Email:** `demo@stampbook.com`
- **Contraseña:** `demo123456`

¡Disfruta explorando el mundo con Stampbook! 🌍✈️ 🎒