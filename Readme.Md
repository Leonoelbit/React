### UC13 - Executar os Processos de Codificação, Manutenção e Documentação de Aplicativos Computacionais para Desktop

## Exercícios - Aula 09

### Objetivo
Este documento detalha os exercícios da Aula 09, onde aprendemos a adicionar um novo componente ao aplicativo React, incorporarando dados a esse componente e atualizando o aplicativo para exibir sobre informações sobre um restaurante na página da web.

---

## Exercício 1 - Adicionando Componentes ao Aplicativo React

```javascript
import React, { useState } from 'react'; // Importa React e o hook useState do React
import { Media } from 'reactstrap'; // Importa o componente Media do Reactstrap

// Define o componente funcional Menu
const Menu = () => {
  // Define o estado inicial com uma lista de pratos usando o hook useState
  const [dishes] = useState([
    {
      id: 0,
      name: 'Uthappizza',
      image: 'assets/images/uthappizza.png',
      category: 'mains',
      label: 'Hot',
      price: '4.99',
      description: 'A unique combination of Indian Uthappam (pancake) and Italian pizza, topped with Cerignola olives, ripe vine cherry tomatoes, Vidalia onion, Guntur chillies and Buffalo Paneer.'
    },
    {
      id: 1,
      name: 'Zucchipakoda',
      image: 'assets/images/zucchipakoda.png',
      category: 'appetizer',
      label: '',
      price: '1.99',
      description: 'Deep fried Zucchini coated with mildly spiced Chickpea flour batter accompanied with a sweet-tangy tamarind sauce'
    },
    {
      id: 2,
      name: 'Vadonut',
      image: 'assets/images/vadonut.png',
      category: 'appetizer',
      label: 'New',
      price: '1.99',
      description: 'A quintessential ConFusion experience, is it a vada or is it a donut?'
    },
    {
      id: 3,
      name: 'ElaiCheese Cake',
      image: 'assets/images/elaicheesecake.png',
      category: 'dessert',
      label: '',
      price: '2.99',
      description: 'A delectable, semi-sweet New York Style Cheese Cake, with Graham cracker crust and spiced with Indian cardamoms'
    }
  ]);

  // Mapeia a lista de pratos para criar elementos JSX para cada prato
  const menu = dishes.map((dish) => {
    return (
      <div key={dish.id} className="col-12 mt-5">
        <Media tag="li">
          <Media left middle>
            <Media object src={dish.image} alt={dish.name} /> {/* Exibe a imagem do prato */}
          </Media>
          <Media body className="ml-5">
            <Media heading>{dish.name}</Media> {/* Exibe o nome do prato */}
            <p>{dish.description}</p> {/* Exibe a descrição do prato */}
          </Media>
        </Media>
      </div>
    );
  });

  // Retorna o JSX que representa o menu
  return (
    <div className="container">
      <div className="row">
        <Media list>
          {menu} {/* Renderiza a lista de pratos */}
        </Media>
      </div>
    </div>
  );
};

export default Menu; // Exporta o componente Menu como padrão
```

### Explicação do Código

1. **Importações:**
   - `React` e `useState` são importados do pacote `react`. `useState` é um hook que permite adicionar o estado ao componente funcional.
   - `Media` é importado do `reactstrap`, uma biblioteca de componentes React baseada no Bootstrap.

2. **Definição do Componente `Menu`:**
   - O componente `Menu` é definido como uma função que utiliza o hook `useState` para armazenar uma lista de pratos (`dishes`).
   - A lista de pratos (`dishes`) é inicializada com um array de objetos, onde cada objeto representa um prato com propriedades como `id`, `name`, `image`, `category`, `label`, `price` e `description`.

3. **Mapeamento dos Pratos:**
   - A função `map` é usada para iterar sobre a lista de pratos e retornar um elemento JSX para cada prato.
   - Cada prato é renderizado dentro de um `div` com classes Bootstrap para layout (`col-12 mt-5`).
   - O componente `Media` do `reactstrap` é usado para estruturar a exibição de cada prato, incluindo a imagem (`Media object`), o nome (`Media heading`) e a descrição (`p`).

4. **Renderização do Menu:**
   - O JSX retornado pelo componente `Menu` inclui um contêiner (`div` com classe `container`) e uma linha (`div` com classe `row`).
   - Dentro da linha, a lista de pratos (`menu`) é renderizada usando o componente `Media list`.

5. **Exportação do Componente:**
   - O componente `Menu` é exportado como padrão para que possa ser importado e usado em outros arquivos, como `App.js`.
   
###  Conclusão
   - Ao completar os exercícios da Aula 09, adquirimos habilidades essenciais para trabalhar com componentes em React. Aprendemos a adicionar um novo componente ao aplicativo, incorporar dados a esse componente e atualizar a interface do usuário. Este processo envolveu o uso de hooks como useState para gerenciar o estado e a biblioteca reactstrap para estilizar os componentes.