# PrivateCAConnectorforSCEP module

> [Index](../README.md) > PrivateCAConnectorforSCEP


!!! note ""

    Auto-generated documentation for [PrivateCAConnectorforSCEP](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep.html#privatecaconnectorforscep)
    type annotations stubs module [types-aiobotocore-pca-connector-scep](https://pypi.org/project/types-aiobotocore-pca-connector-scep/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
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
- [CreateChallengeRequestTypeDef](./type_defs.md#createchallengerequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteChallengeRequestTypeDef](./type_defs.md#deletechallengerequesttypedef)
- [DeleteConnectorRequestTypeDef](./type_defs.md#deleteconnectorrequesttypedef)
- [GetChallengeMetadataRequestTypeDef](./type_defs.md#getchallengemetadatarequesttypedef)
- [GetChallengePasswordRequestTypeDef](./type_defs.md#getchallengepasswordrequesttypedef)
- [GetConnectorRequestTypeDef](./type_defs.md#getconnectorrequesttypedef)
- [IntuneConfigurationTypeDef](./type_defs.md#intuneconfigurationtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListChallengeMetadataRequestTypeDef](./type_defs.md#listchallengemetadatarequesttypedef)
- [ListConnectorsRequestTypeDef](./type_defs.md#listconnectorsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [CreateChallengeResponseTypeDef](./type_defs.md#createchallengeresponsetypedef)
- [CreateConnectorResponseTypeDef](./type_defs.md#createconnectorresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetChallengeMetadataResponseTypeDef](./type_defs.md#getchallengemetadataresponsetypedef)
- [GetChallengePasswordResponseTypeDef](./type_defs.md#getchallengepasswordresponsetypedef)
- [ListChallengeMetadataResponseTypeDef](./type_defs.md#listchallengemetadataresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [MobileDeviceManagementTypeDef](./type_defs.md#mobiledevicemanagementtypedef)
- [ListChallengeMetadataRequestPaginateTypeDef](./type_defs.md#listchallengemetadatarequestpaginatetypedef)
- [ListConnectorsRequestPaginateTypeDef](./type_defs.md#listconnectorsrequestpaginatetypedef)
- [ConnectorSummaryTypeDef](./type_defs.md#connectorsummarytypedef)
- [ConnectorTypeDef](./type_defs.md#connectortypedef)
- [CreateConnectorRequestTypeDef](./type_defs.md#createconnectorrequesttypedef)
- [ListConnectorsResponseTypeDef](./type_defs.md#listconnectorsresponsetypedef)
- [GetConnectorResponseTypeDef](./type_defs.md#getconnectorresponsetypedef)

