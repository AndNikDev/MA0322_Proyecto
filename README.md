# 🧭 Guía de Contribución – Proyecto Final MA0322 (Álgebra Lineal)

````markdown
# 🧭 Guía de Contribución – Proyecto Final MA0322 (Álgebra Lineal)

## 📘 Descripción general

Este documento explica **cómo colaborar en el repositorio** del Proyecto Final MA0322. El objetivo es mantener un flujo de trabajo ordenado y evitar conflictos. Cada integrante desarrolla su módulo en su rama y carpeta asignada.

---

## 👥 Estructura de colaboración

- Cada integrante trabaja en su carpeta y en su rama feature.
- Evitar modificar archivos de otros módulos sin coordinarlo.

### 🗂 Carpetas asignadas (ejemplo)

| Integrante | Módulo / Carpeta         | Rama                    |
| ---------- | ------------------------ | ----------------------- |
| Nikolayk   | `modulos/triangulos/`    | `feature/triangulos`    |
| Kevin      | `modulos/planos/`        | `feature/planos`        |
| Denilson   | `modulos/determinantes/` | `feature/determinantes` |

---

## 🌱 Flujo de trabajo (sugerido)

1. Mantén `main` actualizado:

```bash
git checkout main
git pull origin main
```
````

2. Crea/usa tu rama feature:

```bash
git checkout -b feature/<tu_nombre_o_modulo>
```

3. Trabaja en tu rama, haz commits claros y push regularmente.

4. Abre Pull Requests contra `main` cuando tu funcionalidad esté lista.

### Buenas prácticas de commits

- Mensajes cortos y descriptivos: `feat(triangulos): añadir clasificación por ángulos`.
- Un commit por idea/cohorte de cambios.

---

## 🧪 Ejecutar la GUI localmente (PowerShell)

Para ejecutar la interfaz gráfica desde la raíz del repositorio (Windows PowerShell):

```powershell
$env:PYTHONPATH = "."; python modulos/triangulos/app_gui.py
```

Notas:

- El script intenta abrir la ventana maximizada en Windows. Si no lo hace, revisa el backend de Tkinter o ejecuta la app en otra máquina con soporte gráfico.
- Si obtienes errores de importación relativos, asegúrate de ejecutar desde la raíz del repositorio y de tener `PYTHONPATH` apuntando a `.`.

## ✅ Pruebas y validaciones (local)

- Para comprobar sintaxis rápida:

```powershell
python -m py_compile modulos\triangulos\*.py
```

- Si añadimos tests en el futuro, usar `pytest` y documentar cómo ejecutarlos aquí.

## 🧹 Estilo y linters

- Mantener código legible: usar funciones pequeñas y docstrings.
- Podemos añadir `flake8` o `pylint` en `requirements.txt` más adelante.

## 🔁 Pull Requests

- Crea PRs contra `main` con título descriptivo y changelog breve.
- Indica en la descripción qué archivos cambiaste y por qué.

```

```
