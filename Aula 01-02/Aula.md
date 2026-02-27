## 📘 Aula 1 (Parte I): Introdução à Web e ao Desenvolvimento

### 🔍 O que é Desenvolvimento Web?

O desenvolvimento web é a área da tecnologia responsável por criar sites, sistemas e aplicações que funcionam através da internet ou de redes locais. Esses sistemas geralmente são compostos por duas partes principais:

#### 🔹 Cliente (Client) x Servidor (Server)

- **Cliente (Client):**  
  O cliente é o computador ou dispositivo do usuário que faz uma requisição (pedido) para acessar uma página ou serviço na internet. Normalmente, esse papel é desempenhado pelo navegador web (Google Chrome, Firefox, Safari, etc.).

  Exemplo:  
  Quando você digita `https://www.google.com` no seu navegador e pressiona Enter, o navegador é o cliente que faz uma solicitação para o servidor do Google.

* **Servidor (Server):**  
  O servidor é uma máquina (computador) que armazena os arquivos e dados de um site ou sistema. Ele recebe as requisições do cliente, processa essas solicitações (se necessário) e envia uma resposta de volta.

  **Exemplo:**  
  O servidor do Google recebe o pedido do seu navegador e devolve a página de busca pronta para ser exibida.

#### 🔹 Front-end x Back-end

- **Front-end:**  
  É a parte do desenvolvimento que lida com o que o usuário vê e interage diretamente no navegador. O front-end é construído com tecnologias como:

  - HTML (estrutura da página)
  - CSS (estilo da página)
  - JavaScript (interatividade da página)

  **Exemplo:**  
  Botões, menus, animações e formulários de um site fazem parte do front-end.

* **Back-end:**  
  É a parte que funciona "por trás dos panos", no servidor. O back-end é responsável por processar dados, acessar bancos de dados, autenticar usuários, etc. As linguagens e tecnologias comuns no back-end incluem:

  - Node.js, Python, Java, PHP, Ruby, etc.
  - Banco de Dados: MySQL, PostgreSQL, MongoDB, etc.

  Exemplo:  
  Quando você faz login em um site, o back-end verifica seu usuário e senha no banco de dados antes de permitir o acesso.

---

📝 **Resumo rápido:**

| Conceito      | O que é?                                                | Exemplo                                  |
|--------------|---------------------------------------------------------|------------------------------------------|
| Cliente      | Dispositivo/navegador que faz uma requisição ao servidor | Seu navegador acessando um site          |
| Servidor     | Computador que armazena e envia os dados da aplicação    | Servidor do Google enviando a página     |
| Front-end    | Parte visível da aplicação que o usuário interage        | Botão, formulário, menu em um site       |
| Back-end     | Parte que processa dados e regras no servidor            | Verificação de login, acesso ao banco de dados |

---

### 🔍 Como funciona a Web: HTTP, URL, Navegador e Servidor

A internet funciona através da troca de informações entre dois pontos principais: **cliente** e **servidor**. Essa troca é realizada usando regras bem definidas chamadas de **protocolo**. O principal protocolo da web é o **HTTP**.

#### 🔹 HTTP – HyperText Transfer Protocol

- O **HTTP (Protocolo de Transferência de Hipertexto)** é o conjunto de regras que define como os dados são enviados e recebidos entre o cliente (navegador) e o servidor.
- Ele permite, por exemplo, que você abra páginas web, envie formulários e acesse APIs.

**Exemplo de requisição:**

- Cliente (Navegador) → faz um pedido HTTP → Servidor (Web)
- Servidor (Web) → envia uma resposta HTTP → Cliente (Navegador)


##### ▻ Principais métodos HTTP:
- **GET** – Requisitar (buscar) informações de um servidor.
- **POST** – Enviar dados para serem processados no servidor.
- **PUT** – Atualizar dados existentes no servidor.
- **DELETE** – Remover dados do servidor.

---

#### 🔹 URL – Uniform Resource Locator

