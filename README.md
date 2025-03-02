# curso-spark-scala

## Configuración del Entorno con PySpark en Docker
### ✅ Incluye: PySpark + Apache Toree-Scala

La imagen de PySpark utilizada en el curso cuenta con Apache Toree-Scala y está disponible en Docker Hub:  

🔗 [Visitar Docker Hub](https://hub.docker.com/r/josechval/pythonista-pyspark-scala)  

### Instrucciones para GNU/Linux y MacOS
- Ejecuta el siguiente comando en la terminal:  

**docker run --rm -d -v $HOME:/home/jovyan/work -p 8888:8888 -p 4040:4040 -p 4041:4041 --name pyspark josechval/pythonista-pyspark-scala**

### 📌 **Explicación:**

- Inicia un contenedor en segundo plano (-d).
- Monta el directorio $HOME en la ruta del contenedor /home/jovyan/work.
- Expone los puertos necesarios:
  - 8888 para Jupyter Notebook
  - 4040 y 4041 para la interfaz web de Spark UI
- Asigna el nombre pyspark al contenedor.
  
### Para acceder a Jupyter Notebook, abre un navegador y dirígete a:

🔗 [Visitar Jupyter](http://localhost:8888)  
🔑 Contraseña: Jupyter


### Instrucciones para Windows
- Ejecuta el siguiente comando en PowerShell o CMD, reemplazando <RUTA> por la ruta de tu directorio de trabajo:  

**docker run --rm -d -v <RUTA>:/home/jovyan/work -p 8888:8888 -p 4040:4040 -p 4041:4041 --name pyspark josechval/pythonista-pyspark-scala**

### 📌 **Explicación:**

- Igual que en Linux/Mac, pero debes definir la ruta de tu directorio en <RUTA>, por ejemplo:  

**docker run --rm -d -v "C:/Users/Rossella/Escritorio/Proyecto Spark-Scala:/home/jovyan/work" -p 8888:8888 -p 4040:4040 -p 4041:4041 --name pyspark josechval/pythonista-pyspark-scala**

### Para acceder a Jupyter Notebook, abre un navegador y dirígete a:  

🔗 [Visitar Jupyter](http://localhost:8888)  
🔑 Contraseña: Jupyter  


### Detener el Contenedor en Cualquier Plataforma
- Para detener el contenedor ejecuta:  

**docker stop pyspark**






