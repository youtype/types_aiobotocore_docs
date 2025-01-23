# BillingandCostManagementDataExportsClient

> [Index](../README.md) > [BillingandCostManagementDataExports](./README.md) > BillingandCostManagementDataExportsClient

!!! note ""

    Auto-generated documentation for [BillingandCostManagementDataExports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#billingandcostmanagementdataexports)
    type annotations stubs module [types-aiobotocore-bcm-data-exports](https://pypi.org/project/types-aiobotocore-bcm-data-exports/).

## BillingandCostManagementDataExportsClient

Type annotations and code completion for `#!python session.create_client("bcm-data-exports")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports.Client)

```python
# BillingandCostManagementDataExportsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bcm_data_exports.client import BillingandCostManagementDataExportsClient

session = get_session()
async with session.create_client("bcm-data-exports") as client:
    client: BillingandCostManagementDataExportsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bcm-data-exports").exceptions` structure.

```python
# BillingandCostManagementDataExportsClient.exceptions usage example

async with session.create_client("bcm-data-exports") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# BillingandCostManagementDataExportsClient usage type checking example

from types_aiobotocore_bcm_data_exports.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("bcm-data-exports").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("bcm-data-exports").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### create\_export

Creates a data export and specifies the data query, the delivery preference,
and any optional resource tags.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").create_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/create_export.html)

```python
# create_export method definition

await def create_export(
    self,
    *,
    Export: ExportTypeDef,  # (1)
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
) -> CreateExportResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExportTypeDef](./type_defs.md#exporttypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-braces: CreateExportResponseTypeDef](./type_defs.md#createexportresponsetypedef) 


```python
# create_export method usage example with argument unpacking

kwargs: CreateExportRequestRequestTypeDef = {  # (1)
    "Export": ...,
}

parent.create_export(**kwargs)
```

1. See [:material-code-braces: CreateExportRequestRequestTypeDef](./type_defs.md#createexportrequestrequesttypedef) 

### delete\_export

Deletes an existing data export.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").delete_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/delete_export.html)

```python
# delete_export method definition

await def delete_export(
    self,
    *,
    ExportArn: str,
) -> DeleteExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteExportResponseTypeDef](./type_defs.md#deleteexportresponsetypedef) 


```python
# delete_export method usage example with argument unpacking

kwargs: DeleteExportRequestRequestTypeDef = {  # (1)
    "ExportArn": ...,
}

parent.delete_export(**kwargs)
```

1. See [:material-code-braces: DeleteExportRequestRequestTypeDef](./type_defs.md#deleteexportrequestrequesttypedef) 

### get\_execution

Exports data based on the source data update.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").get_execution` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/get_execution.html)

```python
# get_execution method definition

await def get_execution(
    self,
    *,
    ExecutionId: str,
    ExportArn: str,
) -> GetExecutionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExecutionResponseTypeDef](./type_defs.md#getexecutionresponsetypedef) 


```python
# get_execution method usage example with argument unpacking

kwargs: GetExecutionRequestRequestTypeDef = {  # (1)
    "ExecutionId": ...,
    "ExportArn": ...,
}

parent.get_execution(**kwargs)
```

1. See [:material-code-braces: GetExecutionRequestRequestTypeDef](./type_defs.md#getexecutionrequestrequesttypedef) 

### get\_export

Views the definition of an existing data export.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").get_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/get_export.html)

```python
# get_export method definition

await def get_export(
    self,
    *,
    ExportArn: str,
) -> GetExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetExportResponseTypeDef](./type_defs.md#getexportresponsetypedef) 


```python
# get_export method usage example with argument unpacking

kwargs: GetExportRequestRequestTypeDef = {  # (1)
    "ExportArn": ...,
}

parent.get_export(**kwargs)
```

1. See [:material-code-braces: GetExportRequestRequestTypeDef](./type_defs.md#getexportrequestrequesttypedef) 

### get\_table

Returns the metadata for the specified table and table properties.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").get_table` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/get_table.html)

```python
# get_table method definition

await def get_table(
    self,
    *,
    TableName: str,
    TableProperties: Mapping[str, str] = ...,
) -> GetTableResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTableResponseTypeDef](./type_defs.md#gettableresponsetypedef) 


```python
# get_table method usage example with argument unpacking

kwargs: GetTableRequestRequestTypeDef = {  # (1)
    "TableName": ...,
}

parent.get_table(**kwargs)
```

1. See [:material-code-braces: GetTableRequestRequestTypeDef](./type_defs.md#gettablerequestrequesttypedef) 

### list\_executions

Lists the historical executions for the export.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").list_executions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/list_executions.html)

```python
# list_executions method definition

await def list_executions(
    self,
    *,
    ExportArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListExecutionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExecutionsResponseTypeDef](./type_defs.md#listexecutionsresponsetypedef) 


```python
# list_executions method usage example with argument unpacking

kwargs: ListExecutionsRequestRequestTypeDef = {  # (1)
    "ExportArn": ...,
}

parent.list_executions(**kwargs)
```

1. See [:material-code-braces: ListExecutionsRequestRequestTypeDef](./type_defs.md#listexecutionsrequestrequesttypedef) 

### list\_exports

Lists all data export definitions.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").list_exports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/list_exports.html)

```python
# list_exports method definition

await def list_exports(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListExportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListExportsResponseTypeDef](./type_defs.md#listexportsresponsetypedef) 


```python
# list_exports method usage example with argument unpacking

kwargs: ListExportsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_exports(**kwargs)
```

1. See [:material-code-braces: ListExportsRequestRequestTypeDef](./type_defs.md#listexportsrequestrequesttypedef) 

### list\_tables

Lists all available tables in data exports.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").list_tables` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/list_tables.html)

```python
# list_tables method definition

await def list_tables(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTablesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTablesResponseTypeDef](./type_defs.md#listtablesresponsetypedef) 


```python
# list_tables method usage example with argument unpacking

kwargs: ListTablesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_tables(**kwargs)
```

1. See [:material-code-braces: ListTablesRequestRequestTypeDef](./type_defs.md#listtablesrequestrequesttypedef) 

### list\_tags\_for\_resource

List tags associated with an existing data export.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Adds tags for an existing data export definition.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    ResourceTags: Sequence[ResourceTagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "ResourceTags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deletes tags associated with an existing data export definition.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    ResourceTagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "ResourceTagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_export

Updates an existing data export by overwriting all export parameters.

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").update_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports/client/update_export.html)

```python
# update_export method definition

await def update_export(
    self,
    *,
    Export: ExportTypeDef,  # (1)
    ExportArn: str,
) -> UpdateExportResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExportTypeDef](./type_defs.md#exporttypedef) 
2. See [:material-code-braces: UpdateExportResponseTypeDef](./type_defs.md#updateexportresponsetypedef) 


```python
# update_export method usage example with argument unpacking

kwargs: UpdateExportRequestRequestTypeDef = {  # (1)
    "Export": ...,
    "ExportArn": ...,
}

parent.update_export(**kwargs)
```

1. See [:material-code-braces: UpdateExportRequestRequestTypeDef](./type_defs.md#updateexportrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bcm-data-exports").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bcm-data-exports").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#BillingandCostManagementDataExports.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("bcm-data-exports").get_paginator` method with overloads.

- `client.get_paginator("list_executions")` -> [ListExecutionsPaginator](./paginators.md#listexecutionspaginator)
- `client.get_paginator("list_exports")` -> [ListExportsPaginator](./paginators.md#listexportspaginator)
- `client.get_paginator("list_tables")` -> [ListTablesPaginator](./paginators.md#listtablespaginator)



