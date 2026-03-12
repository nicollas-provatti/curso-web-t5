# 📘 Aula 3 - CSS: Modelo de Caixa, Unidades de Medida, Cores e Fontes

---

## 🔵 Box Model

O **Box Model** é um conceito fundamental do CSS que define como os elementos HTML são renderizados e ocupam espaço na página.

Cada elemento é considerado como uma "caixa" composta por 4 áreas:
- **Content**: conteúdo real do elemento (texto, imagem, etc.)
- **Padding**: espaço interno, entre o conteúdo e a borda
- **Border**: borda ao redor do padding e conteúdo
- **Margin**: espaço externo, fora da borda	

Veja a representação abaixo:

![](https://media.gcflearnfree.org/content/5ef2084faaf0ac46dc9c10be_06_23_2020/box_model.png)

<br>

**Importante:**
- O valor do tamanho total de um elemento normalmente é calculado assim:

```arduino
Largura Total = width + padding esquerdo + padding direito + border esquerdo + border direito + margin esquerdo + margin direito

```

- Para alterar esse comportamento, usamos:

```css
box-sizing: border-box;
```

Com isso, `padding` e `border` passam a ser incluídos dentro da largura definida (`width`).

---

## 🔵 Propriedades de Largura e Altura

As propriedades `width` e `height` definem a **largura e altura** dos elementos em CSS.


### 1. `width` (largura)

- Define a largura do elemento.

```css
width: 300px;
```

- Pode ser definida em:
  - **Pixels (px)**: valor fixo.
  - **Porcentagem (%)**: valor relativo ao elemento pai.
  - **Viewport (vw/vh)**: relativo ao tamanho da tela (1vw = 1% da largura da tela).

**Exemplos:**
```css
width: 500px;   /* Largura fixa */
width: 80%;     /* 80% da largura do elemento pai */
width: 50vw;    /* 50% da largura da janela (viewport) */
```

---

### 2. height (altura)
- Define a altura do elemento.

```css
height: 200px;
```

- Funciona com as mesmas unidades que width.

**Exemplos:**
```css
height: 300px;  /* Altura fixa */
height: 100vh;  /* 100% da altura da janela (viewport) */
```
---

### 3. max-width e min-width

- Define o tamanho máximo ou mínimo que um elemento pode ter, independentemente de seu conteúdo ou da tela:

```css
max-width: 100%;
min-width: 300px;
```

---

### 4. max-height e min-height

- Controla a altura máxima ou mínima de um elemento:

```css
max-height: 400px;
min-height: 100px;
```

---

## 🔵 Unidades de Medida
As unidades de medida definem o **tamanho dos elementos** na tela — como larguras, fontes, margens, etc. Entender as unidades ajuda a controlar o layout e a garantir que seu site fique bonito em diferentes dispositivos.

### 🔹 Tipos de Unidades

#### 1. Unidades Absolutas
Têm um valor **fixo**, que **não se adapta** ao tamanho da tela.

| Unidade | Significado             | Exemplo           |
|---------|-------------------------|-------------------|
| `px`      | Pixels                  | `font-size: 16px;` |
| `cm`      | Centímetros             | `width: 5cm;`      |
| `mm`      | Milímetros              | `width: 50mm;`     |
| `in`      | Polegadas               | `width: 2in;`      |
| `pt`      | Pontos (1/72 in)        | `font-size: 12pt;` |
| `pc`      | Picas (12 pt)           | `font-size: 1pc;`  |


A mais usada é o `px`. É boa boa para elementos fixos ou pequenos ajustes.

<br>

#### 2. Unidades Relativas
Se adaptam ao **contexto**, sendo melhores para layouts **responsivos**.

| Unidade | Base de cálculo                          | Exemplo             |
|---------|-------------------------------------------|---------------------|
| `%`       | Percentual do elemento pai                | `width: 50%;`       |
| `em`      | Relativo ao tamanho da fonte do elemento pai | `padding: 2em;`     |
| `rem`     | Relativo à fonte raiz (html)              | `font-size: 1.2rem;`|
| `vw`      | 1% da largura da janela (viewport width)  | `width: 50vw;`      |
| `vh`      | 1% da altura da janela (viewport height)  | `height: 80vh;`     |
| `vmin`    | 1% do menor lado da janela                | `font-size: 2vmin;` |
| `vmax`    | 1% do maior lado da janela                | `font-size: 2vmax;` |


As mais usadas são `%`, `em`, `rem`, `vw`, `vh`. São boas para fontes adaptáveis, containers fluidos e responsividade.

---


## 🔵 Cores em CSS
As cores em CSS são utilizadas para estilizar elementos com propriedades como `color` (texto), `background-color` (fundo), `border-color` (bordas), entre outras. 

### 🔹 Principais Formas de Definir Cores

| Tipo       | Exemplo                       | Descrição                                                                 |
|------------|-------------------------------|---------------------------------------------------------------------------|
| Nome       | `color: red;`                 | Usa nomes pré-definidos pelo CSS (ex: red, blue, green, etc.)            |
| Hexadecimal| `color: #ff0000;`             | Usa 3 ou 6 dígitos hexadecimais (`#RGB` ou `#RRGGBB`)                     |
| RGB        | `color: rgb(255, 0, 0);`      | Define as cores com valores de 0 a 255 para vermelho, verde e azul       |
| RGBA       | `color: rgba(255, 0, 0, 0.5);`| Igual ao RGB, mas com transparência (alpha de 0 a 1)                     |
| HSL        | `color: hsl(0, 100%, 50%);`   | Define a cor por matiz (hue), saturação e luminosidade                   |
| HSLA       | `color: hsla(0, 100%, 50%, 0.5);` | Igual ao HSL, com transparência                                       |


---

## 🔵 Fontes
As fontes são fundamentais para a legibilidade e o estilo visual de um site. Com CSS, você pode configurar tipo, tamanho, espaçamento e outras propriedades tipográficas.

### 🔹 Famílias de Fontes em CSS
A propriedade `font-family` define a tipografia usada no texto. Ela pode receber uma lista de fontes específicas e, por fim, uma família genérica como fallback.

**Exemplo:**
```css
font-family: "Roboto", Arial, sans-serif;
```

Se a primeira fonte não estiver disponível, o navegador usará a próxima da lista.

<br>

#### Principais Famílias Genéricas
| Família      | Características                                      | Quando usar                                                  |
|-------------|------------------------------------------------------|-------------------------------------------------------------|
| serif       | Possui “serifas” (pequenos traços nas extremidades)    | Textos longos em impressão ou sites formais (jornais, livros) |
| sans-serif  | Sem serifas, design limpo e moderno                     | Sites modernos, telas digitais, textos curtos                |
| monospace   | Todas as letras têm a mesma largura                      | Códigos, tabelas, interfaces de programação                  |
| cursive     | Estilo manuscrito                                        | Convites, títulos decorativos                                |
| fantasy     | Fontes criativas, ornamentadas                            | Logotipos, títulos artísticos     |

<br>

### 🔹 Principais Propriedades
| Propriedade        | Exemplo                              | Descrição                                      |
|--------------------|--------------------------------------|-----------------------------------------------|
| font-family        | `font-family: Arial, sans-serif;`     | Define o tipo de fonte                        |
| font-size          | `font-size: 16px;`                   | Define o tamanho da fonte                     |
| font-weight        | `font-weight: bold;`                 | Define a espessura (normal, bold, 100–900)   |
| font-style         | `font-style: italic;`                | Define estilo como itálico ou normal          |
| text-transform     | `text-transform: uppercase;`         | Controla letras maiúsculas/minúsculas          |
| text-decoration    | `text-decoration: underline;`        | Sublinhado, risco ou nenhum                   |
| line-height        | `line-height: 1.5;`                  | Altura da linha                               |
| letter-spacing     | `letter-spacing: 1px;`               | Espaço entre letras                           |
| word-spacing       | `word-spacing: 5px;`                 | Espaço entre palavras                         |
| text-align         | `text-align: center;`                | Alinhamento do texto                          |

---