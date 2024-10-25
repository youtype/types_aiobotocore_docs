# Artifact module

> [Index](../README.md) > Artifact


!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Artifact` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[artifact]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[artifact]'


# standalone installation
python -m pip install types-aiobotocore-artifact
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-artifact
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ArtifactClient

Type annotations and code completion for  `#!python session.create_client("artifact")` as [ArtifactClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client)

```python
# ArtifactClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_artifact.client import ArtifactClient


session = get_session()
async with session.create_client("artifact") as client:
    client: ArtifactClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("artifact").get_paginator("...")`.

```python
# ListReportsPaginator usage example

from types_aiobotocore_artifact.paginator import ListReportsPaginator

def get_list_reports_paginator() -> ListReportsPaginator:
    return client.get_paginator("list_reports"))
```

- [ListReportsPaginator](./paginators.md#listreportspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AcceptanceTypeType usage example

from types_aiobotocore_artifact.literals import AcceptanceTypeType

def get_value() -> AcceptanceTypeType:
    return "EXPLICIT"
```

- [AcceptanceTypeType](./literals.md#acceptancetypetype)
- [ListReportsPaginatorName](./literals.md#listreportspaginatorname)
- [NotificationSubscriptionStatusType](./literals.md#notificationsubscriptionstatustype)
- [PublishedStateType](./literals.md#publishedstatetype)
- [UploadStateType](./literals.md#uploadstatetype)
- [ArtifactServiceName](./literals.md#artifactservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetReportMetadataRequestRequestTypeDef](./type_defs.md#getreportmetadatarequestrequesttypedef)
- [ReportDetailTypeDef](./type_defs.md#reportdetailtypedef)
- [GetReportRequestRequestTypeDef](./type_defs.md#getreportrequestrequesttypedef)
- [GetTermForReportRequestRequestTypeDef](./type_defs.md#gettermforreportrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListReportsRequestRequestTypeDef](./type_defs.md#listreportsrequestrequesttypedef)
- [ReportSummaryTypeDef](./type_defs.md#reportsummarytypedef)
- [PutAccountSettingsRequestRequestTypeDef](./type_defs.md#putaccountsettingsrequestrequesttypedef)
- [GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef)
- [GetReportResponseTypeDef](./type_defs.md#getreportresponsetypedef)
- [GetTermForReportResponseTypeDef](./type_defs.md#gettermforreportresponsetypedef)
- [PutAccountSettingsResponseTypeDef](./type_defs.md#putaccountsettingsresponsetypedef)
- [GetReportMetadataResponseTypeDef](./type_defs.md#getreportmetadataresponsetypedef)
- [ListReportsRequestListReportsPaginateTypeDef](./type_defs.md#listreportsrequestlistreportspaginatetypedef)
- [ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef)

