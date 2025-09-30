# 🌱 Semillero Agrotech con Inteligencia Artificial

## 1. Descripción del Problema (Pitch)
Los pequeños agricultores en Colombia enfrentan dificultades para vender directamente a los consumidores finales, perdiendo rentabilidad frente a intermediarios.  
Además, carecen de herramientas tecnológicas accesibles para monitoreo de cultivos, lo que los deja expuestos a plagas, enfermedades y pérdidas.  
**Agrotech** propone un Marketplace con Inteligencia Artificial que conecta productores y compradores, mejorando ingresos y productividad.

---

## 2. Estado del Arte
Se analizaron aplicaciones similares como Orbit, E-Agro, DigiAgro y TuAgro.  
Aunque ofrecen funciones de monitoreo, Marketplace o educación, carecen de una integración robusta entre **IA, Marketplace y monitoreo accesible**, lo que representa la oportunidad de valor diferencial para Agrotech.  
*(Ver documento detallado en `/docs/estado-del-arte.md`)*

---

## 3. Objetivos
**Objetivo General:**  
Desarrollar un prototipo de plataforma Agrotech con IA que funcione como Marketplace, con módulos de monitoreo básico y herramientas de gestión para pequeños productores.  

**Objetivos Específicos:**  
- Crear un prototipo funcional de Marketplace agro para productores locales.  
- Implementar un módulo de monitoreo simple de cultivos con IA y datos abiertos.  
- Validar el prototipo mediante pruebas piloto con agricultores.  

---

## 4. Alcance
Incluye:  
- Diseño del prototipo.  
- Desarrollo del Marketplace (listado de productos, carrito de pedidos).  
- Panel de administración básico.  
- Módulo inicial de monitoreo con IA (detección simple usando datasets abiertos).  

No incluye en esta fase:  
- Sensores físicos instalados en campo.  
- Logística de entrega.  
- Pasarela de pagos real.  

---

## 5. Stack Tecnológico
- **Frontend:** React 18, TailwindCSS 3  
- **Backend / BaaS:** Supabase (PostgreSQL 15, autenticación)  
- **Lenguajes:**  
  - JavaScript (ES6+) para frontend.  
  - Python 3.11 (prototipo IA con Scikit-learn / TensorFlow).  
- **Infraestructura:**  
  - Vercel (deploy frontend).  
  - Supabase Cloud (backend/DB).  
- **Control de versiones:** GitHub (rama `main`).  

---

## 6. Guía de Instalación y Ejecución Local

### Requisitos previos
- Node.js v20+  
- npm v10+  
- Git  

### Pasos
```bash
# 1. Clonar repositorio
git clone https://github.com/usuario/agrotech.git
cd agrotech

# 2. Instalar dependencias
npm install

# 3. Configurar variables de entorno
# Crear archivo .env.local con:
# NEXT_PUBLIC_SUPABASE_URL="https://xxx.supabase.co"
# NEXT_PUBLIC_SUPABASE_ANON_KEY="clave_anon"

# 4. Ejecutar en local
npm run dev
