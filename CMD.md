## Commands

```bash
az appservice plan create --name wk-azure-api --resource-group wk-azure --sku FREE
az webapp create --name wk-azure-api --resource-group wk-azure --plan wk-azure-api
az webapp deployment source config-local-git -n wk-azure-api -g wk-azure --query [url] -o tsv
```