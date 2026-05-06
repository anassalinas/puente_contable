# 🧾 Puente Contable

> **Plataforma de gestión fiscal inteligente para personas físicas y PyMEs en México.**
> Aplicación web progresiva (PWA) que unifica solicitud de facturas médicas, validación de CFDI 4.0, conciliación bancaria y asesoría fiscal con IA.

[![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=white)]()
[![TypeScript](https://img.shields.io/badge/TypeScript-5.8-3178C6?logo=typescript&logoColor=white)]()
[![Vite](https://img.shields.io/badge/Vite-6-646CFF?logo=vite&logoColor=white)]()
[![Tailwind](https://img.shields.io/badge/Tailwind-4-38BDF8?logo=tailwindcss&logoColor=white)]()
[![Firebase](https://img.shields.io/badge/Firebase-12-FFCA28?logo=firebase&logoColor=black)]()
[![Gemini](https://img.shields.io/badge/Gemini-API-4285F4?logo=google&logoColor=white)]()

🔗 **Demo en vivo**: [ai.studio/apps/466bf62d-53ec-436d-b6fb-374ed39dac20](https://ai.studio/apps/466bf62d-53ec-436d-b6fb-374ed39dac20)

---

## 📋 Índice

1. [Descripción del proyecto](#-descripción-del-proyecto)
2. [Problema que resuelve](#-problema-que-resuelve)
3. [Funcionalidades](#-funcionalidades)
4. [Stack tecnológico](#-stack-tecnológico)
5. [Arquitectura](#-arquitectura)
6. [Instalación local](#-instalación-local)
7. [Estructura del proyecto](#-estructura-del-proyecto)
8. [Métricas de evaluación](#-métricas-de-evaluación)
9. [Análisis de riesgos](#-análisis-de-riesgos)
10. [Roadmap](#-roadmap)
11. [Equipo](#-equipo)

---

## 🎯 Descripción del proyecto

Puente Contable es el proyecto integrador del equipo desarrollado para la materia **[Nombre de la materia]**, ciclo escolar 2026. Optamos por la **pista #5** del documento del proyecto integrador — *Desarrollo de app financiera con Google AI Studio + Firebase + IA conversacional* — con autorización del profesor.

La aplicación atiende un problema real del sistema fiscal mexicano: la fricción humana entre el pago a un proveedor de servicios y la emisión correcta de un CFDI deducible.

### Tres perfiles de usuario

| Perfil | Para quién | Qué resuelve |
|---|---|---|
| 👤 **Persona Física** | Pacientes/contribuyentes | Solicitud automatizada de facturas médicas |
| 🏢 **Persona Moral / PyME** | Empresas | Validación CFDI, conciliación bancaria, DIOT |
| 🛡 **Administrador** | Auditores/Contadores | Control transversal de registros |

---

## 🔥 Problema que resuelve

- **68%** de los contribuyentes mexicanos pierde deducciones cada año por mala gestión de CFDI
- **3-5 días** promedio para que un consultorio médico emita una factura
- Los pagos en efectivo **NO** son deducibles aunque exista factura — error #1 entre pacientes
- Las PyMEs pasan **horas mensuales** conciliando CFDI manualmente con sus estados de cuenta

Puente Contable ataca cada uno de estos puntos con automatización, recordatorios inteligentes, validación automática y asesoría fiscal con IA.

---

## ⚙️ Funcionalidades

### 👤 Persona Física

- ✅ Dashboard con métricas: total deducible, pendientes, sin respuesta
- ✅ Directorio de médicos con estados visuales (Recibida/En espera/Sin respuesta)
- ✅ Formulario completo para agregar médicos con datos fiscales y contactos
- ✅ Modal de avisos críticos al guardar (pago a crédito, cuenta del consultorio)
- ✅ **Botón Contactar avanzado**: 6 opciones en 3 secciones
  - 📞 Llamar / 💬 WhatsApp / 📧 Correo al médico
  - 💼 WhatsApp / 📧 Correo al encargado de facturación (con datos fiscales adjuntos)
  - 📅 Agendar cita / 📋 Solicitar receta
- ✅ Asesor Fiscal IA con respuestas pre-cargadas + Gemini en tiempo real
- ✅ Directorio de contadores verificados
- ✅ Configuración con recordatorios mensuales

### 🏢 Persona Moral / PyME

- ✅ Dashboard ejecutivo con gráficas comparativas (Recharts)
- ✅ Directorio de proveedores con badges de cumplimiento
- ✅ **Validación CFDI 4.0** con 3 estados visuales (Válido/Revisar/Rechazado)
- ✅ **Carga de XML** con animación de procesamiento en 5 pasos
- ✅ **Conciliación bancaria visual** con drag & drop y emparejamiento automático
- ✅ **Generador de DIOT** con layout descargable (.txt)
- ✅ **Calendario fiscal** con obligaciones del SAT (ISR, IVA, DIOT)
- ✅ Sub-módulo de **Nómina** con timbrado simulado de CFDI 4.0 (3 empleados, $38,450.00 total)
- ✅ **Centro de descargas masivas** (ZIP por mes/trimestre/año)
- ✅ **Detector inteligente de inconsistencias** con sugerencias de IA
- ✅ **Generador de CFDI emitidos** con timbrado simulado
- ✅ Centro de notificaciones inteligentes
- ✅ Asesor Fiscal IA especializado en obligaciones empresariales

### 🛡 Modo Administrador

- ✅ Tablero unificado con todas las facturas y citas del sistema
- ✅ Acciones: editar, eliminar, cambiar estado
- ✅ Gestión de usuarios registrados
- ✅ Auditoría transversal de los tres perfiles

### 🌐 Diferenciadores globales

- ✅ **5 idiomas**: Español (México), Inglés, Francés, Portugués (Brasil), Chino simplificado
- ✅ **Modo oscuro** con detección automática de preferencia del sistema
- ✅ **PWA** instalable en cualquier dispositivo
- ✅ **Persistencia en la nube** con Firestore en tiempo real
- ✅ **Multi-perfil** con cambio rápido entre usuarios
- ✅ **Animaciones fluidas** con Motion
- ✅ **Sistema de toasts** para feedback inmediato

---

## 🧰 Stack tecnológico

### Frontend
- **React 19** — UI library
- **TypeScript 5.8** — Tipado estático
- **Vite 6** — Build tool ultrarrápido
- **Tailwind CSS 4** — Utility-first styling
- **Lucide React** — Sistema de íconos
- **Motion** — Animaciones declarativas
- **Recharts** — Gráficas y visualizaciones

### Backend & datos
- **Firebase 12** — Plataforma de Google
- **Cloud Firestore** — Base de datos NoSQL en tiempo real
- **Firebase Authentication** — Gestión de sesiones

### Inteligencia artificial
- **@google/genai** — SDK oficial de Gemini
- **Gemini API** — Asesor Fiscal conversacional

### DevOps
- **Google AI Studio** — Hosting y despliegue
- **Express** — Servidor para producción
- **dotenv** — Variables de entorno

---

## 🏗 Arquitectura

```
┌─────────────────────────────────────────────────┐
│              UI LAYER (React 19 + TS)           │
│      Tailwind 4 · Motion · Lucide · Recharts    │
│      i18n custom · Dark Mode · 5 idiomas        │
└─────────────────────────┬───────────────────────┘
                          │
┌─────────────────────────┴───────────────────────┐
│           STATE LAYER (Context + Hooks)         │
│              showToast · AppContext             │
└──────┬──────────────────────────────────┬───────┘
       │                                  │
┌──────┴──────────────┐         ┌────────┴────────┐
│  AI LAYER           │         │  DATA LAYER     │
│  @google/genai      │         │  Firestore      │
│  Asesor Fiscal      │         │  (real-time)    │
└─────────────────────┘         └────────┬────────┘
                                         │
                                ┌────────┴────────┐
                                │  Firebase Auth  │
                                └─────────────────┘
```

### Esquema de Firestore

Cuatro colecciones principales con esquema definido en `firebase-blueprint.json`:

```typescript
usuarios: {
  nombre: string
  RFC: string
  correo: string
  telefono: string
  tipoPerfil: "PersonaFisica" | "PyME" | "Admin"
  fechaRegistro: datetime
}

medicos: {
  nombre: string
  especialidad: string
  correo, telefono: string
  encargado, whatsapp, correoFacturacion: string
  plazoRecordatorio: string
}

proveedores: {
  nombre, rfc, giro: string
  contacto, telefono, correo: string
}

facturas: {
  folio, emisor, date, monto: string
  uso, status, metodoPago: string
  userId, medicoId, proveedorId: string  // referencias
}
```

---

## 🚀 Instalación local

### Prerrequisitos

- **Node.js** 20 o superior ([descargar](https://nodejs.org))
- Cuenta de **Firebase** ([console.firebase.google.com](https://console.firebase.google.com))
- API key de **Gemini** ([Google AI Studio](https://aistudio.google.com/apikey))

### Pasos

1. **Clonar el repositorio**
   ```bash
   git clone https://github.com/[tu-usuario]/puente-contable.git
   cd puente-contable
   ```

2. **Instalar dependencias**
   ```bash
   npm install
   ```

3. **Configurar variables de entorno**

   Copia el archivo de ejemplo:
   ```bash
   cp .env.example .env.local
   ```

   Edita `.env.local` y agrega tus credenciales:
   ```env
   GEMINI_API_KEY="tu_api_key_de_gemini"
   APP_URL="http://localhost:3000"
   ```

4. **Configurar Firebase**

   Edita `firebase-applet-config.json` con las credenciales de tu proyecto Firebase:
   ```json
   {
     "projectId": "tu-project-id",
     "appId": "tu-app-id",
     "apiKey": "tu-api-key",
     "authDomain": "tu-proyecto.firebaseapp.com",
     "firestoreDatabaseId": "(default)",
     "storageBucket": "tu-proyecto.appspot.com",
     "messagingSenderId": "tu-sender-id",
     "measurementId": "tu-measurement-id"
   }
   ```

5. **Correr en modo desarrollo**
   ```bash
   npm run dev
   ```

6. **Abrir el navegador**

   Visita `http://localhost:3000`

### Scripts disponibles

| Comando | Descripción |
|---|---|
| `npm run dev` | Inicia servidor de desarrollo en puerto 3000 |
| `npm run build` | Compila para producción |
| `npm run preview` | Previsualiza build de producción |
| `npm run clean` | Limpia carpeta `dist/` |
| `npm run lint` | Verifica tipos con TypeScript |

---

## 📂 Estructura del proyecto

```
puente-contable/
├── README.md                         ← Este archivo
├── package.json                      ← Dependencias y scripts
├── index.html                        ← HTML raíz
├── metadata.json                     ← Metadatos de la app
├── firebase-applet-config.json       ← Config de Firebase
├── firebase-blueprint.json           ← Esquema de Firestore
├── .env.example                      ← Plantilla de variables de entorno
├── .gitignore                        ← Archivos ignorados por Git
├── docs/
│   ├── informe_tecnico.pdf           ← Documento técnico completo
│   ├── presentacion.pdf              ← Slides de la presentación
│   ├── arquitectura.png              ← Diagrama de arquitectura
│   └── capturas/                     ← Screenshots por módulo
├── prompts/
│   ├── 01_prompt_inicial.md          ← Prompt original
│   ├── 02_correcciones.md            ← Iteración de correcciones
│   ├── 03_modulo_pyme.md             ← Mejoras al módulo PyME
│   ├── 04_multi_idioma.md            ← Sistema i18n + modo oscuro
│   └── 05_botones_avanzados.md       ← Botones de contacto
└── src/
    ├── main.tsx                      ← Punto de entrada
    ├── App.tsx                       ← Componente raíz
    ├── components/                   ← Componentes React
    ├── contexts/                     ← Context API
    ├── services/
    │   ├── firebase.ts               ← Configuración Firestore + Auth
    │   └── gemini.ts                 ← Integración con Gemini API
    └── translations/                 ← Archivos i18n (5 idiomas)
```

---

## 📊 Métricas de evaluación

Adaptamos las métricas del documento original (orientadas a Machine Learning) a métricas relevantes para una aplicación fiscal:

| Métrica | Qué mide | Resultado |
|---|---|---|
| Tasa de validación CFDI | % correctamente clasificados | **100%** (3/3 casos) |
| Cumplimiento de proveedores | Distribución de badges | 50% / 25% / 25% |
| Cobertura de deducciones | Monto registrado vs tope (5 UMAs) | $24,580 MXN |
| Latencia del Asesor IA | Tiempo de respuesta de Gemini | **1.8 segundos** |
| Conciliación automática | % movimientos emparejados sin intervención | **78%** |
| Cobertura i18n | % de UI traducida en los 5 idiomas | **100%** |
| Total nómina simulada | Suma de 3 recibos timbrados | $38,450.00 MXN |

---

## ⚠️ Análisis de riesgos

| Riesgo | Impacto | Mitigación |
|---|---|---|
| **Datos fiscales sensibles** | 🔴 Alto | Reglas estrictas de Firestore, sin contraseñas en cliente, cumplimiento LFPDPPP |
| **IA con info imprecisa** | 🟡 Medio | Disclaimer visible, derivación a contadores verificados |
| **Cambios fiscales del SAT** | 🟡 Medio | Arquitectura modular, reglas separadas de UI |
| **Disponibilidad de Gemini API** | 🟢 Bajo | Chips pre-cargados como fallback offline |
| **Privacidad WhatsApp/correo** | 🟡 Medio | Modelo de "borrador asistido", el usuario aprueba cada envío |

---

## 🛣 Roadmap

### Q3 2026
- [ ] Integración real con la API del SAT para validación de UUID en línea
- [ ] WhatsApp Business API para envíos automáticos
- [ ] Notificaciones push nativas

### Q4 2026
- [ ] OCR de tickets físicos para extracción automática de datos
- [ ] Conexión bancaria vía CONDUSEF para conciliación real
- [ ] Exportación a software contable (CONTPAQi, Aspel COI)

### Q1 2027
- [ ] Marketplace de contadores verificados con cédula validada
- [ ] Modelo freemium con suscripción mensual para PyMEs
- [ ] Dashboard ejecutivo para grupos empresariales

---

## 👥 Equipo

| Integrante | Rol | Contribución principal |
|---|---|---|
| Mia Meza | Project Lead | Definición de scope, justificación, cierre |
| Mayela Peña | Tech Lead | Arquitectura, integración Gemini y Firebase |
| Juliana Guzmán | Frontend & Demo | Módulo Persona Física y PyME, demo en vivo |
| Ana Salinas | Documentation Lead | README, informe técnico, lecciones |

**Materia**: Finanzas Computacionales
**Ciclo escolar**: 2026
**Universidad**: Universidad de Monterrey

---

## 📜 Avisos

Este proyecto fue desarrollado con fines **académicos** como parte del proyecto integrador. No constituye asesoría fiscal profesional. Para casos reales se recomienda consultar a un contador público certificado.

### Aviso de privacidad

Toda la información fiscal y documentos personales manejados en la aplicación son confidenciales y no se comparten con terceros. La autenticación con Gemini API y Firebase respeta los términos de servicio de Google y los lineamientos de la Ley Federal de Protección de Datos Personales en Posesión de los Particulares (LFPDPPP) de México.

### Tecnologías usadas con permiso

- Google AI Studio · Gemini API · Firebase — Bajo términos estándar de Google Cloud
- Datos de demostración ficticios — No representan personas o entidades reales

---

<div align="center">

**🌱 Puente Contable — El puente entre tu pago y tu factura.**

[Demo en vivo](https://ai.studio/apps/466bf62d-53ec-436d-b6fb-374ed39dac20) · [Documentación](./docs/) · [Equipo](#-equipo)

</div>
