# ElementalInferenceClient

> [Index](../README.md) > [ElementalInference](./README.md) > ElementalInferenceClient

!!! note ""

    Auto-generated documentation for [ElementalInference](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#elementalinference)
    type annotations stubs module [types-aiobotocore-elementalinference](https://pypi.org/project/types-aiobotocore-elementalinference/).

## ElementalInferenceClient

Type annotations and code completion for `#!python session.create_client("elementalinference")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#ElementalInference.Client)

```python
# ElementalInferenceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_elementalinference.client import ElementalInferenceClient

session = get_session()
async with session.create_client("elementalinference") as client:
    client: ElementalInferenceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("elementalinference").exceptions` structure.

```python
# ElementalInferenceClient.exceptions usage example

async with session.create_client("elementalinference") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerErrorException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.TooManyRequestException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# ElementalInferenceClient usage type checking example

from types_aiobotocore_elementalinference.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("elementalinference").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("elementalinference").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/generate_presigned_url.html)

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


### associate\_feed

Associates a resource with the feed.

Type annotations and code completion for `#!python session.create_client("elementalinference").associate_feed` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/associate_feed.html)

```python
# associate_feed method definition

await def associate_feed(
    self,
    *,
    id: str,
    associatedResourceName: str,
    outputs: Sequence[CreateOutputTypeDef],  # (1)
    dryRun: bool = ...,
) -> AssociateFeedResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[CreateOutputTypeDef]`
2. See [:material-code-braces: AssociateFeedResponseTypeDef](./type_defs.md#associatefeedresponsetypedef)


```python
# associate_feed method usage example with argument unpacking

kwargs: AssociateFeedRequestTypeDef = {  # (1)
    "id": ...,
    "associatedResourceName": ...,
    "outputs": ...,
}

parent.associate_feed(**kwargs)
```

1. See [:material-code-braces: AssociateFeedRequestTypeDef](./type_defs.md#associatefeedrequesttypedef)

### create\_feed

Creates a feed.

Type annotations and code completion for `#!python session.create_client("elementalinference").create_feed` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/create_feed.html)

```python
# create_feed method definition

await def create_feed(
    self,
    *,
    name: str,
    outputs: Sequence[CreateOutputTypeDef],  # (1)
    tags: Mapping[str, str] = ...,
) -> CreateFeedResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[CreateOutputTypeDef]`
2. See [:material-code-braces: CreateFeedResponseTypeDef](./type_defs.md#createfeedresponsetypedef)


```python
# create_feed method usage example with argument unpacking

kwargs: CreateFeedRequestTypeDef = {  # (1)
    "name": ...,
    "outputs": ...,
}

parent.create_feed(**kwargs)
```

1. See [:material-code-braces: CreateFeedRequestTypeDef](./type_defs.md#createfeedrequesttypedef)

### delete\_feed

Deletes the specified feed.

Type annotations and code completion for `#!python session.create_client("elementalinference").delete_feed` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/delete_feed.html)

```python
# delete_feed method definition

await def delete_feed(
    self,
    *,
    id: str,
) -> DeleteFeedResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFeedResponseTypeDef](./type_defs.md#deletefeedresponsetypedef)


```python
# delete_feed method usage example with argument unpacking

kwargs: DeleteFeedRequestTypeDef = {  # (1)
    "id": ...,
}

parent.delete_feed(**kwargs)
```

1. See [:material-code-braces: DeleteFeedRequestTypeDef](./type_defs.md#deletefeedrequesttypedef)

### disassociate\_feed

Releases the resource (for example, an MediaLive channel) that is associated
with this feed.

Type annotations and code completion for `#!python session.create_client("elementalinference").disassociate_feed` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/disassociate_feed.html)

```python
# disassociate_feed method definition

await def disassociate_feed(
    self,
    *,
    id: str,
    associatedResourceName: str,
    dryRun: bool = ...,
) -> DisassociateFeedResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateFeedResponseTypeDef](./type_defs.md#disassociatefeedresponsetypedef)


```python
# disassociate_feed method usage example with argument unpacking

kwargs: DisassociateFeedRequestTypeDef = {  # (1)
    "id": ...,
    "associatedResourceName": ...,
}

parent.disassociate_feed(**kwargs)
```

1. See [:material-code-braces: DisassociateFeedRequestTypeDef](./type_defs.md#disassociatefeedrequesttypedef)

### get\_feed

Retrieves information about the specified feed.

Type annotations and code completion for `#!python session.create_client("elementalinference").get_feed` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/get_feed.html)

```python
# get_feed method definition

await def get_feed(
    self,
    *,
    id: str,
) -> GetFeedResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFeedResponseTypeDef](./type_defs.md#getfeedresponsetypedef)


```python
# get_feed method usage example with argument unpacking

kwargs: GetFeedRequestTypeDef = {  # (1)
    "id": ...,
}

parent.get_feed(**kwargs)
```

1. See [:material-code-braces: GetFeedRequestTypeDef](./type_defs.md#getfeedrequesttypedef)

### list\_feeds

Displays a list of feeds that belong to this AWS account.

Type annotations and code completion for `#!python session.create_client("elementalinference").list_feeds` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/list_feeds.html)

```python
# list_feeds method definition

await def list_feeds(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFeedsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFeedsResponseTypeDef](./type_defs.md#listfeedsresponsetypedef)


```python
# list_feeds method usage example with argument unpacking

kwargs: ListFeedsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_feeds(**kwargs)
```

1. See [:material-code-braces: ListFeedsRequestTypeDef](./type_defs.md#listfeedsrequesttypedef)

### list\_tags\_for\_resource

List all tags that are on an Elemental Inference resource in the current region.

Type annotations and code completion for `#!python session.create_client("elementalinference").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/list_tags_for_resource.html)

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

Associates the specified tags to the resource identified by the specified
resourceArn in the current region.

Type annotations and code completion for `#!python session.create_client("elementalinference").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)

### untag\_resource

Deletes specified tags from the specified resource in the current region.

Type annotations and code completion for `#!python session.create_client("elementalinference").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)


```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_feed

Updates the name and/or outputs in a feed.

Type annotations and code completion for `#!python session.create_client("elementalinference").update_feed` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference/client/update_feed.html)

```python
# update_feed method definition

await def update_feed(
    self,
    *,
    name: str,
    id: str,
    outputs: Sequence[UpdateOutputTypeDef],  # (1)
) -> UpdateFeedResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[UpdateOutputTypeDef]`
2. See [:material-code-braces: UpdateFeedResponseTypeDef](./type_defs.md#updatefeedresponsetypedef)


```python
# update_feed method usage example with argument unpacking

kwargs: UpdateFeedRequestTypeDef = {  # (1)
    "name": ...,
    "id": ...,
    "outputs": ...,
}

parent.update_feed(**kwargs)
```

1. See [:material-code-braces: UpdateFeedRequestTypeDef](./type_defs.md#updatefeedrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("elementalinference").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#ElementalInference.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("elementalinference").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elementalinference.html#ElementalInference.Client)

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

Type annotations and code completion for `#!python session.create_client("elementalinference").get_paginator` method with overloads.

- `client.get_paginator("list_feeds")` -> [ListFeedsPaginator](./paginators.md#listfeedspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("elementalinference").get_waiter` method with overloads.

- `client.get_waiter("feed_deleted")` -> [FeedDeletedWaiter](./waiters.md#feeddeletedwaiter)

