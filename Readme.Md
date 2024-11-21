### UC13 - Executar os Processos de Codificação, Manutenção e Documentação de Aplicativos Computacionais para Desktop

## Exercícios - Aula 07

### Objetivo
Este documento detalha os exercícios da Aula 07, com o objetivo de configurar um projeto React para usar Reactstrap e adicionar um componente de navegação.

---

## Exercício 1 - Configurando o Projeto React para Usar Reactstrap

**Prosseguimento**:

1. **Instalação das Dependências**:
   - No terminal, navegue até o diretório do seu projeto React.
   - Instale as dependências necessárias:
     ```bash
     npm install reactstrap react react-dom
     npm install --save bootstrap
     npm install react-popper @popperjs/core
     ```

2. **Configuração do Bootstrap**:
   - Abra o arquivo `index.js` na pasta `src` e adicione a seguinte linha aos imports:
     ```javascript
     import 'bootstrap/dist/css/bootstrap.min.css';
     ```

3. **Adição de uma Barra de Navegação**:
   - Abra o arquivo `App.js` na pasta `src`, delete tudo entre `<header>` e atualize-o conforme abaixo:
     ```javascript
     import React from 'react';
     import { Navbar, NavbarBrand } from 'reactstrap';
     import 'bootstrap/dist/css/bootstrap.min.css';

     function App() {
       return (
         <div className="App">
           <Navbar color="light" light expand="md">
             <NavbarBrand href="/">Ristorante Con Fusion</NavbarBrand>
           </Navbar>
         </div>
       );
     }

     export default App;
     ```

### Passo a Passo 1

1. **Criação da Pasta do Projeto**:
   - Crie uma nova pasta para o seu projeto:
     ```bash
     mkdir nome-do-projeto
     cd nome-do-projeto
     ```

2. **Inicialização do Projeto React**:
   - Inicialize o projeto React:
     ```bash
     npx create-react-app nome-do-projeto
     cd nome-do-projeto
     ```

3. **Instalação das Dependências**:
   - Instale as dependências necessárias:
     ```bash
     npm install reactstrap react react-dom
     npm install --save bootstrap
     npm install react-popper @popperjs/core
     ```

4. **Configuração do Bootstrap**:
   - Abra o arquivo `index.js` na pasta `src` e adicione a seguinte linha aos imports:
     ```javascript
     import 'bootstrap/dist/css/bootstrap.min.css';
     ```

5. **Adição de uma Barra de Navegação**:
   - Abra o arquivo `App.js` na pasta `src`, delete tudo entre `<header>` e atualize-o conforme abaixo:
     ```javascript
     import React from 'react';
     import { Navbar, NavbarBrand } from 'reactstrap';
     import 'bootstrap/dist/css/bootstrap.min.css';

     function App() {
       return (
         <div className="App">
           <Navbar color="light" light expand="md">
             <NavbarBrand href="/">Ristorante Con Fusion</NavbarBrand>
           </Navbar>
         </div>
       );
     }

     export default App;
     ```

1. **Importações**:
   ```javascript
   import React from 'react';
   import { Navbar, NavbarBrand } from 'reactstrap';
   import 'bootstrap/dist/css/bootstrap.min.css';
   ```
   - `import React from 'react';`: Importa a biblioteca React, que é essencial para criar componentes em React.
   - `import { Navbar, NavbarBrand } from 'reactstrap';`: Importa os componentes `Navbar` e `NavbarBrand` da biblioteca `reactstrap`, que é uma coleção de componentes React baseados no Bootstrap.
   - `import 'bootstrap/dist/css/bootstrap.min.css';`: Importa o arquivo CSS do Bootstrap para estilizar os componentes.

2. **Função App**:
   ```javascript
   function App() {
     return (
       <Navbar>
         <NavbarBrand>Ristorante Con Fusion</NavbarBrand>
       </Navbar>
     );
   }
   ```
   - `function App() { ... }`: Define um componente funcional chamado `App`.
   - `return ( ... )`: Retorna o JSX que será renderizado na tela.
   - `<Navbar>`: Componente de barra de navegação fornecido pelo `reactstrap`.
   - `<NavbarBrand>Ristorante Con Fusion</NavbarBrand>`: Componente de marca da barra de navegação que exibe o texto "Ristorante Con Fusion".

3. **Exportação**:
   ```javascript
   export default App;
   ```
   - `export default App;`: Exporta o componente `App` como padrão, permitindo que ele seja importado e usado em outras partes da aplicação.

Em resumo, este código cria uma aplicação React simples que exibe uma barra de navegação com o nome "Ristorante Con Fusion" usando componentes do `reactstrap` e estilos do Bootstrap.

### Conclusão & Anotações

Ao completar esses exercícios, aprendi a configurar um projeto React para usar Reactstrap e adicionar componentes de navegação. Aqui estão algumas anotações e situações encontradas:

- **Erro ao Instalar Dependências**:
  - Certifique-se de que todas as dependências estão corretamente instaladas. Um erro comum é esquecer de adicionar `--save` ao instalar pacotes, o que pode resultar em dependências não sendo salvas no `package.json`.

- **Configuração do Bootstrap**:
  - A importação correta do CSS do Bootstrap é crucial para garantir que os estilos sejam aplicados corretamente aos componentes Reactstrap.

- **Adição de Componentes**:
  - A adição de componentes Reactstrap é simples e direta, mas certifique-se de importar corretamente os componentes necessários no seu arquivo React.

  ![imagem navbar](navbar.png)