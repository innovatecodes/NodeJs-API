# Tube Server Manager - Detalhes da API

- **Descrição**: API que permite criar e gerenciar listas personalizadas de vídeos do YouTube. Escolha seus vídeos preferidos e organize-os em playlists para entrega sob demanda.
- **Versão**: 1.0
- **Autor**: Ronaldo Lopes <contato@innovatecodes.com>
- **Criado em**: 2024-12-04 13:17:14
- **Última atualização**: Não definida

## Licença

- **Tipo**: MIT
- **URL**: [MIT License](https://opensource.org/licenses/MIT)
- **Termos**: Permite a utilização, cópia, modificação, fusão, publicação, distribuição, sublicenciamento e/ou venda de cópias do Software, desde que a cópia do aviso de copyright e a permissão sejam incluídas em todas as cópias do Software.

## Funcionalidades

- **Criação de Playlists**: Adicione vídeos do YouTube manualmente a playlists personalizadas.
- **Entrega de Vídeos**: Sirva vídeos de suas playlists para usuários de forma eficiente.
- **Gerenciamento Personalizado**: Organize suas listas e edite a seleção de vídeos a qualquer momento.

## Endpoints da API

### `GET /api/v1/videos/`
- **Descrição**: Lista todos os vídeos.
- **Método HTTP**: GET
- **Resposta esperada**: Retorna todos os vídeos registrados.

### `POST /api/v1/videos/`
- **Descrição**: Cria um novo vídeo.
- **Método HTTP**: POST
- **Corpo da requisição**: Necessário enviar dados do vídeo (categoria, descrição, título, link).
- **Resposta esperada**: Retorna o vídeo criado com o status de sucesso.

### `GET /api/v1/videos/{id}`
- **Descrição**: Busca um vídeo específico pelo ID.
- **Método HTTP**: GET
- **Parâmetros**: `{id}` - Id do vídeo a ser buscado.
- **Resposta esperada**: Retorna o vídeo correspondente ao ID informado.

### `PUT /api/v1/videos/{id}`
- **Descrição**: Atualiza um vídeo específico.
- **Método HTTP**: PUT
- **Parâmetros**: `{id}` - Id do vídeo a ser atualizado.
- **Corpo da requisição**: Necessário enviar dados atualizados do vídeo.
- **Resposta esperada**: Retorna o vídeo atualizado.

### `DELETE /api/v1/videos/{id}`
- **Descrição**: Deleta um vídeo específico.
- **Método HTTP**: DELETE
- **Parâmetros**: `{id}` - Id do vídeo a ser deletado.
- **Resposta esperada**: Retorna uma confirmação de que o vídeo foi deletado com sucesso.
