<a id="paginators-for-aiobotocore-lexmodelbuildingservice-module"></a>

# Paginators for aiobotocore LexModelBuildingService module

> [Index](..) > [LexModelBuildingService](.) > Paginators

Auto-generated documentation for
[LexModelBuildingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
type annotations stubs module
[types-aiobotocore-lex-models](https://pypi.org/project/types-aiobotocore-lex-models/).

- [Paginators for aiobotocore LexModelBuildingService module](#paginators-for-aiobotocore-lexmodelbuildingservice-module)
  - [GetBotAliasesPaginator](#getbotaliasespaginator)
  - [GetBotChannelAssociationsPaginator](#getbotchannelassociationspaginator)
  - [GetBotVersionsPaginator](#getbotversionspaginator)
  - [GetBotsPaginator](#getbotspaginator)
  - [GetBuiltinIntentsPaginator](#getbuiltinintentspaginator)
  - [GetBuiltinSlotTypesPaginator](#getbuiltinslottypespaginator)
  - [GetIntentVersionsPaginator](#getintentversionspaginator)
  - [GetIntentsPaginator](#getintentspaginator)
  - [GetSlotTypeVersionsPaginator](#getslottypeversionspaginator)
  - [GetSlotTypesPaginator](#getslottypespaginator)

<a id="getbotaliasespaginator"></a>

## GetBotAliasesPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_bot_aliases")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetBotAliasesPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetBotAliasesPaginator = client.get_paginator("get_bot_aliases")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetBotAliases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases)

Arguments for `GetBotAliasesPaginator.paginate` method:

- `botName`: `str` *(required)*
- `nameContains`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBotAliasesPaginator.paginate` returns
`_PageIterator`\[[GetBotAliasesResponseTypeDef](./type_defs.md#getbotaliasesresponsetypedef)\].

<a id="getbotchannelassociationspaginator"></a>

## GetBotChannelAssociationsPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_bot_channel_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetBotChannelAssociationsPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetBotChannelAssociationsPaginator = client.get_paginator("get_bot_channel_associations")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetBotChannelAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations)

Arguments for `GetBotChannelAssociationsPaginator.paginate` method:

- `botName`: `str` *(required)*
- `botAlias`: `str` *(required)*
- `nameContains`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBotChannelAssociationsPaginator.paginate` returns
`_PageIterator`\[[GetBotChannelAssociationsResponseTypeDef](./type_defs.md#getbotchannelassociationsresponsetypedef)\].

<a id="getbotversionspaginator"></a>

## GetBotVersionsPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_bot_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetBotVersionsPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetBotVersionsPaginator = client.get_paginator("get_bot_versions")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetBotVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)

Arguments for `GetBotVersionsPaginator.paginate` method:

- `name`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBotVersionsPaginator.paginate` returns
`_PageIterator`\[[GetBotVersionsResponseTypeDef](./type_defs.md#getbotversionsresponsetypedef)\].

<a id="getbotspaginator"></a>

## GetBotsPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_bots")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetBotsPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetBotsPaginator = client.get_paginator("get_bots")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetBots](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)

Arguments for `GetBotsPaginator.paginate` method:

- `nameContains`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBotsPaginator.paginate` returns
`_PageIterator`\[[GetBotsResponseTypeDef](./type_defs.md#getbotsresponsetypedef)\].

<a id="getbuiltinintentspaginator"></a>

## GetBuiltinIntentsPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_builtin_intents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetBuiltinIntentsPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetBuiltinIntentsPaginator = client.get_paginator("get_builtin_intents")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetBuiltinIntents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents)

Arguments for `GetBuiltinIntentsPaginator.paginate` method:

- `locale`: [LocaleType](./literals.md#localetype)
- `signatureContains`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBuiltinIntentsPaginator.paginate` returns
`_PageIterator`\[[GetBuiltinIntentsResponseTypeDef](./type_defs.md#getbuiltinintentsresponsetypedef)\].

<a id="getbuiltinslottypespaginator"></a>

## GetBuiltinSlotTypesPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_builtin_slot_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetBuiltinSlotTypesPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetBuiltinSlotTypesPaginator = client.get_paginator("get_builtin_slot_types")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetBuiltinSlotTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes)

Arguments for `GetBuiltinSlotTypesPaginator.paginate` method:

- `locale`: [LocaleType](./literals.md#localetype)
- `signatureContains`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetBuiltinSlotTypesPaginator.paginate` returns
`_PageIterator`\[[GetBuiltinSlotTypesResponseTypeDef](./type_defs.md#getbuiltinslottypesresponsetypedef)\].

<a id="getintentversionspaginator"></a>

## GetIntentVersionsPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_intent_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetIntentVersionsPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetIntentVersionsPaginator = client.get_paginator("get_intent_versions")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetIntentVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)

Arguments for `GetIntentVersionsPaginator.paginate` method:

- `name`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetIntentVersionsPaginator.paginate` returns
`_PageIterator`\[[GetIntentVersionsResponseTypeDef](./type_defs.md#getintentversionsresponsetypedef)\].

<a id="getintentspaginator"></a>

## GetIntentsPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_intents")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetIntentsPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetIntentsPaginator = client.get_paginator("get_intents")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetIntents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)

Arguments for `GetIntentsPaginator.paginate` method:

- `nameContains`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetIntentsPaginator.paginate` returns
`_PageIterator`\[[GetIntentsResponseTypeDef](./type_defs.md#getintentsresponsetypedef)\].

<a id="getslottypeversionspaginator"></a>

## GetSlotTypeVersionsPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_slot_type_versions")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetSlotTypeVersionsPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetSlotTypeVersionsPaginator = client.get_paginator("get_slot_type_versions")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetSlotTypeVersions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)

Arguments for `GetSlotTypeVersionsPaginator.paginate` method:

- `name`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSlotTypeVersionsPaginator.paginate` returns
`_PageIterator`\[[GetSlotTypeVersionsResponseTypeDef](./type_defs.md#getslottypeversionsresponsetypedef)\].

<a id="getslottypespaginator"></a>

## GetSlotTypesPaginator

Type annotations for
`session.create_client("lex-models").get_paginator("get_slot_types")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_lex_models.paginator import GetSlotTypesPaginator

session = get_session()
async with session.create_client("lex-models") as client:
    client: LexModelBuildingServiceClient
    paginator: GetSlotTypesPaginator = client.get_paginator("get_slot_types")
```

Boto3 documentation:
[LexModelBuildingService.Paginator.GetSlotTypes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)

Arguments for `GetSlotTypesPaginator.paginate` method:

- `nameContains`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetSlotTypesPaginator.paginate` returns
`_PageIterator`\[[GetSlotTypesResponseTypeDef](./type_defs.md#getslottypesresponsetypedef)\].
