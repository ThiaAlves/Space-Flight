# Space-Flight-News
 Back-end Challenge 🏅 2021 - Space Flight News - By [Coodesh](https://coodesh.com/).


Seguem os atributos da tabela:

## - Articles:
1. Featured;
2. Title;
3. Url;
4. ImageUrl;
5. NewsSite;
6. Summary;
7. PublishedAt;

## Configuração do projeto para execução


### EXECUÇÂO DIRETA

1) Clone esse repositório para a sua máquina:
```git clone https://github.com/ThiaAlves/Space-Flight.git```

2) Instale as dependências necessárias para execução do projeto
```composer install```

3) Copie e renomeie o arquivo .env.example para .env
 
4) Importar o banco de dados:
```php artisan migrate```

5) Gerar a chave para execução do projeto:
```php artisan key:generate```

6) Para iniciar o servidor Laravel Execute:

```php artisan serve```
 
 
### EXECUÇÂO EM DOCKER (Padrão)
O projeto utiliza Docker e Docker Compose como padrão para criação do ambiente de desenvolvimento.

### Build e execução dos containers Docker
Observação: A configuração do docker-compose.yml foi configurado para ser executado 
em uma máquina linux, em execuções no windows será necessário fazer alguns ajustes.

1) Clone esse repositório para a sua máquina:
```git clone https://github.com/ThiaAlves/Space-Flight.git```

2) Copie o arquivo .env.example para o diretorio do projeto com o comando:
```cp .env.example .env```

3) Para construir a imagem do app
```docker-compose build app```

4) Para iniciar os containers do app
```docker-compose up -d```

### Para ver os containers rodando
```docker ps```

### Para instalar as dependências do composer
```docker exec -it space-news composer install```

### Definir chave do app
```docker exec -it space-news php artisan key:generate```

### Para construir o banco de dados
```docker exec -it space-news php artisan migrate```

### Acessar projeto pelo Browser
```localhost:8080```

#### Para executar o Teste;
Para executar o teste, execute o comando ```docker exec -it space-news php artisan test``` 
A saída do comando acima deverá ser:
```
PHPUnit 9.5.8 by Sebastian Bergmann and contributors.

..                                                                  2 / 2 (100%)

Time: 00:00.068, Memory: 20.00 MB

OK (2 tests, 2 assertions)
```

#### Link para vizualizar a documentação da API 
```localhost:8080/api/documentation```

#### Executar o Seed Manualmente
```php artisan db:seed```

#### Executar o teste de Tarefas agendadas do Laravel
```php artisan schedule:test```



### Apresentação
[Space-news](https://www.loom.com/share/014c84afd7f442d3a663cd87f865867d).

This is Challenge By [Coodesh](https://coodesh.com/).


