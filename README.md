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
Criar arquivo -> cypress.d.ts
import { mount } from "cypress/react";

declare global{
    namespace Cypress{
        interface Chainable{
            mount: typeof mount;
        }
    }
}
------------------------------------------------------------------------------------------------------------------------------------------
