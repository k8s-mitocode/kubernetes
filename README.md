# CURSO DE KUBERNETES-MITOCODE



Trabajo Final Docker Kubernetes

## 1. Crear una imagen pública del aplicativo en Docker Registry
``` 
k8s/punto-01/00-image-registry.txt

```
## 2. Crear un cluster de Kubernetes de preferencia en GKE (puede usar cualquier otro pero que este en la nube)
``` 
k8s/punto-02/00-cluster.txt

```
## 3. Crear un Pod simple (dentro del Namespace default) que ejecute el aplicativo y la base de datos MySQL realizando la comunicación por medio de localhost
``` 
k8s/punto-03/00-mysql-pod.yaml

```
## 4. Realizar pruebas de funcionamiento mediante un Pod que contenga un contenedor que permita hacer un curl a los métodos del aplicativo
``` 
k8s/punto-04/00-curl-pod.yaml

```
## 5. Crear dos Namespaces llamados name1 y name2
``` 
k8s/punto-05/00-namespace.yaml

k8s/punto-05/01-namespace.yaml

```
## 6. En el Namespaces name1 realizar la siguiente implementación:

``` 
k8s/punto-06/*.yaml

```

- a. Crear la base de datos en un Pod

- b. Crear un Service de tipo ClusterIP que permita exponer la base de datos

- c. Crear un ConfigMap que permita desacoplar la configuración del aplicativo

- d. Crear la aplicación en un ReplicaSet con 2 replicas que use el ConfigMap y se conecte al Service de la base de datos

- e. Crear un Service de tipo ClusterIP que permita exponer el aplicativo

- f. Realizar pruebas de funcionamiento mediante un Pod que contenga un contenedor que permita hacer un curl a los métodos del aplicativo

## 7. En el Namespaces name2 realizar la siguiente implementación:
``` 

k8s/punto-07/*.yaml

```
- a. Crear la base de datos en un Statefulset

- b. Crear un Service de tipo headless que permita exponer la base de datos

- c. Crear un Secret que permita desacoplar la configuración del aplicativo

- d. Crear la aplicación en un Deployment con 4 replicas que use el Secret y se conecte al Service de la base de datos
- e. Crear un Service de tipo LoadBalancer que libere el aplicativo

- f. Realizar las pruebas mediante Postman
