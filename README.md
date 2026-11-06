# loomi · prototipo navegable (HackaToB 2026 · Equipo 09)

Mock de alta fidelidad, solo con datos de ejemplo. **No es una app funcional.** No hay backend, cuentas, pagos ni QR certificable. Los QR de pantalla son dibujos ilustrativos.

Importado del zip de Josué (jvalles.cr). Esta carpeta es el espacio de trabajo de ese artefacto, no un producto nuevo. Paleta, tipografías, logos y copys de marca se conservan. Los logos en `img/` son provisionales (P4a): no son un logo oficial cerrado.

## Abrir en línea

Prototipo público (mock estático): https://milasur.github.io/loomi-prototipo-hackatob2026/

Repo: https://github.com/Milasur/loomi-prototipo-hackatob2026

## Abrir en local

Las fuentes y las imágenes van en `fonts/` e `img/`, así que el mock también abre directo con `index.html`.

Para probarlo como sitio:

```bash
python3 -m http.server 47231
```

Luego abrí `http://127.0.0.1:47231`. En escritorio se ve dentro de un marco de teléfono (390×844). En el celular ocupa toda la pantalla.

## Modo demo

1. Tocá el botón **DEMO** arriba a la derecha. Si estás en el inicio, el demo salta al mapa.
2. Usá las flechas **‹ ›** para avanzar o retroceder.

El arreglo `FLUJO_DEMO` en `index.html` recorre: mapa → piñero (registro, plan, recolección, listo) → acopio (QR, recibido, no apto, ruta atrasada, impacto) → comprador (escaneo, lote).

## Pantallas

| id | Rol | Qué muestra |
|---|---|---|
| `inicio` | — | Selector de rol + tagline |
| `mapa` | todos | Mapa vivo Zona Norte (SVG offline) |
| `p-home` … `p-bono` | piñero | Finca, plan 44021, recolección, QR, bono |
| `a-home` | acopio | Rutas, alertas de ejemplo (no apto y ruta atrasada) |
| `a-qr`, `a-recibido` | acopio | Escaneo simulado y recepción |
| `a-no-apto` | acopio | Lote de ejemplo con corte después del químico, reasignado a incorporación en verde |
| `a-ruta-atrasada` | acopio | Ruta 2 atrasada; Reprogramar solo cambia la pantalla |
| `a-impacto` | acopio | Hectáreas y kilos de ejemplo, lotes, estado de rutas y alertas |
| `c-market` … `c-lote` | comprador | Marketplace, escaneo y trazabilidad, incluido un lote reasignado |

## Identidad

Paleta IRIS · Tinta `#14210F` · Hoja `#1E6B3A` · Brote `#B7E04A` · Piña `#F5B800` · Cáscara `#E8761E` · Fibra `#FFF6DC` · Tierra `#8A5A2B`. Tipografías Bricolage Grotesque / Inter / IBM Plex Mono. Fondos con los degradados suaves ya presentes en el marco de escritorio.

## Datos de ejemplo

Fincas, personas, lotes, fechas, pesos, rutas y el nombre «Coopepiña» en las pantallas son muestras del mock. No describen un convenio, una entrevista ni una operación real. Toda cifra del panel de impacto es de demostración.

## Carpetas

- `shots/` — capturas originales del prototipo, a 390×844
- `fonts/`, `img/` — assets locales
- `v1-borrador/` — el README original nombraba esta carpeta, pero **no venía en el zip** y no está en este espacio
