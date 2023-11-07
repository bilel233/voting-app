# On utilise l'image de base de python 
FROM python:3.11-alpine

# On definit le repertoir de travail
WORKDIR /vote

# On copie requirement.txt dans requirments.txt
COPY requirements.txt requirements.txt 

# On execute les dependances python
RUN pip install -r requirements.txt

# Copie du repertoire vote dans le conteneur
COPY . /vote/

# On execute l'application
CMD [ "python","app.py" ]


