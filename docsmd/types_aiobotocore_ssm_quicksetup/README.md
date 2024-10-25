# SystemsManagerQuickSetup module

> [Index](../README.md) > SystemsManagerQuickSetup


!!! note ""

    Auto-generated documentation for [SystemsManagerQuickSetup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup)
    type annotations stubs module [types-aiobotocore-ssm-quicksetup](https://pypi.org/project/types-aiobotocore-ssm-quicksetup/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `SystemsManagerQuickSetup` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ssm-quicksetup]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ssm-quicksetup]'


# standalone installation
python -m pip install types-aiobotocore-ssm-quicksetup
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ssm-quicksetup
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SystemsManagerQuickSetupClient

Type annotations and code completion for  `#!python session.create_client("ssm-quicksetup")` as [SystemsManagerQuickSetupClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#SystemsManagerQuickSetup.Client)

```python
# SystemsManagerQuickSetupClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_quicksetup.client import SystemsManagerQuickSetupClient


session = get_session()
async with session.create_client("ssm-quicksetup") as client:
    client: SystemsManagerQuickSetupClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("ssm-quicksetup").get_paginator("...")`.

```python
# ListConfigurationManagersPaginator usage example

from types_aiobotocore_ssm_quicksetup.paginator import ListConfigurationManagersPaginator

def get_list_configuration_managers_paginator() -> ListConfigurationManagersPaginator:
    return client.get_paginator("list_configuration_managers"))
```

- [ListConfigurationManagersPaginator](./paginators.md#listconfigurationmanagerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListConfigurationManagersPaginatorName usage example

from types_aiobotocore_ssm_quicksetup.literals import ListConfigurationManagersPaginatorName

def get_value() -> ListConfigurationManagersPaginatorName:
    return "list_configuration_managers"
```

- [ListConfigurationManagersPaginatorName](./literals.md#listconfigurationmanagerspaginatorname)
- [StatusType](./literals.md#statustype)
- [StatusTypeType](./literals.md#statustypetype)
- [SystemsManagerQuickSetupServiceName](./literals.md#systemsmanagerquicksetupservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ConfigurationDefinitionInputTypeDef](./type_defs.md#configurationdefinitioninputtypedef)
- [ConfigurationDefinitionSummaryTypeDef](./type_defs.md#configurationdefinitionsummarytypedef)
- [ConfigurationDefinitionTypeDef](./type_defs.md#configurationdefinitiontypedef)
- [StatusSummaryTypeDef](./type_defs.md#statussummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteConfigurationManagerInputRequestTypeDef](./type_defs.md#deleteconfigurationmanagerinputrequesttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetConfigurationManagerInputRequestTypeDef](./type_defs.md#getconfigurationmanagerinputrequesttypedef)
- [ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [QuickSetupTypeOutputTypeDef](./type_defs.md#quicksetuptypeoutputtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagEntryTypeDef](./type_defs.md#tagentrytypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateConfigurationDefinitionInputRequestTypeDef](./type_defs.md#updateconfigurationdefinitioninputrequesttypedef)
- [UpdateConfigurationManagerInputRequestTypeDef](./type_defs.md#updateconfigurationmanagerinputrequesttypedef)
- [UpdateServiceSettingsInputRequestTypeDef](./type_defs.md#updateservicesettingsinputrequesttypedef)
- [CreateConfigurationManagerInputRequestTypeDef](./type_defs.md#createconfigurationmanagerinputrequesttypedef)
- [ConfigurationManagerSummaryTypeDef](./type_defs.md#configurationmanagersummarytypedef)
- [CreateConfigurationManagerOutputTypeDef](./type_defs.md#createconfigurationmanageroutputtypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetConfigurationManagerOutputTypeDef](./type_defs.md#getconfigurationmanageroutputtypedef)
- [ListConfigurationManagersInputRequestTypeDef](./type_defs.md#listconfigurationmanagersinputrequesttypedef)
- [GetServiceSettingsOutputTypeDef](./type_defs.md#getservicesettingsoutputtypedef)
- [ListConfigurationManagersInputListConfigurationManagersPaginateTypeDef](./type_defs.md#listconfigurationmanagersinputlistconfigurationmanagerspaginatetypedef)
- [ListQuickSetupTypesOutputTypeDef](./type_defs.md#listquicksetuptypesoutputtypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListConfigurationManagersOutputTypeDef](./type_defs.md#listconfigurationmanagersoutputtypedef)

