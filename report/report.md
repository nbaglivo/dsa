# Resumen DSA


## Grupo 2017 - 12

En la documentación se lee que el endpoint acepta un parámetro **fields** para filtrar las propiedades del usuario que querramos obtener, podemos abusar de esto para obtener los password de los usuarios.

![g12_users](https://github.com/nbaglivo/dsa/blob/master/report/imgs/g12_users.png "G12 Users")

Ahora tengo el password hasheado en md5, para conseguir el password original utilizo una rainbow table, md5 es rapido asi que hay chances de crackearlo rapidamente.

![g12_crackpass](https://github.com/nbaglivo/dsa/blob/master/report/imgs/g12_crackpass.png "G12 Pass Crack")

Una vez que tenemos el password podemos loguearnos !

![g12_login](https://github.com/nbaglivo/dsa/blob/master/report/imgs/g12_login.png "G12 Login")


Finalmente si le pegamos al endpoint /auth/current podemos obtener la información del usuario logueado y el flag !

![g12_flag](https://github.com/nbaglivo/dsa/blob/master/report/imgs/g12_login.png "G12 Flag")


