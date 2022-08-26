# Paginators

> [Index](../README.md) > [DynamoDB](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## ListBackupsPaginator

Type annotations and code completion for `#!python session.create_client("dynamodb").get_paginator("list_backups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListBackups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.paginator import ListBackupsPaginator

session = get_session()
async with session.create_client("dynamodb") as client:  # (1)
    paginator: ListBackupsPaginator = client.get_paginator("list_backups")  # (2)
    async for item in paginator.paginate(...):
        item: ListBackupsOutputTableTypeDef
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [ListBackupsPaginator](./paginators.md#listbackupspaginator)
3. item: [:material-code-braces: ListBackupsOutputTableTypeDef](./type_defs.md#listbackupsoutputtabletypedef) 


### paginate

Type annotations and code completion for `#!python ListBackupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TableName: str = ...,
    TimeRangeLowerBound: Union[datetime, str] = ...,
    TimeRangeUpperBound: Union[datetime, str] = ...,
    BackupType: BackupTypeFilterType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListBackupsOutputTableTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBackupsOutputTableTypeDef](./type_defs.md#listbackupsoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: ListBackupsInputListBackupsPaginateTypeDef = {  # (1)
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBackupsInputListBackupsPaginateTypeDef](./type_defs.md#listbackupsinputlistbackupspaginatetypedef) 
## ListTablesPaginator

Type annotations and code completion for `#!python session.create_client("dynamodb").get_paginator("list_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTables)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.paginator import ListTablesPaginator

session = get_session()
async with session.create_client("dynamodb") as client:  # (1)
    paginator: ListTablesPaginator = client.get_paginator("list_tables")  # (2)
    async for item in paginator.paginate(...):
        item: ListTablesOutputTableTypeDef
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [ListTablesPaginator](./paginators.md#listtablespaginator)
3. item: [:material-code-braces: ListTablesOutputTableTypeDef](./type_defs.md#listtablesoutputtabletypedef) 


### paginate

Type annotations and code completion for `#!python ListTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTablesOutputTableTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTablesOutputTableTypeDef](./type_defs.md#listtablesoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: ListTablesInputListTablesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTablesInputListTablesPaginateTypeDef](./type_defs.md#listtablesinputlisttablespaginatetypedef) 
## ListTagsOfResourcePaginator

Type annotations and code completion for `#!python session.create_client("dynamodb").get_paginator("list_tags_of_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.ListTagsOfResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.paginator import ListTagsOfResourcePaginator

session = get_session()
async with session.create_client("dynamodb") as client:  # (1)
    paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsOfResourceOutputTableTypeDef
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [ListTagsOfResourcePaginator](./paginators.md#listtagsofresourcepaginator)
3. item: [:material-code-braces: ListTagsOfResourceOutputTableTypeDef](./type_defs.md#listtagsofresourceoutputtabletypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsOfResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsOfResourceOutputTableTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsOfResourceOutputTableTypeDef](./type_defs.md#listtagsofresourceoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef](./type_defs.md#listtagsofresourceinputlisttagsofresourcepaginatetypedef) 
## QueryPaginator

Type annotations and code completion for `#!python session.create_client("dynamodb").get_paginator("query")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Query)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.paginator import QueryPaginator

session = get_session()
async with session.create_client("dynamodb") as client:  # (1)
    paginator: QueryPaginator = client.get_paginator("query")  # (2)
    async for item in paginator.paginate(...):
        item: QueryOutputTableTypeDef
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [QueryPaginator](./paginators.md#querypaginator)
3. item: [:material-code-braces: QueryOutputTableTypeDef](./type_defs.md#queryoutputtabletypedef) 


### paginate

Type annotations and code completion for `#!python QueryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TableName: str,
    IndexName: str = ...,
    Select: SelectType = ...,  # (1)
    AttributesToGet: Sequence[str] = ...,
    ConsistentRead: bool = ...,
    KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (4)
    ScanIndexForward: bool = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (5)
    ProjectionExpression: str = ...,
    FilterExpression: str = ...,
    KeyConditionExpression: str = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> AsyncIterator[QueryOutputTableTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
7. See [:material-code-braces: QueryOutputTableTypeDef](./type_defs.md#queryoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: QueryInputQueryPaginateTypeDef = {  # (1)
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: QueryInputQueryPaginateTypeDef](./type_defs.md#queryinputquerypaginatetypedef) 
## ScanPaginator

Type annotations and code completion for `#!python session.create_client("dynamodb").get_paginator("scan")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB.Paginator.Scan)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dynamodb.paginator import ScanPaginator

session = get_session()
async with session.create_client("dynamodb") as client:  # (1)
    paginator: ScanPaginator = client.get_paginator("scan")  # (2)
    async for item in paginator.paginate(...):
        item: ScanOutputTableTypeDef
        print(item)  # (3)
```

1. client: [DynamoDBClient](./client.md)
2. paginator: [ScanPaginator](./paginators.md#scanpaginator)
3. item: [:material-code-braces: ScanOutputTableTypeDef](./type_defs.md#scanoutputtabletypedef) 


### paginate

Type annotations and code completion for `#!python ScanPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TableName: str,
    IndexName: str = ...,
    AttributesToGet: Sequence[str] = ...,
    Select: SelectType = ...,  # (1)
    ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (3)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (4)
    TotalSegments: int = ...,
    Segment: int = ...,
    ProjectionExpression: str = ...,
    FilterExpression: str = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
    ConsistentRead: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (5)
) -> AsyncIterator[ScanOutputTableTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ScanOutputTableTypeDef](./type_defs.md#scanoutputtabletypedef) 


```python title="Usage example with kwargs"
kwargs: ScanInputScanPaginateTypeDef = {  # (1)
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ScanInputScanPaginateTypeDef](./type_defs.md#scaninputscanpaginatetypedef) 
