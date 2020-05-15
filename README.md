# Demo of End-to-End testing using [Cypress.io](https://www.cypress.io/)

## Setup of KeyCloak

Using a `non-prod` KeyCloak Realm, follow instructions as per https://developers.redhat.com/blog/2020/01/29/api-login-and-jwt-token-generation-using-keycloak/ to set up a specific KeyCloak Client using:

- `Direct Grant` Flow and
- `Client Id and Secret` Credentials

Alternatively, you may import the sample [KeyCloak Client](./sample.kc-client.json) and customize for your application.

Note the Client ID and Client Secret (under the `Credentials` tab), as you'll need both for the next step,

## Application Setup

Customize the credentials for your application.

- copy [sample.cypress.env.json](./sample.cypress.env.json) to `cypress.env.json`
- set the variable values, including `auth_client_id` and `auth_client_secret` from the previous step

## Local Install

- clone this repo
- `npm install`
- `npm run test:e2e`

## Docker Test
