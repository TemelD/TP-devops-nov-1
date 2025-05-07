# Utilise une image de base Ubuntu
FROM ubuntu:20.04

# Empêche les prompts interactifs durant les installs
ENV DEBIAN_FRONTEND=noninteractive

# Met à jour et installe nginx
RUN apt-get update && \
    apt-get install -y nginx && \
    apt-get clean

# Expose le port HTTP
EXPOSE 80

# Commande par défaut pour démarrer nginx en mode non-démon
CMD ["nginx", "-g", "daemon off;"]
