# QLDBSessionClient

> [Index](../README.md) > [QLDBSession](./README.md) > QLDBSessionClient

!!! note ""

    Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
    type annotations stubs module [types-aiobotocore-qldb-session](https://pypi.org/project/types-aiobotocore-qldb-session/).

## QLDBSessionClient

Type annotations and code completion for `#!python session.create_client("qldb-session")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_qldb_session.client import QLDBSessionClient

session = get_session()
async with session.create_client("qldb-session") as client:
    client: QLDBSessionClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("qldb-session").exceptions` structure.

```python title="Usage example"
async with session.create_client("qldb-session") as client:
    try:
        do_something(client)
    except (
            client.BadRequestException,
        client.CapacityExceededException,
        client.ClientError,
        client.InvalidSessionException,
        client.LimitExceededException,
        client.OccConflictException,
        client.RateExceededException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_qldb_session.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("qldb-session").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("qldb-session").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("qldb-session").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### send\_command

Sends a command to an Amazon QLDB ledger.

Type annotations and code completion for `#!python session.create_client("qldb-session").send_command` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.send_command)

```python title="Method definition"
await def send_command(
    self,
    *,
    SessionToken: str = ...,
    StartSession: StartSessionRequestTypeDef = ...,  # (1)
    StartTransaction: Mapping[str, Any] = ...,
    EndSession: Mapping[str, Any] = ...,
    CommitTransaction: CommitTransactionRequestTypeDef = ...,  # (2)
    AbortTransaction: Mapping[str, Any] = ...,
    ExecuteStatement: ExecuteStatementRequestTypeDef = ...,  # (3)
    FetchPage: FetchPageRequestTypeDef = ...,  # (4)
) -> SendCommandResultTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: StartSessionRequestTypeDef](./type_defs.md#startsessionrequesttypedef) 
2. See [:material-code-braces: CommitTransactionRequestTypeDef](./type_defs.md#committransactionrequesttypedef) 
3. See [:material-code-braces: ExecuteStatementRequestTypeDef](./type_defs.md#executestatementrequesttypedef) 
4. See [:material-code-braces: FetchPageRequestTypeDef](./type_defs.md#fetchpagerequesttypedef) 
5. See [:material-code-braces: SendCommandResultTypeDef](./type_defs.md#sendcommandresulttypedef) 


```python title="Usage example with kwargs"
kwargs: SendCommandRequestRequestTypeDef = {  # (1)
    "SessionToken": ...,
}

parent.send_command(**kwargs)
```

1. See [:material-code-braces: SendCommandRequestRequestTypeDef](./type_defs.md#sendcommandrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("qldb-session").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> QLDBSessionClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("qldb-session").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





