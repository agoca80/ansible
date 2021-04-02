https://learn.hashicorp.com/tutorials/vault/ha-with-consul
https://learn.hashicorp.com/tutorials/vault/getting-started-deploy#initializing-the-vault

```
export VAULT_ADDR=http://vault11:8200
export VAULT_TOKEN="..."

# Initialization
vault operator init -key-shares=1 -key-threshold=1

# Login
vault login
vault kv get  -field=credentials kv/aws
vault kv put kv/aws credentials=@$HOME/.aws/credentials
```
