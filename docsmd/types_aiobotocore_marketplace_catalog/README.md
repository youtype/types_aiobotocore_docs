# MarketplaceCatalog module

> [Index](../README.md) > MarketplaceCatalog


!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `MarketplaceCatalog`.

### From PyPI with pip

Install `types-aiobotocore` for `MarketplaceCatalog` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[marketplace-catalog]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[marketplace-catalog]'


# standalone installation
python -m pip install types-aiobotocore-marketplace-catalog
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-marketplace-catalog
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MarketplaceCatalogClient

Type annotations and code completion for  `#!python session.create_client("marketplace-catalog")` as [MarketplaceCatalogClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient


session = get_session()
async with session.create_client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_marketplace_catalog.literals import ChangeStatusType

def get_value() -> ChangeStatusType:
    return "APPLYING"
```

- [ChangeStatusType](./literals.md#changestatustype)
- [FailureCodeType](./literals.md#failurecodetype)
- [SortOrderType](./literals.md#sortordertype)
- [MarketplaceCatalogServiceName](./literals.md#marketplacecatalogservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef

def get_value() -> CancelChangeSetRequestRequestTypeDef:
    return {
        "Catalog": ...,
        "ChangeSetId": ...,
    }
```

- [CancelChangeSetRequestRequestTypeDef](./type_defs.md#cancelchangesetrequestrequesttypedef)
- [CancelChangeSetResponseTypeDef](./type_defs.md#cancelchangesetresponsetypedef)
- [ChangeSetSummaryListItemTypeDef](./type_defs.md#changesetsummarylistitemtypedef)
- [ChangeSummaryTypeDef](./type_defs.md#changesummarytypedef)
- [ChangeTypeDef](./type_defs.md#changetypedef)
- [DescribeChangeSetRequestRequestTypeDef](./type_defs.md#describechangesetrequestrequesttypedef)
- [DescribeChangeSetResponseTypeDef](./type_defs.md#describechangesetresponsetypedef)
- [DescribeEntityRequestRequestTypeDef](./type_defs.md#describeentityrequestrequesttypedef)
- [DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef)
- [EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef)
- [EntityTypeDef](./type_defs.md#entitytypedef)
- [ErrorDetailTypeDef](./type_defs.md#errordetailtypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [ListChangeSetsRequestRequestTypeDef](./type_defs.md#listchangesetsrequestrequesttypedef)
- [ListChangeSetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef)
- [ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef)
- [ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SortTypeDef](./type_defs.md#sorttypedef)
- [StartChangeSetRequestRequestTypeDef](./type_defs.md#startchangesetrequestrequesttypedef)
- [StartChangeSetResponseTypeDef](./type_defs.md#startchangesetresponsetypedef)
