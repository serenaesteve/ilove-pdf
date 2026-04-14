# s.pdf — Herramientas PDF online

Clon de iLovePDF con diseño dark editorial + rosa.

## Herramientas incluidas
- Unir PDF
- Dividir PDF
- Comprimir PDF
- PDF a Word
- PDF a JPG
- Word a PDF
- JPG a PDF
- Proteger PDF
- Rotar PDF

## Instalación

```bash
cd spdf

# Instalar dependencias Python
pip install -r requirements.txt --break-system-packages

# Dependencias del sistema (para PDF a JPG y Word a PDF)
sudo apt install poppler-utils libreoffice

# Ejecutar
python app.py
```

Abre http://localhost:5000

## Estructura

```
spdf/
├── app.py
├── requirements.txt
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── tool.html
│   └── 404.html
└── static/
    ├── css/main.css
    └── js/main.js
```

## Notas
- `PDF a JPG` requiere `poppler-utils`: `sudo apt install poppler-utils`
- `Word a PDF` requiere `LibreOffice`: `sudo apt install libreoffice`
- El resto de herramientas funcionan sin dependencias del sistema
