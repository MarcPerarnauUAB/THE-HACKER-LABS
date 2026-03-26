# 🔍 Writeup OSINT: [Nombre del Reto]

**Plataforma:** [The Hacker Labs](https://labs.thehackerslabs.com/)
**Dificultad:** 🟢 Principiante
**Categoría:** OSINT / Geolocalización / SOCMINT

---

## 📝 Descripción del Escenario
> [Pega aquí el texto que te da el reto, por ejemplo: "Se ha recibido un correo de extorsión, ¿puedes encontrar la ubicación del atacante?"]

---

## 🎯 Objetivos
- [ ] Hallar el nombre real del sospechoso.
- [ ] Localizar la ubicación exacta de la fotografía.
- [ ] Encontrar la flag final.

---

## 🛠️ Herramientas Utilizadas
- **Google Lens / Yandex Images:** Para búsqueda visual inversa.
- **ExifTool:** Para extracción de metadatos de imágenes.
- **Google Maps / Street View:** Para confirmación de geolocalización.
- **Phonebook.cz / Intelligence X:** Para búsqueda de correos o dominios.

---

## 🕵️ Paso a Paso (Investigación)

### 1. Análisis Inicial de la Pista
Al descargar el archivo `pista.jpg`, lo primero que hice fue analizar visualmente la imagen. Observé un edificio con un logo peculiar y una matrícula de coche que parece ser de [País].

### 2. Extracción de Metadatos (Metadata Analysis)
Ejecuté `exiftool` para ver si la imagen contenía coordenadas GPS o información del dispositivo:
```bash
exiftool pista.jpg