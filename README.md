# Como Instalar

Para realizar a instalação é necessário garantir que haja um serviço de MySQL rodando em localhost com as seguintes credenciais de acesso: usuário com nome **root** e a senha uma **string vazia**

```javascript
   user: 'root';
   password: '';
```

Também é importanta haver no banco de dados um database nomeado **confiax**, pois o ORM irá procurar por ele para fazer suas instalações.

Atendido o primeiro passo, podemos prosseguir com a instalação da API, basta baixar este projeto e rodar o seguinte comando na pasta do projeto para que ele atualize todos os pacotes.

```javascript
   yarn
``` 

Em seguida, rodar o comando de migration no servidor:

```javascript
   yarn migration:run
```

E agora basta rodar o comando para inicializar o serviço

```javascript
   yarn run start
```

O Servidor está programado para ouvir a porta 4000. Então se está porta estiver ocupada, haverá conflitos na execução.
