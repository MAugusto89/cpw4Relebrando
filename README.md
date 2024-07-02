<!--Evitar possíveis erros durante o teste-->
cypress.d.ts
import { mount } from "cypress/react";

declare global{
    namespace Cypress{
        interface Chainable{
            mount: typeof mount;
        }
    }
}
