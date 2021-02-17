# A Lowdefy Survey Example

This is a simple customer survey example built with Lowdefy. With this example we demonstrate how simple it is to define a public webform and thank you page in Lowdefy.

This example queries all employees with the "Sales person" role from a [Google sheet](https://docs.google.com/spreadsheets/d/1wldNzkdP7-qSBz8pdtYrx8dlTw01vqQ9gn6KfXPg5DU/edit?usp=sharing#gid=841255153) on page initialization. This list of sales people names are used to populate a dropdown selector in the webform. The webform contains some conditional logic which demonstrates Lowdefy's ability to express advanced custom logic in simple readable app config. See the logic in action by writing a complaint about Dwight. Upon completion, the captured data is saved as a new entry to the Google sheet.

All this in less than 400 lines of YAML config. View the source in the [lowdefy.yaml](https://github.com/lowdefy/lowdefy-example-survey/blob/main/lowdefy.yaml) file in this repository.

## Running this example

- Clone this repository or copy the content of the `lowdefy.yaml` into a `lowdefy.yaml` file in your local folder.
- Create a Google sheet and share the sheet with a GService API account, see [the getting started tutorial](https://docs.lowdefy.com/tutorial-setup) or [the Google sheets Lowdefy docs](https://docs.lowdefy.com/GoogleSheet) for an in depth guide on linking a Google sheet.
- Create `.env` file and set both the `LOWDEFY_SECRET_SHEETS_CLIENT_EMAIL` and `LOWDEFY_SECRET_SHEETS_PRIVATE_KEY` environment variables. (Make sure to never commit your secrets to your code repository.)
- Run the Lowdefy CLI from the cloned repository folder `npx lowdefy@latest dev`.

## Deploying this example

This simplest solution is to deploy this example to [Netlify](https://netlify.com). See [the Netlify Deployment instructions](https://docs.lowdefy.com/deployment) for more detail on how to deploy a Lowdefy app to Netlify.

### More Lowdefy resources

- Getting started with Lowdefy - https://docs.lowdefy.com/tutorial-setup
- Lowdefy docs - https://docs.lowdefy.com
- Lowdefy website - https://lowdefy.com

## Licence: MIT

See the LICENSE.md file for license rights and limitations.
