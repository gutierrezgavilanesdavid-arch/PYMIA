# PYMIA ANTIGRAV — Contexto del Proyecto

## Qué es este proyecto

**PYMIA ANTIGRAV** es una startup de consultoría para PYMEs colombianas fundada por David Gutierrez. Está en etapa inicial (0-5 clientes) y este repositorio contiene todos los activos operativos de la empresa: SOPs, plantillas de onboarding, documentos legales y documentos en Word listos para entregar a clientes.

El dueño está aprendiendo Claude Code mientras construye la empresa — el enfoque es producir resultados reales al mismo tiempo que aprende la herramienta.

---

## Los 3 servicios de consultoría

### 1. Automatización de Procesos
Ayuda a PYMEs a automatizar tareas repetitivas usando herramientas sin/bajo código.
- Herramientas: Make, Zapier, n8n, Google Apps Script, Twilio
- Duración típica del proyecto: 4 semanas
- SOP: `SOPs/SOP-Automatizacion.md`
- Onboarding: `Onboarding/Onboarding-Automatizacion.md`

### 2. Consultoría Financiera
Ayuda a dueños de PYMEs a entender sus finanzas, ordenar su contabilidad básica y tomar decisiones basadas en datos.
- Herramientas: Google Sheets, Siigo, Alegra
- Duración típica del proyecto: 4 semanas
- SOP: `SOPs/SOP-Financiero.md`
- Onboarding: `Onboarding/Onboarding-Financiero.md`

### 3. Consultoría de Marketing Digital
Ayuda a PYMEs a construir presencia digital, atraer clientes y medir resultados.
- Herramientas: Meta Ads, Google Business, Metricool, Canva, MailerLite
- Duración típica del proyecto: 4 semanas (primer mes de contenido incluido)
- SOP: `SOPs/SOP-Marketing.md`
- Onboarding: `Onboarding/Onboarding-Marketing.md`

---

## Estructura del repositorio

```
PYMIA ANTIGRAV/
├── CLAUDE.md                      ← Este archivo (contexto para Claude Code)
├── .gitignore
├── SOPs/
│   ├── SOP-Automatizacion.md
│   ├── SOP-Financiero.md
│   └── SOP-Marketing.md
├── Onboarding/
│   ├── Onboarding-Automatizacion.md
│   ├── Onboarding-Financiero.md
│   └── Onboarding-Marketing.md
├── Documentos DOCX/               ← Versiones Word de los SOPs y onboarding
│   ├── SOP-Automatizacion.docx
│   ├── SOP-Financiero.docx
│   ├── SOP-Marketing.docx
│   ├── Onboarding-Automatizacion.docx
│   ├── Onboarding-Financiero.docx
│   └── Onboarding-Marketing.docx
└── Documentos Legales/            ← Documentos legales internos de PYMIA
    ├── PYMIA_Contrato_Trabajo DESPUES.docx
    ├── PYMIA_Estatutos_SAS.docx
    ├── PYMIA_Estatuto F.docx
    ├── PYMIA_Founder_Agreement.docx
    ├── PYMIA_IP_Assignment.docx
    ├── PYMIA_Legal_Compliance_Checklist.docx
    ├── PYMIA_NDA.docx
    ├── PYMIA_Offer_Letter.docx
    ├── PYMIA_Privacy_Policy.docx
    ├── PYMIA_Reglamento_Interno.docx
    └── PYMIA_Terms_of_Service.docx
```

---

## Repositorio GitHub

- **URL:** https://github.com/gutierrezgavilanesdavid-arch/PYMIA
- **Rama principal:** main
- **Visibilidad:** privado
- **Usuario Git:** David Gutierrez / gutierrezgavilanesdavid@gmail.com

---

## Formato de los documentos

- Los archivos fuente están en **Markdown (.md)** — editables directamente en VS Code o Claude Code
- Los archivos en **Documentos DOCX/** son exportaciones en Word para entregar a clientes
- Para convertir Markdown a Word se usa **Pandoc**

### Convertir un archivo .md a .docx
```powershell
pandoc SOPs\SOP-Automatizacion.md -o "Documentos DOCX\SOP-Automatizacion.docx"
```

### Convertir todos los archivos de una carpeta
```powershell
foreach ($f in Get-ChildItem SOPs\*.md) {
    pandoc $f.FullName -o "Documentos DOCX\$($f.BaseName).docx"
}
```

> Si `pandoc` no se reconoce, usar la ruta completa:
> `C:\Users\DAVID-GTZ\AppData\Local\Microsoft\WinGet\Packages\JohnMacFarlane.Pandoc_Microsoft.Winget.Source_8wekyb3d8bbwe\pandoc-3.9.0.2\pandoc.exe`

---

## Flujo de trabajo con Git

### Subir cambios o archivos nuevos
```powershell
cd "c:\Users\DAVID-GTZ\Documents\PYMIA\PYMIA ANTIGRAV"
git add .
git commit -m "Descripción del cambio"
git push
```

### Copiar un documento desde otra carpeta del PC y subirlo
```powershell
Copy-Item "C:\ruta\del\archivo.docx" "c:\Users\DAVID-GTZ\Documents\PYMIA\PYMIA ANTIGRAV\Carpeta-destino\archivo.docx"
git add .
git commit -m "Agrego [nombre del archivo]"
git push
```

### Bajar el repositorio en un PC nuevo
```powershell
git clone https://github.com/gutierrezgavilanesdavid-arch/PYMIA.git
cd PYMIA
```

---

## Herramientas instaladas en el PC principal (Windows 10)

| Herramienta | Para qué | Cómo verificar |
|-------------|----------|----------------|
| Git 2.53 | Control de versiones | `git --version` |
| GitHub CLI (gh) | Crear repos, autenticarse | `gh --version` |
| Pandoc 3.9 | Convertir .md a .docx | `pandoc --version` |
| VS Code | Editor con Claude Code integrado | — |

> GitHub CLI y Pandoc requieren abrir una terminal nueva después de instalarse para que el PATH se actualice.

---

## Pendientes y próximos pasos sugeridos

- [ ] Crear plantillas de propuesta comercial para cada servicio
- [ ] Crear contrato de servicios estándar por servicio
- [ ] Crear plantilla de Acta de Entrega
- [ ] Crear caso de estudio / portafolio del primer cliente
- [ ] Crear README.md del repositorio con descripción pública del proyecto
- [ ] Definir precios y estructura de tarifas por servicio

---

## Notas de contexto para Claude Code

- Los precios y montos siempre van en **COP (pesos colombianos)**
- El mercado objetivo son **PYMEs colombianas** — lenguaje directo, práctico, sin jerga técnica excesiva
- El dueño está aprendiendo Claude Code: explicar brevemente qué herramienta se usó y para qué cuando sea relevante
- Preferencia de formato: **Markdown exportable a Notion o Google Docs** (no diseño complejo)
- Startup en etapa inicial: priorizar soluciones simples y de bajo costo antes que soluciones sofisticadas
