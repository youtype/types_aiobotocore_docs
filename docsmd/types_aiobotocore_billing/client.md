# BillingClient

> [Index](../README.md) > [Billing](./README.md) > BillingClient

!!! note ""

    Auto-generated documentation for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing)
    type annotations stubs module [types-aiobotocore-billing](https://pypi.org/project/types-aiobotocore-billing/).

## BillingClient

Type annotations and code completion for `#!python session.create_client("billing")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# BillingClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_billing.client import BillingClient

session = get_session()
async with session.create_client("billing") as client:
    client: BillingClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("billing").exceptions` structure.

```python
# BillingClient.exceptions usage example

async with session.create_client("billing") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# BillingClient usage type checking example

from types_aiobotocore_billing.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("billing").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("billing").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/generate_presigned_url.html)

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


### create\_billing\_view

Creates a billing view with the specified billing view attributes.

Type annotations and code completion for `#!python session.create_client("billing").create_billing_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/create_billing_view.html)

```python
# create_billing_view method definition

await def create_billing_view(
    self,
    *,
    name: str,
    sourceViews: Sequence[str],
    description: str = ...,
    dataFilterExpression: ExpressionUnionTypeDef = ...,  # (1)
    clientToken: str = ...,
    resourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
) -> CreateBillingViewResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-braces: CreateBillingViewResponseTypeDef](./type_defs.md#createbillingviewresponsetypedef) 


```python
# create_billing_view method usage example with argument unpacking

kwargs: CreateBillingViewRequestTypeDef = {  # (1)
    "name": ...,
    "sourceViews": ...,
}

parent.create_billing_view(**kwargs)
```

1. See [:material-code-braces: CreateBillingViewRequestTypeDef](./type_defs.md#createbillingviewrequesttypedef) 

### delete\_billing\_view

Deletes the specified billing view.

Type annotations and code completion for `#!python session.create_client("billing").delete_billing_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/delete_billing_view.html)

```python
# delete_billing_view method definition

await def delete_billing_view(
    self,
    *,
    arn: str,
) -> DeleteBillingViewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteBillingViewResponseTypeDef](./type_defs.md#deletebillingviewresponsetypedef) 


```python
# delete_billing_view method usage example with argument unpacking

kwargs: DeleteBillingViewRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_billing_view(**kwargs)
```

1. See [:material-code-braces: DeleteBillingViewRequestTypeDef](./type_defs.md#deletebillingviewrequesttypedef) 

### get\_billing\_view

Returns the metadata associated to the specified billing view ARN.

Type annotations and code completion for `#!python session.create_client("billing").get_billing_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/get_billing_view.html)

```python
# get_billing_view method definition

await def get_billing_view(
    self,
    *,
    arn: str,
) -> GetBillingViewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBillingViewResponseTypeDef](./type_defs.md#getbillingviewresponsetypedef) 


```python
# get_billing_view method usage example with argument unpacking

kwargs: GetBillingViewRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.get_billing_view(**kwargs)
```

1. See [:material-code-braces: GetBillingViewRequestTypeDef](./type_defs.md#getbillingviewrequesttypedef) 

### get\_resource\_policy

Returns the resource-based policy document attached to the resource in
<code>JSON</code> format.

Type annotations and code completion for `#!python session.create_client("billing").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/get_resource_policy.html)

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

### list\_billing\_views

Lists the billing views available for a given time period.

Type annotations and code completion for `#!python session.create_client("billing").list_billing_views` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/list_billing_views.html)

```python
# list_billing_views method definition

await def list_billing_views(
    self,
    *,
    activeTimeRange: ActiveTimeRangeTypeDef = ...,  # (1)
    arns: Sequence[str] = ...,
    billingViewTypes: Sequence[BillingViewTypeType] = ...,  # (2)
    ownerAccountId: str = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListBillingViewsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ActiveTimeRangeTypeDef](./type_defs.md#activetimerangetypedef) 
2. See [:material-code-brackets: BillingViewTypeType](./literals.md#billingviewtypetype) 
3. See [:material-code-braces: ListBillingViewsResponseTypeDef](./type_defs.md#listbillingviewsresponsetypedef) 


```python
# list_billing_views method usage example with argument unpacking

kwargs: ListBillingViewsRequestTypeDef = {  # (1)
    "activeTimeRange": ...,
}

parent.list_billing_views(**kwargs)
```

1. See [:material-code-braces: ListBillingViewsRequestTypeDef](./type_defs.md#listbillingviewsrequesttypedef) 

### list\_source\_views\_for\_billing\_view

Lists the source views (managed Amazon Web Services billing views) associated
with the billing view.

Type annotations and code completion for `#!python session.create_client("billing").list_source_views_for_billing_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/list_source_views_for_billing_view.html)

```python
# list_source_views_for_billing_view method definition

await def list_source_views_for_billing_view(
    self,
    *,
    arn: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSourceViewsForBillingViewResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSourceViewsForBillingViewResponseTypeDef](./type_defs.md#listsourceviewsforbillingviewresponsetypedef) 


```python
# list_source_views_for_billing_view method usage example with argument unpacking

kwargs: ListSourceViewsForBillingViewRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.list_source_views_for_billing_view(**kwargs)
```

1. See [:material-code-braces: ListSourceViewsForBillingViewRequestTypeDef](./type_defs.md#listsourceviewsforbillingviewrequesttypedef) 

### list\_tags\_for\_resource

Lists tags associated with the billing view resource.

Type annotations and code completion for `#!python session.create_client("billing").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/list_tags_for_resource.html)

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

An API operation for adding one or more tags (key-value pairs) to a resource.

Type annotations and code completion for `#!python session.create_client("billing").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    resourceTags: Sequence[ResourceTagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 


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

Removes one or more tags from a resource.

Type annotations and code completion for `#!python session.create_client("billing").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    resourceTagKeys: Sequence[str],
) -> Dict[str, Any]:
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

### update\_billing\_view

An API to update the attributes of the billing view.

Type annotations and code completion for `#!python session.create_client("billing").update_billing_view` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing/client/update_billing_view.html)

```python
# update_billing_view method definition

await def update_billing_view(
    self,
    *,
    arn: str,
    name: str = ...,
    description: str = ...,
    dataFilterExpression: ExpressionUnionTypeDef = ...,  # (1)
) -> UpdateBillingViewResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExpressionTypeDef](./type_defs.md#expressiontypedef) [:material-code-braces: ExpressionOutputTypeDef](./type_defs.md#expressionoutputtypedef) 
2. See [:material-code-braces: UpdateBillingViewResponseTypeDef](./type_defs.md#updatebillingviewresponsetypedef) 


```python
# update_billing_view method usage example with argument unpacking

kwargs: UpdateBillingViewRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.update_billing_view(**kwargs)
```

1. See [:material-code-braces: UpdateBillingViewRequestTypeDef](./type_defs.md#updatebillingviewrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("billing").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("billing").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#Billing.Client)

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

Type annotations and code completion for `#!python session.create_client("billing").get_paginator` method with overloads.

- `client.get_paginator("list_billing_views")` -> [ListBillingViewsPaginator](./paginators.md#listbillingviewspaginator)
- `client.get_paginator("list_source_views_for_billing_view")` -> [ListSourceViewsForBillingViewPaginator](./paginators.md#listsourceviewsforbillingviewpaginator)



