# Où stocker ce plan d’action ?
- Le plan d’action doit être stocké dans le store (ou dans un service central) afin qu’il soit partagé entre plusieurs composants sans refaire l’appel API.

# Pourquoi éviter les variables globales ?
- Il faut éviter les variables globales pour que les données ne soient pas accessibles ou modifiables depuis n’importe quel composant, ce qui pourrait causer des incohérences

# Pourquoi Angular utilise RxJS ?
- Angular utilise RxJS pour gérer les flux de données (data streams) qui arrivent soit une seule fois soit progressivement dans le temps.

