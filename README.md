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
- name: Deploy word press to azure app service
        uses: ./ # Uses an action in the root directory
        id: deploy
        with:
          client-id: ${{ secrets.AZURE_CLIENT_ID }}
          tenant-id: ${{ secrets.AZURE_TENANT_ID }}
          subscription-id: ${{ secrets.AZURE_SUBSCRIPTION_ID }}
          resource-group-name: ${{ secrets.AZURE_RG }}
```
