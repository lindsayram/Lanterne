# Validation

## les requêtes exécutées sur l’URL publique

- `GET /api/health`

Status code attendu : 200 

Status code obtenu : 200

![image](./img/test1.png)

- `GET /api/curiosities`

Status code attendu : 200 

Status code obtenu : 200

![image](./img/test2.png)

- `GET /api/curiosities?q=canal&limit=5`

Status code attendu : 200 

Status code obtenu : 200

![image](./img/test3.png)

- `GET /api/curiosities/:slug`

Status code attendu : 404 

Status code obtenu : 404

![image](./img/test4.png)

- `GET /api/curiosities/passage-bleu`

Status code attendu : 200 

Status code obtenu : 200

![image](./img/tests5.png)