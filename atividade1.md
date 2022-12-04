# ***Por que devemos fazer testes automatizados nas aplicações que desenvolvemos?***
Pois com os testes automatizados o sistema é otimizado com precisão e agilidade, nessa hora que encontrará bugs, falhas de segurança e qualquer outro problema que prejudique o uso da aplicação, ou seja, é o momento em que a equipe avalia se o programa funciona como o esperado.

# ***O que são testes unitários?***
Se refere a um teste de uma parte do código de uma aplicação, uma
funcionalidade, ou um simples campo que poderá ser testado separadamente do restante do código.

# ***O que são testes automatizados?***
É a aplicação de ferramentas de software para automatizar um processo manual, conduzido por humanos, de revisão e validação de um produto de software.

# ***Escolha uma pirâmide de testes e descreva com suas palavras cada secção da pirâmide.***
### **Teste de pirâmide voltada a uma aplicação front-end.**

## ***Base:***
## **Teste Unitário**
Teste mais popular que usa uma parte do código de uma aplicação, funcionalidade, ou um simple campo que é testado separadamente do restante do código. É um teste rápido e fácil de se escrever, menos custoso. Para o desenvolvimento front-end, que trabalhamos com componentes, o teste unitário vai permitir garantir que os componentes funcionem como esperado de forma isolada, porem é preciso saber se o mesmo vai funcionar quando utilizado de forma conjunta.

Exemplos de ferramentas: **Jest, Jasmine e Chai.**

## ***Meio:***
## **Teste de Integração**
Costatamos que as unidades do código estão funcionando corretamente de forma isolada, mas para garantir que quando uma parte se comunicar com a outra as coisas vão funcionar como esperado, se utilizará o teste de integração. Por exemplo, um formulário contendo vários inputs diferentes e com um botão de enviar os dados. Iremos testar se ao preencher todos os dados corretamente e clicar no botão de enviar veremos a mensagem de sucesso esperada.

Exemplos de ferramentas: **Jest e Cypress.**

## ***Topo:***
## **Teste UI**
### **Teste E2E**
Teste End-to-end, com ele trabalhamos todos os componentes de forma integrada, só que pensando na forma como o usuário vai utilizar passo a passo, ou seja, a jornada do usuário, será utilizado ferramentas automatizadas que vai simular ações com um contexto real feita pelo usuário. tipo, navegando em uma página e realizando ações como clicar em botões, preencher campos, entre outras, ate verificar se o resultado está como esperado. Requer muito investimento, esforço e ele demora para roda, porém tras muita confiança, com isso tudo torna-se um teste muito custoso.

Exemplos de ferramentas: **Cypress, TestCafe e Puppeteer.**

### **Teste de Snapshot**
É um teste voltado mais para a interface, com ele temos a certeza de que quandom for realizado qualquer alteração, ele não mudará inesperadamente. Basicamente o teste vai renderizar um componente, depois vai tirar uma especie de "print" do que foi renderizado e vai guardar essa imagem. Cada vez que o teste for rodado ele vai renderizar outra imagem e vai comparar com a imagem que estava guardada, se tiver alguma diferença o teste vai falhar e vamos saber que a interface foi alterada sem a necessidade de rodar toda a aplicação.

Exemplo de ferramenta: **Jest.**

### **Teste Acessibilidade**
Uma das principais etapas, pois é imprescindível a acessibilidade de um software. Removendo qualquer empecilho que posso complicar a usuário de utilizar nosso aplicação.

Exemplos de ferramentas: **Jest Axe e Pa11y.**