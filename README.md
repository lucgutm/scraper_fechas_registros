
#  Recopilador de fechas de vencimiento de registros sanitarios

Requisitos de usuario: Queremos un excel que nos vaya indicando cuántos días van faltando para que se renueve el registro sanitario.

# Features

Webscraping con selenium para obtener la fecha de vencimiento del registro sanitario de un producto y calcular cuántos días faltan para que se renueve.

1. Se abre el navegador y se va a la página https://registrosanitario.ispch.gob.cl/
2. Se descarga un archivo el cual lista todos los productos buscados
3. Se obtiene la fecha de vencimiento del registro sanitario de cada producto
4. Se ordenan los productos por "Fecha Próxima renovación", equivalente al siguiente día hábil (según expresado en el requisito).
5. Se exporta en formato csv.

# Cómo usarlo

1. Clonar el repositorio y abrir `main.ipynb` en un jupyter notebook
2. Instalar las dependencias
    - python 3.12 
    - Selenium 4.18
    - Pandas 2.2.1
3. Ejecutar celda por celda
4. Se generará un archivo csv con los productos ordenados por "Fecha Próxima renovación"
