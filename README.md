Projeto Final - "Meus Links"
Descrição do Projeto
O projeto final, intitulado "Meus Links", é uma aplicação web de gerenciamento de links pessoais que permite aos usuários criar, editar, excluir e visualizar links personalizados. Este projeto abrange tanto o desenvolvimento do frontend quanto do backend e utiliza as seguintes tecnologias:

Front-end: Reagir
Back-end: Node.js, Express, Prisma, PostgreSQL
Objetivos
O objetivo principal deste projeto é proporcionar aos alunos a oportunidade de aplicar os conhecimentos adquiridos em Full Stack Web Development para criar uma aplicação completa e funcional. Os objetivos específicos incluem:

Desenvolver parte do frontend da aplicação usando React.
Implementar backend usando Node.js, Express, Prisma e PostgreSQL.
Crie um sistema de autenticação de usuário.
Habilite os usuários a gerenciar seus links personalizados.
Consumir uma API para interagir com os dados do usuário e links.
Praticar boas práticas de desenvolvimento, como organização de código, gerenciamento de dependências e testes.
Requisitos Funcionais
Cadastro de Usuário

Os usuários devem poder criar uma conta fornecendo um nome de usuário, email e senha.
Os dados de nome de usuário, email e senha devem ser válidos e atender aos critérios de validação.
Após o cadastro, os usuários deverão poder fazer login no sistema.
Login do usuário

Os usuários devem poder fazer login no sistema usando suas credenciais de nome de usuário e senha.
As credenciais de login deverão ser autenticadas e verificadas pela API.
Após o login bem-sucedido, os usuários deverão ser redirecionados para a página principal da aplicação.
Adicionar Link

Os usuários devem poder adicionar um novo link personalizado fornecendo um título descritivo, URL.
Todos os campos obrigatórios devem ser preenchidos para adicionar o link.
Editar link

Os usuários deverão poder editar um link existente, modificando o título, URL.
A edição de um link deve ser permitida apenas pelo proprietário do link.
Os usuários deverão poder salvar as alterações feitas no link.
Link de Apagar

Os usuários devem poder excluir um link existente.
A exclusão de um link deve ser permitida apenas ao proprietário do link.
Ao excluir o link, ele deverá ser removido da lista de links do usuário.
Desativar Link

Os usuários deverão poder desativar um link existente.
A desativação de um link deve ser permitida apenas pelo proprietário do link.
Ao desativar o link, ele deverá ser removido apenas da página de links do usuário.
Página do Usuário

Ao acessar uma rota como.
A página de detalhes deve mostrar a biografia do usuário e uma lista de links personalizados associados a ele.
Requisitos do Projeto
Front-end
Crie páginas para registro e login do usuário.
Implemente a funcionalidade de adicionar, editar e excluir links.
Exibir uma lista de links do usuário logado.
Exibir uma lista de todos os usuários cadastrados e permitir a visualização dos detalhes de cada usuário.
Usar React Router Dom para gerenciar as rotas da aplicação.
Consumir a API fornecida para acesso aos dados do usuário e links.
Processo interno
Configure o servidor Node.js com Express.
Crie rotas para registro, login e gerenciamento de links.
Implementar autenticação de usuário usando tokens JWT.
Conecte-se a um banco de dados PostgreSQL com o Prisma.
Validar dados de entrada e implementação de autorização para ações do usuário.
Definições de Rotas do Backend
POST /usuarios: Rota para registrar um novo usuário.
POST /usuarios/login: Rota para autenticar um usuário e gerar um token JWT.
GET /usuarios: Rota para listar todos os usuários cadastrados.
GET /usuarios/:id: Rota para obter os detalhes de um usuário específico.
POST /links: Rota para adicionar um novo link para o usuário autenticado.
PUT /links/:id: Rota para atualizar um link existente do usuário autenticado.
DELETE /links/:id: Rota para excluir um link existente do usuário autenticado.
Diagrama de Entidade e Relacionamento (DER)
Unable to render rich display

Diagram error not found.

For more information, see https://docs.github.com/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams#creating-mermaid-diagrams
erDiagrama
    Usuário ||--o{ Link : has
    Usuário {
        id INT (chave primária)
        nome STRING
        nome de usuário STRING
        e-mail STRING
        senha STRING
    }
    Link {
        id INT (chave primária)
        urlSTRING
        título STRING
        ativo BOOLEAN
        usuario_id INT (chave estrangeira)
    }
Neste diagrama de entidade e relacionamento, temos duas entidades: “User” e “Link”, e o relacionamento entre elas indica que um usuário pode ter muitos links.

Recursos Úteis
Aqui estão alguns recursos que podem ser úteis durante o desenvolvimento do projeto:

Documentação oficial do React: https://react.dev/
Documentação oficial do Axios: https://axios-http.com/ptbr/docs/intro
Documentação oficial do React Router Dom: https://reactrouter.com/en/main
Documentação do Prisma: https://www.prisma.io/docs/getting-started
Documentação do Express.js: https://expressjs.com/pt-br/
Documentação do PostgreSQL: https://www.postgresql.org/docs/
Entrega do Projeto
A entrega do projeto deve ser feita até [data de entrega] .
Crie um repositório Git compartilhado para o projeto e compartilhe-o.
-se incluir um arquivo verifique README.md no repositório com instruções de como executar a aplicação localmente.


