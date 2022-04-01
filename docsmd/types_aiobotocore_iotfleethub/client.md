# IoTFleetHubClient

> [Index](../README.md) > [IoTFleetHub](./README.md) > IoTFleetHubClient

!!! note ""

    Auto-generated documentation for [IoTFleetHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
    type annotations stubs module [types-aiobotocore-iotfleethub](https://pypi.org/project/types-aiobotocore-iotfleethub/).

## IoTFleetHubClient

Type annotations and code completion for `#!python session.create_client("iotfleethub")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_iotfleethub.client import IoTFleetHubClient

session = get_session()
async with session.create_client("iotfleethub") as client:
    client: IoTFleetHubClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iotfleethub").exceptions` structure.

```python title="Usage example"
async with session.create_client("iotfleethub") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ConflictException,
        client.InternalFailureException,
        client.InvalidRequestException,
        client.LimitExceededException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_iotfleethub.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("iotfleethub").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### create\_application

Creates a Fleet Hub for AWS IoT Device Management web application.

Type annotations and code completion for `#!python session.create_client("iotfleethub").create_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.create_application)

```python title="Method definition"
await def create_application(
    self,
    *,
    applicationName: str,
    roleArn: str,
    applicationDescription: str = ...,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateApplicationResponseTypeDef](./type_defs.md#createapplicationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: CreateApplicationRequestRequestTypeDef = {  # (1)
    "applicationName": ...,
    "roleArn": ...,
}

parent.create_application(**kwargs)
```

1. See [:material-code-braces: CreateApplicationRequestRequestTypeDef](./type_defs.md#createapplicationrequestrequesttypedef) 

### delete\_application

Deletes a Fleet Hub for AWS IoT Device Management web application.

Type annotations and code completion for `#!python session.create_client("iotfleethub").delete_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.delete_application)

```python title="Method definition"
await def delete_application(
    self,
    *,
    applicationId: str,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: DeleteApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.delete_application(**kwargs)
```

1. See [:material-code-braces: DeleteApplicationRequestRequestTypeDef](./type_defs.md#deleteapplicationrequestrequesttypedef) 

### describe\_application

Gets information about a Fleet Hub for AWS IoT Device Management web
application.

Type annotations and code completion for `#!python session.create_client("iotfleethub").describe_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.describe_application)

```python title="Method definition"
await def describe_application(
    self,
    *,
    applicationId: str,
) -> DescribeApplicationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeApplicationResponseTypeDef](./type_defs.md#describeapplicationresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.describe_application(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationRequestRequestTypeDef](./type_defs.md#describeapplicationrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("iotfleethub").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.generate_presigned_url)

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


### list\_applications

Gets a list of Fleet Hub for AWS IoT Device Management web applications for the
current account.

Type annotations and code completion for `#!python session.create_client("iotfleethub").list_applications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.list_applications)

```python title="Method definition"
await def list_applications(
    self,
    *,
    nextToken: str = ...,
) -> ListApplicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListApplicationsRequestRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_applications(**kwargs)
```

1. See [:material-code-braces: ListApplicationsRequestRequestTypeDef](./type_defs.md#listapplicationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("iotfleethub").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.list_tags_for_resource)

```python title="Method definition"
await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### tag\_resource

Adds to or modifies the tags of the specified resource.

Type annotations and code completion for `#!python session.create_client("iotfleethub").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.tag_resource)

```python title="Method definition"
await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes the specified tags (metadata) from the resource.

Type annotations and code completion for `#!python session.create_client("iotfleethub").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.untag_resource)

```python title="Method definition"
await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_application

Updates information about a Fleet Hub for a AWS IoT Device Management web
application.

Type annotations and code completion for `#!python session.create_client("iotfleethub").update_application` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.update_application)

```python title="Method definition"
await def update_application(
    self,
    *,
    applicationId: str,
    applicationName: str = ...,
    applicationDescription: str = ...,
    clientToken: str = ...,
) -> Dict[str, Any]:
    ...
```



```python title="Usage example with kwargs"
kwargs: UpdateApplicationRequestRequestTypeDef = {  # (1)
    "applicationId": ...,
}

parent.update_application(**kwargs)
```

1. See [:material-code-braces: UpdateApplicationRequestRequestTypeDef](./type_defs.md#updateapplicationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iotfleethub").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> IoTFleetHubClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iotfleethub").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("iotfleethub").get_paginator` method with overloads.

- `client.get_paginator("list_applications")` -> [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)



