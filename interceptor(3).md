# Où stocker le token ?
- Le token doit etre stocké dans le local storage

# Pourquoi ne pas l’ajouter manuellement dans chaque service ?
- Si on ajoute le token manuellement dans chaque service, cela complique l’application et on n’utilise pas l’Interceptor, qui est fait pour automatiser cette tâche


# Interceptor :

# Quand est-il exécuté ?
- L’Interceptor est exécuté à chaque fois qu’une requête HTTP est effectuée. Il récupère le token stocké dans le local storage et l’ajoute automatiquement à chaque requête


# Que fait-il exactement ?
- L’Interceptor gère à la fois les requêtes envoyées depuis le frontend et les réponses reçues du backend.


# Que se passe-t-il si le token est expiré ?
- Si le token est expiré, l’Interceptor provoque la déconnexion de l’utilisateur (logout)


# Que doit faire l’application si l’API retourne 401 ?
- Si l’API retourne 401, cela signifie que l’utilisateur n’est pas authentifié, donc l’application doit le rediriger vers la page de login
