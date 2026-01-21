# Artifact module

> [Index](../README.md) > Artifact


!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Artifact` service.
1. Use provided commands to install generated packages.



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
# ListCustomerAgreementsPaginator usage example

from types_aiobotocore_artifact.paginator import ListCustomerAgreementsPaginator

def get_list_customer_agreements_paginator() -> ListCustomerAgreementsPaginator:
    return client.get_paginator("list_customer_agreements"))
```

- [ListCustomerAgreementsPaginator](./paginators.md#listcustomeragreementspaginator)
- [ListReportVersionsPaginator](./paginators.md#listreportversionspaginator)
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
- [AgreementTypeType](./literals.md#agreementtypetype)
- [CustomerAgreementStateType](./literals.md#customeragreementstatetype)
- [ListCustomerAgreementsPaginatorName](./literals.md#listcustomeragreementspaginatorname)
- [ListReportVersionsPaginatorName](./literals.md#listreportversionspaginatorname)
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
- [CustomerAgreementSummaryTypeDef](./type_defs.md#customeragreementsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetReportMetadataRequestTypeDef](./type_defs.md#getreportmetadatarequesttypedef)
- [ReportDetailTypeDef](./type_defs.md#reportdetailtypedef)
- [GetReportRequestTypeDef](./type_defs.md#getreportrequesttypedef)
- [GetTermForReportRequestTypeDef](./type_defs.md#gettermforreportrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCustomerAgreementsRequestTypeDef](./type_defs.md#listcustomeragreementsrequesttypedef)
- [ListReportVersionsRequestTypeDef](./type_defs.md#listreportversionsrequesttypedef)
- [ReportSummaryTypeDef](./type_defs.md#reportsummarytypedef)
- [ListReportsRequestTypeDef](./type_defs.md#listreportsrequesttypedef)
- [PutAccountSettingsRequestTypeDef](./type_defs.md#putaccountsettingsrequesttypedef)
- [GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef)
- [GetReportResponseTypeDef](./type_defs.md#getreportresponsetypedef)
- [GetTermForReportResponseTypeDef](./type_defs.md#gettermforreportresponsetypedef)
- [ListCustomerAgreementsResponseTypeDef](./type_defs.md#listcustomeragreementsresponsetypedef)
- [PutAccountSettingsResponseTypeDef](./type_defs.md#putaccountsettingsresponsetypedef)
- [GetReportMetadataResponseTypeDef](./type_defs.md#getreportmetadataresponsetypedef)
- [ListCustomerAgreementsRequestPaginateTypeDef](./type_defs.md#listcustomeragreementsrequestpaginatetypedef)
- [ListReportVersionsRequestPaginateTypeDef](./type_defs.md#listreportversionsrequestpaginatetypedef)
- [ListReportsRequestPaginateTypeDef](./type_defs.md#listreportsrequestpaginatetypedef)
- [ListReportVersionsResponseTypeDef](./type_defs.md#listreportversionsresponsetypedef)
- [ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef)

