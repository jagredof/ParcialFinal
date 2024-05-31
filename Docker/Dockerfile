# Usar una imagen base de Python
FROM python:3.9-slim

# Establecer el directorio de trabajo
WORKDIR /app

# Copiar el archivo de requisitos y la aplicación
COPY requirements.txt requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Copiar el contenido del directorio webapp al directorio de trabajo
COPY webapp/ .

# Exponer el puerto en el que la aplicación se ejecuta
EXPOSE 5000

# Comando para ejecutar la aplicación
CMD ["python", "run.py"]

