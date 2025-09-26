1\) Méthodes GET et POST



GET : les données sont envoyées dans l’URL, sous forme de paramètres de requête



POST : les données sont envoyées dans le corps (body) de la requête HTTP, non visibles dans l’URL



2\) Comparaison GET vs POST (tableau)



Critère:



Sécurité (surface)

GET : Faible : données exposées dans l’URL, stockées dans l’historique et les logs serveurs

POST : Plus sûr : données dans le corps, non visibles dans l’URL (mais toujours chiffrer avec HTTPS)



Cas d’usage typiques

GET : Lecture de données, recherches, navigation, partage d’URL

POST : Envoi de formulaires, création/mise à jour de ressources, upload de fichiers



Longueur utile

GET : Limitée par la taille maximale de l’URL (2k–8k caractères selon navigateurs)

POST : Pratiquement illimitée (gros formulaires, JSON, fichiers)



Mise en cache

GET : Oui, souvent mis en cache par navigateurs et proxys

POST : Non, rarement mis en cache



Idempotence

GET : Oui : répéter une requête ne modifie pas l’état du serveur

POST : Non : répéter peut créer plusieurs entrées ou déclencher plusieurs actions



Visibilité des données

GET : Très visible (URL, historique, logs, signets)

POST : Cachée dans le corps de la requête, non visible dans l’URL

