# OAuth2.0 + OICD OpenId  - Demonstração (Web APP)

Essa uma demonstração do modelo Delegated Authorization Flow onde:
1. Convivem aplicação web (Client) + Servidor de autenticação (auth0) + Servidor de Recursos (API)
2. Aqui estão detalhes da camada client
3. A aplicação WEB ou APP delega a autenticação de seus usuários para um servidor de autenticação (auth0)
4. O servdidor verifica a autenticação e se sucesso retorna para a página logada (/callback)
5. Juntamente com o redirect o servidor retorna um authorization_code que identifica o usuário autenticado
6. Ao receber o authorization_code o cliente (aplicação web) usa o authorization_code para obter um access_token
7. Com esse access_token a aplicação web poderá consumir a os recursos do Servidor de Recursos (API)

Como testar

1. Tenha certeza que configurou o projeto API relacionado e já iniciou o servidor API na porta `3001`.
2. Faça clone do repositório
3. Execute `npm install`
4. Execute `npm start`
5. Acesse `http://localhost:3000`
6. Clique em fazer login
7. Contate o adminstrador para solicitar um usuario de testes
8. Após o login você deverá ver os tokens ID e AccessToken que foram gerados.

