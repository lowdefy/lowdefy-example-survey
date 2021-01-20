# A Lowdefy Survey Example

This is a simple customer survey example built with Lowdefy. With this example we demonstrate how simple it is to define a public webform and thank you page in Lowdefy config code.

This example queries all employees with the "Sales person" role from a Google sheet on page initialization. This list of sales people names are used to populate a dropdown selector in the webform. The webform contains some conditional logic which demonstrates Lowdefy's ability to express advanced custom logic in a simple readable app config. See the logic in action by writing a complaint about Dwight. Upon completion, the captured data is saved as a new entry to the Google sheet.

All this in less than 370 lines of YAML config. View the source in the [lowdefy.yaml](https://github.com/lowdefy/lowdefy-example-survey/blob/main/lowdefy.yaml) file in this repository.

## Running this example

- Clone this repository.
- Create a Google sheet and share the sheet with a GService API account, see [the getting started tutorial](https://docs.lowdefy.com/getting-started) or [the Google sheets Lowdefy docs](https://docs.lowdefy.com/google-sheets) for an in depth guide on linking a Google sheet.
- Create .env file and set both the `LOWDEFY_SECRET_SHEETS_CLIENT_EMAIL` and `LOWDEFY_SECRET_SHEETS_PRIVATE_KEY` environment variables. (Make sure to never commit your secrets to your code repository.)
- Run the Lowdefy CLI from the cloned repository folder `npx @lowdefy/cli dev`.

## Deploying this example

This simplest solution is to deploy this example to [Netlify](https://netlify.com). See [this tutorial](https://docs.lowdefy.com) for more detail on how to deploy a Lowdefy app to Netlify.
For more Lowdefy deployment solutions, see [the Lowdefy deployment docs](https://docs.lowdefy.com/deployments).

### More Lowdefy resources

- Lowdefy website - https://lowdefy.com
- Lowdefy docs - https://docs.lowdefy.com
- More Lowdefy examples - https://docs.lowdefy.com/examples

## Licence

This example configuration is licensed under the MIT license. See the LICENSE.md file for license rights and limitations.
