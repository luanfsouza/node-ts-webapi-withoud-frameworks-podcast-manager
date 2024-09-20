## Podcast Manager

**## Podcast Manager**

### Descrição

Aplicativo web que centraliza episódios de podcasts em vídeo, organizados em categorias, proporcionando uma experiência similar à plataforma Netflix.

### Objetivo

Oferecer uma interface intuitiva para os usuários encontrarem e assistirem seus podcasts favoritos, filtrados por categorias e nomes específicos.

### Tecnologias Utilizadas

* **TypeScript:** Linguagem de programação de tipagem estática usada para desenvolver o projeto. [https://www.typescriptlang.org/]
* **tsx:** Compilador TypeScript para JavaScript. [https://www.typescriptlang.org/docs/handbook/jsx.html]
* **Node.js:** Gerenciador de pacotes para Node.js. [https://nodejs.org/]
* **npm:** Ambiente de execução JavaScript para o lado do servidor. [https://www.npmjs.com/]

### Estrutura do Projeto

* **Backend:**
    * **Rotas:**
        * `/api/episodes`: Retorna a lista completa de episódios.
        * `/api/episodes?podcast=nome_do_podcast`: Retorna os episódios de um podcast específico.
    * **Modelos:** Define a estrutura dos dados dos episódios (podcastName, episodio, cover, videoId, link, category).
    * **Controladores:** Controla as requisições HTTP e a lógica de negócio.
* **Frontend:**
    * **Componentes:**
        * `EpisodeList`: Lista os episódios com filtros e busca.
        * `EpisodeCard`: Exibe as informações de cada episódio.
    * **States:** Gerencia o estado da aplicação (lista de episódios, filtros ativos).

### Como Usar

1. **Clonar o repositório:**
   ```bash
   git clone https://github.com/seu_usuario/podcast-manager.git
   ```
2. **Instalar as dependências:**
   ```bash
   cd podcast-manager
   npm install
   ```
3. **Iniciar o servidor:**
   ```bash
   npm run start:prod
   ```
4. **Acessar o aplicativo:**
   Abrir o navegador e acessar `http://localhost:3637` (ou a porta configurada no aqruivo .env).

### Estrutura de Dados (Exemplo)

```json
[
  {
    "podcastName": "Flow Podcast",
    "episodio": "Conversa com o Presidente",
    "cover": "https://example.com/cover.jpg",
    "videoId": "1234567890",
    "link": "https://www.youtube.com/watch?v=1234567890",
    "category": ["política", "entrevistas"]
  },
  // ... outros episódios
]
```

### Próximos Passos

* **Implementar a busca:** Permitir que o usuário busque por palavras-chave nos títulos dos episódios.
* **Adicionar autenticação:** Permitir que os usuários criem contas e personalizem suas listas de favoritos.
* **Melhorar a interface do usuário:** Desenvolver uma interface mais intuitiva e visualmente atraente.
* **Integrar com outras plataformas:** Permitir a importação de podcasts de outras plataformas (Spotify, Apple Podcasts).
* **Implementar um sistema de recomendação:** Sugerir episódios com base no histórico de visualização do usuário.

### Contribuições

Contribuições são bem-vindas! Para contribuir, siga estes passos:

1. Fork este repositório.
2. Crie um novo branch para sua feature.
3. Faça suas alterações e commit.
4. Envie um pull request.

### Licença
[MIT]