# api_rest_restful
Conceitos aprendidos sobre API, REST e RESTful

## API

Acronimo de Application Programming Interface (Interface de Programação de Aplicações), é basicamente um conjunto de rotinas e padrões estabelecidos por uma aplicação, para que outras aplicações possam utilizar as funcionalidades desta aplicação.

- Responsável por estabelecer comunicação entre diferentes serviços.
- Meio de campo entre as tecnologias.
- Intermediador para troca de informações.

Exemplo: 

* Cliente (Client)
* Garçon (pedidos, levar seus pedidos, para a cozinha) (API)
* Cozinha (Server)

## REST

Um acrônimo para REpresentational State Transfer (Transferência de Estado Representativo).

Será feita a transferência de dados de uma maneira simbólica, figurativa, representativa, de maneira didática.

A transferência de dados, geralmente, usando o protocolo HTTP.

O Rest, delimita algumas obrigações nessas transferências de dados. 

### 6 Necessidades (constraints) para ser RESTful

RESTful, é a aplicação dos padrões REST.

_Client-server_: Separação do cliente e do armazenamento de dados (servidor), dessa forma, poderemos ter uma portabilidade do nosso sistema, usando o React para WEB e React Native para o smartphone, por exemplo.

_Stateless_: Cada requisição que o cliente faz para o servidor, deverá conter todas as informações necessárias para o servidor entender e responder (RESPONSE) a requisição (REQUEST).

_Cacheable_: As respostas para uma requisição, deverão ser explicitas ao dizer se aquela requisição, pode ou não, ser cacheada pelo cliente.

_Layered System_: O cliente acessa um endpoint, sem precisar saber da complexidade, de quais passos estão sendo necessários para o servidor responder a requisição, ou quais outras camadas o servidor estará lidando, para que a requisição seja respondida.

_Uniform Interface_: Manter a uniformidade na criação da interface de comunicação da sua API.

_Code on demand (optional)_: Dá a possibilidade da nossa aplicação pegar códigos, como o javascript, por exemplo, e executar no cliente.

### Boas Práticas:

- Utilizar verbos HTTP para nossas requisições
- Utilizar plural ou singular na criação dos endpoints? _NÃO IMPORTA!_ use um padrão.
- Não deixar barra no final do endpoint
- Nunca deixe o cliente sem resposta

### Verbos HTTP

- GET: Receber dados de um Resource
- POST: Enviar dados ou informações para serem processados por um Resource
- PUT: Atualizar dados de um Resource
- DELETE: Deletar um Resource

### Status das Respostas

- 1xx: Informação
- 2xx: Sucesso
	- 200: OK
	- 201: CREATED
	- 204: Não tem conteúdo PUT POST DELETE
- 3xx: Redirection
- 4xx: Client Error
	- 400: Bad Request
	- 404: Not Found
- 5xx: Server Error
	- 500: Internal Server Error

## Referências:
#### Vídeo canal Rocketseat: [O que é API? REST e RESTful? | Mayk Brito](https://www.youtube.com/watch?v=ghTrp1x_1As)
