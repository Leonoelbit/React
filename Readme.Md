### Exercício: Primeiros Passos com o React

### Objetivo
Este documento detalha os exercícios iniciais com o React, com o objetivo de instalar e configurar o create-react-app, criar um aplicativo React básico e configurar um repositório Git para o projeto.

---

## Instruções

### Instalação do Yarn ou npm

1. **Instalação do Yarn**:
   - O Yarn é um gerenciador de pacotes eficiente para trabalhar com aplicativos React. Para instalar o Yarn, siga as instruções específicas para sua plataforma no site oficial do Yarn.

2. **Alternativa com npm**:
   - Caso prefira não instalar o Yarn, você pode usar o npm, que também é um gerenciador de pacotes adequado para aplicativos React.

### Instalação do create-react-app

1. **Instalação Global**:
   - A CLI create-react-app facilita a criação de aplicativos React seguindo as melhores práticas da comunidade. Para instalar, use um dos seguintes comandos:
     ```bash
     npm install -g create-react-app
     ```
     ou
     ```bash
     yarn global add create-react-app
     ```

### Criação e Servindo um Projeto React

1. **Criação do Projeto**:
   - Em um local conveniente no seu computador, crie uma pasta chamada `React` e navegue até essa pasta. Em seguida, crie um novo aplicativo React chamado `confusion`:
     ```bash
     npx create-react-app confusion
     ```
     ou
     ```bash
     yarn create react-app confusion
     ```

2. **Servindo o Projeto**:
   - Navegue até a pasta `confusion` e inicie o servidor de desenvolvimento:
     ```bash
     cd confusion
     npm start
     ```
     ou
     ```bash
     yarn start
     ```
   - Isso compilará o projeto e abrirá uma guia no seu navegador padrão no endereço `http://localhost:3000`.

### Inicialização do Repositório Git

1. **Inicialização do Repositório**:
   - Inicialize o projeto como um repositório Git:
     ```bash
     git init
     ```

2. **Adição e Commit dos Arquivos**:
   - Adicione os arquivos ao staging e faça o commit inicial:
     ```bash
     git add .
     git commit -m "Initial Setup"
     ```

3. **Configuração do Repositório Remoto**:
   - Configure um repositório Git on-line (por exemplo, no GitHub) e associe-o ao repositório local:
     ```bash
     git remote add origin https://github.com/usuario/nome-do-repositorio.git
     git push -u origin master
     ```

---

### Conclusão

Neste exercício, você instalou a ferramenta CLI create-react-app, criou um projeto React básico e apresentou o projeto compilado no navegador. Além disso, você inicializou o projeto como um repositório Git e configurou um repositório remoto para sincronização.