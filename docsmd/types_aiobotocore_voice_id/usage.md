# Examples

> [Index](../README.md) > [VoiceID](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [VoiceID](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#voiceid)
    type annotations stubs module [types-aiobotocore-voice-id](https://pypi.org/project/types-aiobotocore-voice-id/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[voice-id]` package installed.

Write your `VoiceID` code as usual,
type checking and code completion should work out of the box.



```python
# VoiceIDClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("voice-id") as client:  # (1)
    result = await client.associate_fraudster()  # (2)
```

1. client: [VoiceIDClient](./client.md)
2. result: [:material-code-braces: AssociateFraudsterResponseTypeDef](./type_defs.md#associatefraudsterresponsetypedef) 



```python
# ListDomainsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("voice-id") as client:  # (1)
    paginator = client.get_paginator("list_domains")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [VoiceIDClient](./client.md)
2. paginator: [ListDomainsPaginator](./paginators.md#listdomainspaginator)
3. item: [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[voice-id]`
or a standalone `types_aiobotocore_voice_id` package, you have to explicitly specify
`client: VoiceIDClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# VoiceIDClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.client import VoiceIDClient
from types_aiobotocore_voice_id.type_defs import AssociateFraudsterResponseTypeDef
from types_aiobotocore_voice_id.type_defs import AssociateFraudsterRequestTypeDef


session = get_session()

async with session.create_client("voice-id") as client:
    client: VoiceIDClient
    kwargs: AssociateFraudsterRequestTypeDef = {...}
    result: AssociateFraudsterResponseTypeDef = await client.associate_fraudster(**kwargs)
```



```python
# ListDomainsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_voice_id.client import VoiceIDClient
from types_aiobotocore_voice_id.paginator import ListDomainsPaginator
from types_aiobotocore_voice_id.type_defs import ListDomainsResponseTypeDef


session = get_session()

async with session.create_client("voice-id") as client:
    client: VoiceIDClient
    paginator: ListDomainsPaginator = client.get_paginator("list_domains")
    async for item in paginator.paginate(...):
        item: ListDomainsResponseTypeDef
        print(item)
```


