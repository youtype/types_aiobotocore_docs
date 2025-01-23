# Paginators

> [Index](../README.md) > [ChimeSDKVoice](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ChimeSDKVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#chimesdkvoice)
    type annotations stubs module [types-aiobotocore-chime-sdk-voice](https://pypi.org/project/types-aiobotocore-chime-sdk-voice/).

## ListSipMediaApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_paginator("list_sip_media_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice/paginator/ListSipMediaApplications.html#ChimeSDKVoice.Paginator.ListSipMediaApplications)

```python
# ListSipMediaApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_voice.paginator import ListSipMediaApplicationsPaginator

session = get_session()
async with session.create_client("chime-sdk-voice") as client:  # (1)
    paginator: ListSipMediaApplicationsPaginator = client.get_paginator("list_sip_media_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListSipMediaApplicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. paginator: [ListSipMediaApplicationsPaginator](./paginators.md#listsipmediaapplicationspaginator)
3. item: [:material-code-braces: ListSipMediaApplicationsResponseTypeDef](./type_defs.md#listsipmediaapplicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSipMediaApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSipMediaApplicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSipMediaApplicationsResponseTypeDef](./type_defs.md#listsipmediaapplicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSipMediaApplicationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSipMediaApplicationsRequestPaginateTypeDef](./type_defs.md#listsipmediaapplicationsrequestpaginatetypedef) 
## ListSipRulesPaginator

Type annotations and code completion for `#!python session.create_client("chime-sdk-voice").get_paginator("list_sip_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice/paginator/ListSipRules.html#ChimeSDKVoice.Paginator.ListSipRules)

```python
# ListSipRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_chime_sdk_voice.paginator import ListSipRulesPaginator

session = get_session()
async with session.create_client("chime-sdk-voice") as client:  # (1)
    paginator: ListSipRulesPaginator = client.get_paginator("list_sip_rules")  # (2)
    async for item in paginator.paginate(...):
        item: ListSipRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ChimeSDKVoiceClient](./client.md)
2. paginator: [ListSipRulesPaginator](./paginators.md#listsiprulespaginator)
3. item: [:material-code-braces: ListSipRulesResponseTypeDef](./type_defs.md#listsiprulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSipRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SipMediaApplicationId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSipRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSipRulesResponseTypeDef](./type_defs.md#listsiprulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSipRulesRequestPaginateTypeDef = {  # (1)
    "SipMediaApplicationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSipRulesRequestPaginateTypeDef](./type_defs.md#listsiprulesrequestpaginatetypedef) 
