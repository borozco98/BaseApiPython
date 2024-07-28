
# Activar entorno virtual

python -m venv venv
source venv/bin/activate  # Para Linux/Mac
.\venv\Scripts\activate   # Para Windows

deactivate


# Instalar dependencias 

pip install -r requirements.txt

# Inicializar la base de datos:

flask db init
flask db migrate -m "Initial migration."
flask db upgrade

# Correr App
flask run
