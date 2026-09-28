# 🤖 Ejercicios de Machine Learning en Python

> Regresión lineal con scikit-learn que predice grados Fahrenheit a partir de Celsius.

## Qué hace

El script `Regresion lineal para calcular grados centigrados a fahrenheit.py` (49 líneas) carga `celcius.csv` con pandas (columnas `celcios` y `fahrenheit`), grafica la dispersión con seaborn, entrena un `LinearRegression`, predice para 8 °C y 1233 °C, e imprime el `score` del modelo. Es un ejercicio introductorio de regresión, no una librería ni varios ejercicios.

## Estructura

```text
ml-exercises-python/
├── Regresion lineal para calcular grados centigrados a fahrenheit.py  # pandas + seaborn +
│                                                                      # LinearRegression: lee celcius.csv,
│                                                                      # entrena, predice e imprime score
└── README.md  # Este archivo
```

## Requisitos

- Python 3.x
- `pandas`, `seaborn`, `scikit-learn`

## Cómo correr

```bash
git clone https://github.com/nahataen/Python-Regresion.git
cd Python-Regresion
pip install pandas seaborn scikit-learn
python "Regresion lineal para calcular grados centigrados a fahrenheit.py"
```

> ⚠️ El archivo `celcius.csv` que el script lee (`pd.read_csv("celcius.csv")`) **no está versionado en el repo**: debes crearlo en la misma carpeta con columnas `celcios,fahrenheit` antes de ejecutar, o el script fallará con `FileNotFoundError`.

## Notas

- El nombre del comando de ejecución del README anterior (`temperatura_prediction.py`) no existe en el repo; el archivo real es el citado arriba, con espacios en el nombre (por eso va entre comillas).
- Ejercicio con fines de aprendizaje; el modelo es la recta teórica °F = °C × 9/5 + 32 ajustada a los datos del CSV.
