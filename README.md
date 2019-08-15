# API-REST-RESTFULL
Studying api-rest/restfull

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
