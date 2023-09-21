# ARM sablonok Azure

## Alapok és előkészületek

https://github.com/cloudsteak/trn-azure-commandline

## 1. Virtuálisgép létrehozása ARM sablonból

### Erőforráscsoport

- PowerShell

```PowerShell
New-AzResourceGroup -Name app-vms -Location northeurope -Tag @{"Component"="Group"; "OS"="Linux"}
```

- Azure-Cli

```bash
az group create -n app-vms -l northeurope --tags Component=Group OS=Linux
```

### Üzembehelyezés

- PowerShell

```PowerShell
New-AzResourceGroupDeployment -ResourceGroupName app-vms -Name LinuxVM -TemplateFile ./01-linux-vm/template.json
```

- Azure-Cli

```bash
az deployment group create --resource-group app-vms -n LinuxVM --template-file 01-linux-vm/template.json
```
