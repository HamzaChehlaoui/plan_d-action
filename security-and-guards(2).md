# Quelles pages doivent être protégées ?
- Les pages qui doivent être protégées par les Guards sont : 
le dashboard de la formatrice et le dashboard de l’apprenant 

# Que se passe-t-il si un apprenant essaie d’accéder à une page formatrice ?
- droit d’accéder à cette page (erreur 403) et il est redirigé vers sa propre page/dashboard


# Guards :

# C’est quoi un AuthGuard ?
- Un AuthGuard est responsable de vérifier si l’utilisateur est connecté (logged in). Il ne permet pas d’accéder aux pages protégées si l’utilisateur n’est pas authentifié

# C’est quoi un RoleGuard ?
- Un RoleGuard est responsable de protéger les pages en vérifiant si l’utilisateur possède le rôle approprié. Il contrôle les autorisations d’accès selon le rôle de l’utilisateur.

# Quelle différence entre être connecté et avoir le bon rôle ?
- Être connecté = utilisateur authentifié , Avoir le bon rôle = utilisateur autorisé pour la page 


# Pourquoi la route /formatrice/submissions doit être protégée par un RoleGuard et pas seulement un AuthGuard ?
- La route /formatrice/submissions doit être protégée par un RoleGuard et pas seulement un AuthGuard, car il est nécessaire de vérifier le rôle avant d’accorder l’accès. Un apprenant n’a pas le droit d’accéder à cette page


