# Resumen DSA


## Grupo 2017 - 12

1. En la documentación se lee que el endpoint acepta un parámetro **fields** para filtrar las propiedades del usuario que querramos obtener, podemos abusar de esto para obtener los password de los usuarios.

![](imgs/g12_users.png)

2. Ahora tengo el password hasheado en md5, para conseguir el password original utilizo una rainbow table, md5 es rapido asi que hay chances de crackearlo rapidamente.

![](imgs/g12_crackpass.png)

3. Una vez que tenemos el password podemos loguearnos !

![](imgs/g12_login.png)


4. Finalmente si le pegamos al endpoint /auth/current podemos obtener la información del usuario logueado y el flag !

![](imgs/g12_flag.png)


## Grupo 2017 - 11

1. Puse cualquier path en la url para chequear si estaba en debug mode. Me encontré con todas las rutas de la app y noté que había una API.

![](imgs/g11_routes.png)

2. Le pegue a la API con el id de un post y encontré el flag.

![](imgs/g11_flag.png)

### Grupo 2017 - 6 - ** Intento fallido **

1. Encontré un link a un archivo que parecía ser un diccionario.

![](imgs/g6_dict.png)

2. Probé un ataque de diccionario contra el login pero no funcionó

3. Luego encontré una imagen sospechosa de un personaje animado, no recordaba el nombre pero google images me dijo que era Gir

![](imgs/g6_gir.png)

4. Volví a hacer un ataque de diccionario pero esta vez usando como usuario  Gir, no hubo suerte

![](imgs/g6_dict_attack.png)
