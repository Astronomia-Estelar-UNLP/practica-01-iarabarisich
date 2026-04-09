# Práctica 01 — Radiación Estelar y Cuerpo Negro

**Astronomía Estelar 2026 — UNLP**

Autores: J.P. Calderón & Roberto Gamen

## 🎯 Objetivos

En esta práctica vas a:

- **Implementar y validar** las leyes de radiación estelar: Planck, Wien y Rayleigh-Jeans.
- **Graficar** espectros de emisión en escala log-log y analizar comportamientos asintóticos.
- **Calcular numéricamente** longitudes de onda características (λ_max según Wien).
- **Integrar** el flujo visible (4000–7000 Å) y comprender su dependencia con temperatura.
- **Entender** dónde cada aproximación es válida mediante análisis de error porcentual.

## 🚀 Cómo comenzar

### Opción 1: GitHub Classroom (recomendado)
1. Accedé al link de Classroom desde el campus virtual.
2. Se creará automáticamente tu repositorio individual.
3. Abre el repo en **Codespaces** (botón verde `<> Code` → Codespaces).

### Opción 2: Local
1. Clona este repositorio.
2. Instala dependencias:
   ```bash
   conda activate ae
   pip install -r requirements.txt
   ```

## ⚠️ Seleccionar kernel (Codespaces)

Al abrir `notebooks/practica_01.ipynb`:
1. Arriba a la derecha: **Select Kernel**
2. Eligí: `Python (Practica 01)`

## 📓 Contenido del Notebook

El notebook está dividido en 3 ejercicios:

| Ejercicio | Tema | Destrezas |
|---|---|---|
| **1** | Implementar Planck, Wien, RJ | Astropy.units, manejo de constantes |
| **2** | Graficar espectros | Matplotlib en escala log, bandas de color |
| **3** | Integración de flujo visible | Scipy.integrate.quad, Stefan-Boltzmann |

### Workflow recomendado
- Ejecutá las celdas **en orden**.
- Lée los comentarios y docstrings.
- Respondé las preguntas implícitas en los `# TODO`.
- Guardá cambios: **Ctrl+S** (o Git → Commit).

## 📦 Estructura del repositorio

```
practica-01/
├── notebooks/
│   └── practica_01.ipynb          # Notebook principal (completar aquí)
├── src/
│   └── (utilities si es necesario — opcional)
├── data/
│   └── Gaia_Sample-practica_00.parquet  (muestra fallback)
├── informe/
│   └── (colocar pdf generado aquí)
├── requirements.txt               # Dependencias
├── README.md                      # Este archivo
└── .devcontainer/
    └── devcontainer.json         # Config Codespaces
```

## 🧪 Librerías requeridas

- `numpy`, `matplotlib`, `scipy` — cálculo y gráficos.
- `astropy` — constantes físicas y manejo de unidades.

Todas pre-instaladas en Codespaces; para local:
```bash
pip install -r requirements.txt
```

## ✅ Entrega

Cuando termines:
1. **Notebook completado** con todos los ejercicios resueltos y gráficos generados.
2. **Informe PDF** (opcional) con:
   - Gráficos y resultados númericos.
   - Interpretación física de los resultados.
   - Respuesta a preguntas sobre dónde es válida cada aproximación.

3. **Git**: 
   - Commit tus cambios: `git commit -m "Resuelve práctica 01"`
   - Push: `git push`

## 🤖 Uso de IA generativa

Está **permitido** usar Copilot, ChatGPT o similares, pero:
- ✅ Para **entender código**, explicaciones de fórmulas.
- ✅ Para **debuguear** errores.
- ❌ **No** para reemplazar tu comprensión.
- ✅ **Documenta** si la IA contribuyó sustancialmente (comment en código).

**Principio clave**: Todo código que entregues debe poder **explicarlo línea por línea**.

## ⚠️ Problemas comunes

| Problema | Solución |
|---|---|
| Kernel no aparece | Esperar a que termine la instalación automática (2–3 min) |
| `ModuleNotFoundError` | Verificar kernel seleccionado y recargar navegador |
| Unidades no funcionan en astropy | Revisar que constantes usen `.cgs` o `.si` |
| Gráfico no aparece | Asegurar `plt.show()` al final, no dentro de loops |

## 📚 Material de apoyo

- [Diapositivas de clase](https://docs.google.com/presentation/d/1BREae6IG-hLh2smZpntcGcBcftKR7xIgpjXwBBXuhVw/edit?usp=sharing)
- [Overleaf](https://www.overleaf.com/read/gwmxrtwffkxf#efb746)
- [Página del curso](https://astronomiaestelarlp.pbworks.com/)
- Documentación: [Astropy](https://docs.astropy.org) | [Scipy](https://docs.scipy.org) | [Numpy](https://numpy.org)

---

**Nota final**: El rigor físico manda. Si obtenés un número raro, preguntáte primero si tiene sentido astronómicamente, no si el código "funcionó".

## Entrega

1. Notebook completo.
2. Informe en PDF.
3. Commits y push al repositorio individual.
