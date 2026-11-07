# Landing page de arquitetura — Desafio 1 DNC

Desenvolvi esta landing page como meu primeiro desafio de desenvolvimento web na Escola DNC. A proposta foi transformar uma referência visual em uma página para uma **empresa fictícia de arquitetura**, apresentando seus serviços, sua experiência e um formulário de contato.

Neste projeto, pratiquei a estruturação com HTML, a estilização com CSS e a configuração de um formulário integrado ao Sheet Monkey. Organizei a página para conduzir a visita da apresentação da empresa até o contato com seus serviços.

**[Acessar a demonstração](https://emanoel-desafio-1-dnc.netlify.app/)** · **[Consultar a planilha vinculada ao projeto](https://docs.google.com/spreadsheets/d/12dzx7m244vIniTKbuZVq0IPBQqiWvhWMXoR83FlyIHo/edit?usp=sharing)**

## Contexto do desafio

Recebi um cenário de avaliação técnica no qual um gerente de recrutamento solicitava a criação de uma landing page para uma empresa de arquitetura. Meu objetivo foi desenvolver a interface a partir do layout proposto, respeitando a sequência das seções e a identidade visual da referência.

Trabalhei com uma página única, dividida em quatro partes:

1. Apresentação dos serviços de arquitetura residencial e comercial.
2. Indicadores de experiência e atuação da empresa.
3. Seção institucional com texto e imagem de um ambiente.
4. Formulário para captar o nome e o e-mail de pessoas interessadas.

Os números e as informações institucionais fazem parte do conteúdo demonstrativo do desafio.

## Referência visual

![Layout proposto no Figma para a landing page de arquitetura](https://github.com/EmanoelAngelo/projeto1-dnc/assets/155268752/0b2e7ba0-b95f-4895-bc9e-c179045783c6)

Utilizei o layout apresentado no Figma como referência para definir a ordem do conteúdo, os blocos de cor e a distribuição dos elementos. A proposta combina áreas escuras de abertura e contato com seções claras para os indicadores e a apresentação institucional.

A imagem acima registra a referência recebida. Nas capturas seguintes, mostro como organizei a versão que desenvolvi.

## Apresentação e indicadores

![Versão desenvolvida com título de apresentação e faixa de indicadores da empresa fictícia](https://github.com/EmanoelAngelo/projeto1-dnc/assets/155268752/33e957db-cf21-4591-b0fc-31a1c3827527)

Na abertura, destaquei a frase **“Tradição em projetos de arquitetura”**, acompanhada de **“Arquitetura residencial e comercial”**. Utilizei um fundo escuro e texto branco para criar contraste e comunicar o segmento da empresa logo no início da visita.

Na sequência, incluí uma faixa clara com três indicadores presentes na referência:

| Indicador demonstrativo | Informação apresentada |
| --- | --- |
| 850 | Empreendimentos construídos. |
| 40 | Anos de mercado e experiência. |
| 2.000.000 m² | Área em projetos construídos. |

Com essa transição, procurei apresentar primeiro a proposta da empresa e depois os dados que contextualizam sua experiência. Nesta implementação, inseri a composição dos indicadores como uma imagem no HTML.

## Seção institucional

![Seção institucional com texto sobre a empresa de arquitetura e imagem de um ambiente interno](https://github.com/EmanoelAngelo/projeto1-dnc/assets/155268752/36a6d309-c539-47b8-8edb-b0d28f30b841)

Nesta seção, apresentei o conteúdo **“Arquitetos com História e Experiência”**, acompanhado de uma descrição sobre projetos, gerenciamento de obras e criação de ambientes personalizados.

Mantive o texto à esquerda e a imagem do ambiente à direita, seguindo a composição da referência. Minha intenção foi complementar a abertura com uma apresentação mais detalhada dos serviços e com uma imagem relacionada ao trabalho de arquitetura.

No código desta versão, inseri essa composição institucional como uma imagem que reúne o texto e a fotografia. O posicionamento e os espaços ao redor foram definidos no CSS.

## Formulário de contato

![Formulário com campos de nome e e-mail e botão Fale Conosco](https://github.com/EmanoelAngelo/projeto1-dnc/assets/155268752/f80220fe-4358-4bbd-9fe2-80b2a2ac4e67)

Ao final da página, criei a chamada **“Conheça mais sobre nossos serviços”** e um formulário com os campos de nome e e-mail. Destaquei o botão **“Fale Conosco”** em uma cor diferente do fundo para facilitar a identificação da ação principal.

| Elemento | Como implementei |
| --- | --- |
| Nome | Campo de texto obrigatório para identificar o contato. |
| E-mail | Campo obrigatório do tipo `email`, com validação nativa do navegador. |
| Data e hora | Campo oculto configurado para o preenchimento pelo Sheet Monkey. |
| Envio | Formulário configurado com o método `POST` para o serviço Sheet Monkey. |
| Botão | Efeito de mudança de cor, deslocamento e sombra ao passar o cursor. |

Configurei a integração com o Sheet Monkey para encaminhar os dados do formulário à planilha vinculada ao projeto, sem implementar um servidor próprio para receber esses contatos.

## Tecnologias e recursos utilizados

| Tecnologia ou recurso | Como utilizei |
| --- | --- |
| HTML | Estruturei as seções, os títulos, as imagens e os campos do formulário. |
| CSS | Defini cores, tipografia, dimensões, espaçamentos e o efeito do botão. |
| Google Fonts | Carreguei as fontes Inter e Raleway utilizadas na apresentação. |
| Sheet Monkey | Configurei o recebimento dos dados enviados pelo formulário. |
| Netlify | Publiquei a demonstração indicada no início deste README. |
| Figma | Consultei a referência visual fornecida no desafio. |

A página desta versão funciona com **HTML e CSS**, além da integração externa do formulário. Mantive o arquivo `index.js` no repositório, mas ele está vazio e não contém lógica de interação.

## Organização do projeto

| Arquivo ou pasta | Conteúdo |
| --- | --- |
| [`index.html`](index.html) | Estrutura da página e configuração do formulário. |
| [`style.css`](style.css) | Estilos das seções, campos e botão. |
| [`index.js`](index.js) | Arquivo reservado, sem implementação nesta versão. |
| [`imagem/`](imagem/) | Imagens utilizadas na composição da página. |
| [`README.md`](README.md) | Apresentação e documentação do projeto. |

## O que aprendi e apliquei

- Transformei uma referência visual em uma página web.
- Organizei o conteúdo em seções com uma sequência de apresentação.
- Trabalhei com contraste, fontes, espaçamentos e alinhamento.
- Configurei campos obrigatórios e validação nativa de e-mail.
- Integrei um formulário HTML a um serviço externo de recebimento de dados.
- Apliquei um efeito visual de interação ao botão de contato.
- Publiquei o projeto e documentei o resultado com capturas de tela.

## Como visualizar localmente

Para consultar a página no seu computador:

```bash
git clone https://github.com/EmanoelAngelo/projeto1-dnc.git
cd projeto1-dnc
```

Depois, abra o arquivo `index.html` no navegador ou utilize um servidor local de arquivos estáticos, como o Live Server.

Não é necessário instalar dependências ou executar um processo de build. O formulário continua apontando para o serviço externo configurado no HTML.

## Autor

Sou **Emanoel Angelo** e desenvolvi este projeto durante minha formação na Escola DNC.

[GitHub](https://github.com/EmanoelAngelo) · [LinkedIn](https://www.linkedin.com/in/emanoelangelo/)
