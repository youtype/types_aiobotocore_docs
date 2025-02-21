# CloudFrontKeyValueStoreClient

> [Index](../README.md) > [CloudFrontKeyValueStore](./README.md) > CloudFrontKeyValueStoreClient

!!! note ""

    Auto-generated documentation for [CloudFrontKeyValueStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#cloudfrontkeyvaluestore)
    type annotations stubs module [types-aiobotocore-cloudfront-keyvaluestore](https://pypi.org/project/types-aiobotocore-cloudfront-keyvaluestore/).

## CloudFrontKeyValueStoreClient

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore.Client)

```python
# CloudFrontKeyValueStoreClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cloudfront_keyvaluestore.client import CloudFrontKeyValueStoreClient

session = get_session()
async with session.create_client("cloudfront-keyvaluestore") as client:
    client: CloudFrontKeyValueStoreClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudfront-keyvaluestore").exceptions` structure.

```python
# CloudFrontKeyValueStoreClient.exceptions usage example

async with session.create_client("cloudfront-keyvaluestore") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# CloudFrontKeyValueStoreClient usage type checking example

from types_aiobotocore_cloudfront_keyvaluestore.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/generate_presigned_url.html)

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


### delete\_key

Deletes the key value pair specified by the key.

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").delete_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/delete_key.html)

```python
# delete_key method definition

await def delete_key(
    self,
    *,
    KvsARN: str,
    Key: str,
    IfMatch: str,
) -> DeleteKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteKeyResponseTypeDef](./type_defs.md#deletekeyresponsetypedef) 


```python
# delete_key method usage example with argument unpacking

kwargs: DeleteKeyRequestTypeDef = {  # (1)
    "KvsARN": ...,
    "Key": ...,
    "IfMatch": ...,
}

parent.delete_key(**kwargs)
```

1. See [:material-code-braces: DeleteKeyRequestTypeDef](./type_defs.md#deletekeyrequesttypedef) 

### describe\_key\_value\_store

Returns metadata information about Key Value Store.

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").describe_key_value_store` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/describe_key_value_store.html)

```python
# describe_key_value_store method definition

await def describe_key_value_store(
    self,
    *,
    KvsARN: str,
) -> DescribeKeyValueStoreResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeKeyValueStoreResponseTypeDef](./type_defs.md#describekeyvaluestoreresponsetypedef) 


```python
# describe_key_value_store method usage example with argument unpacking

kwargs: DescribeKeyValueStoreRequestTypeDef = {  # (1)
    "KvsARN": ...,
}

parent.describe_key_value_store(**kwargs)
```

1. See [:material-code-braces: DescribeKeyValueStoreRequestTypeDef](./type_defs.md#describekeyvaluestorerequesttypedef) 

### get\_key

Returns a key value pair.

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").get_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/get_key.html)

```python
# get_key method definition

await def get_key(
    self,
    *,
    KvsARN: str,
    Key: str,
) -> GetKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetKeyResponseTypeDef](./type_defs.md#getkeyresponsetypedef) 


```python
# get_key method usage example with argument unpacking

kwargs: GetKeyRequestTypeDef = {  # (1)
    "KvsARN": ...,
    "Key": ...,
}

parent.get_key(**kwargs)
```

1. See [:material-code-braces: GetKeyRequestTypeDef](./type_defs.md#getkeyrequesttypedef) 

### list\_keys

Returns a list of key value pairs.

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").list_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/list_keys.html)

```python
# list_keys method definition

await def list_keys(
    self,
    *,
    KvsARN: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListKeysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListKeysResponseTypeDef](./type_defs.md#listkeysresponsetypedef) 


```python
# list_keys method usage example with argument unpacking

kwargs: ListKeysRequestTypeDef = {  # (1)
    "KvsARN": ...,
}

parent.list_keys(**kwargs)
```

1. See [:material-code-braces: ListKeysRequestTypeDef](./type_defs.md#listkeysrequesttypedef) 

### put\_key

Creates a new key value pair or replaces the value of an existing key.

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").put_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/put_key.html)

```python
# put_key method definition

await def put_key(
    self,
    *,
    Key: str,
    Value: str,
    KvsARN: str,
    IfMatch: str,
) -> PutKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutKeyResponseTypeDef](./type_defs.md#putkeyresponsetypedef) 


```python
# put_key method usage example with argument unpacking

kwargs: PutKeyRequestTypeDef = {  # (1)
    "Key": ...,
    "Value": ...,
    "KvsARN": ...,
    "IfMatch": ...,
}

parent.put_key(**kwargs)
```

1. See [:material-code-braces: PutKeyRequestTypeDef](./type_defs.md#putkeyrequesttypedef) 

### update\_keys

Puts or Deletes multiple key value pairs in a single, all-or-nothing operation.

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").update_keys` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore/client/update_keys.html)

```python
# update_keys method definition

await def update_keys(
    self,
    *,
    KvsARN: str,
    IfMatch: str,
    Puts: Sequence[PutKeyRequestListItemTypeDef] = ...,  # (1)
    Deletes: Sequence[DeleteKeyRequestListItemTypeDef] = ...,  # (2)
) -> UpdateKeysResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PutKeyRequestListItemTypeDef](./type_defs.md#putkeyrequestlistitemtypedef) 
2. See [:material-code-braces: DeleteKeyRequestListItemTypeDef](./type_defs.md#deletekeyrequestlistitemtypedef) 
3. See [:material-code-braces: UpdateKeysResponseTypeDef](./type_defs.md#updatekeysresponsetypedef) 


```python
# update_keys method usage example with argument unpacking

kwargs: UpdateKeysRequestTypeDef = {  # (1)
    "KvsARN": ...,
    "IfMatch": ...,
}

parent.update_keys(**kwargs)
```

1. See [:material-code-braces: UpdateKeysRequestTypeDef](./type_defs.md#updatekeysrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#CloudFrontKeyValueStore.Client)

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

Type annotations and code completion for `#!python session.create_client("cloudfront-keyvaluestore").get_paginator` method with overloads.

- `client.get_paginator("list_keys")` -> [ListKeysPaginator](./paginators.md#listkeyspaginator)



