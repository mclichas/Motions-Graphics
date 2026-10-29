# Motions Graphics

Proyecto de Motion Graphics con [HyperFrames](https://hyperframes.heygen.com) (HTML renderizado a video).

## Archivos

- `index.html` — composición principal (10s, 1920×1080, GSAP).
- `motion-graphics.zip` — proyecto comprimido listo para subir a Colab.
- `render_colab.ipynb` — notebook de Colab (usa apt para Node/FFmpeg/Chromium).
- `render_colab_python.ipynb` — notebook de Colab (usa pip: imageio-ffmpeg + Playwright + nvm). **Recomendado.**

## Renderizar en la nube (Colab)

1. Abre el notebook en Colab desde GitHub: **File → Open notebook → GitHub** → `mclichas/Motions-Graphics`.
2. Ejecuta las celdas en orden.
3. En la celda de upload, sube `motion-graphics.zip`.
4. Descarga `output.mp4`.

## Notas

- El timeline está pausado (`paused: true`) para el render determinista de HyperFrames; en el navegador se auto-reproduce como preview.
- Para renderizar localmente se necesita Node.js 22+, FFmpeg y Chrome (headless). En Colab se instalan automáticamente.
- HyperFrames: https://hyperframes.heygen.com