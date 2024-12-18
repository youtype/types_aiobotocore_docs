# SupplyChain module

> [Index](../README.md) > SupplyChain


!!! note ""

    Auto-generated documentation for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain)
    type annotations stubs module [types-aiobotocore-supplychain](https://pypi.org/project/types-aiobotocore-supplychain/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SupplyChain` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SupplyChain` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[supplychain]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[supplychain]'

# standalone installation
python -m pip install types-aiobotocore-supplychain
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-supplychain
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SupplyChainClient

Type annotations and code completion for  `#!python session.create_client("supplychain")` as [SupplyChainClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#SupplyChain.Client)

```python
# SupplyChainClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_supplychain.client import SupplyChainClient


session = get_session()
async with session.create_client("supplychain") as client:
    client: SupplyChainClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("supplychain").get_paginator("...")`.

```python
# ListDataIntegrationFlowsPaginator usage example

from types_aiobotocore_supplychain.paginator import ListDataIntegrationFlowsPaginator

def get_list_data_integration_flows_paginator() -> ListDataIntegrationFlowsPaginator:
    return client.get_paginator("list_data_integration_flows"))
```

- [ListDataIntegrationFlowsPaginator](./paginators.md#listdataintegrationflowspaginator)
- [ListDataLakeDatasetsPaginator](./paginators.md#listdatalakedatasetspaginator)
- [ListInstancesPaginator](./paginators.md#listinstancespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConfigurationJobStatusType usage example

from types_aiobotocore_supplychain.literals import ConfigurationJobStatusType

def get_value() -> ConfigurationJobStatusType:
    return "FAILED"
```

- [ConfigurationJobStatusType](./literals.md#configurationjobstatustype)
- [DataIntegrationEventTypeType](./literals.md#dataintegrationeventtypetype)
- [DataIntegrationFlowFileTypeType](./literals.md#dataintegrationflowfiletypetype)
- [DataIntegrationFlowLoadTypeType](./literals.md#dataintegrationflowloadtypetype)
- [DataIntegrationFlowSourceTypeType](./literals.md#dataintegrationflowsourcetypetype)
- [DataIntegrationFlowTargetTypeType](./literals.md#dataintegrationflowtargettypetype)
- [DataIntegrationFlowTransformationTypeType](./literals.md#dataintegrationflowtransformationtypetype)
- [DataLakeDatasetSchemaFieldTypeType](./literals.md#datalakedatasetschemafieldtypetype)
- [InstanceStateType](./literals.md#instancestatetype)
- [ListDataIntegrationFlowsPaginatorName](./literals.md#listdataintegrationflowspaginatorname)
- [ListDataLakeDatasetsPaginatorName](./literals.md#listdatalakedatasetspaginatorname)
- [ListInstancesPaginatorName](./literals.md#listinstancespaginatorname)
- [SupplyChainServiceName](./literals.md#supplychainservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BillOfMaterialsImportJobTypeDef](./type_defs.md#billofmaterialsimportjobtypedef)
- [CreateBillOfMaterialsImportJobRequestRequestTypeDef](./type_defs.md#createbillofmaterialsimportjobrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateInstanceRequestRequestTypeDef](./type_defs.md#createinstancerequestrequesttypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [DataIntegrationFlowDatasetOptionsTypeDef](./type_defs.md#dataintegrationflowdatasetoptionstypedef)
- [DataIntegrationFlowS3OptionsTypeDef](./type_defs.md#dataintegrationflows3optionstypedef)
- [DataIntegrationFlowSQLTransformationConfigurationTypeDef](./type_defs.md#dataintegrationflowsqltransformationconfigurationtypedef)
- [DataLakeDatasetSchemaFieldTypeDef](./type_defs.md#datalakedatasetschemafieldtypedef)
- [DeleteDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#deletedataintegrationflowrequestrequesttypedef)
- [DeleteDataLakeDatasetRequestRequestTypeDef](./type_defs.md#deletedatalakedatasetrequestrequesttypedef)
- [DeleteInstanceRequestRequestTypeDef](./type_defs.md#deleteinstancerequestrequesttypedef)
- [GetBillOfMaterialsImportJobRequestRequestTypeDef](./type_defs.md#getbillofmaterialsimportjobrequestrequesttypedef)
- [GetDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#getdataintegrationflowrequestrequesttypedef)
- [GetDataLakeDatasetRequestRequestTypeDef](./type_defs.md#getdatalakedatasetrequestrequesttypedef)
- [GetInstanceRequestRequestTypeDef](./type_defs.md#getinstancerequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDataIntegrationFlowsRequestRequestTypeDef](./type_defs.md#listdataintegrationflowsrequestrequesttypedef)
- [ListDataLakeDatasetsRequestRequestTypeDef](./type_defs.md#listdatalakedatasetsrequestrequesttypedef)
- [ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDataLakeDatasetRequestRequestTypeDef](./type_defs.md#updatedatalakedatasetrequestrequesttypedef)
- [UpdateInstanceRequestRequestTypeDef](./type_defs.md#updateinstancerequestrequesttypedef)
- [CreateBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#createbillofmaterialsimportjobresponsetypedef)
- [CreateDataIntegrationFlowResponseTypeDef](./type_defs.md#createdataintegrationflowresponsetypedef)
- [DeleteDataIntegrationFlowResponseTypeDef](./type_defs.md#deletedataintegrationflowresponsetypedef)
- [DeleteDataLakeDatasetResponseTypeDef](./type_defs.md#deletedatalakedatasetresponsetypedef)
- [GetBillOfMaterialsImportJobResponseTypeDef](./type_defs.md#getbillofmaterialsimportjobresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [SendDataIntegrationEventResponseTypeDef](./type_defs.md#senddataintegrationeventresponsetypedef)
- [CreateInstanceResponseTypeDef](./type_defs.md#createinstanceresponsetypedef)
- [DeleteInstanceResponseTypeDef](./type_defs.md#deleteinstanceresponsetypedef)
- [GetInstanceResponseTypeDef](./type_defs.md#getinstanceresponsetypedef)
- [ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)
- [UpdateInstanceResponseTypeDef](./type_defs.md#updateinstanceresponsetypedef)
- [DataIntegrationFlowDatasetSourceConfigurationTypeDef](./type_defs.md#dataintegrationflowdatasetsourceconfigurationtypedef)
- [DataIntegrationFlowDatasetTargetConfigurationTypeDef](./type_defs.md#dataintegrationflowdatasettargetconfigurationtypedef)
- [DataIntegrationFlowS3SourceConfigurationTypeDef](./type_defs.md#dataintegrationflows3sourceconfigurationtypedef)
- [DataIntegrationFlowS3TargetConfigurationTypeDef](./type_defs.md#dataintegrationflows3targetconfigurationtypedef)
- [DataIntegrationFlowTransformationTypeDef](./type_defs.md#dataintegrationflowtransformationtypedef)
- [DataLakeDatasetSchemaOutputTypeDef](./type_defs.md#datalakedatasetschemaoutputtypedef)
- [DataLakeDatasetSchemaTypeDef](./type_defs.md#datalakedatasetschematypedef)
- [ListDataIntegrationFlowsRequestListDataIntegrationFlowsPaginateTypeDef](./type_defs.md#listdataintegrationflowsrequestlistdataintegrationflowspaginatetypedef)
- [ListDataLakeDatasetsRequestListDataLakeDatasetsPaginateTypeDef](./type_defs.md#listdatalakedatasetsrequestlistdatalakedatasetspaginatetypedef)
- [ListInstancesRequestListInstancesPaginateTypeDef](./type_defs.md#listinstancesrequestlistinstancespaginatetypedef)
- [SendDataIntegrationEventRequestRequestTypeDef](./type_defs.md#senddataintegrationeventrequestrequesttypedef)
- [DataIntegrationFlowSourceTypeDef](./type_defs.md#dataintegrationflowsourcetypedef)
- [DataIntegrationFlowTargetTypeDef](./type_defs.md#dataintegrationflowtargettypedef)
- [DataLakeDatasetTypeDef](./type_defs.md#datalakedatasettypedef)
- [CreateDataLakeDatasetRequestRequestTypeDef](./type_defs.md#createdatalakedatasetrequestrequesttypedef)
- [CreateDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#createdataintegrationflowrequestrequesttypedef)
- [DataIntegrationFlowTypeDef](./type_defs.md#dataintegrationflowtypedef)
- [UpdateDataIntegrationFlowRequestRequestTypeDef](./type_defs.md#updatedataintegrationflowrequestrequesttypedef)
- [CreateDataLakeDatasetResponseTypeDef](./type_defs.md#createdatalakedatasetresponsetypedef)
- [GetDataLakeDatasetResponseTypeDef](./type_defs.md#getdatalakedatasetresponsetypedef)
- [ListDataLakeDatasetsResponseTypeDef](./type_defs.md#listdatalakedatasetsresponsetypedef)
- [UpdateDataLakeDatasetResponseTypeDef](./type_defs.md#updatedatalakedatasetresponsetypedef)
- [GetDataIntegrationFlowResponseTypeDef](./type_defs.md#getdataintegrationflowresponsetypedef)
- [ListDataIntegrationFlowsResponseTypeDef](./type_defs.md#listdataintegrationflowsresponsetypedef)
- [UpdateDataIntegrationFlowResponseTypeDef](./type_defs.md#updatedataintegrationflowresponsetypedef)

