# Devops.Works helm charts

This repository hosts [Devops.Works](http://devops.works/) helm charts.

## Authors

[@devops-works](https://github.com/devops-works)

Para el taller de helm Escogí el despliegue de Cyberchef, antes de empezar con la implementacion, hay que tener activo un cluster de Kubernetes.
y modificar el valor de un puerto en el archivo values.yaml que se encuentra en la carpeta de cyberchef.

Una vez solucionado esto, instalamos cyberchef con helf y verificamos con

````
helm list
````
<img width="1732" height="289" alt="image" src="https://github.com/user-attachments/assets/1a90ddee-c390-42f4-9a37-099cff01b635" />
Despues de esto podemos verificar que el servicio este levantado
<img width="1565" height="231" alt="image" src="https://github.com/user-attachments/assets/b9591700-d015-4a17-82de-a7d94e65fd71" />

y podemos acceder a el 
````
kubectl port-forward svc/cyberchef 8000:8000

http://localhost:8000/
````


<img width="1917" height="929" alt="image" src="https://github.com/user-attachments/assets/81ac308d-47d0-42c3-bb89-64d5aaa1bc23" />



