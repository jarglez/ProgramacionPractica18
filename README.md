# Práctica 18: 

Elaboró: Carlos Alejandro Jarero Gonzalez <al255813@alumnos.uacj.mx>

Matrícula: 255813

El presente Notebook fue relizado en equipo local con Kernel Python 3.11.8 en VS Code.

## Objetivos

El objetivo de esta actividad que el alumno haga un Exploratory Descriptive Analysis (EDA).

## Instrucciones de uso

Este notebook puede extraer datos del archivo ```AirQuality.csv```, para analizar la información presente.

Si quieres cambiar el archivo, o la dirección del mismo, solo ve a la sección de parameters y cambia el ```input_path```.

Puedes cambiar la semilla en ```seed``` o poner None para mayor aleatoriedad.

### Si usas Google Colab

1. Ve a la sección de Files y asegurate de tener habilitado el acceso a tu Google Drive, de lo contrario hablitalo y dale los permisos correspondientes.
2. Si ya has realizado el paso anterior verás en tu notebook la siguiente instrucción de python para montar un volumen en el caso de linux ```/content/drive```, esto puede cambiar en diferentes sistemas operativos.
![Drive Mounting](./assets/DriveMount.png)
3. Asegurate de ejecutar la sección previa, dependidendo si ya has dado o no los permisos en este paso puede que de nuevo te solicite darle permiso. 
4. Ahora verás um directorio llamado drive donde encontarás tu Drive, ahí sube el archvio a procesar.
5. Copia el path absoluto de archivo de ```AirQuality.csv``` en ```input_path```.

## Descripción del conjunto de datos

Utiliza el conjunto de datos "Air Quality" disponible al final de esta practica. Este conjunto contiene datos horarios de sensores de calidad del aire, incluyendo niveles de CO, NOx, y otros contaminantes. El conjunto de datos tiene valores faltantes y columnas categóricas (por ejemplo, el día de la semana).


## Instrucciones para los estudiantes:

1. Descargar el archivo AirQuality.csv desde el enlace proporcionado.

2. Realizar un EDA completo, incluyendo:

- Descripción de los datos (medias, medianas, desviaciones estándar, etc.).
- Histogramas para las columnas numéricas.
- Gráficas de barras para las columnas categóricas (por ejemplo, DayOfWeek).
- Boxplots para identificar outliers en las columnas numéricas.
- Matriz de correlación y mapa de calor.
- Pairplot para visualizar relaciones entre variables numéricas.
- Pruebas de normalidad (Shapiro-Wilk, Anderson-Darling, Kolmogorov-Smirnov) y QQplot para las columnas numéricas.

3. Identificar y tratar los datos faltantes utilizando técnicas como imputación por media, mediana o moda, o eliminación de filas/columnas según sea apropiado.

4. Repetir el EDA después del tratamiento de datos faltantes y comparar los resultados.

5. Responde a estas preguntas y sube tus conclusiones a un PDF (se verificará el uso de IA)

A) Análisis Exploratorio de Datos (EDA):

- ¿Qué patrones o tendencias observaste en los histogramas y gráficas de densidad (PDF)? ¿Alguna variable parece seguir una distribución normal?
- ¿Qué información útil obtuviste de las gráficas de barras para las variables categóricas (por ejemplo, DayOfWeek)?
- ¿Identificaste outliers en los boxplots? ¿Cómo podrían afectar estos outliers al modelo de regresión lineal?

B) Pruebas de Normalidad:

- ¿Qué conclusiones obtuviste de las pruebas de normalidad (Shapiro-Wilk, Anderson-Darling, Kolmogorov-Smirnov)? ¿Qué variables no siguen una distribución normal?
- ¿Cómo interpretas los QQplots? ¿Qué variables se desvían significativamente de la normalidad?

C) Tratamiento de Datos Faltantes:

- ¿Qué estrategia utilizaste para manejar los datos faltantes? ¿Por qué elegiste esa estrategia?
- ¿Cómo cambió el EDA después de la imputación de datos? ¿Observaste diferencias significativas en las distribuciones de las variables?

D) Matriz de Correlación y Pairplot:

- ¿Qué relaciones lineales identificaste en la matriz de correlación y el pairplot? ¿Alguna variable tiene una correlación fuerte con la variable objetivo?
- ¿Cómo podrías utilizar esta información para seleccionar características (features) en un modelo de regresión lineal?