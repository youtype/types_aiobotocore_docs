# Paginators

> [Index](../README.md) > [Support](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Support](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#support)
    type annotations stubs module [types-aiobotocore-support](https://pypi.org/project/types-aiobotocore-support/).

## DescribeCasesPaginator

Type annotations and code completion for `#!python session.create_client("support").get_paginator("describe_cases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/paginator/DescribeCases.html#Support.Paginator.DescribeCases)

```python
# DescribeCasesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_support.paginator import DescribeCasesPaginator

session = get_session()
async with session.create_client("support") as client:  # (1)
    paginator: DescribeCasesPaginator = client.get_paginator("describe_cases")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCasesResponseTypeDef
        print(item)  # (3)
```

1. client: [SupportClient](./client.md)
2. paginator: [DescribeCasesPaginator](./paginators.md#describecasespaginator)
3. item: [:material-code-braces: DescribeCasesResponseTypeDef](./type_defs.md#describecasesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCasesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    caseIdList: Sequence[str] = ...,
    displayId: str = ...,
    afterTime: str = ...,
    beforeTime: str = ...,
    includeResolvedCases: bool = ...,
    language: str = ...,
    includeCommunications: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeCasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeCasesResponseTypeDef](./type_defs.md#describecasesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCasesRequestPaginateTypeDef = {  # (1)
    "caseIdList": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCasesRequestPaginateTypeDef](./type_defs.md#describecasesrequestpaginatetypedef) 
## DescribeCommunicationsPaginator

Type annotations and code completion for `#!python session.create_client("support").get_paginator("describe_communications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/paginator/DescribeCommunications.html#Support.Paginator.DescribeCommunications)

```python
# DescribeCommunicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_support.paginator import DescribeCommunicationsPaginator

session = get_session()
async with session.create_client("support") as client:  # (1)
    paginator: DescribeCommunicationsPaginator = client.get_paginator("describe_communications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCommunicationsResponseTypeDef
        print(item)  # (3)
```

1. client: [SupportClient](./client.md)
2. paginator: [DescribeCommunicationsPaginator](./paginators.md#describecommunicationspaginator)
3. item: [:material-code-braces: DescribeCommunicationsResponseTypeDef](./type_defs.md#describecommunicationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCommunicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    caseId: str,
    beforeTime: str = ...,
    afterTime: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeCommunicationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeCommunicationsResponseTypeDef](./type_defs.md#describecommunicationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCommunicationsRequestPaginateTypeDef = {  # (1)
    "caseId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCommunicationsRequestPaginateTypeDef](./type_defs.md#describecommunicationsrequestpaginatetypedef) 
