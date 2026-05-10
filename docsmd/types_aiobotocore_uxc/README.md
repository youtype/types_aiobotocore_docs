# UserExperienceCustomization module

> [Index](../README.md) > UserExperienceCustomization


!!! note ""

    Auto-generated documentation for [UserExperienceCustomization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/uxc.html#userexperiencecustomization)
    type annotations stubs module [types-aiobotocore-uxc](https://pypi.org/project/types-aiobotocore-uxc/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.7.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `UserExperienceCustomization` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `UserExperienceCustomization` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[uxc]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[uxc]'

# standalone installation
python -m pip install types-aiobotocore-uxc
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-uxc
```

## Usage

Code samples can be found in [Examples](./usage.md).

## UserExperienceCustomizationClient

Type annotations and code completion for  `#!python session.create_client("uxc")` as [UserExperienceCustomizationClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/uxc.html#UserExperienceCustomization.Client)

```python
# UserExperienceCustomizationClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_uxc.client import UserExperienceCustomizationClient


session = get_session()
async with session.create_client("uxc") as client:
    client: UserExperienceCustomizationClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("uxc").get_paginator("...")`.

```python
# ListServicesPaginator usage example

from types_aiobotocore_uxc.paginator import ListServicesPaginator

def get_list_services_paginator() -> ListServicesPaginator:
    return client.get_paginator("list_services"))
```

- [ListServicesPaginator](./paginators.md#listservicespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AccountColorType usage example

from types_aiobotocore_uxc.literals import AccountColorType

def get_value() -> AccountColorType:
    return "darkBlue"
```

- [AccountColorType](./literals.md#accountcolortype)
- [ListServicesPaginatorName](./literals.md#listservicespaginatorname)
- [UserExperienceCustomizationServiceName](./literals.md#userexperiencecustomizationservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListServicesInputTypeDef](./type_defs.md#listservicesinputtypedef)
- [UpdateAccountCustomizationsInputTypeDef](./type_defs.md#updateaccountcustomizationsinputtypedef)
- [GetAccountCustomizationsOutputTypeDef](./type_defs.md#getaccountcustomizationsoutputtypedef)
- [ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef)
- [UpdateAccountCustomizationsOutputTypeDef](./type_defs.md#updateaccountcustomizationsoutputtypedef)
- [ListServicesInputPaginateTypeDef](./type_defs.md#listservicesinputpaginatetypedef)

