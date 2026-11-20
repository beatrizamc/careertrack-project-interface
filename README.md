# CareerTrack — Portal de Vagas e Estágios

> Projeto acadêmico de desenvolvimento front-end para pesquisa de oportunidades profissionais e gerenciamento de candidaturas, com foco em estudantes e profissionais da área de Tecnologia da Informação.

## 1. Sobre o projeto

O **CareerTrack** reúne oportunidades de emprego e estágio em uma interface na qual o usuário pode pesquisar vagas, aplicar filtros, registrar candidaturas e acompanhar o andamento dos processos seletivos.

O site também oferece recursos de personalização e acessibilidade visual, como modo escuro, alto contraste e ajuste do tamanho da fonte.

O projeto foi desenvolvido com **HTML5, CSS3 e JavaScript puro**, sem framework JavaScript ou backend. As vagas são dados demonstrativos e as informações do perfil e das candidaturas são armazenadas localmente no navegador por meio do `localStorage`.

## 2. Tecnologias utilizadas

| Tecnologia/recurso | Utilização |
|---|---|
| HTML5 | Estrutura e organização do conteúdo e dos formulários. |
| CSS3 | Identidade visual, layouts, componentes e responsividade. |
| JavaScript (ES6+) | Interações, filtros, formulários e gerenciamento das candidaturas. |
| DOM API | Manipulação dos elementos e eventos da página. |
| localStorage | Armazenamento local do perfil e das candidaturas. |
| Google Fonts e Unsplash | Fonte Inter e imagens ilustrativas. |

## 3. Estrutura dos arquivos

```text
CareerTrack/
├── index.html    # Estrutura do site
├── style.css     # Estilos e responsividade
├── script.js     # Funcionalidades
└── README.md     # Documentação
```

Os três arquivos principais devem permanecer na mesma pasta, pois o HTML referencia o CSS e o JavaScript por caminhos relativos.

## 4. Construção do site — passo a passo

### 1. Planejamento e estrutura HTML

Primeiramente, foi definida a proposta do CareerTrack: facilitar a busca por oportunidades e organizar o acompanhamento de candidaturas. Em seguida, a estrutura foi desenvolvida em HTML5 e dividida em seções: acesso, navegação, apresentação inicial, destaques, explicação de funcionamento, listagem de vagas, candidaturas, contato e rodapé.

Também foram utilizados formulários e elementos de entrada para permitir a interação do usuário.

### 2. Identidade visual e responsividade com CSS

O arquivo `style.css` define a identidade visual do projeto, baseada principalmente em tons de roxo e azul, com fundos claros e cores neutras. Variáveis CSS foram utilizadas para manter a consistência de cores, fontes, bordas e sombras.

O layout utiliza **Flexbox** e **CSS Grid** para organizar os componentes. Media queries ajustam a disposição dos elementos para telas menores, tornando a interface mais adaptável a computadores, tablets e celulares.

### 3. Funcionalidades com JavaScript

O arquivo `script.js` implementa as interações da aplicação. As vagas de demonstração são organizadas em uma lista de objetos e exibidas dinamicamente na página.

Entre as principais funcionalidades estão:

- Busca de vagas por cargo, empresa ou área.
- Filtros por categoria, incluindo Tecnologia da Informação, Dados e estágio.
- Formulário de candidatura exibido em uma janela modal.
- Listagem, atualização de status e exclusão de candidaturas.
- Carrossel de conteúdos com navegação manual e automática.
- Controles de acessibilidade visual: aumento e redução da fonte, modo escuro e alto contraste.
- Formulário de contato com confirmação visual de envio.

### 4. Gerenciamento e armazenamento dos dados

Ao realizar uma candidatura, o sistema valida os campos, registra as informações da vaga e do candidato e define o status inicial como **Em análise**. O usuário pode acompanhar o registro e alterar seu status entre as opções disponíveis.

O `localStorage` é utilizado para manter o perfil e as candidaturas no navegador, mesmo após a atualização da página. Assim, os dados permanecem disponíveis no mesmo navegador, mas não são sincronizados entre dispositivos.

### 5. Finalização e testes

Após a implementação, foram organizadas as seções, os estilos e os eventos de interação. As funcionalidades podem ser verificadas diretamente no navegador: busca, filtros, candidatura, alteração de status, exclusão, carrossel e controles de acessibilidade.

## 5. Como executar

1. Baixe ou clone o repositório.
2. Mantenha `index.html`, `style.css` e `script.js` na mesma pasta.
3. Abra o arquivo `index.html` em um navegador atualizado.
4. Navegue pelo site e teste as funcionalidades disponíveis.

Também é possível abrir o projeto no Visual Studio Code e executá-lo com a extensão Live Server. Não é necessário instalar dependências ou configurar um servidor backend.

**Observação:** a fonte do Google Fonts e as imagens externas dependem de conexão com a internet.

## 6. Limitações do projeto

O CareerTrack é um protótipo acadêmico front-end. Portanto:

- O acesso e o cadastro são demonstrativos e não realizam autenticação real.
- As vagas são informações estáticas definidas no JavaScript.
- As candidaturas e o perfil ficam armazenados apenas no navegador utilizado.
- O formulário de contato exibe uma confirmação na interface, mas não envia mensagens para um servidor.
- O projeto não possui backend, banco de dados remoto ou integração com plataformas de emprego.

Uma evolução futura pode incluir autenticação segura, banco de dados, integração com uma API de vagas e sincronização das candidaturas entre dispositivos.
