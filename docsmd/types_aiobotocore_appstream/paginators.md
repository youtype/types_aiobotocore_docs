# Paginators

> [Index](../README.md) > [AppStream](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#appstream)
    type annotations stubs module [types-aiobotocore-appstream](https://pypi.org/project/types-aiobotocore-appstream/).

## DescribeDirectoryConfigsPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_directory_configs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeDirectoryConfigs.html#AppStream.Paginator.DescribeDirectoryConfigs)

```python
# DescribeDirectoryConfigsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeDirectoryConfigsPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeDirectoryConfigsPaginator = client.get_paginator("describe_directory_configs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDirectoryConfigsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeDirectoryConfigsPaginator](./paginators.md#describedirectoryconfigspaginator)
3. item: [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDirectoryConfigsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DirectoryNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDirectoryConfigsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDirectoryConfigsResultTypeDef](./type_defs.md#describedirectoryconfigsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDirectoryConfigsRequestPaginateTypeDef = {  # (1)
    "DirectoryNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDirectoryConfigsRequestPaginateTypeDef](./type_defs.md#describedirectoryconfigsrequestpaginatetypedef) 
## DescribeFleetsPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeFleets.html#AppStream.Paginator.DescribeFleets)

```python
# DescribeFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeFleetsPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeFleetsPaginator = client.get_paginator("describe_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFleetsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeFleetsPaginator](./paginators.md#describefleetspaginator)
3. item: [:material-code-braces: DescribeFleetsResultTypeDef](./type_defs.md#describefleetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeFleetsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeFleetsResultTypeDef](./type_defs.md#describefleetsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFleetsRequestPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetsRequestPaginateTypeDef](./type_defs.md#describefleetsrequestpaginatetypedef) 
## DescribeImageBuildersPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_image_builders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeImageBuilders.html#AppStream.Paginator.DescribeImageBuilders)

```python
# DescribeImageBuildersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeImageBuildersPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeImageBuildersPaginator = client.get_paginator("describe_image_builders")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageBuildersResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeImageBuildersPaginator](./paginators.md#describeimagebuilderspaginator)
3. item: [:material-code-braces: DescribeImageBuildersResultTypeDef](./type_defs.md#describeimagebuildersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImageBuildersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeImageBuildersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeImageBuildersResultTypeDef](./type_defs.md#describeimagebuildersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImageBuildersRequestPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageBuildersRequestPaginateTypeDef](./type_defs.md#describeimagebuildersrequestpaginatetypedef) 
## DescribeImagesPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeImages.html#AppStream.Paginator.DescribeImages)

```python
# DescribeImagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeImagesPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImagesResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
3. item: [:material-code-braces: DescribeImagesResultTypeDef](./type_defs.md#describeimagesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    Arns: Sequence[str] = ...,
    Type: VisibilityTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeImagesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: VisibilityTypeType](./literals.md#visibilitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImagesResultTypeDef](./type_defs.md#describeimagesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImagesRequestPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestPaginateTypeDef](./type_defs.md#describeimagesrequestpaginatetypedef) 
## DescribeSessionsPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeSessions.html#AppStream.Paginator.DescribeSessions)

```python
# DescribeSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeSessionsPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeSessionsPaginator = client.get_paginator("describe_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSessionsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeSessionsPaginator](./paginators.md#describesessionspaginator)
3. item: [:material-code-braces: DescribeSessionsResultTypeDef](./type_defs.md#describesessionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str,
    FleetName: str,
    UserId: str = ...,
    AuthenticationType: AuthenticationTypeType = ...,  # (1)
    InstanceId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeSessionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSessionsResultTypeDef](./type_defs.md#describesessionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSessionsRequestPaginateTypeDef = {  # (1)
    "StackName": ...,
    "FleetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSessionsRequestPaginateTypeDef](./type_defs.md#describesessionsrequestpaginatetypedef) 
## DescribeStacksPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_stacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeStacks.html#AppStream.Paginator.DescribeStacks)

```python
# DescribeStacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeStacksPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeStacksPaginator = client.get_paginator("describe_stacks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStacksResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeStacksPaginator](./paginators.md#describestackspaginator)
3. item: [:material-code-braces: DescribeStacksResultTypeDef](./type_defs.md#describestacksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Names: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeStacksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStacksResultTypeDef](./type_defs.md#describestacksresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStacksRequestPaginateTypeDef = {  # (1)
    "Names": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStacksRequestPaginateTypeDef](./type_defs.md#describestacksrequestpaginatetypedef) 
## DescribeUserStackAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_user_stack_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeUserStackAssociations.html#AppStream.Paginator.DescribeUserStackAssociations)

```python
# DescribeUserStackAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeUserStackAssociationsPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeUserStackAssociationsPaginator = client.get_paginator("describe_user_stack_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUserStackAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeUserStackAssociationsPaginator](./paginators.md#describeuserstackassociationspaginator)
3. item: [:material-code-braces: DescribeUserStackAssociationsResultTypeDef](./type_defs.md#describeuserstackassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUserStackAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str = ...,
    UserName: str = ...,
    AuthenticationType: AuthenticationTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeUserStackAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeUserStackAssociationsResultTypeDef](./type_defs.md#describeuserstackassociationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUserStackAssociationsRequestPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUserStackAssociationsRequestPaginateTypeDef](./type_defs.md#describeuserstackassociationsrequestpaginatetypedef) 
## DescribeUsersPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("describe_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/DescribeUsers.html#AppStream.Paginator.DescribeUsers)

```python
# DescribeUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import DescribeUsersPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: DescribeUsersPaginator = client.get_paginator("describe_users")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeUsersResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [DescribeUsersPaginator](./paginators.md#describeuserspaginator)
3. item: [:material-code-braces: DescribeUsersResultTypeDef](./type_defs.md#describeusersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AuthenticationType: AuthenticationTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeUsersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeUsersResultTypeDef](./type_defs.md#describeusersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeUsersRequestPaginateTypeDef = {  # (1)
    "AuthenticationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeUsersRequestPaginateTypeDef](./type_defs.md#describeusersrequestpaginatetypedef) 
## ListAssociatedFleetsPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("list_associated_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/ListAssociatedFleets.html#AppStream.Paginator.ListAssociatedFleets)

```python
# ListAssociatedFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import ListAssociatedFleetsPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: ListAssociatedFleetsPaginator = client.get_paginator("list_associated_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedFleetsResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [ListAssociatedFleetsPaginator](./paginators.md#listassociatedfleetspaginator)
3. item: [:material-code-braces: ListAssociatedFleetsResultTypeDef](./type_defs.md#listassociatedfleetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    StackName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssociatedFleetsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedFleetsResultTypeDef](./type_defs.md#listassociatedfleetsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociatedFleetsRequestPaginateTypeDef = {  # (1)
    "StackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedFleetsRequestPaginateTypeDef](./type_defs.md#listassociatedfleetsrequestpaginatetypedef) 
## ListAssociatedStacksPaginator

Type annotations and code completion for `#!python session.create_client("appstream").get_paginator("list_associated_stacks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream/paginator/ListAssociatedStacks.html#AppStream.Paginator.ListAssociatedStacks)

```python
# ListAssociatedStacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_appstream.paginator import ListAssociatedStacksPaginator

session = get_session()
async with session.create_client("appstream") as client:  # (1)
    paginator: ListAssociatedStacksPaginator = client.get_paginator("list_associated_stacks")  # (2)
    async for item in paginator.paginate(...):
        item: ListAssociatedStacksResultTypeDef
        print(item)  # (3)
```

1. client: [AppStreamClient](./client.md)
2. paginator: [ListAssociatedStacksPaginator](./paginators.md#listassociatedstackspaginator)
3. item: [:material-code-braces: ListAssociatedStacksResultTypeDef](./type_defs.md#listassociatedstacksresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListAssociatedStacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FleetName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListAssociatedStacksResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAssociatedStacksResultTypeDef](./type_defs.md#listassociatedstacksresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAssociatedStacksRequestPaginateTypeDef = {  # (1)
    "FleetName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAssociatedStacksRequestPaginateTypeDef](./type_defs.md#listassociatedstacksrequestpaginatetypedef) 
