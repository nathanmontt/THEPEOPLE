# THEPEOPLE

Pessoas conectando pessoas.

### ÍNDICE

* [Sobre o Projeto](#about)
* [Linguagens](#langs)
* [IDE](#ide)
* [Setup](#setup)
* [Créditos](#credits)

<h1 id="about">Sobre o Projeto</h1>

*THEPEOPLE* foi criado com o intuito de estudo. Inicialmente, o "estudar a _framework_ **vue.js**" foi (e está sendo) feito. Agora, colocando a prova desses estudos, surge o projeto. Ele trás em si uma simples _landing page_ que conta a história de uma empresa que quer conectar pessoas através do mundo.


<h1 id="langs">Linguagens</h1>

A aplicação veio com o inutuito de treinar o uso da _framework_ **vue.js**, consequentemente se tornando a principal ferramenta do projeto. Outras primárias, como **HTML e JavaScript** não podem deixar de ser citadas. 

O projeto também contou com uma nova adição ao meu portifólio pessoal de aprendizado: **TailwindCSS**.


<h1 id="ide">Setup de IDE Recomendado</h1>

[VSCode](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (e disabilitar Vetur). Para configurações, visite o [Vite Configuration Reference](https://vite.dev/config/).


<h1 id="setup">Setup do Projeto</h1>

#### Instalação

```sh
npm install
npm run dev
```

#### Instalação de Dependências
```sh
npm install tailwindcss @tailwindcss/vite
```

#### Configurando o Vite Plugin
```sh
import { defineConfig } from 'vite'
import tailwindcss from '@tailwindcss/vite'
export default defineConfig({
  plugins: [
    tailwindcss(),
  ],
})
```

#### Importando TailwindCSS
Colocar em um arquivo ```.css``` para utilizar
```sh
@import "tailwindcss";
```

#### Compilação e _"Minify"_  Production

```sh
npm run build
```


<h1 id="credits"> Créditos </h1>

Copyright © 2025, Nathan Monteiro
