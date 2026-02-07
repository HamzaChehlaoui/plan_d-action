# Router apprenant 
- /apprenant/dashboard , /apprendrant/submission/

# Router formatrice 
- /formatrice/dashboard , /formatrice/createPlanDation 

# Guards associés
- RoleGuard : vérifier role , AuthGuard : vérifier l'authentification 


# AuthService 
- AuthService est responsable de l’authentification de l’utilisateur, de la gestion du token, de la récupération du rôle et de la redirection vers les routes appropriées selon le rôle (apprenant ou formatrice)

# ActionPlanService 
- ActionPlanService est resonsable de la gestion des plans d'action 

# SubmissionService 
- SubmissionService est responsable de la gestion des submissions : envoi des réponses des apprenants vers l’API et récupération des submissions pour la formatrice


# Concepts Angular utilisés

# AuthGuard :
- utilisé pour protéjer des route et vérifier que l'utilisateur est authontifié avant d'accéder à l'application 

# RoleGuard :
- utilisé pour vérifier les autorisations selon le role 

# Interceptor : 
- utilisé pour intercepter toutes les requêtes et réponses HTTP, ajouter automatiquement le token JWT dans les headers et gérer les erreurs d’authentification comme le 401.

# Resolver : 
- resolver est utilisé pour charger les donner avant l'affichage des pages 

# Observables RxJs :
- Les Observables et RxJS sont utilisés pour gérer les données actuelles et future

# State management :
- utilisé pour centraliser l’état de l’application (authentification, plan d’action, submissions) dans un service ou un store 

