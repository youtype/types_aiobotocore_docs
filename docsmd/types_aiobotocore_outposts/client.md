# OutpostsClient

> [Index](../README.md) > [Outposts](./README.md) > OutpostsClient

!!! note ""

    Auto-generated documentation for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts)
    type annotations stubs module [types-aiobotocore-outposts](https://pypi.org/project/types-aiobotocore-outposts/).

## OutpostsClient

Type annotations and code completion for `#!python session.create_client("outposts")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client)

```python
# OutpostsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_outposts.client import OutpostsClient

session = get_session()
async with session.create_client("outposts") as client:
    client: OutpostsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("outposts").exceptions` structure.

```python
# OutpostsClient.exceptions usage example

async with session.create_client("outposts") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.NotFoundException,
        client.ServiceQuotaExceededException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# OutpostsClient usage type checking example

from types_aiobotocore_outposts.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("outposts").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_capacity\_task

Cancels the capacity task.

Type annotations and code completion for `#!python session.create_client("outposts").cancel_capacity_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.cancel_capacity_task)

```python
# cancel_capacity_task method definition

await def cancel_capacity_task(
    self,
    *,
    CapacityTaskId: str,
    OutpostIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_capacity_task method usage example with argument unpacking

kwargs: CancelCapacityTaskInputRequestTypeDef = {  # (1)
    "CapacityTaskId": ...,
    "OutpostIdentifier": ...,
}

parent.cancel_capacity_task(**kwargs)
```

1. See [:material-code-braces: CancelCapacityTaskInputRequestTypeDef](./type_defs.md#cancelcapacitytaskinputrequesttypedef) 

### cancel\_order

Cancels the specified order for an Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").cancel_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.cancel_order)

```python
# cancel_order method definition

await def cancel_order(
    self,
    *,
    OrderId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_order method usage example with argument unpacking

kwargs: CancelOrderInputRequestTypeDef = {  # (1)
    "OrderId": ...,
}

parent.cancel_order(**kwargs)
```

1. See [:material-code-braces: CancelOrderInputRequestTypeDef](./type_defs.md#cancelorderinputrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("outposts").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_order

Creates an order for an Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").create_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_order)

```python
# create_order method definition

await def create_order(
    self,
    *,
    OutpostIdentifier: str,
    LineItems: Sequence[LineItemRequestTypeDef],  # (1)
    PaymentOption: PaymentOptionType,  # (2)
    PaymentTerm: PaymentTermType = ...,  # (3)
) -> CreateOrderOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: LineItemRequestTypeDef](./type_defs.md#lineitemrequesttypedef) 
2. See [:material-code-brackets: PaymentOptionType](./literals.md#paymentoptiontype) 
3. See [:material-code-brackets: PaymentTermType](./literals.md#paymenttermtype) 
4. See [:material-code-braces: CreateOrderOutputTypeDef](./type_defs.md#createorderoutputtypedef) 


```python
# create_order method usage example with argument unpacking

kwargs: CreateOrderInputRequestTypeDef = {  # (1)
    "OutpostIdentifier": ...,
    "LineItems": ...,
    "PaymentOption": ...,
}

parent.create_order(**kwargs)
```

1. See [:material-code-braces: CreateOrderInputRequestTypeDef](./type_defs.md#createorderinputrequesttypedef) 

### create\_outpost

Creates an Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").create_outpost` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_outpost)

```python
# create_outpost method definition

await def create_outpost(
    self,
    *,
    Name: str,
    SiteId: str,
    Description: str = ...,
    AvailabilityZone: str = ...,
    AvailabilityZoneId: str = ...,
    Tags: Mapping[str, str] = ...,
    SupportedHardwareType: SupportedHardwareTypeType = ...,  # (1)
) -> CreateOutpostOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SupportedHardwareTypeType](./literals.md#supportedhardwaretypetype) 
2. See [:material-code-braces: CreateOutpostOutputTypeDef](./type_defs.md#createoutpostoutputtypedef) 


```python
# create_outpost method usage example with argument unpacking

kwargs: CreateOutpostInputRequestTypeDef = {  # (1)
    "Name": ...,
    "SiteId": ...,
}

parent.create_outpost(**kwargs)
```

1. See [:material-code-braces: CreateOutpostInputRequestTypeDef](./type_defs.md#createoutpostinputrequesttypedef) 

### create\_site

Creates a site for an Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").create_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.create_site)

```python
# create_site method definition

await def create_site(
    self,
    *,
    Name: str,
    Description: str = ...,
    Notes: str = ...,
    Tags: Mapping[str, str] = ...,
    OperatingAddress: AddressTypeDef = ...,  # (1)
    ShippingAddress: AddressTypeDef = ...,  # (1)
    RackPhysicalProperties: RackPhysicalPropertiesTypeDef = ...,  # (3)
) -> CreateSiteOutputTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: RackPhysicalPropertiesTypeDef](./type_defs.md#rackphysicalpropertiestypedef) 
4. See [:material-code-braces: CreateSiteOutputTypeDef](./type_defs.md#createsiteoutputtypedef) 


```python
# create_site method usage example with argument unpacking

kwargs: CreateSiteInputRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_site(**kwargs)
```

1. See [:material-code-braces: CreateSiteInputRequestTypeDef](./type_defs.md#createsiteinputrequesttypedef) 

### delete\_outpost

Deletes the specified Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").delete_outpost` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.delete_outpost)

```python
# delete_outpost method definition

await def delete_outpost(
    self,
    *,
    OutpostId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_outpost method usage example with argument unpacking

kwargs: DeleteOutpostInputRequestTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.delete_outpost(**kwargs)
```

1. See [:material-code-braces: DeleteOutpostInputRequestTypeDef](./type_defs.md#deleteoutpostinputrequesttypedef) 

### delete\_site

Deletes the specified site.

Type annotations and code completion for `#!python session.create_client("outposts").delete_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.delete_site)

```python
# delete_site method definition

await def delete_site(
    self,
    *,
    SiteId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_site method usage example with argument unpacking

kwargs: DeleteSiteInputRequestTypeDef = {  # (1)
    "SiteId": ...,
}

parent.delete_site(**kwargs)
```

1. See [:material-code-braces: DeleteSiteInputRequestTypeDef](./type_defs.md#deletesiteinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("outposts").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.generate_presigned_url)

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


### get\_capacity\_task

Gets details of the specified capacity task.

Type annotations and code completion for `#!python session.create_client("outposts").get_capacity_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_capacity_task)

```python
# get_capacity_task method definition

await def get_capacity_task(
    self,
    *,
    CapacityTaskId: str,
    OutpostIdentifier: str,
) -> GetCapacityTaskOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCapacityTaskOutputTypeDef](./type_defs.md#getcapacitytaskoutputtypedef) 


```python
# get_capacity_task method usage example with argument unpacking

kwargs: GetCapacityTaskInputRequestTypeDef = {  # (1)
    "CapacityTaskId": ...,
    "OutpostIdentifier": ...,
}

parent.get_capacity_task(**kwargs)
```

1. See [:material-code-braces: GetCapacityTaskInputRequestTypeDef](./type_defs.md#getcapacitytaskinputrequesttypedef) 

### get\_catalog\_item

Gets information about the specified catalog item.

Type annotations and code completion for `#!python session.create_client("outposts").get_catalog_item` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_catalog_item)

```python
# get_catalog_item method definition

await def get_catalog_item(
    self,
    *,
    CatalogItemId: str,
) -> GetCatalogItemOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCatalogItemOutputTypeDef](./type_defs.md#getcatalogitemoutputtypedef) 


```python
# get_catalog_item method usage example with argument unpacking

kwargs: GetCatalogItemInputRequestTypeDef = {  # (1)
    "CatalogItemId": ...,
}

parent.get_catalog_item(**kwargs)
```

1. See [:material-code-braces: GetCatalogItemInputRequestTypeDef](./type_defs.md#getcatalogiteminputrequesttypedef) 

### get\_connection

.

Type annotations and code completion for `#!python session.create_client("outposts").get_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_connection)

```python
# get_connection method definition

await def get_connection(
    self,
    *,
    ConnectionId: str,
) -> GetConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef) 


```python
# get_connection method usage example with argument unpacking

kwargs: GetConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.get_connection(**kwargs)
```

1. See [:material-code-braces: GetConnectionRequestRequestTypeDef](./type_defs.md#getconnectionrequestrequesttypedef) 

### get\_order

Gets information about the specified order.

Type annotations and code completion for `#!python session.create_client("outposts").get_order` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_order)

```python
# get_order method definition

await def get_order(
    self,
    *,
    OrderId: str,
) -> GetOrderOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOrderOutputTypeDef](./type_defs.md#getorderoutputtypedef) 


```python
# get_order method usage example with argument unpacking

kwargs: GetOrderInputRequestTypeDef = {  # (1)
    "OrderId": ...,
}

parent.get_order(**kwargs)
```

1. See [:material-code-braces: GetOrderInputRequestTypeDef](./type_defs.md#getorderinputrequesttypedef) 

### get\_outpost

Gets information about the specified Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").get_outpost` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_outpost)

```python
# get_outpost method definition

await def get_outpost(
    self,
    *,
    OutpostId: str,
) -> GetOutpostOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOutpostOutputTypeDef](./type_defs.md#getoutpostoutputtypedef) 


```python
# get_outpost method usage example with argument unpacking

kwargs: GetOutpostInputRequestTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.get_outpost(**kwargs)
```

1. See [:material-code-braces: GetOutpostInputRequestTypeDef](./type_defs.md#getoutpostinputrequesttypedef) 

### get\_outpost\_instance\_types

Gets the instance types for the specified Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").get_outpost_instance_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_outpost_instance_types)

```python
# get_outpost_instance_types method definition

await def get_outpost_instance_types(
    self,
    *,
    OutpostId: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetOutpostInstanceTypesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOutpostInstanceTypesOutputTypeDef](./type_defs.md#getoutpostinstancetypesoutputtypedef) 


```python
# get_outpost_instance_types method usage example with argument unpacking

kwargs: GetOutpostInstanceTypesInputRequestTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.get_outpost_instance_types(**kwargs)
```

1. See [:material-code-braces: GetOutpostInstanceTypesInputRequestTypeDef](./type_defs.md#getoutpostinstancetypesinputrequesttypedef) 

### get\_outpost\_supported\_instance\_types

Gets the instance types that an Outpost can support in `InstanceTypeCapacity`.

Type annotations and code completion for `#!python session.create_client("outposts").get_outpost_supported_instance_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_outpost_supported_instance_types)

```python
# get_outpost_supported_instance_types method definition

await def get_outpost_supported_instance_types(
    self,
    *,
    OutpostIdentifier: str,
    OrderId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetOutpostSupportedInstanceTypesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOutpostSupportedInstanceTypesOutputTypeDef](./type_defs.md#getoutpostsupportedinstancetypesoutputtypedef) 


```python
# get_outpost_supported_instance_types method usage example with argument unpacking

kwargs: GetOutpostSupportedInstanceTypesInputRequestTypeDef = {  # (1)
    "OutpostIdentifier": ...,
    "OrderId": ...,
}

parent.get_outpost_supported_instance_types(**kwargs)
```

1. See [:material-code-braces: GetOutpostSupportedInstanceTypesInputRequestTypeDef](./type_defs.md#getoutpostsupportedinstancetypesinputrequesttypedef) 

### get\_site

Gets information about the specified Outpost site.

Type annotations and code completion for `#!python session.create_client("outposts").get_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_site)

```python
# get_site method definition

await def get_site(
    self,
    *,
    SiteId: str,
) -> GetSiteOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSiteOutputTypeDef](./type_defs.md#getsiteoutputtypedef) 


```python
# get_site method usage example with argument unpacking

kwargs: GetSiteInputRequestTypeDef = {  # (1)
    "SiteId": ...,
}

parent.get_site(**kwargs)
```

1. See [:material-code-braces: GetSiteInputRequestTypeDef](./type_defs.md#getsiteinputrequesttypedef) 

### get\_site\_address

Gets the site address of the specified site.

Type annotations and code completion for `#!python session.create_client("outposts").get_site_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.get_site_address)

```python
# get_site_address method definition

await def get_site_address(
    self,
    *,
    SiteId: str,
    AddressType: AddressTypeType,  # (1)
) -> GetSiteAddressOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AddressTypeType](./literals.md#addresstypetype) 
2. See [:material-code-braces: GetSiteAddressOutputTypeDef](./type_defs.md#getsiteaddressoutputtypedef) 


```python
# get_site_address method usage example with argument unpacking

kwargs: GetSiteAddressInputRequestTypeDef = {  # (1)
    "SiteId": ...,
    "AddressType": ...,
}

parent.get_site_address(**kwargs)
```

1. See [:material-code-braces: GetSiteAddressInputRequestTypeDef](./type_defs.md#getsiteaddressinputrequesttypedef) 

### list\_assets

Lists the hardware assets for the specified Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").list_assets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_assets)

```python
# list_assets method definition

await def list_assets(
    self,
    *,
    OutpostIdentifier: str,
    HostIdFilter: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    StatusFilter: Sequence[AssetStateType] = ...,  # (1)
) -> ListAssetsOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AssetStateType](./literals.md#assetstatetype) 
2. See [:material-code-braces: ListAssetsOutputTypeDef](./type_defs.md#listassetsoutputtypedef) 


```python
# list_assets method usage example with argument unpacking

kwargs: ListAssetsInputRequestTypeDef = {  # (1)
    "OutpostIdentifier": ...,
}

parent.list_assets(**kwargs)
```

1. See [:material-code-braces: ListAssetsInputRequestTypeDef](./type_defs.md#listassetsinputrequesttypedef) 

### list\_capacity\_tasks

Lists the capacity tasks for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("outposts").list_capacity_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_capacity_tasks)

```python
# list_capacity_tasks method definition

await def list_capacity_tasks(
    self,
    *,
    OutpostIdentifierFilter: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    CapacityTaskStatusFilter: Sequence[CapacityTaskStatusType] = ...,  # (1)
) -> ListCapacityTasksOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: CapacityTaskStatusType](./literals.md#capacitytaskstatustype) 
2. See [:material-code-braces: ListCapacityTasksOutputTypeDef](./type_defs.md#listcapacitytasksoutputtypedef) 


```python
# list_capacity_tasks method usage example with argument unpacking

kwargs: ListCapacityTasksInputRequestTypeDef = {  # (1)
    "OutpostIdentifierFilter": ...,
}

parent.list_capacity_tasks(**kwargs)
```

1. See [:material-code-braces: ListCapacityTasksInputRequestTypeDef](./type_defs.md#listcapacitytasksinputrequesttypedef) 

### list\_catalog\_items

Lists the items in the catalog.

Type annotations and code completion for `#!python session.create_client("outposts").list_catalog_items` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_catalog_items)

```python
# list_catalog_items method definition

await def list_catalog_items(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    ItemClassFilter: Sequence[CatalogItemClassType] = ...,  # (1)
    SupportedStorageFilter: Sequence[SupportedStorageEnumType] = ...,  # (2)
    EC2FamilyFilter: Sequence[str] = ...,
) -> ListCatalogItemsOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: CatalogItemClassType](./literals.md#catalogitemclasstype) 
2. See [:material-code-brackets: SupportedStorageEnumType](./literals.md#supportedstorageenumtype) 
3. See [:material-code-braces: ListCatalogItemsOutputTypeDef](./type_defs.md#listcatalogitemsoutputtypedef) 


```python
# list_catalog_items method usage example with argument unpacking

kwargs: ListCatalogItemsInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_catalog_items(**kwargs)
```

1. See [:material-code-braces: ListCatalogItemsInputRequestTypeDef](./type_defs.md#listcatalogitemsinputrequesttypedef) 

### list\_orders

Lists the Outpost orders for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("outposts").list_orders` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_orders)

```python
# list_orders method definition

await def list_orders(
    self,
    *,
    OutpostIdentifierFilter: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListOrdersOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOrdersOutputTypeDef](./type_defs.md#listordersoutputtypedef) 


```python
# list_orders method usage example with argument unpacking

kwargs: ListOrdersInputRequestTypeDef = {  # (1)
    "OutpostIdentifierFilter": ...,
}

parent.list_orders(**kwargs)
```

1. See [:material-code-braces: ListOrdersInputRequestTypeDef](./type_defs.md#listordersinputrequesttypedef) 

### list\_outposts

Lists the Outposts for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("outposts").list_outposts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_outposts)

```python
# list_outposts method definition

await def list_outposts(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    LifeCycleStatusFilter: Sequence[str] = ...,
    AvailabilityZoneFilter: Sequence[str] = ...,
    AvailabilityZoneIdFilter: Sequence[str] = ...,
) -> ListOutpostsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOutpostsOutputTypeDef](./type_defs.md#listoutpostsoutputtypedef) 


```python
# list_outposts method usage example with argument unpacking

kwargs: ListOutpostsInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_outposts(**kwargs)
```

1. See [:material-code-braces: ListOutpostsInputRequestTypeDef](./type_defs.md#listoutpostsinputrequesttypedef) 

### list\_sites

Lists the Outpost sites for your Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("outposts").list_sites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_sites)

```python
# list_sites method definition

await def list_sites(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    OperatingAddressCountryCodeFilter: Sequence[str] = ...,
    OperatingAddressStateOrRegionFilter: Sequence[str] = ...,
    OperatingAddressCityFilter: Sequence[str] = ...,
) -> ListSitesOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSitesOutputTypeDef](./type_defs.md#listsitesoutputtypedef) 


```python
# list_sites method usage example with argument unpacking

kwargs: ListSitesInputRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_sites(**kwargs)
```

1. See [:material-code-braces: ListSitesInputRequestTypeDef](./type_defs.md#listsitesinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("outposts").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.list_tags_for_resource)

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

### start\_capacity\_task

Starts the specified capacity task.

Type annotations and code completion for `#!python session.create_client("outposts").start_capacity_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.start_capacity_task)

```python
# start_capacity_task method definition

await def start_capacity_task(
    self,
    *,
    OutpostIdentifier: str,
    OrderId: str,
    InstancePools: Sequence[InstanceTypeCapacityTypeDef],  # (1)
    DryRun: bool = ...,
) -> StartCapacityTaskOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InstanceTypeCapacityTypeDef](./type_defs.md#instancetypecapacitytypedef) 
2. See [:material-code-braces: StartCapacityTaskOutputTypeDef](./type_defs.md#startcapacitytaskoutputtypedef) 


```python
# start_capacity_task method usage example with argument unpacking

kwargs: StartCapacityTaskInputRequestTypeDef = {  # (1)
    "OutpostIdentifier": ...,
    "OrderId": ...,
    "InstancePools": ...,
}

parent.start_capacity_task(**kwargs)
```

1. See [:material-code-braces: StartCapacityTaskInputRequestTypeDef](./type_defs.md#startcapacitytaskinputrequesttypedef) 

### start\_connection

.

Type annotations and code completion for `#!python session.create_client("outposts").start_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.start_connection)

```python
# start_connection method definition

await def start_connection(
    self,
    *,
    AssetId: str,
    ClientPublicKey: str,
    NetworkInterfaceDeviceIndex: int,
    DeviceSerialNumber: str = ...,
) -> StartConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartConnectionResponseTypeDef](./type_defs.md#startconnectionresponsetypedef) 


```python
# start_connection method usage example with argument unpacking

kwargs: StartConnectionRequestRequestTypeDef = {  # (1)
    "AssetId": ...,
    "ClientPublicKey": ...,
    "NetworkInterfaceDeviceIndex": ...,
}

parent.start_connection(**kwargs)
```

1. See [:material-code-braces: StartConnectionRequestRequestTypeDef](./type_defs.md#startconnectionrequestrequesttypedef) 

### tag\_resource

Adds tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("outposts").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("outposts").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_outpost

Updates an Outpost.

Type annotations and code completion for `#!python session.create_client("outposts").update_outpost` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_outpost)

```python
# update_outpost method definition

await def update_outpost(
    self,
    *,
    OutpostId: str,
    Name: str = ...,
    Description: str = ...,
    SupportedHardwareType: SupportedHardwareTypeType = ...,  # (1)
) -> UpdateOutpostOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SupportedHardwareTypeType](./literals.md#supportedhardwaretypetype) 
2. See [:material-code-braces: UpdateOutpostOutputTypeDef](./type_defs.md#updateoutpostoutputtypedef) 


```python
# update_outpost method usage example with argument unpacking

kwargs: UpdateOutpostInputRequestTypeDef = {  # (1)
    "OutpostId": ...,
}

parent.update_outpost(**kwargs)
```

1. See [:material-code-braces: UpdateOutpostInputRequestTypeDef](./type_defs.md#updateoutpostinputrequesttypedef) 

### update\_site

Updates the specified site.

Type annotations and code completion for `#!python session.create_client("outposts").update_site` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site)

```python
# update_site method definition

await def update_site(
    self,
    *,
    SiteId: str,
    Name: str = ...,
    Description: str = ...,
    Notes: str = ...,
) -> UpdateSiteOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateSiteOutputTypeDef](./type_defs.md#updatesiteoutputtypedef) 


```python
# update_site method usage example with argument unpacking

kwargs: UpdateSiteInputRequestTypeDef = {  # (1)
    "SiteId": ...,
}

parent.update_site(**kwargs)
```

1. See [:material-code-braces: UpdateSiteInputRequestTypeDef](./type_defs.md#updatesiteinputrequesttypedef) 

### update\_site\_address

Updates the address of the specified site.

Type annotations and code completion for `#!python session.create_client("outposts").update_site_address` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_address)

```python
# update_site_address method definition

await def update_site_address(
    self,
    *,
    SiteId: str,
    AddressType: AddressTypeType,  # (1)
    Address: AddressTypeDef,  # (2)
) -> UpdateSiteAddressOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: AddressTypeType](./literals.md#addresstypetype) 
2. See [:material-code-braces: AddressTypeDef](./type_defs.md#addresstypedef) 
3. See [:material-code-braces: UpdateSiteAddressOutputTypeDef](./type_defs.md#updatesiteaddressoutputtypedef) 


```python
# update_site_address method usage example with argument unpacking

kwargs: UpdateSiteAddressInputRequestTypeDef = {  # (1)
    "SiteId": ...,
    "AddressType": ...,
    "Address": ...,
}

parent.update_site_address(**kwargs)
```

1. See [:material-code-braces: UpdateSiteAddressInputRequestTypeDef](./type_defs.md#updatesiteaddressinputrequesttypedef) 

### update\_site\_rack\_physical\_properties

Update the physical and logistical details for a rack at a site.

Type annotations and code completion for `#!python session.create_client("outposts").update_site_rack_physical_properties` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.update_site_rack_physical_properties)

```python
# update_site_rack_physical_properties method definition

await def update_site_rack_physical_properties(
    self,
    *,
    SiteId: str,
    PowerDrawKva: PowerDrawKvaType = ...,  # (1)
    PowerPhase: PowerPhaseType = ...,  # (2)
    PowerConnector: PowerConnectorType = ...,  # (3)
    PowerFeedDrop: PowerFeedDropType = ...,  # (4)
    UplinkGbps: UplinkGbpsType = ...,  # (5)
    UplinkCount: UplinkCountType = ...,  # (6)
    FiberOpticCableType: FiberOpticCableTypeType = ...,  # (7)
    OpticalStandard: OpticalStandardType = ...,  # (8)
    MaximumSupportedWeightLbs: MaximumSupportedWeightLbsType = ...,  # (9)
) -> UpdateSiteRackPhysicalPropertiesOutputTypeDef:  # (10)
    ...
```

1. See [:material-code-brackets: PowerDrawKvaType](./literals.md#powerdrawkvatype) 
2. See [:material-code-brackets: PowerPhaseType](./literals.md#powerphasetype) 
3. See [:material-code-brackets: PowerConnectorType](./literals.md#powerconnectortype) 
4. See [:material-code-brackets: PowerFeedDropType](./literals.md#powerfeeddroptype) 
5. See [:material-code-brackets: UplinkGbpsType](./literals.md#uplinkgbpstype) 
6. See [:material-code-brackets: UplinkCountType](./literals.md#uplinkcounttype) 
7. See [:material-code-brackets: FiberOpticCableTypeType](./literals.md#fiberopticcabletypetype) 
8. See [:material-code-brackets: OpticalStandardType](./literals.md#opticalstandardtype) 
9. See [:material-code-brackets: MaximumSupportedWeightLbsType](./literals.md#maximumsupportedweightlbstype) 
10. See [:material-code-braces: UpdateSiteRackPhysicalPropertiesOutputTypeDef](./type_defs.md#updatesiterackphysicalpropertiesoutputtypedef) 


```python
# update_site_rack_physical_properties method usage example with argument unpacking

kwargs: UpdateSiteRackPhysicalPropertiesInputRequestTypeDef = {  # (1)
    "SiteId": ...,
}

parent.update_site_rack_physical_properties(**kwargs)
```

1. See [:material-code-braces: UpdateSiteRackPhysicalPropertiesInputRequestTypeDef](./type_defs.md#updatesiterackphysicalpropertiesinputrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("outposts").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "OutpostsClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("outposts").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#Outposts.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("outposts").get_paginator` method with overloads.

- `client.get_paginator("get_outpost_instance_types")` -> [GetOutpostInstanceTypesPaginator](./paginators.md#getoutpostinstancetypespaginator)
- `client.get_paginator("get_outpost_supported_instance_types")` -> [GetOutpostSupportedInstanceTypesPaginator](./paginators.md#getoutpostsupportedinstancetypespaginator)
- `client.get_paginator("list_assets")` -> [ListAssetsPaginator](./paginators.md#listassetspaginator)
- `client.get_paginator("list_capacity_tasks")` -> [ListCapacityTasksPaginator](./paginators.md#listcapacitytaskspaginator)
- `client.get_paginator("list_catalog_items")` -> [ListCatalogItemsPaginator](./paginators.md#listcatalogitemspaginator)
- `client.get_paginator("list_orders")` -> [ListOrdersPaginator](./paginators.md#listorderspaginator)
- `client.get_paginator("list_outposts")` -> [ListOutpostsPaginator](./paginators.md#listoutpostspaginator)
- `client.get_paginator("list_sites")` -> [ListSitesPaginator](./paginators.md#listsitespaginator)



