# Mobile module

> [Index](../README.md) > Mobile


!!! note ""

    Auto-generated documentation for [Mobile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
    type annotations stubs module [types-aiobotocore-mobile](https://pypi.org/project/types-aiobotocore-mobile/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Mobile` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mobile]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mobile]'


# standalone installation
python -m pip install types-aiobotocore-mobile
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mobile
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MobileClient

Type annotations and code completion for  `#!python session.create_client("mobile")` as [MobileClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_mobile.client import MobileClient


session = get_session()
async with session.create_client("mobile") as client:
    client: MobileClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mobile").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_mobile.paginator import ListBundlesPaginator

def get_list_bundles_paginator() -> ListBundlesPaginator:
    return client.get_paginator("list_bundles"))
```

- [ListBundlesPaginator](./paginators.md#listbundlespaginator)
- [ListProjectsPaginator](./paginators.md#listprojectspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mobile.literals import ListBundlesPaginatorName

def get_value() -> ListBundlesPaginatorName:
    return "list_bundles"
```

- [ListBundlesPaginatorName](./literals.md#listbundlespaginatorname)
- [ListProjectsPaginatorName](./literals.md#listprojectspaginatorname)
- [PlatformType](./literals.md#platformtype)
- [ProjectStateType](./literals.md#projectstatetype)
- [MobileServiceName](./literals.md#mobileservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_mobile.type_defs import BundleDetailsTypeDef

def get_value() -> BundleDetailsTypeDef:
    return {
        "bundleId": ...,
    }
```

- [BundleDetailsTypeDef](./type_defs.md#bundledetailstypedef)
- [CreateProjectRequestRequestTypeDef](./type_defs.md#createprojectrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteProjectRequestRequestTypeDef](./type_defs.md#deleteprojectrequestrequesttypedef)
- [ResourceTypeDef](./type_defs.md#resourcetypedef)
- [DescribeBundleRequestRequestTypeDef](./type_defs.md#describebundlerequestrequesttypedef)
- [DescribeProjectRequestRequestTypeDef](./type_defs.md#describeprojectrequestrequesttypedef)
- [ExportBundleRequestRequestTypeDef](./type_defs.md#exportbundlerequestrequesttypedef)
- [ExportProjectRequestRequestTypeDef](./type_defs.md#exportprojectrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListBundlesRequestRequestTypeDef](./type_defs.md#listbundlesrequestrequesttypedef)
- [ListProjectsRequestRequestTypeDef](./type_defs.md#listprojectsrequestrequesttypedef)
- [ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef)
- [UpdateProjectRequestRequestTypeDef](./type_defs.md#updateprojectrequestrequesttypedef)
- [DescribeBundleResultTypeDef](./type_defs.md#describebundleresulttypedef)
- [ExportBundleResultTypeDef](./type_defs.md#exportbundleresulttypedef)
- [ExportProjectResultTypeDef](./type_defs.md#exportprojectresulttypedef)
- [ListBundlesResultTypeDef](./type_defs.md#listbundlesresulttypedef)
- [DeleteProjectResultTypeDef](./type_defs.md#deleteprojectresulttypedef)
- [ProjectDetailsTypeDef](./type_defs.md#projectdetailstypedef)
- [ListBundlesRequestListBundlesPaginateTypeDef](./type_defs.md#listbundlesrequestlistbundlespaginatetypedef)
- [ListProjectsRequestListProjectsPaginateTypeDef](./type_defs.md#listprojectsrequestlistprojectspaginatetypedef)
- [ListProjectsResultTypeDef](./type_defs.md#listprojectsresulttypedef)
- [CreateProjectResultTypeDef](./type_defs.md#createprojectresulttypedef)
- [DescribeProjectResultTypeDef](./type_defs.md#describeprojectresulttypedef)
- [UpdateProjectResultTypeDef](./type_defs.md#updateprojectresulttypedef)

