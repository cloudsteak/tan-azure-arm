# tan-azure-arm
ARM sablonok Azure

## Alapok és előkészületek

https://github.com/cloudsteak/trn-azure-commandline



## Erőforráscsoportok létrehozása

### 1. Erőforrás típusonként

```bash
az group create -n app-vms -l northeurope --tags domain=app os=linux type=vm;
az group create -n app-network -l northeurope --tags domain=app os=linux type=network;
az group create -n app-storage -l northeurope --tags domain=app os=linux type=storage;
```

