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

19. Criar o novo teste para verificar se o texto ainda permanece armazenado, mesmo
    após a limpeza e renderização da DOM

20. Ir no componente e criar as funcionalidades para persistir os dados

21. Como o teste não deve realizar integrações com APIs ou elementos de browser externos,
    a melhor alternativa para validar o teste é criar um mock, logo instalar a lib abaixo
    `yarn add jest-localstorage-mock -D`

22. Configurar no package.json em setupFilesAfterEnv adicionando o mock

23. Com o mock instalado, podemos criar um novo expect() para verificar se determinada
    função foi chamada e aprimorar o nosso teste.

### Mock do useSelector

24. Criar um novo test enxuto e renomear o antigo para não ser lido como teste

25. Fazer o mesmo para o index.js e apagar o useEffect da nova cópia

26. Instalar o redux
    `yarn add redux react-redux`

27. Aplicar o useSelector no index.js

28. Aplicar também o useDispatch no index.js

29. Configurar o test implementando o mock para funcionar o teste do useSelector

### Mock do useDispatch

30. Criar um novo teste `it()` para verificar o uso do useDispatch

31. Para o tste ficar ainda mais parecido com a situação real, emcapsular a action
    seguindo a estrutura de pastas e arquivos.
    src/store/modules/techs/actions.js

32. Importar a action no dentro do componente

33. Importar a action em TechList.test.js também.

34. Alterar o expect para usar a função encapsulada

### Testando reducers

35. Testar reducers, para isso, primeiro criar arquivo
    src/store/modules/techs/reducers.js

36. Instalar o Immer que auxilia na produção de estado imutável
    `yarn add immer`

37. Desenvolver o reducer usando o immer

38. Criar um novo test em
    src/\_\_testes\_\_/store/reducers/tech.test.js

39. Importar as actions e reducers, e conferir se a chamada executa da forma esperada
