# Spring boot and Microservice with docker 

## Related to OKTA Configuration
Créez d'abord une nouvelle application dans Okta. Le type d'application doit être une application d'identification ouverte.
Le serveur d'authentification a une configuration liée au jeton d'accès et à la validité du jeton d'actualisation.

Go to security -> API -> default audience to modify access policies and timing.

Pour obtenir un refresh token, nous devons nous assurer que nous avons un refresh token de type d'octroi pour l'application et que la portée est également offline_access provided lors retriving tokens. Reportez-vous au fichier yaml application propereties de l'app  cloud gateway.
