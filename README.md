# crud-react-backend
Servidor utilizando spring-boot rest 
Aplicação feita pra servir como backend pra cadastro de músicas utilizando react JS.


### Pré-requisitos
Para executar aplicação é necessário instalar 2 ferramentas: **Docker** & **Docker Compose**.

**Docker**
Para ambientes [Linux](https://docs.docker.com/install/linux/docker-ce/ubuntu/), [Windows](https://docs.docker.com/docker-for-windows/install/) e [Mac](https://docs.docker.com/docker-for-mac/install/) .

**Docker Compose** 
Nos ambientes *Windows* e *Mac* já são instalados juntos com o Docker, para Linux basta [seguir as instruções](https://docs.docker.com/compose/install/) .

### Como rodar a aplicação?
## Docker compose ##
Para construir aplicação:

```
$ docker-compose build
```

Para subir aplicação:

```
$ docker-compose up -d
```

Para parar aplicação:

```
$ docker-compose down
```

## Rodando em servidor local ##
Necessário executar comandos dentro da pasta onde contém os arquivos do projeto com o pom.xml
Para construir e testar build: 

```
$ maven package
```
Ou

```
$ mvn install
```

Executar aplicação via jar

```
$ java -jar target/crud-react-backend-0.0.1-SNAPSHOT
```

Via plugin do maven

```
$ mvn crud-react-backend:run
```

Apenas gerar arquivo .jar:

```
$ mvn install -DskipTests
```
