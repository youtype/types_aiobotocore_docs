# SimpleDBClient

> [Index](../README.md) > [SimpleDB](./README.md) > SimpleDBClient

!!! note ""

    Auto-generated documentation for [SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#simpledb)
    type annotations stubs module [types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).

## SimpleDBClient

Type annotations and code completion for `#!python session.create_client("sdb")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client)

```python
# SimpleDBClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sdb.client import SimpleDBClient

session = get_session()
async with session.create_client("sdb") as client:
    client: SimpleDBClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sdb").exceptions` structure.

```python
# SimpleDBClient.exceptions usage example

async with session.create_client("sdb") as client:
    try:
        do_something(client)
    except (
            client.AttributeDoesNotExist,
        client.ClientError,
        client.DuplicateItemName,
        client.InvalidNextToken,
        client.InvalidNumberPredicates,
        client.InvalidNumberValueTests,
        client.InvalidParameterValue,
        client.InvalidQueryExpression,
        client.MissingParameter,
        client.NoSuchDomain,
        client.NumberDomainAttributesExceeded,
        client.NumberDomainBytesExceeded,
        client.NumberDomainsExceeded,
        client.NumberItemAttributesExceeded,
        client.NumberSubmittedAttributesExceeded,
        client.NumberSubmittedItemsExceeded,
        client.RequestTimeout,
        client.TooManyRequestedAttributes,
    ) as e:
        print(e)
```

```python
# SimpleDBClient usage type checking example

from types_aiobotocore_sdb.client import Exceptions

def handle_error(exc: Exceptions.AttributeDoesNotExist) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("sdb").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("sdb").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/generate_presigned_url.html)

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


### batch\_delete\_attributes

Performs multiple DeleteAttributes operations in a single call, which reduces
round trips and latencies.

Type annotations and code completion for `#!python session.create_client("sdb").batch_delete_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/batch_delete_attributes.html)

```python
# batch_delete_attributes method definition

await def batch_delete_attributes(
    self,
    *,
    DomainName: str,
    Items: Sequence[DeletableItemTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DeletableItemTypeDef](./type_defs.md#deletableitemtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# batch_delete_attributes method usage example with argument unpacking

kwargs: BatchDeleteAttributesRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Items": ...,
}

parent.batch_delete_attributes(**kwargs)
```

1. See [:material-code-braces: BatchDeleteAttributesRequestTypeDef](./type_defs.md#batchdeleteattributesrequesttypedef) 

### batch\_put\_attributes

The <code>BatchPutAttributes</code> operation creates or replaces attributes
within one or more items.

Type annotations and code completion for `#!python session.create_client("sdb").batch_put_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/batch_put_attributes.html)

```python
# batch_put_attributes method definition

await def batch_put_attributes(
    self,
    *,
    DomainName: str,
    Items: Sequence[ReplaceableItemTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ReplaceableItemTypeDef](./type_defs.md#replaceableitemtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# batch_put_attributes method usage example with argument unpacking

kwargs: BatchPutAttributesRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Items": ...,
}

parent.batch_put_attributes(**kwargs)
```

1. See [:material-code-braces: BatchPutAttributesRequestTypeDef](./type_defs.md#batchputattributesrequesttypedef) 

### create\_domain

The <code>CreateDomain</code> operation creates a new domain.

Type annotations and code completion for `#!python session.create_client("sdb").create_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/create_domain.html)

```python
# create_domain method definition

await def create_domain(
    self,
    *,
    DomainName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_domain method usage example with argument unpacking

kwargs: CreateDomainRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.create_domain(**kwargs)
```

1. See [:material-code-braces: CreateDomainRequestTypeDef](./type_defs.md#createdomainrequesttypedef) 

### delete\_attributes

Deletes one or more attributes associated with an item.

Type annotations and code completion for `#!python session.create_client("sdb").delete_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/delete_attributes.html)

```python
# delete_attributes method definition

await def delete_attributes(
    self,
    *,
    DomainName: str,
    ItemName: str,
    Attributes: Sequence[AttributeTypeDef] = ...,  # (1)
    Expected: UpdateConditionTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: UpdateConditionTypeDef](./type_defs.md#updateconditiontypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_attributes method usage example with argument unpacking

kwargs: DeleteAttributesRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ItemName": ...,
}

parent.delete_attributes(**kwargs)
```

1. See [:material-code-braces: DeleteAttributesRequestTypeDef](./type_defs.md#deleteattributesrequesttypedef) 

### delete\_domain

The <code>DeleteDomain</code> operation deletes a domain.

Type annotations and code completion for `#!python session.create_client("sdb").delete_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/delete_domain.html)

```python
# delete_domain method definition

await def delete_domain(
    self,
    *,
    DomainName: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_domain method usage example with argument unpacking

kwargs: DeleteDomainRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.delete_domain(**kwargs)
```

1. See [:material-code-braces: DeleteDomainRequestTypeDef](./type_defs.md#deletedomainrequesttypedef) 

### domain\_metadata

Returns information about the domain, including when the domain was created,
the number of items and attributes in the domain, and the size of the attribute
names and values.

Type annotations and code completion for `#!python session.create_client("sdb").domain_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/domain_metadata.html)

```python
# domain_metadata method definition

await def domain_metadata(
    self,
    *,
    DomainName: str,
) -> DomainMetadataResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DomainMetadataResultTypeDef](./type_defs.md#domainmetadataresulttypedef) 


```python
# domain_metadata method usage example with argument unpacking

kwargs: DomainMetadataRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.domain_metadata(**kwargs)
```

1. See [:material-code-braces: DomainMetadataRequestTypeDef](./type_defs.md#domainmetadatarequesttypedef) 

### get\_attributes

Returns all of the attributes associated with the specified item.

Type annotations and code completion for `#!python session.create_client("sdb").get_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/get_attributes.html)

```python
# get_attributes method definition

await def get_attributes(
    self,
    *,
    DomainName: str,
    ItemName: str,
    AttributeNames: Sequence[str] = ...,
    ConsistentRead: bool = ...,
) -> GetAttributesResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAttributesResultTypeDef](./type_defs.md#getattributesresulttypedef) 


```python
# get_attributes method usage example with argument unpacking

kwargs: GetAttributesRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ItemName": ...,
}

parent.get_attributes(**kwargs)
```

1. See [:material-code-braces: GetAttributesRequestTypeDef](./type_defs.md#getattributesrequesttypedef) 

### list\_domains

The <code>ListDomains</code> operation lists all domains associated with the
Access Key ID.

Type annotations and code completion for `#!python session.create_client("sdb").list_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/list_domains.html)

```python
# list_domains method definition

await def list_domains(
    self,
    *,
    MaxNumberOfDomains: int = ...,
    NextToken: str = ...,
) -> ListDomainsResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef) 


```python
# list_domains method usage example with argument unpacking

kwargs: ListDomainsRequestTypeDef = {  # (1)
    "MaxNumberOfDomains": ...,
}

parent.list_domains(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestTypeDef](./type_defs.md#listdomainsrequesttypedef) 

### put\_attributes

The PutAttributes operation creates or replaces attributes in an item.

Type annotations and code completion for `#!python session.create_client("sdb").put_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/put_attributes.html)

```python
# put_attributes method definition

await def put_attributes(
    self,
    *,
    DomainName: str,
    ItemName: str,
    Attributes: Sequence[ReplaceableAttributeTypeDef],  # (1)
    Expected: UpdateConditionTypeDef = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ReplaceableAttributeTypeDef](./type_defs.md#replaceableattributetypedef) 
2. See [:material-code-braces: UpdateConditionTypeDef](./type_defs.md#updateconditiontypedef) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# put_attributes method usage example with argument unpacking

kwargs: PutAttributesRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ItemName": ...,
    "Attributes": ...,
}

parent.put_attributes(**kwargs)
```

1. See [:material-code-braces: PutAttributesRequestTypeDef](./type_defs.md#putattributesrequesttypedef) 

### select

The <code>Select</code> operation returns a set of attributes for
<code>ItemNames</code> that match the select expression.

Type annotations and code completion for `#!python session.create_client("sdb").select` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb/client/select.html)

```python
# select method definition

await def select(
    self,
    *,
    SelectExpression: str,
    NextToken: str = ...,
    ConsistentRead: bool = ...,
) -> SelectResultTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SelectResultTypeDef](./type_defs.md#selectresulttypedef) 


```python
# select method usage example with argument unpacking

kwargs: SelectRequestTypeDef = {  # (1)
    "SelectExpression": ...,
}

parent.select(**kwargs)
```

1. See [:material-code-braces: SelectRequestTypeDef](./type_defs.md#selectrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sdb").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sdb").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client)

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

Type annotations and code completion for `#!python session.create_client("sdb").get_paginator` method with overloads.

- `client.get_paginator("list_domains")` -> [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- `client.get_paginator("select")` -> [SelectPaginator](./paginators.md#selectpaginator)



