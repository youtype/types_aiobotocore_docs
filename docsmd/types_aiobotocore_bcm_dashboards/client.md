# BillingandCostManagementDashboardsClient

> [Index](../README.md) > [BillingandCostManagementDashboards](./README.md) > BillingandCostManagementDashboardsClient

!!! note ""

    Auto-generated documentation for [BillingandCostManagementDashboards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards.html#billingandcostmanagementdashboards)
    type annotations stubs module [types-aiobotocore-bcm-dashboards](https://pypi.org/project/types-aiobotocore-bcm-dashboards/).

## BillingandCostManagementDashboardsClient

Type annotations and code completion for `#!python session.create_client("bcm-dashboards")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards.html#BillingandCostManagementDashboards.Client)

```python
# BillingandCostManagementDashboardsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bcm_dashboards.client import BillingandCostManagementDashboardsClient

session = get_session()
async with session.create_client("bcm-dashboards") as client:
    client: BillingandCostManagementDashboardsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bcm-dashboards").exceptions` structure.

```python
# BillingandCostManagementDashboardsClient.exceptions usage example

async with session.create_client("bcm-dashboards") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
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
# BillingandCostManagementDashboardsClient usage type checking example

from types_aiobotocore_bcm_dashboards.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("bcm-dashboards").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("bcm-dashboards").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/generate_presigned_url.html)

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


### create\_dashboard

Creates a new dashboard that can contain multiple widgets displaying cost and
usage data.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").create_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/create_dashboard.html)

```python
# create_dashboard method definition

await def create_dashboard(
    self,
    *,
    name: str,
    widgets: Sequence[WidgetUnionTypeDef],  # (1)
    description: str = ...,
    resourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
) -> CreateDashboardResponseTypeDef:  # (3)
    ...
```

1. See `Sequence[WidgetUnionTypeDef]`
2. See `Sequence[ResourceTagTypeDef]`
3. See [:material-code-braces: CreateDashboardResponseTypeDef](./type_defs.md#createdashboardresponsetypedef)


```python
# create_dashboard method usage example with argument unpacking

kwargs: CreateDashboardRequestTypeDef = {  # (1)
    "name": ...,
    "widgets": ...,
}

parent.create_dashboard(**kwargs)
```

1. See [:material-code-braces: CreateDashboardRequestTypeDef](./type_defs.md#createdashboardrequesttypedef)

### delete\_dashboard

Deletes a specified dashboard.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").delete_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/delete_dashboard.html)

```python
# delete_dashboard method definition

await def delete_dashboard(
    self,
    *,
    arn: str,
) -> DeleteDashboardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDashboardResponseTypeDef](./type_defs.md#deletedashboardresponsetypedef)


```python
# delete_dashboard method usage example with argument unpacking

kwargs: DeleteDashboardRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_dashboard(**kwargs)
```

1. See [:material-code-braces: DeleteDashboardRequestTypeDef](./type_defs.md#deletedashboardrequesttypedef)

### get\_dashboard

Retrieves the configuration and metadata of a specified dashboard, including
its widgets and layout settings.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").get_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/get_dashboard.html)

```python
# get_dashboard method definition

await def get_dashboard(
    self,
    *,
    arn: str,
) -> GetDashboardResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDashboardResponseTypeDef](./type_defs.md#getdashboardresponsetypedef)


```python
# get_dashboard method usage example with argument unpacking

kwargs: GetDashboardRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_dashboard(**kwargs)
```

1. See [:material-code-braces: GetDashboardRequestTypeDef](./type_defs.md#getdashboardrequesttypedef)

### get\_resource\_policy

Retrieves the resource-based policy attached to a dashboard, showing sharing
configurations and permissions.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/get_resource_policy.html)

```python
# get_resource_policy method definition

await def get_resource_policy(
    self,
    *,
    resourceArn: str,
) -> GetResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourcePolicyResponseTypeDef](./type_defs.md#getresourcepolicyresponsetypedef)


```python
# get_resource_policy method usage example with argument unpacking

kwargs: GetResourcePolicyRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyRequestTypeDef](./type_defs.md#getresourcepolicyrequesttypedef)

### list\_dashboards

Returns a list of all dashboards in your account.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").list_dashboards` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/list_dashboards.html)

```python
# list_dashboards method definition

await def list_dashboards(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDashboardsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDashboardsResponseTypeDef](./type_defs.md#listdashboardsresponsetypedef)


```python
# list_dashboards method usage example with argument unpacking

kwargs: ListDashboardsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_dashboards(**kwargs)
```

1. See [:material-code-braces: ListDashboardsRequestTypeDef](./type_defs.md#listdashboardsrequesttypedef)

### list\_tags\_for\_resource

Returns a list of all tags associated with a specified dashboard resource.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)

### tag\_resource

Adds or updates tags for a specified dashboard resource.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    resourceTags: Sequence[ResourceTagTypeDef],  # (1)
) -> dict[str, Any]:
    ...
```

1. See `Sequence[ResourceTagTypeDef]`


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "resourceTags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Removes specified tags from a dashboard resource.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    resourceTagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "resourceTagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_dashboard

Updates an existing dashboard's properties, including its name, description,
and widget configurations.

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").update_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards/client/update_dashboard.html)

```python
# update_dashboard method definition

await def update_dashboard(
    self,
    *,
    arn: str,
    name: str = ...,
    description: str = ...,
    widgets: Sequence[WidgetUnionTypeDef] = ...,  # (1)
) -> UpdateDashboardResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[WidgetUnionTypeDef]`
2. See [:material-code-braces: UpdateDashboardResponseTypeDef](./type_defs.md#updatedashboardresponsetypedef)


```python
# update_dashboard method usage example with argument unpacking

kwargs: UpdateDashboardRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_dashboard(**kwargs)
```

1. See [:material-code-braces: UpdateDashboardRequestTypeDef](./type_defs.md#updatedashboardrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bcm-dashboards").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards.html#BillingandCostManagementDashboards.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bcm-dashboards").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards.html#BillingandCostManagementDashboards.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("bcm-dashboards").get_paginator` method with overloads.

- `client.get_paginator("list_dashboards")` -> [ListDashboardsPaginator](./paginators.md#listdashboardspaginator)



