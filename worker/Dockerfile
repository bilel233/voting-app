# Utilisation de l'image de base .NET Core 7
FROM mcr.microsoft.com/dotnet/sdk:7.0

# Definition du repertoire de travail dans le conteneur
WORKDIR /worker

# Copie du contenu du répertoire "worker" dans le conteneur
COPY . /worker/

#Installation des dependances
RUN dotnet restore

# Production de l'executable
RUN dotnet publish -c release --self-contained false --no-restore

# Commande pour lancer le serveur
CMD ["dotnet", "bin/release/net7.0/Worker.dll"]


