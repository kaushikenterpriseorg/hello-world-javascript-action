# Deploy word-press to app service on Azure javascript action

This action deploys IaaS resources required to launch a word press website running on App service on Azure

## Inputs

### `client-id`

**Required** Application ID of the App registration with Azure Entra.

### `tenant-id`

**Required** Microsoft Azure Tenant ID.

### `subscription-id`

**Required** Microsoft Azure subscription ID.

### `resource-group-name`

**Required** Name of the resource group your resources will be deployed to.


## Example usage

```yaml
uses: actions/hello-world-javascript-action@e76147da8e5c81eaf017dede5645551d4b94427b
with:
  who-to-greet: 'Mona the Octocat'
```
