# Paginators

> [Index](../README.md) > [CustomerProfiles](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#customerprofiles)
    type annotations stubs module [types-aiobotocore-customer-profiles](https://pypi.org/project/types-aiobotocore-customer-profiles/).

## GetSimilarProfilesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("get_similar_profiles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/GetSimilarProfiles.html#CustomerProfiles.Paginator.GetSimilarProfiles)

```python
# GetSimilarProfilesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import GetSimilarProfilesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: GetSimilarProfilesPaginator = client.get_paginator("get_similar_profiles")  # (2)
    async for item in paginator.paginate(...):
        item: GetSimilarProfilesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [GetSimilarProfilesPaginator](./paginators.md#getsimilarprofilespaginator)
3. item: [:material-code-braces: GetSimilarProfilesResponseTypeDef](./type_defs.md#getsimilarprofilesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetSimilarProfilesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    MatchType: MatchTypeType,  # (1)
    SearchKey: str,
    SearchValue: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetSimilarProfilesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: MatchTypeType](./literals.md#matchtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetSimilarProfilesResponseTypeDef](./type_defs.md#getsimilarprofilesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetSimilarProfilesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
    "MatchType": ...,
    "SearchKey": ...,
    "SearchValue": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSimilarProfilesRequestPaginateTypeDef](./type_defs.md#getsimilarprofilesrequestpaginatetypedef) 
## ListEventStreamsPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_event_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListEventStreams.html#CustomerProfiles.Paginator.ListEventStreams)

```python
# ListEventStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListEventStreamsPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListEventStreamsPaginator = client.get_paginator("list_event_streams")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventStreamsResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListEventStreamsPaginator](./paginators.md#listeventstreamspaginator)
3. item: [:material-code-braces: ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventStreamsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventStreamsResponseTypeDef](./type_defs.md#listeventstreamsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventStreamsRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventStreamsRequestPaginateTypeDef](./type_defs.md#listeventstreamsrequestpaginatetypedef) 
## ListEventTriggersPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_event_triggers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListEventTriggers.html#CustomerProfiles.Paginator.ListEventTriggers)

```python
# ListEventTriggersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListEventTriggersPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListEventTriggersPaginator = client.get_paginator("list_event_triggers")  # (2)
    async for item in paginator.paginate(...):
        item: ListEventTriggersResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListEventTriggersPaginator](./paginators.md#listeventtriggerspaginator)
3. item: [:material-code-braces: ListEventTriggersResponseTypeDef](./type_defs.md#listeventtriggersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEventTriggersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEventTriggersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEventTriggersResponseTypeDef](./type_defs.md#listeventtriggersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEventTriggersRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEventTriggersRequestPaginateTypeDef](./type_defs.md#listeventtriggersrequestpaginatetypedef) 
## ListObjectTypeAttributesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_object_type_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListObjectTypeAttributes.html#CustomerProfiles.Paginator.ListObjectTypeAttributes)

```python
# ListObjectTypeAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListObjectTypeAttributesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListObjectTypeAttributesPaginator = client.get_paginator("list_object_type_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: ListObjectTypeAttributesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListObjectTypeAttributesPaginator](./paginators.md#listobjecttypeattributespaginator)
3. item: [:material-code-braces: ListObjectTypeAttributesResponseTypeDef](./type_defs.md#listobjecttypeattributesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListObjectTypeAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    ObjectTypeName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListObjectTypeAttributesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListObjectTypeAttributesResponseTypeDef](./type_defs.md#listobjecttypeattributesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListObjectTypeAttributesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
    "ObjectTypeName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListObjectTypeAttributesRequestPaginateTypeDef](./type_defs.md#listobjecttypeattributesrequestpaginatetypedef) 
## ListRuleBasedMatchesPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_rule_based_matches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListRuleBasedMatches.html#CustomerProfiles.Paginator.ListRuleBasedMatches)

```python
# ListRuleBasedMatchesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListRuleBasedMatchesPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListRuleBasedMatchesPaginator = client.get_paginator("list_rule_based_matches")  # (2)
    async for item in paginator.paginate(...):
        item: ListRuleBasedMatchesResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListRuleBasedMatchesPaginator](./paginators.md#listrulebasedmatchespaginator)
3. item: [:material-code-braces: ListRuleBasedMatchesResponseTypeDef](./type_defs.md#listrulebasedmatchesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListRuleBasedMatchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRuleBasedMatchesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRuleBasedMatchesResponseTypeDef](./type_defs.md#listrulebasedmatchesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRuleBasedMatchesRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRuleBasedMatchesRequestPaginateTypeDef](./type_defs.md#listrulebasedmatchesrequestpaginatetypedef) 
## ListSegmentDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("customer-profiles").get_paginator("list_segment_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles/paginator/ListSegmentDefinitions.html#CustomerProfiles.Paginator.ListSegmentDefinitions)

```python
# ListSegmentDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_customer_profiles.paginator import ListSegmentDefinitionsPaginator

session = get_session()
async with session.create_client("customer-profiles") as client:  # (1)
    paginator: ListSegmentDefinitionsPaginator = client.get_paginator("list_segment_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: ListSegmentDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [CustomerProfilesClient](./client.md)
2. paginator: [ListSegmentDefinitionsPaginator](./paginators.md#listsegmentdefinitionspaginator)
3. item: [:material-code-braces: ListSegmentDefinitionsResponseTypeDef](./type_defs.md#listsegmentdefinitionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSegmentDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DomainName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSegmentDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSegmentDefinitionsResponseTypeDef](./type_defs.md#listsegmentdefinitionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSegmentDefinitionsRequestPaginateTypeDef = {  # (1)
    "DomainName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSegmentDefinitionsRequestPaginateTypeDef](./type_defs.md#listsegmentdefinitionsrequestpaginatetypedef) 
