# dssd-unlp-2021-grupo11-laradock

# Comenzando 🚀

_Sigue las siguientes instrucciones para clonar este repositorio en tu máquina local_

### Pre-requisitos 📋

docker-compose
https://docs.docker.com/compose/install/

### Instalación 🔧

_Sigue las siguientes instrucciones para clonar el repositorio_

_Clone el repositorio_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-laradock.git
```

_Clone el repositorio del backend_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-backend.git
```

_Clone el repositorio del servicio de paises y estados_

```
git clone git@github.com:juliancasaburi/dssd-unlp-2021-grupo11-paises-estados-service.git
```

La estructura del directorio quedará de la siguiente forma:

```
.git
.README.MD
└── laradock
└── dssd-unlp-2021-grupo11-paises-estados-service
└── dssd-unlp-2021-grupo11-backend
```

## Iniciar el servidor 🖥️ 🆙
Puede indicar los contenedores a iniciar. Como mínimo deberá iniciar nginx, postgres y workspace
```
cd ./laradock
sudo docker-compose up -d nginx postgres workspace
```

Por ejemplo, puede agregar redis y pgadmin

```
cd ./laradock
sudo docker-compose up -d nginx postgres redis pgadmin workspace
```