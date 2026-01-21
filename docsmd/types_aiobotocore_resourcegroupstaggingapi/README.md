# ResourceGroupsTaggingAPI module

> [Index](../README.md) > ResourceGroupsTaggingAPI


!!! note ""

    Auto-generated documentation for [ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#resourcegroupstaggingapi)
    type annotations stubs module [types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ResourceGroupsTaggingAPI` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ResourceGroupsTaggingAPI` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[resourcegroupstaggingapi]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[resourcegroupstaggingapi]'

# standalone installation
python -m pip install types-aiobotocore-resourcegroupstaggingapi
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-resourcegroupstaggingapi
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ResourceGroupsTaggingAPIClient

Type annotations and code completion for  `#!python session.create_client("resourcegroupstaggingapi")` as [ResourceGroupsTaggingAPIClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Client)

```python
# ResourceGroupsTaggingAPIClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient


session = get_session()
async with session.create_client("resourcegroupstaggingapi") as client:
    client: ResourceGroupsTaggingAPIClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("resourcegroupstaggingapi").get_paginator("...")`.

```python
# GetComplianceSummaryPaginator usage example

from types_aiobotocore_resourcegroupstaggingapi.paginator import GetComplianceSummaryPaginator

def get_get_compliance_summary_paginator() -> GetComplianceSummaryPaginator:
    return client.get_paginator("get_compliance_summary"))
```

- [GetComplianceSummaryPaginator](./paginators.md#getcompliancesummarypaginator)
- [GetResourcesPaginator](./paginators.md#getresourcespaginator)
- [GetTagKeysPaginator](./paginators.md#gettagkeyspaginator)
- [GetTagValuesPaginator](./paginators.md#gettagvaluespaginator)
- [ListRequiredTagsPaginator](./paginators.md#listrequiredtagspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ErrorCodeType usage example

from types_aiobotocore_resourcegroupstaggingapi.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "InternalServiceException"
```

- [ErrorCodeType](./literals.md#errorcodetype)
- [GetComplianceSummaryPaginatorName](./literals.md#getcompliancesummarypaginatorname)
- [GetResourcesPaginatorName](./literals.md#getresourcespaginatorname)
- [GetTagKeysPaginatorName](./literals.md#gettagkeyspaginatorname)
- [GetTagValuesPaginatorName](./literals.md#gettagvaluespaginatorname)
- [GroupByAttributeType](./literals.md#groupbyattributetype)
- [ListRequiredTagsPaginatorName](./literals.md#listrequiredtagspaginatorname)
- [TargetIdTypeType](./literals.md#targetidtypetype)
- [ResourceGroupsTaggingAPIServiceName](./literals.md#resourcegroupstaggingapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ComplianceDetailsTypeDef](./type_defs.md#compliancedetailstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FailureInfoTypeDef](./type_defs.md#failureinfotypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [GetComplianceSummaryInputTypeDef](./type_defs.md#getcompliancesummaryinputtypedef)
- [SummaryTypeDef](./type_defs.md#summarytypedef)
- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [GetTagKeysInputTypeDef](./type_defs.md#gettagkeysinputtypedef)
- [GetTagValuesInputTypeDef](./type_defs.md#gettagvaluesinputtypedef)
- [ListRequiredTagsInputTypeDef](./type_defs.md#listrequiredtagsinputtypedef)
- [RequiredTagTypeDef](./type_defs.md#requiredtagtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [StartReportCreationInputTypeDef](./type_defs.md#startreportcreationinputtypedef)
- [TagResourcesInputTypeDef](./type_defs.md#tagresourcesinputtypedef)
- [UntagResourcesInputTypeDef](./type_defs.md#untagresourcesinputtypedef)
- [DescribeReportCreationOutputTypeDef](./type_defs.md#describereportcreationoutputtypedef)
- [GetTagKeysOutputTypeDef](./type_defs.md#gettagkeysoutputtypedef)
- [GetTagValuesOutputTypeDef](./type_defs.md#gettagvaluesoutputtypedef)
- [TagResourcesOutputTypeDef](./type_defs.md#tagresourcesoutputtypedef)
- [UntagResourcesOutputTypeDef](./type_defs.md#untagresourcesoutputtypedef)
- [GetComplianceSummaryInputPaginateTypeDef](./type_defs.md#getcompliancesummaryinputpaginatetypedef)
- [GetTagKeysInputPaginateTypeDef](./type_defs.md#gettagkeysinputpaginatetypedef)
- [GetTagValuesInputPaginateTypeDef](./type_defs.md#gettagvaluesinputpaginatetypedef)
- [ListRequiredTagsInputPaginateTypeDef](./type_defs.md#listrequiredtagsinputpaginatetypedef)
- [GetComplianceSummaryOutputTypeDef](./type_defs.md#getcompliancesummaryoutputtypedef)
- [GetResourcesInputPaginateTypeDef](./type_defs.md#getresourcesinputpaginatetypedef)
- [GetResourcesInputTypeDef](./type_defs.md#getresourcesinputtypedef)
- [ListRequiredTagsOutputTypeDef](./type_defs.md#listrequiredtagsoutputtypedef)
- [ResourceTagMappingTypeDef](./type_defs.md#resourcetagmappingtypedef)
- [GetResourcesOutputTypeDef](./type_defs.md#getresourcesoutputtypedef)

