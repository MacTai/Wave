# Wave
Aplicação Web de Consulta de Filmes com Next.js e OMDb API  
## Estrutura do Projeto

```bash
npx create-next-app movie-query-app
cd movie-query-app
npm install axios
Este relatório detalha o desenvolvimento de uma aplicação web que permite aos usuários pesquisar por filmes, visualizar informações detalhadas e salvar seus favoritos. A aplicação foi desenvolvida utilizando a API pública do OMDb como fonte de dados e seguindo os requisitos estabelecidos.

Arquitetura da Aplicação
Tecnologias Utilizadas:

Frontend: React.js (biblioteca JavaScript para construção de interfaces de usuário)
Backend: Não há um backend específico neste projeto, pois todas as interações com a API são realizadas diretamente do frontend.
Styling: Material UI (biblioteca de componentes para React)
API: OMDb API (serviço de banco de dados de filmes online)
Estrutura:

A aplicação foi organizada em componentes funcionais, cada um responsável por uma parte específica da interface do usuário:

Página de Busca: Componente para a entrada de texto e exibição dos resultados da busca.
Card de Filme: Componente reutilizável para exibir as informações básicas de um filme nos resultados da busca.
Página de Detalhes: Componente para exibir informações detalhadas de um filme específico.
Lista de Favoritos: Componente para gerenciar a lista de filmes favoritos do usuário (local storage).
Implementação
Integração com a OMDb API:

Chave de API: Uma chave de API gratuita foi obtida do site da OMDb e configurada como uma variável de ambiente no projeto.
Requisições: As requisições à API foram realizadas utilizando a biblioteca axios para fazer chamadas HTTP. Os parâmetros de busca, como o título do filme, foram passados como query params na URL da requisição.
Tratamento de Dados: Os dados retornados pela API foram processados para extrair as informações relevantes e renderizar a interface do usuário de acordo.
Funcionalidades:

Busca de Filmes: O usuário pode digitar o título de um filme na caixa de busca e os resultados são exibidos em tempo real.
Página de Detalhes: Ao clicar em um resultado da busca, o usuário é direcionado para uma página com informações detalhadas sobre o filme.
Lista de Favoritos: Os filmes podem ser adicionados à lista de favoritos clicando em um botão. A lista é armazenada no local storage do navegador para persistência.
Estilização: A aplicação utiliza o Material UI para garantir uma interface consistente e agradável ao usuário.
Funcionalidades Opcionais Implementadas:

Paginação: A busca de filmes foi implementada com paginação, permitindo que o usuário navegue por mais resultados.
Filtros: Foram adicionados filtros básicos à busca, como o ano de lançamento.
Testes
Foram realizados testes manuais para garantir o funcionamento correto de todas as funcionalidades da aplicação. Os testes incluíram:

Busca por diferentes títulos de filmes: Verificar se os resultados são relevantes e se a paginação funciona corretamente.
Visualização de detalhes de filmes: Confirmar se todas as informações relevantes são exibidas corretamente.
Gerenciamento da lista de favoritos: Adicionar e remover filmes da lista, verificar se a lista é persistida corretamente.
Próximos Passos
Melhorias na Busca: Implementar uma busca mais robusta, com autocompletar e sugestões.
Mais Filtros: Adicionar mais opções de filtros, como gênero, diretor e ator.
Integração com Banco de Dados: Armazenar a lista de favoritos em um banco de dados para permitir o acesso a partir de diferentes dispositivos.
Responsividade: Otimizar a aplicação para diferentes tamanhos de tela.
Teste Unitários: Implementar testes unitários para garantir a qualidade do código.
Conclusão
A aplicação de busca de filmes foi desenvolvida com sucesso, atendendo aos requisitos estabelecidos e proporcionando uma boa experiência ao usuário. A utilização da API OMDb permitiu a integração com um vasto banco de dados de filmes, enquanto as tecnologias React e Material UI garantiram uma interface moderna e fácil de usar.
