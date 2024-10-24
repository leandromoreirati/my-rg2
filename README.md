<!-- BEGIN_AUTOMATED_TF_DOCS_BLOCK -->
# {{module-name}}

This example do deployment `Azure Resource Group`.

## Dependencies

N/A

## Notes

N/A

## Usage

### Create Plan
```bash
bash build.sh plan
```

### Show Plan

```bash
bash build.sh testplan
```
### Apply

```bash
bash build.sh apply
```

### Destroy

```bash
bash build.sh destroy-plan
```

```bash
bash build.sh destroy-apply
```



## Requirements

| Name | Version |
|------|---------|
| <a name="requirement_terraform"></a> [terraform](#requirement\_terraform) | >= 1.0.0 |
| <a name="requirement_azurerm"></a> [azurerm](#requirement\_azurerm) | >= 3.62.0 |



## Inputs

| Name | Description | Type | Default | Required |
|------|-------------|------|---------|:--------:|
| <a name="input_location"></a> [location](#input\_location) | The location where the resource group should be created. | `string` | `null` | no |
| <a name="input_name"></a> [name](#input\_name) | Name of the resource group. Must be unique on your Azure subscription. | `string` | `null` | no |
| <a name="input_tags"></a> [tags](#input\_tags) | A mapping of tags to assign to the resource. | `map(string)` | `{}` | no |

## Outputs

| Name | Description |
|------|-------------|
| <a name="output_id"></a> [id](#output\_id) | The name of the resource group. Must be unique on your Azure subscription. |
| <a name="output_name"></a> [name](#output\_name) | The name of the resource group. Must be unique on your Azure subscription. |

# External Documentation
* [Azure Resource Group](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/manage-resource-groups-portal#what-is-a-resource-group)
<!-- END_AUTOMATED_TF_DOCS_BLOCK -->