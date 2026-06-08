# precio-viviendas-lima
Modelo de Machine Learning para predecirel precio de viviendasen Lima
Metropolitana.
Este repositorioforma parte del proyecto final del curso **GitHub para Producción
en Data Science** del Instituto de Analítica y Negocios.
## Objetivo del proyecto
Construir unrepositorio profesional deData Science usando GitHub,GitHub Actions,
Pull Requests,releases, herramientas deseguridad y consulta mediante API.
El modelo usadatos sintéticos de viviendas en Lima. El objetivo principal no es
obtener el mejor modelo posible, sinopracticar un flujo profesional de trabajo
con GitHub.
## Tecnologíasutilizadas- Python 3.10+- pandas- numpy- scikit-learn- pytest- GitHub Actions- PyGitHub
## Instalación
Clona el repositorio:
```bash
git clone git@github.com:TU-USUARIO/precio-viviendas-lima.git
cd precio-viviendas-lima
```
Crea y activael entorno virtual:
```bash
python-m venv .venv
source .venv/Scripts/activate
```
Instala dependencias:
```bash
python-m pipinstall-r requirements.txt
```
## Uso rápido
```python
from src.data_loader import generar_datos_lima
df = generar_datos_lima()
print(df.head())
## Ejecutar tests
```bash
python-m pytest tests/-v
```
## Ejecutar entrenamiento
```bash
python-m scripts.entrenar
```
## Estructurageneral
```text
src/ Código fuente del proyecto
tests/ Tests automáticos
scripts/ Scripts ejecutables
docs/ Documentación metodológica
outputs/ Resultados generados localmente
.github/ Workflows y configuración de GitHub
```
## Nota
El archivo `outputs/metrics.json` se generalocalmente o dentro deGitHub Actions,
pero no se sube al repositorio porqueestá ignorado por `.gitignore`.