# Módulo 12 - Testes no ReactJS e React Native

## Installation Steps

### Configurando ambiente

1. Instalar o React app a partir da CLI de create
   `yarn create react-app modulo12`

2. Instalar o Rewired para adicionar novas configurações ao React App, como no
   babel, webpack e no jest
   `yarn add react-app-rewired -D`

3. Trocar os scripts em package.json para o react-app-rewired

4. Limpar os arquivos desnecessários para deixar o mais limpo possível

5. Criar o config-overrides.js necessário ao funcionamento do Rewired

6. Criar uma chave `jest` no package.json e adicionar as configs do jest

7. Criar um mapeamento em package.json para funcionar as importações com o `~`
   `moduleNameMapper`

8. Criar o jsconfig.json para adicionar instruções ao VSCode

9. Instalar outras libs auxialiares para tests
   `yarn add @testing-library/react @testing-library/jest-dom -D`

10. Instalar os types do jest para ter funcionando o autocomplete do VSCode
    `yarn add @types/jest -D`

11. Adicionar no package.json as configs necessárias ao funcionamento das novas libs

### Primeiro teste

12. Criar o componente TechList com o boilerplate de função React só para validar no TDD

13. Excluir o teste antigo e criar um novo arquivo de teste para o componente TechList

14. Criar o novo teste para verificar se há o elemento procurado dentro da lista do componente

15. Ajustar o componente TechList para mostrar a lista ao clicar no botão. E executar teste.

### Testando formulário

16. Alterar o Teste para, não apenas clicar num botão, mas inserir um texto no input
    do componente e dar submit, bem como receber a resposta e validar

17. Adicionar as novas funcionalidades ao Componente TechList

18. Adicionar outro expect() para verificar que o imput esteja vazio

### Mock do LocalStorage

19.
