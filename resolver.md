# Pourquoi ne pas appeler l’API dans ngOnInit ?
- Parce que ngOnInit s’exécute après l’affichage du composant.
Si l’API est lente, le composant s’affiche sans données (écran vide), alors que le Resolver charge les données avant l’affichage de la page.

# Que voit l’utilisateur si l’API est lente (sans Resolver) ?
- L’utilisateur voit une page vide ou partiellement chargée sans données

# À quel moment le Resolver s’exécute ?
- Le Resolver s’exécute avant l’affichage de la page, lors de la navigation, afin de charger les données avant l’accès au composant

# Que se passe-t-il si l’API échoue dans le Resolver ? 
- Si l’API échoue dans le Resolver, l’utilisateur n’accède pas au composant. On peut le rediriger vers une page d’erreur ou afficher un message d’erreur

# Quelle différence avec un simple service ?
Avec un Resolver, le chargement et la vérification des données se font automatiquement avant l’affichage du composant, alors qu’avec un simple service, il faudrait gérer cette logique manuellement dans le composant