# Mini Sintetizador Digital (Web Audio API)

Este proyecto es un mini sintetizador pensado para aprender los bloques básicos de síntesis digital dentro del navegador.

## Qué incluye

- Oscilador por nota (formas: seno, cuadrada, diente de sierra, triangular).
- Envolvente sencilla con **Attack** y **Release**.
- Filtro low-pass para moldear el timbre.
- Volumen maestro.
- Teclas musicales con mouse/touch y también con teclado (`A S D F G H J`).
- Botón de **Silencio total** para detener cualquier nota activa.

## Cómo probarlo localmente

1. Abre una terminal en la carpeta del proyecto.
2. Ejecuta un servidor local:

```bash
python3 -m http.server 8000
```

3. Entra desde tu navegador a:

```text
http://localhost:8000/synth.html
```

4. Haz clic en **Activar audio** (los navegadores lo piden por seguridad).
5. Prueba notas con el mouse o con el teclado y mueve los controles para escuchar los cambios.

## Flujo recomendado para aprender

1. Deja todo en valores por defecto y toca una nota.
2. Cambia la forma de onda y compara cómo cambia el color del sonido.
3. Sube el `Attack` para que la nota entre más suave.
4. Sube el `Release` para que la nota se apague lentamente.
5. Baja el `Cutoff` para escuchar cómo el filtro quita brillo.

---

Si luego quieres, el siguiente paso natural es convertir esto a un plugin real con JUCE (VST3/AU), usando este prototipo como referencia de comportamiento sonoro.
