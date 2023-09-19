# tan-azure-arm
ARM sablonok Azure

## Alapok és előkészületek

https://github.com/cloudsteak/trn-azure-commandline



## Erőforráscsoportok létrehozása

### 1. Erőforrás típusonként

```bash
az group create -n app-vms -l north-europe
az group create -n app-network -l north-europe
az group create -n app-storage -l north-europe
```

