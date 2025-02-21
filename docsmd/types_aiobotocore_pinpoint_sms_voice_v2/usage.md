# Examples

> [Index](../README.md) > [PinpointSMSVoiceV2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PinpointSMSVoiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#pinpointsmsvoicev2)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice-v2](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pinpoint-sms-voice-v2]` package installed.

Write your `PinpointSMSVoiceV2` code as usual,
type checking and code completion should work out of the box.



```python
# PinpointSMSVoiceV2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    result = await client.associate_origination_identity()  # (2)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. result: [:material-code-braces: AssociateOriginationIdentityResultTypeDef](./type_defs.md#associateoriginationidentityresulttypedef) 



```python
# DescribeAccountAttributesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator = client.get_paginator("describe_account_attributes")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeAccountAttributesPaginator](./paginators.md#describeaccountattributespaginator)
3. item: [:material-code-braces: DescribeAccountAttributesResultTypeDef](./type_defs.md#describeaccountattributesresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[pinpoint-sms-voice-v2]`
or a standalone `types_aiobotocore_pinpoint_sms_voice_v2` package, you have to explicitly specify
`client: PinpointSMSVoiceV2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PinpointSMSVoiceV2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.client import PinpointSMSVoiceV2Client
from types_aiobotocore_pinpoint_sms_voice_v2.type_defs import AssociateOriginationIdentityResultTypeDef
from types_aiobotocore_pinpoint_sms_voice_v2.type_defs import AssociateOriginationIdentityRequestTypeDef


session = get_session()

async with session.create_client("pinpoint-sms-voice-v2") as client:
    client: PinpointSMSVoiceV2Client
    kwargs: AssociateOriginationIdentityRequestTypeDef = {...}
    result: AssociateOriginationIdentityResultTypeDef = await client.associate_origination_identity(**kwargs)
```



```python
# DescribeAccountAttributesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.client import PinpointSMSVoiceV2Client
from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeAccountAttributesPaginator
from types_aiobotocore_pinpoint_sms_voice_v2.type_defs import DescribeAccountAttributesResultTypeDef


session = get_session()

async with session.create_client("pinpoint-sms-voice-v2") as client:
    client: PinpointSMSVoiceV2Client
    paginator: DescribeAccountAttributesPaginator = client.get_paginator("describe_account_attributes")
    async for item in paginator.paginate(...):
        item: DescribeAccountAttributesResultTypeDef
        print(item)
```


