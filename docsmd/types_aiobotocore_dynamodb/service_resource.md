# DynamoDBServiceResource

> [Index](../README.md) > [DynamoDB](./README.md) > DynamoDBServiceResource

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#dynamodb)
    type annotations stubs module [types-aiobotocore-dynamodb](https://pypi.org/project/types-aiobotocore-dynamodb/).

## DynamoDBServiceResource

Type annotations and code completion for `#!python session.resource("dynamodb")`, included resources and collections.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/index.html)

```python
# DynamoDBServiceResource usage example

from types_aiobotocore_dynamodb.service_resource import DynamoDBServiceResource

def get_dynamodb_resource() -> DynamoDBServiceResource:
    return session.resource("dynamodb")
```


## Attributes


- `meta`: `DynamoDBResourceMeta`

- `tables`: `ServiceResourceTablesCollection`




## Collections

### ServiceResourceTablesCollection

Provides access to [Table](#table) resource.

Type annotations and code completion for `#!python session.resource("dynamodb").tables` collection.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/tables.html#DynamoDB.ServiceResource.tables)

```python
# ServiceResourceTablesCollection usage example

from types_aiobotocore_dynamodb.service_resource import ServiceResourceTablesCollection

def get_collection() -> ServiceResourceTablesCollection:
    return session.resource("dynamodb").tables
```



## Methods

### DynamoDBServiceResource.get\_available\_subresources method

Returns a list of all the available sub-resources for this resource.

Type annotations and code completion for `#!python session.resource("dynamodb").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


### DynamoDBServiceResource.batch\_get\_item method

The <code>BatchGetItem</code> operation returns the attributes of one or more
items from one or more tables.

Type annotations and code completion for `#!python session.resource("dynamodb").batch_get_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/batch_get_item.html)

```python
# batch_get_item method definition

await def batch_get_item(
    self,
    *,
    RequestItems: Mapping[str, KeysAndAttributesServiceResourceUnionTypeDef],  # (1)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (2)
) -> BatchGetItemOutputServiceResourceTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: KeysAndAttributesServiceResourceTypeDef](./type_defs.md#keysandattributesserviceresourcetypedef) [:material-code-braces: KeysAndAttributesServiceResourceOutputTypeDef](./type_defs.md#keysandattributesserviceresourceoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-braces: BatchGetItemOutputServiceResourceTypeDef](./type_defs.md#batchgetitemoutputserviceresourcetypedef) 


```python
# batch_get_item method usage example with argument unpacking

kwargs: BatchGetItemInputServiceResourceBatchGetItemTypeDef = {  # (1)
    "RequestItems": ...,
}

parent.batch_get_item(**kwargs)
```

1. See [:material-code-braces: BatchGetItemInputServiceResourceBatchGetItemTypeDef](./type_defs.md#batchgetiteminputserviceresourcebatchgetitemtypedef) 

### DynamoDBServiceResource.batch\_write\_item method

The <code>BatchWriteItem</code> operation puts or deletes multiple items in one
or more tables.

Type annotations and code completion for `#!python session.resource("dynamodb").batch_write_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/batch_write_item.html)

```python
# batch_write_item method definition

await def batch_write_item(
    self,
    *,
    RequestItems: Mapping[str, Sequence[WriteRequestServiceResourceUnionTypeDef]],  # (1)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (2)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (3)
) -> BatchWriteItemOutputServiceResourceTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: WriteRequestServiceResourceTypeDef](./type_defs.md#writerequestserviceresourcetypedef) [:material-code-braces: WriteRequestServiceResourceOutputTypeDef](./type_defs.md#writerequestserviceresourceoutputtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
4. See [:material-code-braces: BatchWriteItemOutputServiceResourceTypeDef](./type_defs.md#batchwriteitemoutputserviceresourcetypedef) 


```python
# batch_write_item method usage example with argument unpacking

kwargs: BatchWriteItemInputServiceResourceBatchWriteItemTypeDef = {  # (1)
    "RequestItems": ...,
}

parent.batch_write_item(**kwargs)
```

1. See [:material-code-braces: BatchWriteItemInputServiceResourceBatchWriteItemTypeDef](./type_defs.md#batchwriteiteminputserviceresourcebatchwriteitemtypedef) 

### DynamoDBServiceResource.create\_table method

The <code>CreateTable</code> operation adds a new table to your account.

Type annotations and code completion for `#!python session.resource("dynamodb").create_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/create_table.html)

```python
# create_table method definition

await def create_table(
    self,
    *,
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    LocalSecondaryIndexes: Sequence[LocalSecondaryIndexTypeDef] = ...,  # (3)
    GlobalSecondaryIndexes: Sequence[GlobalSecondaryIndexUnionTypeDef] = ...,  # (4)
    BillingMode: BillingModeType = ...,  # (5)
    ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,  # (6)
    StreamSpecification: StreamSpecificationTypeDef = ...,  # (7)
    SSESpecification: SSESpecificationTypeDef = ...,  # (8)
    Tags: Sequence[TagTypeDef] = ...,  # (9)
    TableClass: TableClassType = ...,  # (10)
    DeletionProtectionEnabled: bool = ...,
    WarmThroughput: WarmThroughputTypeDef = ...,  # (11)
    ResourcePolicy: str = ...,
    OnDemandThroughput: OnDemandThroughputTypeDef = ...,  # (12)
) -> _Table:
    ...
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) [:material-code-braces: GlobalSecondaryIndexOutputTypeDef](./type_defs.md#globalsecondaryindexoutputtypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
7. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
8. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
11. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 
12. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 


```python
# create_table method usage example with argument unpacking

kwargs: CreateTableInputServiceResourceCreateTableTypeDef = {  # (1)
    "AttributeDefinitions": ...,
    "TableName": ...,
    "KeySchema": ...,
}

parent.create_table(**kwargs)
```

1. See [:material-code-braces: CreateTableInputServiceResourceCreateTableTypeDef](./type_defs.md#createtableinputserviceresourcecreatetabletypedef) 

### DynamoDBServiceResource.Table method

Creates a Table resource.

Type annotations and code completion for `#!python session.resource("dynamodb").Table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/service-resource/Table.html)

```python
# Table method definition

await def Table(
    self,
    name: str,
) -> _Table:
    ...
```




## Table

Type annotations and code completion for `#!python session.resource("dynamodb").Table` class.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/index.html#DynamoDB.Table)

```python
# Table usage example

from types_aiobotocore_dynamodb.service_resource import Table

def get_resource() -> Table:
    return session.resource("dynamodb").Table(...)
```


### Table attributes


- `name`: `str`
- `attribute_definitions`: `Awaitable`[`List`[[AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef)]]
- `table_name`: `Awaitable`[`str`]
- `key_schema`: `Awaitable`[`List`[[KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef)]]
- `table_status`: `Awaitable`[[TableStatusType](./literals.md#tablestatustype)]
- `creation_date_time`: `Awaitable`[`datetime`]
- `provisioned_throughput`: `Awaitable`[[ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef)]
- `table_size_bytes`: `Awaitable`[`int`]
- `item_count`: `Awaitable`[`int`]
- `table_arn`: `Awaitable`[`str`]
- `table_id`: `Awaitable`[`str`]
- `billing_mode_summary`: `Awaitable`[[BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef)]
- `local_secondary_indexes`: `Awaitable`[`List`[[LocalSecondaryIndexDescriptionTypeDef](./type_defs.md#localsecondaryindexdescriptiontypedef)]]
- `global_secondary_indexes`: `Awaitable`[`List`[[GlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#globalsecondaryindexdescriptiontypedef)]]
- `stream_specification`: `Awaitable`[[StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef)]
- `latest_stream_label`: `Awaitable`[`str`]
- `latest_stream_arn`: `Awaitable`[`str`]
- `global_table_version`: `Awaitable`[`str`]
- `replicas`: `Awaitable`[`List`[[ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef)]]
- `restore_summary`: `Awaitable`[[RestoreSummaryTypeDef](./type_defs.md#restoresummarytypedef)]
- `sse_description`: `Awaitable`[[SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef)]
- `archival_summary`: `Awaitable`[[ArchivalSummaryTypeDef](./type_defs.md#archivalsummarytypedef)]
- `table_class_summary`: `Awaitable`[[TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef)]
- `deletion_protection_enabled`: `Awaitable`[`bool`]
- `on_demand_throughput`: `Awaitable`[[OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef)]
- `warm_throughput`: `Awaitable`[[TableWarmThroughputDescriptionTypeDef](./type_defs.md#tablewarmthroughputdescriptiontypedef)]
- `multi_region_consistency`: `Awaitable`[[MultiRegionConsistencyType](./literals.md#multiregionconsistencytype)]
- `meta`: `DynamoDBResourceMeta`





### Table methods


#### Table.get\_available\_subresources method

Returns a list of all the available sub-resources for this Table.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").get_available_subresources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/get_available_subresources.html)

```python
# get_available_subresources method definition

await def get_available_subresources(
    self,
) -> Sequence[str]:
    ...
```


#### Table.delete method

The <code>DeleteTable</code> operation deletes a table and all of its items.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/delete.html)

```python
# delete method definition

await def delete(
    self,
) -> DeleteTableOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTableOutputTypeDef](./type_defs.md#deletetableoutputtypedef) 

#### Table.delete\_item method

Deletes a single item in a table by primary key.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").delete_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/delete_item.html)

```python
# delete_item method definition

await def delete_item(
    self,
    *,
    Key: Mapping[str, TableAttributeValueTypeDef],
    Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,  # (1)
    ConditionalOperator: ConditionalOperatorType = ...,  # (2)
    ReturnValues: ReturnValueType = ...,  # (3)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (4)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (5)
    ConditionExpression: ConditionBaseImportTypeDef = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
    ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,  # (6)
) -> DeleteItemOutputTableTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
6. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
7. See [:material-code-braces: DeleteItemOutputTableTypeDef](./type_defs.md#deleteitemoutputtabletypedef) 


```python
# delete_item method usage example with argument unpacking

kwargs: DeleteItemInputTableDeleteItemTypeDef = {  # (1)
    "Key": ...,
}

parent.delete_item(**kwargs)
```

1. See [:material-code-braces: DeleteItemInputTableDeleteItemTypeDef](./type_defs.md#deleteiteminputtabledeleteitemtypedef) 

#### Table.get\_item method

The <code>GetItem</code> operation returns a set of attributes for the item
with the given primary key.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").get_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/get_item.html)

```python
# get_item method definition

await def get_item(
    self,
    *,
    Key: Mapping[str, TableAttributeValueTypeDef],
    AttributesToGet: Sequence[str] = ...,
    ConsistentRead: bool = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (1)
    ProjectionExpression: str = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
) -> GetItemOutputTableTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
2. See [:material-code-braces: GetItemOutputTableTypeDef](./type_defs.md#getitemoutputtabletypedef) 


```python
# get_item method usage example with argument unpacking

kwargs: GetItemInputTableGetItemTypeDef = {  # (1)
    "Key": ...,
}

parent.get_item(**kwargs)
```

1. See [:material-code-braces: GetItemInputTableGetItemTypeDef](./type_defs.md#getiteminputtablegetitemtypedef) 

#### Table.put\_item method

Creates a new item, or replaces an old item with a new item.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").put_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/put_item.html)

```python
# put_item method definition

await def put_item(
    self,
    *,
    Item: Mapping[str, TableAttributeValueTypeDef],
    Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,  # (1)
    ReturnValues: ReturnValueType = ...,  # (2)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (3)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (4)
    ConditionalOperator: ConditionalOperatorType = ...,  # (5)
    ConditionExpression: ConditionBaseImportTypeDef = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
    ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,  # (6)
) -> PutItemOutputTableTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
2. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
3. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
4. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
5. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
6. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
7. See [:material-code-braces: PutItemOutputTableTypeDef](./type_defs.md#putitemoutputtabletypedef) 


```python
# put_item method usage example with argument unpacking

kwargs: PutItemInputTablePutItemTypeDef = {  # (1)
    "Item": ...,
}

parent.put_item(**kwargs)
```

1. See [:material-code-braces: PutItemInputTablePutItemTypeDef](./type_defs.md#putiteminputtableputitemtypedef) 

#### Table.query method

You must provide the name of the partition key attribute and a single value for
that attribute.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").query` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/query.html)

```python
# query method definition

await def query(
    self,
    *,
    IndexName: str = ...,
    Select: SelectType = ...,  # (1)
    AttributesToGet: Sequence[str] = ...,
    Limit: int = ...,
    ConsistentRead: bool = ...,
    KeyConditions: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    QueryFilter: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (4)
    ScanIndexForward: bool = ...,
    ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (5)
    ProjectionExpression: str = ...,
    FilterExpression: ConditionBaseImportTypeDef = ...,
    KeyConditionExpression: ConditionBaseImportTypeDef = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
) -> QueryOutputTableTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: QueryOutputTableTypeDef](./type_defs.md#queryoutputtabletypedef) 


```python
# query method usage example with argument unpacking

kwargs: QueryInputTableQueryTypeDef = {  # (1)
    "IndexName": ...,
}

parent.query(**kwargs)
```

1. See [:material-code-braces: QueryInputTableQueryTypeDef](./type_defs.md#queryinputtablequerytypedef) 

#### Table.scan method

The <code>Scan</code> operation returns one or more items and item attributes
by accessing every item in a table or a secondary index.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").scan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/scan.html)

```python
# scan method definition

await def scan(
    self,
    *,
    IndexName: str = ...,
    AttributesToGet: Sequence[str] = ...,
    Limit: int = ...,
    Select: SelectType = ...,  # (1)
    ScanFilter: Mapping[str, ConditionTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (3)
    ExclusiveStartKey: Mapping[str, TableAttributeValueTypeDef] = ...,
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (4)
    TotalSegments: int = ...,
    Segment: int = ...,
    ProjectionExpression: str = ...,
    FilterExpression: ConditionBaseImportTypeDef = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
    ConsistentRead: bool = ...,
) -> ScanOutputTableTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTableTypeDef](./type_defs.md#conditiontabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-braces: ScanOutputTableTypeDef](./type_defs.md#scanoutputtabletypedef) 


```python
# scan method usage example with argument unpacking

kwargs: ScanInputTableScanTypeDef = {  # (1)
    "IndexName": ...,
}

parent.scan(**kwargs)
```

1. See [:material-code-braces: ScanInputTableScanTypeDef](./type_defs.md#scaninputtablescantypedef) 

#### Table.update method

Modifies the provisioned throughput settings, global secondary indexes, or
DynamoDB Streams settings for a given table.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/update.html)

```python
# update method definition

await def update(
    self,
    *,
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef] = ...,  # (1)
    BillingMode: BillingModeType = ...,  # (2)
    ProvisionedThroughput: ProvisionedThroughputTypeDef = ...,  # (3)
    GlobalSecondaryIndexUpdates: Sequence[GlobalSecondaryIndexUpdateTypeDef] = ...,  # (4)
    StreamSpecification: StreamSpecificationTypeDef = ...,  # (5)
    SSESpecification: SSESpecificationTypeDef = ...,  # (6)
    ReplicaUpdates: Sequence[ReplicationGroupUpdateTypeDef] = ...,  # (7)
    TableClass: TableClassType = ...,  # (8)
    DeletionProtectionEnabled: bool = ...,
    MultiRegionConsistency: MultiRegionConsistencyType = ...,  # (9)
    OnDemandThroughput: OnDemandThroughputTypeDef = ...,  # (10)
    WarmThroughput: WarmThroughputTypeDef = ...,  # (11)
) -> _Table:
    ...
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef) 
5. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
9. See [:material-code-brackets: MultiRegionConsistencyType](./literals.md#multiregionconsistencytype) 
10. See [:material-code-braces: OnDemandThroughputTypeDef](./type_defs.md#ondemandthroughputtypedef) 
11. See [:material-code-braces: WarmThroughputTypeDef](./type_defs.md#warmthroughputtypedef) 


```python
# update method usage example with argument unpacking

kwargs: UpdateTableInputTableUpdateTypeDef = {  # (1)
    "AttributeDefinitions": ...,
}

parent.update(**kwargs)
```

1. See [:material-code-braces: UpdateTableInputTableUpdateTypeDef](./type_defs.md#updatetableinputtableupdatetypedef) 

#### Table.update\_item method

Edits an existing item's attributes, or adds a new item to the table if it does
not already exist.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").update_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/update_item.html)

```python
# update_item method definition

await def update_item(
    self,
    *,
    Key: Mapping[str, TableAttributeValueTypeDef],
    AttributeUpdates: Mapping[str, AttributeValueUpdateTableTypeDef] = ...,  # (1)
    Expected: Mapping[str, ExpectedAttributeValueTableTypeDef] = ...,  # (2)
    ConditionalOperator: ConditionalOperatorType = ...,  # (3)
    ReturnValues: ReturnValueType = ...,  # (4)
    ReturnConsumedCapacity: ReturnConsumedCapacityType = ...,  # (5)
    ReturnItemCollectionMetrics: ReturnItemCollectionMetricsType = ...,  # (6)
    UpdateExpression: str = ...,
    ConditionExpression: ConditionBaseImportTypeDef = ...,
    ExpressionAttributeNames: Mapping[str, str] = ...,
    ExpressionAttributeValues: Mapping[str, TableAttributeValueTypeDef] = ...,
    ReturnValuesOnConditionCheckFailure: ReturnValuesOnConditionCheckFailureType = ...,  # (7)
) -> UpdateItemOutputTableTypeDef:  # (8)
    ...
```

1. See [:material-code-braces: AttributeValueUpdateTableTypeDef](./type_defs.md#attributevalueupdatetabletypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTableTypeDef](./type_defs.md#expectedattributevaluetabletypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
7. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
8. See [:material-code-braces: UpdateItemOutputTableTypeDef](./type_defs.md#updateitemoutputtabletypedef) 


```python
# update_item method usage example with argument unpacking

kwargs: UpdateItemInputTableUpdateItemTypeDef = {  # (1)
    "Key": ...,
}

parent.update_item(**kwargs)
```

1. See [:material-code-braces: UpdateItemInputTableUpdateItemTypeDef](./type_defs.md#updateiteminputtableupdateitemtypedef) 

#### Table.wait\_until\_exists method

Waits until Table is exists.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").wait_until_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/wait_until_exists.html)

```python
# wait_until_exists method definition

await def wait_until_exists(
    self,
) -> None:
    ...
```


#### Table.wait\_until\_not\_exists method

Waits until Table is not_exists.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").wait_until_not_exists` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/wait_until_not_exists.html)

```python
# wait_until_not_exists method definition

await def wait_until_not_exists(
    self,
) -> None:
    ...
```


#### Table.batch\_writer method

Create a batch writer object.

Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").batch_writer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/batch_writer.html)

```python
# batch_writer method definition

def batch_writer(
    self,
    overwrite_by_pkeys: Union[List[str], None] = ...,
    flush_amount: int = ...,
    on_exit_loop_sleep: int = ...,
) -> BatchWriter:
    ...
```



```python
# batch_writer method usage example with argument unpacking

kwargs: TableBatchWriterRequestTypeDef = {  # (1)
    "overwrite_by_pkeys": ...,
}

parent.batch_writer(**kwargs)
```

1. See [:material-code-braces: TableBatchWriterRequestTypeDef](./type_defs.md#tablebatchwriterrequesttypedef) 

#### Table.load method



Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").load` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/load.html)

```python
# load method definition

await def load(
    self,
) -> None:
    ...
```


#### Table.reload method



Type annotations and code completion for `#!python aiobotocore.resource("dynamodb").reload` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb/table/reload.html)

```python
# reload method definition

await def reload(
    self,
) -> None:
    ...
```




