<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://fullcycle.com.br/wp-content/themes/fullcycle-blog/application/img/logo-fullcycle.png"/></a>
</p>

## Descrição

Como iniciar com projeto Django com Docker

### Para Windows 

Lembrar de instalar o WSL2 e Docker. Vejo o vídeo: [https://www.youtube.com/watch?v=g4HKttouVxA](https://www.youtube.com/watch?v=g4HKttouVxA) 

Siga o guia rápido de instalação: [https://gist.github.com/argentinaluiz/6bff167be40a2bf7a6bb879062cd25cd](https://gist.github.com/argentinaluiz/6bff167be40a2bf7a6bb879062cd25cd) 

## Instalação

* Crie o volume do PostgreSQL
``` bash
docker volume create iniciando-django-pgdata
```
* Execute o projeto com o Docker:
``` bash
docker-compose up
```

## Rodar o projeto

* Acesse http://localhost:8000 para acessar o Django
* Acesse http://localhost:9000 para acesso o PgAdmin


## Comandos Úteis

- **Executar o Docker-Compose em bash**
  ``` bash
  docker-compose exec app bash
  ```
- **Criar usuário** (Dentro do Docker)
  ``` bash
  python manage.py createsuperuser
  ```
- **Aplicar migrações** (Dentro do Docker)
  ``` bash
  python manage.py migrate
  ```

## Vídeo Aula
[![](https://img.youtube.com/vi/gS2jULbwI0Q/mqdefault.jpg)](https://youtu.be/gS2jULbwI0Q)
