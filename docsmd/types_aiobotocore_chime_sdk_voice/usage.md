# Examples

> [Index](../README.md) > [ChimeSDKVoice](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ChimeSDKVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#chimesdkvoice)
    type annotations stubs module [types-aiobotocore-chime-sdk-voice](https://pypi.org/project/types-aiobotocore-chime-sdk-voice/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[chime-sdk-voice]` package installed.

Write your `ChimeSDKVoice` code as usual,
type checking and code completion should work out of the box.



```python
# ChimeSDKVoiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chime-sdk-voice") as client:  # (1)
    result = await client.associate_phone_numbers_with_voice_connector()  # (2)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. result: [:material-code-braces: AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef](./type_defs.md#associatephonenumberswithvoiceconnectorresponsetypedef) 



```python
# ListSipMediaApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("chime-sdk-voice") as client:  # (1)
    paginator = client.get_paginator("list_sip_media_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. paginator: [ListSipMediaApplicationsPaginator](./paginators.md#listsipmediaapplicationspaginator)
3. item: [:material-code-braces: ListSipMediaApplicationsResponseTypeDef](./type_defs.md#listsipmediaapplicationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[chime-sdk-voice]`
or a standalone `types_aiobotocore_chime_sdk_voice` package, you have to explicitly specify
`client: ChimeSDKVoiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ChimeSDKVoiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_voice.client import ChimeSDKVoiceClient
from types_aiobotocore_chime_sdk_voice.type_defs import AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef
from types_aiobotocore_chime_sdk_voice.type_defs import AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef


session = get_session()

async with session.create_client("chime-sdk-voice") as client:
    client: ChimeSDKVoiceClient
    kwargs: AssociatePhoneNumbersWithVoiceConnectorRequestTypeDef = {...}
    result: AssociatePhoneNumbersWithVoiceConnectorResponseTypeDef = await client.associate_phone_numbers_with_voice_connector(**kwargs)
```



```python
# ListSipMediaApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_voice.client import ChimeSDKVoiceClient
from types_aiobotocore_chime_sdk_voice.paginator import ListSipMediaApplicationsPaginator
from types_aiobotocore_chime_sdk_voice.type_defs import ListSipMediaApplicationsResponseTypeDef


session = get_session()

async with session.create_client("chime-sdk-voice") as client:
    client: ChimeSDKVoiceClient
    paginator: ListSipMediaApplicationsPaginator = client.get_paginator("list_sip_media_applications")
    async for item in paginator.paginate(...):
        item: ListSipMediaApplicationsResponseTypeDef
        print(item)
```


