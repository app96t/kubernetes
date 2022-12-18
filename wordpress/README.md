# Wordpress y MYSQL
## Implementación

1. Creación del namespace (Opcional)
- Por defecto el namespace esta en default
- Si desea cambiar hay que ir a los yaml y cambiar el valor de namespace
```
kubectl create namespace <Namespace>
```

2. Creación del secreto
- Cambiar la contraseña por defecto del yaml a la deseada.
- Comando deploymnt:
```
kubectl deployment -f secreto/secreto.yaml
```

3. creacion de la BBDD MYSQL
- Comando deployment
```
kubectl deployment -f mysql/mysql.yaml
```

4. creacion de wordpress
- Comando deployment
```
kubectl deployment -f wordpress/wordpress.yaml
```
