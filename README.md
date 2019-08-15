# API-REST-RESTFULL
Studying api-rest/restfull

feature

API: Acronimo de Application Programming Interface (Interface de Programação de Aplicações) é basicamente um conjunto de rotinas e padrões estabelecidos por uma aplicação, para que outras aplicações possam utilizar as funcionalidades desta aplicação.

- Responsável por estabelecer comunicação entre diferentes serviços.
- Meio de campo entre tecnologias.
- Intemediador para troca de informações.

REST: Acrônimo para Representation State Transfer (Transferência de Estado Representativo).

- Será feita a transferência de dados de uma maneira simbólica, figurativa, representativa de maneira didática.
- A transferência de dados, geralmente, usando o protocolo HTTP.
- O Rest, delimita algumas obrigações nessas transferências de dados.
- Resources seria então, uma entidade, um objeto.

6 necessidades (constraints) para ser Restful

1. _Client_Server_: Separação do cliente e do armazenamento de dados (servidor), desta forma, poderemos ter uma portabilidade do nosso sistema, usando React para Web e React Native para smartphone, por exemplo.
2. _Stateless_: Cada requisição que o cliente faz para o servidor, deverá conter todas as informações necessárias para o servidor entender e responder (RESPONSE) a requisição (REQUEST). Exemplo: A sessão do usuário deverá ser enviada em todas as requisições, para saber se aquele usuário está autenticado e apto a usar os serviços, e o servidor não pode lembrar que o cliente foi autenticado na requisição anterior. Nos nossos cursos, temos por padrão usar tokens para as comunicações.
3. _Cacheable_: As respostas para uma requisição, deverão ser explicitas ao dizer se aquela requisição, pode ou não, ser cacheada pelo cliente.
4. _Layered_System_: O cliente acessa a um endpoint, sem precisar saber da complexidade, de quais pessoas estão sendo necessários para o servidor responder a requisição, ou quais outras camadas o servidor estará lidando, para que a requisição seja respondida.
5. _Code on demand (optional)_: Dá a possibilidade da nossa aplicação pegar códigos, como o Javascript por exemplo, e executar no cliente.

#BOAS PRÁTICAS
- Utilizar verbos HTTP para nossas requisições
- Utilizar plural ou singular na criação de endpoints? _NÃO IMPORTA!_ use um padrão;
- Nunca deixe o seu cliente sem resposta.

#STATUS DAS RESPOSTAS
- 1xx: Informações;
- 2xx: Sucesso
  -200: OK
  -201: CREATED
  -204: Não tem conteúdo PUT POST DELETE
-3xx: Redirection
-4xx: Client error
  -400: Bad Request
  -404: Not Found
-5xx: Server Error
-6xx: Internal Server Error
