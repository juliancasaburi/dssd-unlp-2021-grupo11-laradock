# dssd-unlp-2021-grupo11-laradock

# Comenzando 🚀

_Sigue las siguientes instrucciones para clonar este repositorio en tu máquina local_

### Pre-requisitos 📋

docker-compose
https://docs.docker.com/compose/install/

## Instalación 🔧

_Configure /etc/hosts_  
Agregue las siguientes 2 líneas en /etc/hosts

```
127.0.0.1 dssd-unlp-2021-grupo11-backend.test
127.0.0.1 dssd-unlp-2021-grupo11-paises-estados-service.test
```

_Sigue las siguientes instrucciones para clonar el repositorio_

_Clone el repositorio_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-laradock.git
```

_Posicionese sobre el directorio_
```
cd ./dssd-unlp-2021-grupo11-laradock
```

_Clone el repositorio del backend_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-backend.git
```

_Clone el repositorio del servicio de estampillado_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-estampillado-service.git
```

_Clone el repositorio del servicio de paises y estados_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-paises-estados-service.git
```

_Clone el repositorio del servicio de monitoreo_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-monitoreo-service.git
```

La estructura del directorio quedará de la siguiente forma:

```
.git
README.MD
└── dssd-unlp-2021-grupo11-backend
└── dssd-unlp-2021-grupo11-estampillado-service
└── dssd-unlp-2021-grupo11-monitoreo-service
└── dssd-unlp-2021-grupo11-paises-estados-service
└── laradock
```

### Instalación y configuración de los servicios
Luego de obtener la anterior estructura del directorio al clonar los repositorios, siga la guía de instalación de cada servicio. La misma se encuentra en el archivo ```README.MD``` de cada uno de los servicios.

## Iniciar el servidor 🖥️ 🆙
Puede indicar los contenedores a iniciar. Como mínimo deberá iniciar nginx y postgres.
```
cd ./dssd-unlp-2021-grupo11-laradock/laradock
sudo docker-compose up -d nginx postgres
```

Por ejemplo, puede agregar pgadmin

```
cd ./dssd-unlp-2021-grupo11-laradock/laradock
sudo docker-compose up -d nginx postgres pgadmin workspace
```

| Servicio                                      	| Puerto 	|
|-----------------------------------------------	|--------	|
| dssd-unlp-2021-grupo11-backend                	| 80     	|
| dssd-unlp-2021-grupo11-paises-estados-service 	| 81     	|
| dssd-unlp-2021-grupo11-estampillado-service   	| 82     	|
| dssd-unlp-2021-grupo11-monitoreo-service   	    | 83    	|

