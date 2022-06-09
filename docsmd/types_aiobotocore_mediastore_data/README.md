# MediaStoreData module

> [Index](../README.md) > MediaStoreData


!!! note ""

    Auto-generated documentation for [MediaStoreData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
    type annotations stubs module [types-aiobotocore-mediastore-data](https://pypi.org/project/types-aiobotocore-mediastore-data/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `MediaStoreData`.

### From PyPI with pip

Install `types-aiobotocore` for `MediaStoreData` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mediastore-data]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mediastore-data]'


# standalone installation
python -m pip install types-aiobotocore-mediastore-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mediastore-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MediaStoreDataClient

Type annotations and code completion for  `#!python session.create_client("mediastore-data")` as [MediaStoreDataClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mediastore_data.client import MediaStoreDataClient


session = get_session()
async with session.create_client("mediastore-data") as client:
    client: MediaStoreDataClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mediastore-data").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_mediastore_data.paginator import ListItemsPaginator

def get_list_items_paginator() -> ListItemsPaginator:
    return client.get_paginator("list_items"))
```

- [ListItemsPaginator](./paginators.md#listitemspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mediastore_data.literals import ItemTypeType

def get_value() -> ItemTypeType:
    return "FOLDER"
```

- [ItemTypeType](./literals.md#itemtypetype)
- [ListItemsPaginatorName](./literals.md#listitemspaginatorname)
- [StorageClassType](./literals.md#storageclasstype)
- [UploadAvailabilityType](./literals.md#uploadavailabilitytype)
- [MediaStoreDataServiceName](./literals.md#mediastoredataservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mediastore_data.type_defs import DeleteObjectRequestRequestTypeDef

def get_value() -> DeleteObjectRequestRequestTypeDef:
    return {
        "Path": ...,
    }
```

- [DeleteObjectRequestRequestTypeDef](./type_defs.md#deleteobjectrequestrequesttypedef)
- [DescribeObjectRequestRequestTypeDef](./type_defs.md#describeobjectrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetObjectRequestRequestTypeDef](./type_defs.md#getobjectrequestrequesttypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListItemsRequestRequestTypeDef](./type_defs.md#listitemsrequestrequesttypedef)
- [PutObjectRequestRequestTypeDef](./type_defs.md#putobjectrequestrequesttypedef)
- [DescribeObjectResponseTypeDef](./type_defs.md#describeobjectresponsetypedef)
- [GetObjectResponseTypeDef](./type_defs.md#getobjectresponsetypedef)
- [PutObjectResponseTypeDef](./type_defs.md#putobjectresponsetypedef)
- [ListItemsResponseTypeDef](./type_defs.md#listitemsresponsetypedef)
- [ListItemsRequestListItemsPaginateTypeDef](./type_defs.md#listitemsrequestlistitemspaginatetypedef)

