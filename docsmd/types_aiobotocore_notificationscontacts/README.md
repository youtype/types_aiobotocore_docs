# UserNotificationsContacts module

> [Index](../README.md) > UserNotificationsContacts


!!! note ""

    Auto-generated documentation for [UserNotificationsContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#usernotificationscontacts)
    type annotations stubs module [types-aiobotocore-notificationscontacts](https://pypi.org/project/types-aiobotocore-notificationscontacts/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `UserNotificationsContacts` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `UserNotificationsContacts` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[notificationscontacts]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[notificationscontacts]'

# standalone installation
python -m pip install types-aiobotocore-notificationscontacts
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-notificationscontacts
```

## Usage

Code samples can be found in [Examples](./usage.md).

## UserNotificationsContactsClient

Type annotations and code completion for  `#!python session.create_client("notificationscontacts")` as [UserNotificationsContactsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#UserNotificationsContacts.Client)

```python
# UserNotificationsContactsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_notificationscontacts.client import UserNotificationsContactsClient


session = get_session()
async with session.create_client("notificationscontacts") as client:
    client: UserNotificationsContactsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("notificationscontacts").get_paginator("...")`.

```python
# ListEmailContactsPaginator usage example

from types_aiobotocore_notificationscontacts.paginator import ListEmailContactsPaginator

def get_list_email_contacts_paginator() -> ListEmailContactsPaginator:
    return client.get_paginator("list_email_contacts"))
```

- [ListEmailContactsPaginator](./paginators.md#listemailcontactspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EmailContactStatusType usage example

from types_aiobotocore_notificationscontacts.literals import EmailContactStatusType

def get_value() -> EmailContactStatusType:
    return "active"
```

- [EmailContactStatusType](./literals.md#emailcontactstatustype)
- [ListEmailContactsPaginatorName](./literals.md#listemailcontactspaginatorname)
- [UserNotificationsContactsServiceName](./literals.md#usernotificationscontactsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActivateEmailContactRequestRequestTypeDef](./type_defs.md#activateemailcontactrequestrequesttypedef)
- [CreateEmailContactRequestRequestTypeDef](./type_defs.md#createemailcontactrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteEmailContactRequestRequestTypeDef](./type_defs.md#deleteemailcontactrequestrequesttypedef)
- [EmailContactTypeDef](./type_defs.md#emailcontacttypedef)
- [GetEmailContactRequestRequestTypeDef](./type_defs.md#getemailcontactrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEmailContactsRequestRequestTypeDef](./type_defs.md#listemailcontactsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [SendActivationCodeRequestRequestTypeDef](./type_defs.md#sendactivationcoderequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [CreateEmailContactResponseTypeDef](./type_defs.md#createemailcontactresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [GetEmailContactResponseTypeDef](./type_defs.md#getemailcontactresponsetypedef)
- [ListEmailContactsResponseTypeDef](./type_defs.md#listemailcontactsresponsetypedef)
- [ListEmailContactsRequestPaginateTypeDef](./type_defs.md#listemailcontactsrequestpaginatetypedef)

