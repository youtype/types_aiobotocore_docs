# PrivateCAConnectorforSCEP module

> [Index](../README.md) > PrivateCAConnectorforSCEP


!!! note ""

    Auto-generated documentation for [PrivateCAConnectorforSCEP](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep.html#privatecaconnectorforscep)
    type annotations stubs module [types-aiobotocore-pca-connector-scep](https://pypi.org/project/types-aiobotocore-pca-connector-scep/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `PrivateCAConnectorforSCEP` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `PrivateCAConnectorforSCEP` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[pca-connector-scep]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[pca-connector-scep]'

# standalone installation
python -m pip install types-aiobotocore-pca-connector-scep
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-pca-connector-scep
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PrivateCAConnectorforSCEPClient

Type annotations and code completion for  `#!python session.create_client("pca-connector-scep")` as [PrivateCAConnectorforSCEPClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep.html#PrivateCAConnectorforSCEP.Client)

```python
# PrivateCAConnectorforSCEPClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_pca_connector_scep.client import PrivateCAConnectorforSCEPClient


session = get_session()
async with session.create_client("pca-connector-scep") as client:
    client: PrivateCAConnectorforSCEPClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("pca-connector-scep").get_paginator("...")`.

```python
# ListChallengeMetadataPaginator usage example

from types_aiobotocore_pca_connector_scep.paginator import ListChallengeMetadataPaginator

def get_list_challenge_metadata_paginator() -> ListChallengeMetadataPaginator:
    return client.get_paginator("list_challenge_metadata"))
```

- [ListChallengeMetadataPaginator](./paginators.md#listchallengemetadatapaginator)
- [ListConnectorsPaginator](./paginators.md#listconnectorspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConnectorStatusReasonType usage example

from types_aiobotocore_pca_connector_scep.literals import ConnectorStatusReasonType

def get_value() -> ConnectorStatusReasonType:
    return "INTERNAL_FAILURE"
```

- [ConnectorStatusReasonType](./literals.md#connectorstatusreasontype)
- [ConnectorStatusType](./literals.md#connectorstatustype)
- [ConnectorTypeType](./literals.md#connectortypetype)
- [ListChallengeMetadataPaginatorName](./literals.md#listchallengemetadatapaginatorname)
- [ListConnectorsPaginatorName](./literals.md#listconnectorspaginatorname)
- [PrivateCAConnectorforSCEPServiceName](./literals.md#privatecaconnectorforscepservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ChallengeMetadataSummaryTypeDef](./type_defs.md#challengemetadatasummarytypedef)
- [ChallengeMetadataTypeDef](./type_defs.md#challengemetadatatypedef)
- [ChallengeTypeDef](./type_defs.md#challengetypedef)
- [OpenIdConfigurationTypeDef](./type_defs.md#openidconfigurationtypedef)
- [CreateChallengeRequestRequestTypeDef](./type_defs.md#createchallengerequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteChallengeRequestRequestTypeDef](./type_defs.md#deletechallengerequestrequesttypedef)
- [DeleteConnectorRequestRequestTypeDef](./type_defs.md#deleteconnectorrequestrequesttypedef)
- [GetChallengeMetadataRequestRequestTypeDef](./type_defs.md#getchallengemetadatarequestrequesttypedef)
- [GetChallengePasswordRequestRequestTypeDef](./type_defs.md#getchallengepasswordrequestrequesttypedef)
- [GetConnectorRequestRequestTypeDef](./type_defs.md#getconnectorrequestrequesttypedef)
- [IntuneConfigurationTypeDef](./type_defs.md#intuneconfigurationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChallengeMetadataRequestRequestTypeDef](./type_defs.md#listchallengemetadatarequestrequesttypedef)
- [ListConnectorsRequestRequestTypeDef](./type_defs.md#listconnectorsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateChallengeResponseTypeDef](./type_defs.md#createchallengeresponsetypedef)
- [CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetChallengeMetadataResponseTypeDef](./type_defs.md#getchallengemetadataresponsetypedef)
- [GetChallengePasswordResponseTypeDef](./type_defs.md#getchallengepasswordresponsetypedef)
- [ListChallengeMetadataResponseTypeDef](./type_defs.md#listchallengemetadataresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MobileDeviceManagementTypeDef](./type_defs.md#mobiledevicemanagementtypedef)
- [ListChallengeMetadataRequestListChallengeMetadataPaginateTypeDef](./type_defs.md#listchallengemetadatarequestlistchallengemetadatapaginatetypedef)
- [ListConnectorsRequestListConnectorsPaginateTypeDef](./type_defs.md#listconnectorsrequestlistconnectorspaginatetypedef)
- [ConnectorSummaryTypeDef](./type_defs.md#connectorsummarytypedef)
- [ConnectorTypeDef](./type_defs.md#connectortypedef)
- [CreateConnectorRequestRequestTypeDef](./type_defs.md#createconnectorrequestrequesttypedef)
- [ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef)
- [GetConnectorResponseTypeDef](./type_defs.md#getconnectorresponsetypedef)

