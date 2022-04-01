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
async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    paginator: ListBackupsPaginator = client.get_paginator("list_backups")
```


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
) -> AsyncIterator[ListBackupsOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListBackupsOutputTypeDef](./type_defs.md#listbackupsoutputtypedef) 


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
async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    paginator: ListTablesPaginator = client.get_paginator("list_tables")
```


### paginate

Type annotations and code completion for `#!python ListTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTablesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTablesOutputTypeDef](./type_defs.md#listtablesoutputtypedef) 


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
async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    paginator: ListTagsOfResourcePaginator = client.get_paginator("list_tags_of_resource")
```


### paginate

Type annotations and code completion for `#!python ListTagsOfResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsOfResourceOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsOfResourceOutputTypeDef](./type_defs.md#listtagsofresourceoutputtypedef) 


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
async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    paginator: QueryPaginator = client.get_paginator("query")
```


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
    KeyConditions: Mapping[str, ConditionTypeDef] = ...,  # (2)
    QueryFilter: Mapping[str, ConditionTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (4)
    ScanIndexForward: bool = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (5)
    ProjectionExpression: str = ...,
    FilterExpression: str = ...,
    KeyConditionExpression: str = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (6)
) -> AsyncIterator[QueryOutputTypeDef]:  # (7)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
7. See [:material-code-braces: QueryOutputTypeDef](./type_defs.md#queryoutputtypedef) 


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
async with session.create_client("dynamodb") as client:
    client: DynamoDBClient
    paginator: ScanPaginator = client.get_paginator("scan")
```


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
    ScanFilter: Mapping[str, ConditionTypeDef] = ...,  # (2)
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
) -> AsyncIterator[ScanOutputTypeDef]:  # (6)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
6. See [:material-code-braces: ScanOutputTypeDef](./type_defs.md#scanoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ScanInputScanPaginateTypeDef = {  # (1)
    "TableName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ScanInputScanPaginateTypeDef](./type_defs.md#scaninputscanpaginatetypedef) 
