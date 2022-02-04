<a id="type-annotations-for-aiobotocore-personalizeevents-module"></a>

# Type annotations for aiobotocore PersonalizeEvents module

> [Index](..) > PersonalizeEvents

Auto-generated documentation for
[PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#PersonalizeEvents)
type annotations stubs module
[types-aiobotocore-personalize-events](https://pypi.org/project/types-aiobotocore-personalize-events/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[personalize-events]'

# install as a standalone
pip install types-aiobotocore-personalize-events
```

- [Type annotations for aiobotocore PersonalizeEvents module](#type-annotations-for-aiobotocore-personalizeevents-module)
  - [PersonalizeEventsClient](#personalizeeventsclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="personalizeeventsclient"></a>

## PersonalizeEventsClient

Type annotations for `aiobotocore.create_client("personalize-events")` as
[PersonalizeEventsClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_personalize_events.client import PersonalizeEventsClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [put_events](./client.md#put_events)
- [put_items](./client.md#put_items)
- [put_users](./client.md#put_users)

<a id="exceptions"></a>

### Exceptions

PersonalizeEventsClient [exceptions](./client.md#exceptions)

- ClientError
- InvalidInputException
- ResourceInUseException
- ResourceNotFoundException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_personalize_events.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_personalize_events.type_defs import EventTypeDef, ...
```

- [EventTypeDef](./type_defs.md#eventtypedef)
- [ItemTypeDef](./type_defs.md#itemtypedef)
- [PutEventsRequestRequestTypeDef](./type_defs.md#puteventsrequestrequesttypedef)
- [PutItemsRequestRequestTypeDef](./type_defs.md#putitemsrequestrequesttypedef)
- [PutUsersRequestRequestTypeDef](./type_defs.md#putusersrequestrequesttypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
