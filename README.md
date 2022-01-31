#  Desafio do curso de React da Rocketseat - Upload de imagens

## :dart: Objetivo

Nesse desafio, você deverá criar uma aplicação para treinar o que aprendeu até agora no ReactJS

Essa será uma aplicação onde o seu principal objetivo é adicionar alguns trechos de código para que a aplicação de upload de imagens funcione corretamente. Você vai receber uma aplicação com muitas funcionalidades e estilizações já implementadas. Ela deve realizar requisições para sua própria API Next.js que vai retornar os dados do FaunaDB (banco de dados) e do ImgBB (serviço de hospedagem de imagens). A interface implementada deve seguir o layout do Figma. Você terá acesso a 4 arquivos para implementar:

- Infinite Queries e Mutations com React Query;
- Envio de formulário com React Hook Form;
- Exibição de Modal e Toast com Chakra UI;
- Entre outros.

## :white_check_mark: Requisitos

- **should be able to render loading**
    
    Para que esse teste passe você deve renderizar o componente `Loading.tsx` caso o React Query esteja carregando os dados, ou seja, o `isLoading` for `true`.
    
- **should be able to render error**
    
    Para que esse teste passe você deve renderizar o componente `Error.tsx` caso o React Query tenha falhado ao carregar os dados, ou seja, o `isError` for `true`.
    
- **should be able to render images list**
    
    Para que esse teste passe o seu código deve ser capaz de fazer uma requisição GET para rota `images` e renderizar em tela a listagem de imagens cadastradas no banco com as informações de título, descrição e preview da imagem.
    
- **should be able to view an image**
    
    Para que esse teste passe ele deve conseguir fazer as mesmas coisas do teste **should be able to render images list**. Porém, dessa vez o teste irá abrir uma imagem uma específica.
    
    Portanto, também é preciso que o seu código seja capaz de abrir uma modal com a imagem selecionada e o link com o texto `Abrir original` que redireciona para o endereço da imagem hospedada no ImgBB
    
- **should be able to load more images**
    
    Para que esse teste passe ele deve conseguir fazer as mesmas coisas do teste **should be able to render images list**. Porém, dessa vez a API irá retornar na primeira chamada um parâmetro informando que há mais dados a serem carregados.
    
    Portanto, também é preciso que seu código seja capaz de renderizar em tela um botão escrito `Carregar mais` e que, ao clicá-lo, você carregue e concatene as imagens da segunda requisição ao resultado da primeira. Por fim, o botão deve sumir quando não tiverem mais dados a serem carregados.
    
- **should be able to add a new image**
    
    Para que esse teste passe ele deve conseguir fazer as mesmas coisas do teste **should be able to load more images**. Porém, dessa vez também será realizado o cadastro de uma nova imagem que deve ser refletida na sua listagem.
    
    Portanto, também é preciso que o seu código seja capaz de abrir uma modal com um formulário de cadastro de uma nova imagem ao clicar no botão `Adicionar imagem`. Além disso, é preciso que ele possua os campos de input `image`, `title` e `description` para a correta adição da imagem. 
    
    Por fim, ao realizar o envio da imagem, a listagem deve ser automaticamente atualizada com todas as imagens que já apareciam e a nova imagem adicionada.
