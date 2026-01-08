
```markdown
# Dataset de Arquitectura Peruana

Este repositorio contiene un dataset curado de imágenes de arquitectura peruana, organizado en tres categorías principales.  
La estructura actual del directorio es la siguiente:

```
\dataset
│
├── inca/
│   ├── muro inca 1.jpg
│   ├── muro inca 2.jpg
│   └── ...
│
├── sillar/
│   ├── Sillar arequipa 1.jpg
│   ├── Sillar arequipa 2.jpg
│   └── ...
│
└── lima/
    ├── arquitectura limena 1.jpg
    ├── arquitectura limena 2.jpg
    └── ...
```

## 📂 Categorías

- **inca/**  
  Contiene imágenes de muros incas, representando la arquitectura ancestral del Cusco y otras regiones.

- **sillar/**  
  Contiene imágenes de construcciones en sillar arequipeño, característico de la arquitectura colonial y republicana de Arequipa.

- **lima/**  
  Contiene imágenes de arquitectura limeña, incluyendo balcones y fachadas tradicionales.

## ⚙️ Uso del dataset

Este dataset está pensado para entrenamientos de modelos generativos (ej. LoRA, DreamBooth, text-to-image).  
Puedes referenciar las carpetas directamente en tus scripts:

```bash
--train_data_dir="/dataset/inca"
--train_data_dir="/dataset/sillar"
--train_data_dir="/dataset/lima"
```

Si deseas entrenar con todas las categorías juntas:

```bash
--train_data_dir="Z:/dataset/"
```

## 📌 Notas

- Todas las imágenes están en formato `.jpg` y numeradas para facilitar su indexación.  
- El dataset está balanceado con 15 imágenes por categoría (total: 45).  
- Se recomienda estandarizar resolución y captions antes de entrenamiento.  
- Validación sugerida con prompts como:
  - `"inca wall"`
  - `"sillar building"`
  - `"lima balcony"`

---

✍️ Autor: Carlos Oblea Silva  
📅 Última actualización: Enero 2026
```
