# CostandUsageReportServiceClient

> [Index](../README.md) > [CostandUsageReportService](./README.md) > CostandUsageReportServiceClient

!!! note ""

    Auto-generated documentation for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
    type annotations stubs module [types-aiobotocore-cur](https://pypi.org/project/types-aiobotocore-cur/).

## CostandUsageReportServiceClient

Type annotations and code completion for `#!python session.create_client("cur")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_cur.client import CostandUsageReportServiceClient

session = get_session()
async with session.create_client("cur") as client:
    client: CostandUsageReportServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cur").exceptions` structure.

```python title="Usage example"
async with session.create_client("cur") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.DuplicateReportNameException,
        client.InternalErrorException,
        client.ReportLimitReachedException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_cur.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cur").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### delete\_report\_definition

Deletes the specified report.

Type annotations and code completion for `#!python session.create_client("cur").delete_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.delete_report_definition)

```python title="Method definition"
await def delete_report_definition(
    self,
    *,
    ReportName: str = ...,
) -> DeleteReportDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReportDefinitionResponseTypeDef](./type_defs.md#deletereportdefinitionresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DeleteReportDefinitionRequestRequestTypeDef = {  # (1)
    "ReportName": ...,
}

parent.delete_report_definition(**kwargs)
```

1. See [:material-code-braces: DeleteReportDefinitionRequestRequestTypeDef](./type_defs.md#deletereportdefinitionrequestrequesttypedef) 

### describe\_report\_definitions

Lists the AWS Cost and Usage reports available to this account.

Type annotations and code completion for `#!python session.create_client("cur").describe_report_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.describe_report_definitions)

```python title="Method definition"
await def describe_report_definitions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeReportDefinitionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReportDefinitionsResponseTypeDef](./type_defs.md#describereportdefinitionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReportDefinitionsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.describe_report_definitions(**kwargs)
```

1. See [:material-code-braces: DescribeReportDefinitionsRequestRequestTypeDef](./type_defs.md#describereportdefinitionsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cur").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### modify\_report\_definition

Allows you to programatically update your report preferences.

Type annotations and code completion for `#!python session.create_client("cur").modify_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.modify_report_definition)

```python title="Method definition"
await def modify_report_definition(
    self,
    *,
    ReportName: str,
    ReportDefinition: ReportDefinitionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 


```python title="Usage example with kwargs"
kwargs: ModifyReportDefinitionRequestRequestTypeDef = {  # (1)
    "ReportName": ...,
    "ReportDefinition": ...,
}

parent.modify_report_definition(**kwargs)
```

1. See [:material-code-braces: ModifyReportDefinitionRequestRequestTypeDef](./type_defs.md#modifyreportdefinitionrequestrequesttypedef) 

### put\_report\_definition

Creates a new report using the description that you provide.

Type annotations and code completion for `#!python session.create_client("cur").put_report_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.put_report_definition)

```python title="Method definition"
await def put_report_definition(
    self,
    *,
    ReportDefinition: ReportDefinitionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ReportDefinitionTypeDef](./type_defs.md#reportdefinitiontypedef) 


```python title="Usage example with kwargs"
kwargs: PutReportDefinitionRequestRequestTypeDef = {  # (1)
    "ReportDefinition": ...,
}

parent.put_report_definition(**kwargs)
```

1. See [:material-code-braces: PutReportDefinitionRequestRequestTypeDef](./type_defs.md#putreportdefinitionrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cur").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> CostandUsageReportServiceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cur").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("cur").get_paginator` method with overloads.

- `client.get_paginator("describe_report_definitions")` -> [DescribeReportDefinitionsPaginator](./paginators.md#describereportdefinitionspaginator)



