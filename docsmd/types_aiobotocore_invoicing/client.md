# InvoicingClient

> [Index](../README.md) > [Invoicing](./README.md) > InvoicingClient

!!! note ""

    Auto-generated documentation for [Invoicing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#invoicing)
    type annotations stubs module [types-aiobotocore-invoicing](https://pypi.org/project/types-aiobotocore-invoicing/).

## InvoicingClient

Type annotations and code completion for `#!python session.create_client("invoicing")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#Invoicing.Client)

```python
# InvoicingClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_invoicing.client import InvoicingClient

session = get_session()
async with session.create_client("invoicing") as client:
    client: InvoicingClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("invoicing").exceptions` structure.

```python
# InvoicingClient.exceptions usage example

async with session.create_client("invoicing") as client:
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
# InvoicingClient usage type checking example

from types_aiobotocore_invoicing.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("invoicing").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("invoicing").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/generate_presigned_url.html)

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


### batch\_get\_invoice\_profile

This gets the invoice profile associated with a set of accounts.

Type annotations and code completion for `#!python session.create_client("invoicing").batch_get_invoice_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/batch_get_invoice_profile.html)

```python
# batch_get_invoice_profile method definition

await def batch_get_invoice_profile(
    self,
    *,
    AccountIds: Sequence[str],
) -> BatchGetInvoiceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetInvoiceProfileResponseTypeDef](./type_defs.md#batchgetinvoiceprofileresponsetypedef) 


```python
# batch_get_invoice_profile method usage example with argument unpacking

kwargs: BatchGetInvoiceProfileRequestRequestTypeDef = {  # (1)
    "AccountIds": ...,
}

parent.batch_get_invoice_profile(**kwargs)
```

1. See [:material-code-braces: BatchGetInvoiceProfileRequestRequestTypeDef](./type_defs.md#batchgetinvoiceprofilerequestrequesttypedef) 

### create\_invoice\_unit

This creates a new invoice unit with the provided definition.

Type annotations and code completion for `#!python session.create_client("invoicing").create_invoice_unit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/create_invoice_unit.html)

```python
# create_invoice_unit method definition

await def create_invoice_unit(
    self,
    *,
    Name: str,
    InvoiceReceiver: str,
    Rule: InvoiceUnitRuleTypeDef,  # (1)
    Description: str = ...,
    TaxInheritanceDisabled: bool = ...,
    ResourceTags: Sequence[ResourceTagTypeDef] = ...,  # (2)
) -> CreateInvoiceUnitResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InvoiceUnitRuleTypeDef](./type_defs.md#invoiceunitruletypedef) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-braces: CreateInvoiceUnitResponseTypeDef](./type_defs.md#createinvoiceunitresponsetypedef) 


```python
# create_invoice_unit method usage example with argument unpacking

kwargs: CreateInvoiceUnitRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "InvoiceReceiver": ...,
    "Rule": ...,
}

parent.create_invoice_unit(**kwargs)
```

1. See [:material-code-braces: CreateInvoiceUnitRequestRequestTypeDef](./type_defs.md#createinvoiceunitrequestrequesttypedef) 

### delete\_invoice\_unit

This deletes an invoice unit with the provided invoice unit ARN.

Type annotations and code completion for `#!python session.create_client("invoicing").delete_invoice_unit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/delete_invoice_unit.html)

```python
# delete_invoice_unit method definition

await def delete_invoice_unit(
    self,
    *,
    InvoiceUnitArn: str,
) -> DeleteInvoiceUnitResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInvoiceUnitResponseTypeDef](./type_defs.md#deleteinvoiceunitresponsetypedef) 


```python
# delete_invoice_unit method usage example with argument unpacking

kwargs: DeleteInvoiceUnitRequestRequestTypeDef = {  # (1)
    "InvoiceUnitArn": ...,
}

parent.delete_invoice_unit(**kwargs)
```

1. See [:material-code-braces: DeleteInvoiceUnitRequestRequestTypeDef](./type_defs.md#deleteinvoiceunitrequestrequesttypedef) 

### get\_invoice\_unit

This retrieves the invoice unit definition.

Type annotations and code completion for `#!python session.create_client("invoicing").get_invoice_unit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/get_invoice_unit.html)

```python
# get_invoice_unit method definition

await def get_invoice_unit(
    self,
    *,
    InvoiceUnitArn: str,
    AsOf: TimestampTypeDef = ...,
) -> GetInvoiceUnitResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetInvoiceUnitResponseTypeDef](./type_defs.md#getinvoiceunitresponsetypedef) 


```python
# get_invoice_unit method usage example with argument unpacking

kwargs: GetInvoiceUnitRequestRequestTypeDef = {  # (1)
    "InvoiceUnitArn": ...,
}

parent.get_invoice_unit(**kwargs)
```

1. See [:material-code-braces: GetInvoiceUnitRequestRequestTypeDef](./type_defs.md#getinvoiceunitrequestrequesttypedef) 

### list\_invoice\_units

This fetches a list of all invoice unit definitions for a given account, as of
the provided <code>AsOf</code> date.

Type annotations and code completion for `#!python session.create_client("invoicing").list_invoice_units` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/list_invoice_units.html)

```python
# list_invoice_units method definition

await def list_invoice_units(
    self,
    *,
    Filters: FiltersTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
    AsOf: TimestampTypeDef = ...,
) -> ListInvoiceUnitsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FiltersTypeDef](./type_defs.md#filterstypedef) 
2. See [:material-code-braces: ListInvoiceUnitsResponseTypeDef](./type_defs.md#listinvoiceunitsresponsetypedef) 


```python
# list_invoice_units method usage example with argument unpacking

kwargs: ListInvoiceUnitsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_invoice_units(**kwargs)
```

1. See [:material-code-braces: ListInvoiceUnitsRequestRequestTypeDef](./type_defs.md#listinvoiceunitsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for a resource.

Type annotations and code completion for `#!python session.create_client("invoicing").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
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

Adds a tag to a resource.

Type annotations and code completion for `#!python session.create_client("invoicing").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/tag_resource.html)

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

Removes a tag from a resource.

Type annotations and code completion for `#!python session.create_client("invoicing").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/untag_resource.html)

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

### update\_invoice\_unit

You can update the invoice unit configuration at any time, and Amazon Web
Services will use the latest configuration at the end of the month.

Type annotations and code completion for `#!python session.create_client("invoicing").update_invoice_unit` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing/client/update_invoice_unit.html)

```python
# update_invoice_unit method definition

await def update_invoice_unit(
    self,
    *,
    InvoiceUnitArn: str,
    Description: str = ...,
    TaxInheritanceDisabled: bool = ...,
    Rule: InvoiceUnitRuleTypeDef = ...,  # (1)
) -> UpdateInvoiceUnitResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InvoiceUnitRuleTypeDef](./type_defs.md#invoiceunitruletypedef) 
2. See [:material-code-braces: UpdateInvoiceUnitResponseTypeDef](./type_defs.md#updateinvoiceunitresponsetypedef) 


```python
# update_invoice_unit method usage example with argument unpacking

kwargs: UpdateInvoiceUnitRequestRequestTypeDef = {  # (1)
    "InvoiceUnitArn": ...,
}

parent.update_invoice_unit(**kwargs)
```

1. See [:material-code-braces: UpdateInvoiceUnitRequestRequestTypeDef](./type_defs.md#updateinvoiceunitrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("invoicing").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#Invoicing.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("invoicing").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#Invoicing.Client)

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

Type annotations and code completion for `#!python session.create_client("invoicing").get_paginator` method with overloads.

- `client.get_paginator("list_invoice_units")` -> [ListInvoiceUnitsPaginator](./paginators.md#listinvoiceunitspaginator)



