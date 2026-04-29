# 🇪🇸 Calculadora de Jubilación España 2026

Herramienta web completa para calcular la pensión de jubilación en España, basada en la normativa vigente (LGSS, RDL 2/2023, Ley 21/2021).

## ✨ Características

- **Régimen General y RETA (Autónomos)** — cálculo separado con sus especificidades
- **Todas las modalidades**: Ordinaria, Anticipada voluntaria/involuntaria, Demorada, Activa y Parcial
- **Cómputo dual obligatorio** (2026): sistema 25 años vs 27 años — aplica el más favorable
- **Coeficientes reductores** por tabla mensual oficial (2024)
- **Complemento brecha de género** (art. 60 LGSS)
- **Proyección con IPC**, tasa de reemplazo y fiscal IRPF estimada
- **Hoja de ruta personalizada** con fechas estimadas paso a paso
- **Propuestas de mejora** personalizadas para optimizar la pensión
- **Carta editable** para comunicar la jubilación a la empresa, con género y documentación por modalidad
- **Informe PDF imprimible** con todas las secciones
- **Sin dependencias externas** — funciona 100% offline como archivo HTML único

## 🚀 Uso

### Opción A — Directamente en el navegador
1. Descarga el archivo `index.html`
2. Ábrelo con cualquier navegador moderno (Chrome, Firefox, Safari, Edge)
3. No necesita servidor ni conexión a internet

### Opción B — GitHub Pages (recomendado)
1. Haz fork de este repositorio
2. Ve a **Settings → Pages → Source → main branch**
3. La app estará disponible en `https://tu-usuario.github.io/jubilacion-app`

### Opción C — Clonar y ejecutar localmente
```bash
git clone https://github.com/tu-usuario/jubilacion-app.git
cd jubilacion-app
# Abrir index.html en el navegador, o lanzar un servidor local:
npx serve .
# o:
python3 -m http.server 8080
```

## 📋 Normativa integrada

| Norma | Contenido |
|-------|-----------|
| RDL 8/2015 (LGSS) | Marco general de pensiones — art. 205, 207, 208, 210, 214, 215 |
| RDL 2/2023 | Reforma 2023: MEI, cómputo dual obligatorio, convergencia RETA |
| Ley 21/2021 | Jubilación activa ampliada, revalorización garantizada con IPC |
| RD 13/2022 | RETA: nuevo sistema de cotización por rendimientos (15 tramos) |
| Tabla 2024 | Coeficientes reductores mensuales por jubilación anticipada |

## 🧮 Cálculo de la pensión

```
Pensión = Base Reguladora × (% cotización) × (1 ± coef. reductor/incremento) × (1 + % brecha)
```

- **Base Reguladora**: sistema más favorable entre 25 años y 27 años netos (obligatorio desde 2026)
- **% cotización**: tabla mensual LGSS art. 210 — 15 años = 50%; máximo 100% con ~36 años
- **Coef. reductor**: tabla mensual 2024, varía por años cotizados y tipo de anticipación
- **Pensión máxima 2026**: 3.175,04 €/mes (14 pagas)
- **MEI 2026**: 0,80% BC total (0,58% empresa + 0,22% trabajador/a)

## 📁 Estructura

```
jubilacion-app/
├── index.html          # Aplicación completa (HTML + CSS + JS en un solo archivo)
├── README.md           # Este archivo
├── LICENSE             # MIT License
└── .github/
    └── workflows/
        └── deploy.yml  # GitHub Actions para despliegue automático en Pages
```

## ⚠️ Aviso legal

Esta herramienta ofrece **estimaciones orientativas** basadas en la normativa vigente a abril de 2026. Los cálculos definitivos corresponden exclusivamente al **Instituto Nacional de la Seguridad Social (INSS)**. No constituye asesoramiento jurídico ni financiero. La normativa de pensiones puede modificarse por decisión legislativa.

## 🔗 Recursos oficiales

- [Sede Electrónica SS](https://sede.seg-social.gob.es) — Vida laboral, simulador, solicitud
- [Tu Seguridad Social](https://importa.seg-social.gob.es) — App móvil
- [BOE — LGSS](https://www.boe.es/buscar/act.php?id=BOE-A-2015-11724) — Texto consolidado
- [BOE — RDL 2/2023](https://www.boe.es/buscar/doc.php?id=BOE-A-2023-14204) — Reforma 2023

## 📄 Licencia

MIT — libre para uso personal y comercial. Si lo usas, se agradece mención.
