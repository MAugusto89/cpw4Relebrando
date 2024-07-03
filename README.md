ANOTAÇÕES DO PROJETO
------------------------------------------------------------------------------------------------------------------------------------------
--Criar novo projeto
yarn create react-app revisao --template typescript
------------------------------------------------------------------------------------------------------------------------------------------
yarn add -D - o D é de desenvolvimento, serve para evitar que alguns pacotes entram para produção, assim sobrecarregando a aplicação
------------------------------------------------------------------------------------------------------------------------------------------
"cy:open": "cypress open"
yarn cy:open
------------------------------------------------------------------------------------------------------------------------------------------
e2e -> End To End
------------------------------------------------------------------------------------------------------------------------------------------
---Evitar possíveis erros durante o teste

PASSO1
Criar arquivo -> cypress.d.ts
import { mount } from "cypress/react";

declare global{
    namespace Cypress{
        interface Chainable{
            mount: typeof mount;
        }
    }
}
PASSO2
![image](https://github.com/MAugusto89/cpw4Relebrando/assets/69408213/06f9c3b1-17fd-46f4-9c72-2375f010710a)

------------------------------------------------------------------------------------------------------------------------------------------
Criar as seguintes pastas
![image](https://github.com/MAugusto89/cpw4Relebrando/assets/69408213/7186c405-8243-4899-9d5c-2720e6bd6b1b)
Criar os arquivos dentro da pasta SentenceInput
![image](https://github.com/MAugusto89/cpw4Relebrando/assets/69408213/122d796f-d896-428d-9e4b-8b6574223869)
---index.tsx
![image](https://github.com/MAugusto89/cpw4Relebrando/assets/69408213/06a3e6a8-6d84-48df-9be0-8d190b98528a)
---index.cy.tsx
![image](https://github.com/MAugusto89/cpw4Relebrando/assets/69408213/926cae64-40cc-4c4a-9b1a-e57fd918a225)
