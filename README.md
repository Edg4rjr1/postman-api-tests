Postman Library API v2
Esta coleção foi criada por mim como parte do teste para obtenção do certificado oficial do Postman. O objetivo foi montar uma coleção para testar uma API de biblioteca que gerencia livros.

Como criei a coleção
Importei e organizei as requisições para as principais operações da API: listar livros, buscar por gênero, adicionar, atualizar status de empréstimo e deletar livros.

Usei variáveis de coleção para facilitar o reuso de informações, como a URL base da API ({{baseUrl}}) e o ID do livro criado ({{id}}), que é salvo automaticamente após adicionar um livro.

Configurei o cabeçalho com uma variável para a chave de API (api-key), assim posso alterar facilmente o token sem mexer em todas as requisições.

Em algumas requisições, adicionei scripts de teste para extrair dados da resposta e salvar em variáveis, como o id do livro criado, para usar nas próximas chamadas de atualização ou exclusão.

Também incluí exemplos de chamadas com query parameters, como filtrar livros por gênero e status.

Variáveis usadas
{{baseUrl}}: URL base da API (https://library-api.postmanlabs.com)

{{id}}: armazeno o ID do livro criado para atualizar ou deletar depois

api-key (header): chave da API para autenticação, configurada como variável para fácil alteração

Testes e automatização
Usei scripts simples em “Tests” para validar respostas e salvar variáveis automaticamente, otimizando o fluxo de trabalho no Postman.

Isso facilita rodar a coleção completa com o Collection Runner sem precisar atualizar manualmente IDs ou tokens.

