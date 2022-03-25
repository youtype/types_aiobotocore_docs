<a id="type-annotations-for-aiobotocore-resourcegroupstaggingapi-module"></a>

# Type annotations for aiobotocore ResourceGroupsTaggingAPI module

> [Index](../README.md) > ResourceGroupsTaggingAPI

Auto-generated documentation for
[ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
type annotations stubs module
[types-aiobotocore-resourcegroupstaggingapi](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi/).

- [Type annotations for aiobotocore ResourceGroupsTaggingAPI module](#type-annotations-for-aiobotocore-resourcegroupstaggingapi-module)
  - [How to install](#how-to-install)
    - [VSCode extension](#vscode-extension)
    - [From PyPI with pip](#from-pypi-with-pip)
  - [How to uninstall](#how-to-uninstall)
  - [Usage](#usage)
  - [ResourceGroupsTaggingAPIClient](#resourcegroupstaggingapiclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Paginators](#paginators)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="how-to-install"></a>

## How to install

<a id="vscode-extension"></a>

### VSCode extension

Add
[AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `ResourceGroupsTaggingAPI`.

<a id="from-pypi-with-pip"></a>

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

<a id="how-to-uninstall"></a>

## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-resourcegroupstaggingapi
```

<a id="usage"></a>

## Usage

Code samples can be found [here](./usage.md).

<a id="resourcegroupstaggingapiclient"></a>

## ResourceGroupsTaggingAPIClient

Type annotations for `session.create_client("resourcegroupstaggingapi")` as
[ResourceGroupsTaggingAPIClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_resourcegroupstaggingapi.client import ResourceGroupsTaggingAPIClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [describe_report_creation](./client.md#describe_report_creation)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_compliance_summary](./client.md#get_compliance_summary)
- [get_paginator](./client.md#get_paginator)
- [get_resources](./client.md#get_resources)
- [get_tag_keys](./client.md#get_tag_keys)
- [get_tag_values](./client.md#get_tag_values)
- [start_report_creation](./client.md#start_report_creation)
- [tag_resources](./client.md#tag_resources)
- [untag_resources](./client.md#untag_resources)

<a id="exceptions"></a>

### Exceptions

ResourceGroupsTaggingAPIClient [exceptions](./client.md#exceptions)

- ClientError
- ConcurrentModificationException
- ConstraintViolationException
- InternalServiceException
- InvalidParameterException
- PaginationTokenExpiredException
- ThrottledException

<a id="paginators"></a>

## Paginators

Type annotations for [paginators](./paginators.md) from
`boto3.client("resourcegroupstaggingapi").get_paginator("...")`.

Can be used directly:

```python
from types_aiobotocore_resourcegroupstaggingapi.paginator import GetComplianceSummaryPaginator, ...
```

- [GetComplianceSummaryPaginator](./paginators.md#getcompliancesummarypaginator)
- [GetResourcesPaginator](./paginators.md#getresourcespaginator)
- [GetTagKeysPaginator](./paginators.md#gettagkeyspaginator)
- [GetTagValuesPaginator](./paginators.md#gettagvaluespaginator)

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_resourcegroupstaggingapi.literals import ErrorCodeType, ...
```

- [ErrorCodeType](./literals.md#errorcodetype)
- [GetComplianceSummaryPaginatorName](./literals.md#getcompliancesummarypaginatorname)
- [GetResourcesPaginatorName](./literals.md#getresourcespaginatorname)
- [GetTagKeysPaginatorName](./literals.md#gettagkeyspaginatorname)
- [GetTagValuesPaginatorName](./literals.md#gettagvaluespaginatorname)
- [GroupByAttributeType](./literals.md#groupbyattributetype)
- [TargetIdTypeType](./literals.md#targetidtypetype)
- [ResourceGroupsTaggingAPIServiceName](./literals.md#resourcegroupstaggingapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from types_aiobotocore_resourcegroupstaggingapi.type_defs import ComplianceDetailsTypeDef, ...
```

- [ComplianceDetailsTypeDef](./type_defs.md#compliancedetailstypedef)
- [DescribeReportCreationOutputTypeDef](./type_defs.md#describereportcreationoutputtypedef)
- [FailureInfoTypeDef](./type_defs.md#failureinfotypedef)
- [GetComplianceSummaryInputRequestTypeDef](./type_defs.md#getcompliancesummaryinputrequesttypedef)
- [GetComplianceSummaryOutputTypeDef](./type_defs.md#getcompliancesummaryoutputtypedef)
- [GetResourcesInputRequestTypeDef](./type_defs.md#getresourcesinputrequesttypedef)
- [GetResourcesOutputTypeDef](./type_defs.md#getresourcesoutputtypedef)
- [GetTagKeysInputRequestTypeDef](./type_defs.md#gettagkeysinputrequesttypedef)
- [GetTagKeysOutputTypeDef](./type_defs.md#gettagkeysoutputtypedef)
- [GetTagValuesInputRequestTypeDef](./type_defs.md#gettagvaluesinputrequesttypedef)
- [GetTagValuesOutputTypeDef](./type_defs.md#gettagvaluesoutputtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ResourceTagMappingTypeDef](./type_defs.md#resourcetagmappingtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartReportCreationInputRequestTypeDef](./type_defs.md#startreportcreationinputrequesttypedef)
- [SummaryTypeDef](./type_defs.md#summarytypedef)
- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [TagResourcesInputRequestTypeDef](./type_defs.md#tagresourcesinputrequesttypedef)
- [TagResourcesOutputTypeDef](./type_defs.md#tagresourcesoutputtypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [UntagResourcesInputRequestTypeDef](./type_defs.md#untagresourcesinputrequesttypedef)
- [UntagResourcesOutputTypeDef](./type_defs.md#untagresourcesoutputtypedef)