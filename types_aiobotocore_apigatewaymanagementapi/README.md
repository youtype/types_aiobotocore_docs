<a id="type-annotations-for-aiobotocore-apigatewaymanagementapi-module"></a>

# Type annotations for aiobotocore ApiGatewayManagementApi module

> [Index](..) > ApiGatewayManagementApi

Auto-generated documentation for
[ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
type annotations stubs module
[types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[apigatewaymanagementapi]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[apigatewaymanagementapi]'

# standalone installation
pip install types-aiobotocore-apigatewaymanagementapi
```

- [Type annotations for aiobotocore ApiGatewayManagementApi module](#type-annotations-for-aiobotocore-apigatewaymanagementapi-module)
  - [ApiGatewayManagementApiClient](#apigatewaymanagementapiclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="apigatewaymanagementapiclient"></a>

## ApiGatewayManagementApiClient

Type annotations for `session.create_client("apigatewaymanagementapi")` as
[ApiGatewayManagementApiClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [delete_connection](./client.md#delete_connection)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [get_connection](./client.md#get_connection)
- [post_to_connection](./client.md#post_to_connection)

<a id="exceptions"></a>

### Exceptions

ApiGatewayManagementApiClient [exceptions](./client.md#exceptions)

- ClientError
- ForbiddenException
- GoneException
- LimitExceededException
- PayloadTooLargeException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_apigatewaymanagementapi.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef, ...
```

- [DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef)
- [GetConnectionRequestRequestTypeDef](./type_defs.md#getconnectionrequestrequesttypedef)
- [GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [PostToConnectionRequestRequestTypeDef](./type_defs.md#posttoconnectionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
