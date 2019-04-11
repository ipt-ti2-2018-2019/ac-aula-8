# Aula 8 - Ciclo de vida de um componente React + CSS

Objetivos:

- Usar os métodos de "lifecycle" de um componente React para AJAX e afins
- CSS Flexbox
- CSS Grid

O exercício de hoje vai-se basear sobre este repositório: https://github.com/ipt-ti2-2018-2019/todo-app

Vamos usar o CodeSandbox: https://codesandbox.io

---

# CSS Flexbox

Os slides estão no Moodle: https://doctrino.ipt.pt/mod/resource/view.php?id=13231

Recomendo os seguintes recursos:

- https://flexboxfroggy.com/
- http://www.flexboxdefense.com/
- https://css-tricks.com/snippets/css/a-guide-to-flexbox/

# CSS Grid

Recomendo os seguintes recursos:

- https://learncssgrid.com/
- https://cssgridgarden.com/
- https://css-tricks.com/snippets/css/complete-guide-grid/

# React Lifecycle

Um componente React tem várias fases. É possível nós fazermos uso de métodos especiais numa classe React para tratar de coisas como:

- Quando é que o componente "entra na página" (componentDidMount)
- Quando é que o componente "sai da página" (componentWillUnmount)
- Quando é que o componente "atualiza" (componentDidUpdate)

Recomendo os seguintes recursos:

- https://pt-br.reactjs.org/docs/state-and-lifecycle.html#adding-lifecycle-methods-to-a-class
- (Ver gráfico no topo da página) https://medium.com/@_ChrisBradshaw/blogdidmount-2018-guide-to-react-component-lifecycle-methods-1614e0bbe80a

## Métodos principais

Os 3 métodos seguintes são os mais importantes:

### `componentDidMount`

Uso isto muito para ligar timers, fazer chamadas AJAX, ou aceder a recursos como a câmara, ou até o HTML gerado pelo componente.

Exemplo (com AJAX): https://pt-br.reactjs.org/docs/faq-ajax.html

### `componentWillUnmount`

Uso isto quando preciso de limpar recursos (ex: limpar timers com o `clearInterval` ou `clearTimeout`).

### `componentDidUpdate`

Uso isto mais raramente, mas é útil quando preciso de saber quando `props` mudam (ex: mudar o ID de um recurso, para eu fazer um pedido AJAX e ir buscar os dados novos...)
