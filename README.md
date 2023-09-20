# tan-azure-arm
ARM sablonok Azure

## Alapok és előkészületek

https://github.com/cloudsteak/trn-azure-commandline



## 1. Virtuálisgép létrehozása ARM sablonból

### Erőforráscsoport

```bash
az group create -n app-vms -l northeurope --tags Component=VM OS=Linux;
```

### Üzembehelyezés

```bash
az deployment group create --resource-group app-vms --template-file 01-linux-vm/template.json
```
