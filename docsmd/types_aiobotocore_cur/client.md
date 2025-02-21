# CostandUsageReportServiceClient

> [Index](../README.md) > [CostandUsageReportService](./README.md) > CostandUsageReportServiceClient

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#costandusagereportservice)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## CostandUsageReportServiceClient

Type annotations and code completion for `#!python session.create_client("cur")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# CostandUsageReportServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cur.client import CostandUsageReportServiceClient

session = get_session()
async with session.create_client("cur") as client:
    client: CostandUsageReportServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cur").exceptions` structure.

```python
# CostandUsageReportServiceClient.exceptions usage example

async with session.create_client("cur") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.DuplicateReportNameException,
        client.InternalErrorException,
        client.ReportLimitReachedException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CostandUsageReportServiceClient usage type checking example

from types_aiobotocore_cur.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("cur").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("cur").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/generate_presigned_url.html)

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


### delete\_report\_definition

Deletes the specified report.

Type annotations and code completion for `#!python session.create_client("cur").delete_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/delete_report_definition.html)

```python
# delete_report_definition method definition

await def delete_report_definition(
    self,
    *,
    ReportName: str,
) -> DeleteReportDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReportDefinitionResponseTypeDef](./type_defs.md#deletereportdefinitionresponsetypedef) 


```python
# delete_report_definition method usage example with argument unpacking

kwargs: DeleteReportDefinitionRequestTypeDef = {  # (1)
    "ReportName": ...,
}

parent.delete_report_definition(**kwargs)
```

1. See [:material-code-braces: DeleteReportDefinitionRequestTypeDef](./type_defs.md#deletereportdefinitionrequesttypedef) 

### describe\_report\_definitions

Lists the Amazon Web Services Cost and Usage Report available to this account.

Type annotations and code completion for `#!python session.create_client("cur").describe_report_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/describe_report_definitions.html)

```python
# describe_report_definitions method definition

await def describe_report_definitions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeReportDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


```python
# describe_report_definitions method usage example with argument unpacking

kwargs: DescribeReportDefinitionsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_report_definitions(**kwargs)
```

1. See [:material-code-braces: DescribeReportDefinitionsRequestTypeDef](./type_defs.md#describereportdefinitionsrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags associated with the specified report definition.

Type annotations and code completion for `#!python session.create_client("cur").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ReportName: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ReportName": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### modify\_report\_definition

Allows you to programmatically update your report preferences.

Type annotations and code completion for `#!python session.create_client("cur").modify_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/modify_report_definition.html)

```python
# modify_report_definition method definition

await def modify_report_definition(
    self,
    *,
    ReportName: str,
    ReportDefinition: ReportDefinitionUnionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) [:material-code-braces: ReportDefinitionOutputTypeDef](./type_defs.md#reportdefinitionoutputtypedef) 


```python
# modify_report_definition method usage example with argument unpacking

kwargs: ModifyReportDefinitionRequestTypeDef = {  # (1)
    "ReportName": ...,
    "ReportDefinition": ...,
}

parent.modify_report_definition(**kwargs)
```

1. See [:material-code-braces: ModifyReportDefinitionRequestTypeDef](./type_defs.md#modifyreportdefinitionrequesttypedef) 

### put\_report\_definition

Creates a new report using the description that you provide.

Type annotations and code completion for `#!python session.create_client("cur").put_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/put_report_definition.html)

```python
# put_report_definition method definition

await def put_report_definition(
    self,
    *,
    ReportDefinition: ReportDefinitionUnionTypeDef,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) [:material-code-braces: ReportDefinitionOutputTypeDef](./type_defs.md#reportdefinitionoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# put_report_definition method usage example with argument unpacking

kwargs: PutReportDefinitionRequestTypeDef = {  # (1)
    "ReportDefinition": ...,
}

parent.put_report_definition(**kwargs)
```

1. See [:material-code-braces: PutReportDefinitionRequestTypeDef](./type_defs.md#putreportdefinitionrequesttypedef) 

### tag\_resource

Associates a set of tags with a report definition.

Type annotations and code completion for `#!python session.create_client("cur").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ReportName: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ReportName": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Disassociates a set of tags from a report definition.

Type annotations and code completion for `#!python session.create_client("cur").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ReportName: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ReportName": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cur").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cur").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

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

Type annotations and code completion for `#!python session.create_client("cur").get_paginator` method with overloads.

- `client.get_paginator("describe_report_definitions")` -> [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)