- A **URL** é o endereço de um recurso (como uma página ou imagem) na internet.
* Estrutura de uma URL:
![text](https://cwbm.com.br/wp-content/uploads/2019/07/estrutura-de-urls-1024x427.png)


#### Exemplos de URLs:
- `https://www.google.com`
- `https://meusite.com/contato`
- `http://api.exemplo.com/v1/usuarios`

---

#### 🔹 Navegador (Browser)

- O navegador é o programa que interpreta e exibe os arquivos HTML, CSS e JavaScript vindos do servidor.
* Principais navegadores: **Google Chrome, Mozilla Firefox, Safari, Microsoft Edge**.
- O navegador também faz requisições HTTP e renderiza (exibe) o resultado visual para o usuário.

---

#### 🔹 Servidor

- O servidor é responsável por armazenar os arquivos de um site e responder às requisições dos clientes.
* Tipos de servidores:
  - **Servidor Web:** Apache, Nginx
  - **Servidor de Aplicação:** Node.js, Express, Django

---

📝 **Resumo rápido:**

| Termo     | O que é?                                          | Exemplo                                 |
|-----------|---------------------------------------------------|-----------------------------------------|
| HTTP      | Protocolo de comunicação entre cliente e servidor | Carregar uma página web                 |
| URL       | Endereço de um recurso na web                     | https://www.exemplo.com/pagina          |
| Navegador | Programa que interpreta HTML/CSS/JS               | Google Chrome, Firefox                  |
| Servidor  | Computador que armazena e envia os dados          | Servidor do Google, API de um sistema   |

---

### 🔵 Ferramentas Básicas: Editores, Navegadores e DevTools

Para desenvolver sites e aplicações web, utilizamos algumas ferramentas essenciais que facilitam o trabalho do programador.

---

#### 🔹 Editores de Código

O editor de código é o programa onde você escreve seus arquivos HTML, CSS e JavaScript.

##### ▻ Principais editores:
- **Visual Studio Code (VS Code):**  
  Gratuito, leve e com milhares de extensões para facilitar o desenvolvimento web.
- **Sublime Text:**  
  Leve e rápido, mas algumas funções avançadas são pagas.
- **Atom (descontinuado):**  
  Ainda usado por algumas pessoas, mas o suporte foi encerrado.

##### ▻ Por que usar o VS Code?
- Suporte a várias linguagens (HTML, CSS, JS, etc.).
- Extensões úteis: Live Server, Prettier, ESLint.
- Interface amigável.
- Gratuito.

---

#### 🔹 Navegadores

São os programas que abrem e exibem os sites.

##### ▻ Principais navegadores:
- **Google Chrome (recomendado para desenvolvimento)**
- Mozilla Firefox
- Microsoft Edge
- Safari

Cada navegador possui ferramentas internas que ajudam no desenvolvimento (as DevTools).

---

#### 🔹 DevTools (Ferramentas de Desenvolvedor)

As **DevTools** são um conjunto de ferramentas integradas no navegador que permitem:

- Visualizar o HTML gerado da página.
- Alterar o CSS em tempo real.
- Verificar erros de JavaScript.
- Analisar o desempenho e tempo de carregamento.
- Simular tamanhos de tela (responsividade).

##### ▻ Acessando as DevTools:
- Atalho: `F12` ou `Ctrl + Shift + I` (Windows) | `Cmd + Option + I` (Mac)
- Clique com o botão direito na página → **"Inspecionar"**

---

📝 **Resumo rápido:**

| Ferramenta     | Função                                        | Exemplo                         |
|----------------|---------------------------------------------|---------------------------------|
| Editor de Código | Onde você escreve o código do seu site       | VS Code, Sublime Text           |
| Navegador      | Exibe o resultado visual do seu site         | Google Chrome, Firefox          |
| DevTools       | Permite inspecionar e testar o site no navegador | Inspecionar elementos, console JS |

---

### 🔵 Estrutura de um Site

Um site moderno geralmente é composto por **três tipos de arquivos principais**: **HTML, CSS e JavaScript**. Cada um tem um papel específico no funcionamento da página.

---

#### 🔍 Qual o objetivo de cada linguagem?

##### 🔹 1. HTML (HyperText Markup Language)

**Função:**   Responsável pela **estrutura e conteúdo** da página.   O HTML define os elementos visíveis como textos, títulos, imagens, links, listas, formulários, etc.

**Exemplo de código HTML:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Meu Primeiro Site</title>
</head>
<body>
    <h1>Bem-vindo ao meu site!</h1>
    <p>Este é um parágrafo de texto.</p>
</body>
</html>
```

##### 🔹 2. CSS (Cascading Style Sheets)
**Função:** Responsável pelo **estilo e aparência visual** da página. Com o CSS, você define cores, tamanhos de fonte, espaçamento, bordas, posicionamento de elementos e muito mais.

**Exemplo de código CSS:**
```css
body {
  background-color: #f0f0f0;
  font-family: Arial, sans-serif;
}

h1 {
  color: blue;
}
```

##### 🔹 3. JavaScript
**Função:** Responsável pela **interatividade e comportamento** da página. O JavaScript permite criar ações dinâmicas, como responder a cliques de botões, validar formulários, carregar dados de APIs, entre outros.

**Exemplo de código JavaScript:**
```js
function mostrarMensagem() {
  alert('Olá, bem-vindo ao meu site!');
}
```

📝 **Resumo rápido:**

| Linguagem   | Função                          | Exemplo de uso                        |
|------------|---------------------------------|--------------------------------------|
| HTML       | Estrutura e conteúdo da página   | Títulos, parágrafos, imagens, links   |
| CSS        | Estilo e aparência visual        | Cores, fontes, tamanhos, layout       |
| JavaScript | Interatividade e comportamento   | Cliques, validação de dados, animações |

---

### 🔵 GitHub
O GitHub é uma plataforma de **hospedagem de código-fonte** que permite salvar, compartilhar e colaborar em projetos.

**Criar uma conta:**
- Acesse: https://github.com
- Clique em **Sign Up** e preencha os dados.

**Criar um repositório:**
- Após fazer login, clique em **New Repository**
- Dê o nome: C - OxeTech Lab
- Clique em **Create repository**

**Adicionar arquivos manualmente**
- Dentro do repositório, clique em **Add file** > **Upload files**
- Escolha o arquivo `.c` ou pasta do seu computador
- Clique em **Commit changes**

**Estrutura do Repositório:**
```scss
📁 desenvolvimento-web
├── 📁 Aula 1
│   └── (Exercícios da Aula 1)
├── 📁 Aula 2
│   └── (Exercícios da Aula 2)
├── 📁 Aula 3
│   └── (Exercícios da Aula 3)
├── 📁 Aula 4
│   └── (Exercícios da Aula 4)
├── 📁 Aula 5
│   └── (Exercícios da Aula 5)
├── 📁 Aula 6
│   └── (Exercícios da Aula 6)
├── 📁 Aula 7
│   └── (Exercícios da Aula 7)
├── 📁 Aula 8
│   └── (Exercícios da Aula 8)
├── 📁 Aula 9
│   └── (Exercícios da Aula 9)
├── 📁 Aula 10
│   └── (Exercícios da Aula 10)
├── 📁 Aula 11
│   └── (Exercícios da Aula 11)
├── 📁 Aula 12
│   └── (Exercícios da Aula 12)
├── 📁 Aula 13
│   └── (Exercícios da Aula 13)
├── 📁 Aula 14
│   └── (Exercícios da Aula 14)
├── 📁 Projetos
│   └── (Projetos que serão criados ao longo do curso)
├── 📁 Projeto Final
│   └── (Projeto final completo feito ao final do curso)
```

<br>

## 📘 Aula 1 (Parte II): Estrutura e Semântica

### 🔵 Introdução ao HTML (Revisão)

O **HTML (HyperText Markup Language)** é a linguagem de marcação utilizada para estruturar o conteúdo de páginas na web. Ele define o que será exibido no navegador, como textos, imagens, vídeos, links e outros elementos.

---

#### 🔹 Principais Características do HTML:

- **Hipertexto:**  Permite criar links para outras páginas ou recursos.

- **Linguagem de Marcação:**  Utiliza "tags" (etiquetas) para marcar o início e o fim dos elementos da página.

---

##### 🔹 Estrutura de uma Tag HTML:

![](https://www.chiefofdesign.com.br/wp-content/uploads/2018/05/estrutura-de-um-elemento-html.jpg)

---

##### 🔹 Estrutura Mínima de um Documento HTML

```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <title>Meu Primeiro Site</title>
  </head>
  <body>
    <h1>Olá, mundo!</h1>
    <p>Bem-vindo ao meu site.</p>
  </body>
</html>
```

**Explicando cada parte:**
| Parte                    | Função                                                             |
|-------------------------|--------------------------------------------------------------------|
| `<!DOCTYPE html>`        | Informa ao navegador que este é um documento HTML5                  |
| `<html>`                | Elemento raiz do documento                                          |
| `<head>`                | Contém informações da página (não visíveis), como título e metadados |
| `<meta charset="UTF-8">` | Define a codificação de caracteres (importante para acentuação)      |
| `<title>`               | Define o título que aparece na aba do navegador                     |
| `<body>`                | Contém o conteúdo visível da página                                  |

---

#### 🔍 Por que o HTML é importante?

- É a base de toda página web;
- Organiza o conteúdo de forma lógica e estruturada;
- Facilita o trabalho de outras tecnologias, como CSS (estilo) e JavaScript (interatividade).

---

📝 **Resumo rápido:**

| Termo       | O que é?                                                  |
|------------|-----------------------------------------------------------|
| HTML       | Linguagem de marcação usada para estruturar páginas web     |
| Tag        | Elemento que define partes do conteúdo (ex: `<p>`, `<h1>`) |
| Atributo   | Informações extras dentro das tags (ex: `lang="pt-br"`)    |
| Estrutura  | Documento deve ter sempre: `<!DOCTYPE>`, `<html>`, `<head>`, `<body>` |

---

### 🔵 Elementos e Estrutura Básica 

Todo documento HTML possui uma estrutura básica obrigatória, que organiza o conteúdo da página de forma clara e compreensível para o navegador.

---

#### 🔹 Principais Elementos da Estrutura:

#### 1. `<html>`

- **Função:**  Elemento raiz do documento.  Todo o conteúdo da página deve estar dentro dessa tag.

##### Exemplo:
```html
<html lang="pt-br">
  <!-- Conteúdo da página aqui -->
</html>
```

---

#### 2. `<head>`
**Função:** Contém metadados (dados sobre a página) que não são exibidos diretamente ao usuário, mas são essenciais para o funcionamento da página e sua interpretação pelos navegadores e mecanismos de busca.

**Itens comuns no `<head>`:**

- `<meta charset="UTF-8">`: Define a codificação de caracteres.
- `<title>`: Define o título da aba do navegador.
- `<link>`: Importa arquivos externos (CSS, ícones).
- `<script>`: Inclui ou referencia arquivos JavaScript.

**Exemplo:**
```html
<head>
  <meta charset="UTF-8">
  <title>Minha Página</title>
</head>
```

---

#### 3. `<body>`
**Função:** Contém todo o conteúdo visível da página, como textos, imagens, links, listas, tabelas, vídeos e outros elementos interativos.

**Exemplo:**
```html
<body>
  <h1>Bem-vindo!</h1>
  <p>Esta é a minha primeira página HTML.</p>
</body>
```

---

**Exemplo Completo de Estrutura HTML Básica:**
```html
<!DOCTYPE html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8">
    <title>Página Exemplo</title>
  </head>
  <body>
    <h1>Olá, mundo!</h1>
    <p>Esta é uma página simples feita com HTML.</p>
  </body>
</html>

```

---

📝 **Resumo rápido:**

| Elemento  | Função                                             |
|-----------|---------------------------------------------------|
| `<html>`  | Elemento raiz; envolve todo o código da página     |
| `<head>`  | Contém metadados, título, links e scripts externos |
| `<body>`  | Contém o conteúdo visível da página (textos, imagens, etc.) |

---

#### 🔵 Tags Básicas

O HTML oferece diversas tags para estruturar o conteúdo de uma página. Vamos conhecer as mais utilizadas no dia a dia do desenvolvimento web.

---

#### 1. Títulos (`<h1>` a `<h6>`)

- Usados para definir títulos e subtítulos.
- Existem 6 níveis: `<h1>` (mais importante) até `<h6>` (menos importante).

**Exemplo:**
```html
<h1>Título Principal</h1>
<h2>Subtítulo</h2>
```

---

#### 2. Parágrafos (`<p>`)
- Usados para escrever blocos de texto.

**Exemplo:**
```html
<p>Este é um parágrafo de texto.</p>
```

---

#### 3. Listas
**(a) Lista Não Ordenada (`<ul>`)**
- Utilizada para listas sem ordem específica (marcadores).

**Exemplo:**
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```

**(b) Lista Ordenada (`<ol>`)**
- Utilizada para listas numeradas.

**Exemplo:**
```html
<ol>
    <li>Primeiro item</li>
    <li>Segundo item</li>
</ol>
```

A tag `<li>` é usado para definir os itens na lista.

---

#### 4. Links (`<a>`)
- Utilizados para criar hiperlinks para outras páginas, sites ou arquivos.

**Atributo importante:**
- `href`: Define o destino do link.

**Exemplo:**
```html
<a href="https://www.google.com" target="_blank">Ir para o Google</a>
```

---

#### 5. Imagens (<`img>`)
- Usada para exibir imagens na página.

**Atributos importantes:**
- `src`: Caminho da imagem.
- `alt`: Texto alternativo (acessibilidade).

**Exemplo:**
```html
<img src="imagem.jpg" alt="Descrição da imagem">
```

---

📝 **Resumo rápido:**

| Tag    | Função                                      | Exemplo                                  |
|--------|--------------------------------------------|-----------------------------------------|
| `<h1>` a `<h6>` | Títulos e subtítulos                  | `<h1>Olá</h1>`                          |
| `<p>`   | Parágrafos de texto                         | `<p>Texto aqui</p>`                      |
| `<ul>`, `<ol>`, `<li>` | Listas não ordenadas e ordenadas | `<ul><li>Item</li></ul>`               |
| `<a>`   | Links para outras páginas ou sites          | `<a href="url">Link</a>`                 |
| `<img>` | Inserção de imagens                         | `<img src="imagem.jpg" alt="descrição">` |

---

### 🔵  Elementos Semânticos

Elementos semânticos ajudam a dar significado ao conteúdo da página, facilitando a organização, a acessibilidade e a indexação por buscadores.

---

#### 1. `<header>`

- Representa o cabeçalho da página ou de uma seção.
- Normalmente contém logo, título, menu de navegação ou informações introdutórias.

**Exemplo:**
```html
<header>
  <h1>Meu Site</h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#sobre">Sobre</a>
  </nav>
</header>
```

---

#### 2. `<main>`

- Representa o conteúdo principal da página.
- Deve ser único por página (apenas um `<main>)`).
- O conteúdo principal é a parte que difere de uma página para outra.

**Exemplo:**
```html
<main>
  <section>
    <h2>Artigo Principal</h2>
    <p>Conteúdo importante da página.</p>
  </section>
</main>
```

---

#### 3. `<section>`
- Representa uma seção genérica do conteúdo, agrupando conteúdos relacionados.
- Pode ser usada para dividir o conteúdo em blocos temáticos.

**Exemplo:**
```html
<section>
  <h2>Sobre Nós</h2>
  <p>Informações sobre a empresa.</p>
</section>
```

---

#### 4. `<footer>`
- Representa o rodapé da página ou de uma seção.

- Geralmente contém informações de contato, direitos autorais e links adicionais.

**Exemplo:**
```html
<footer>
  <p>© 2025 Meu Site. Todos os direitos reservados.</p>
</footer>
```

---

#### 🔍 Por que usar elementos semânticos?
- Melhoram a acessibilidade para leitores de tela.
- Facilitam o SEO (otimização para buscadores).
- Tornam o código mais organizado e legível para desenvolvedores.

---

📝 **Resumo rápido:**

| Elemento | Função                                      | Exemplo de uso                    |
|----------|---------------------------------------------|----------------------------------|
| `<header>` | Cabeçalho da página ou seção               | Logo, menu, título                |
| `<main>`   | Conteúdo principal da página                | Artigos, informações principais  |
| `<section>`| Seção temática do conteúdo                   | Blocos com assuntos relacionados |
| `<footer>` | Rodapé da página ou seção                    | Contato, direitos autorais       |

---