# Paginators

> [Index](../README.md) > [EC2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#ec2)
    type annotations stubs module [types-aiobotocore-ec2](https://pypi.org/project/types-aiobotocore-ec2/).

## DescribeAddressTransfersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_address_transfers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeAddressTransfers.html#EC2.Paginator.DescribeAddressTransfers)

```python
# DescribeAddressTransfersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeAddressTransfersPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeAddressTransfersPaginator = client.get_paginator("describe_address_transfers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAddressTransfersResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeAddressTransfersPaginator](./paginators.md#describeaddresstransferspaginator)
3. item: `AioPageIterator[DescribeAddressTransfersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAddressTransfersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AllocationIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeAddressTransfersResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeAddressTransfersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAddressTransfersRequestPaginateTypeDef = {  # (1)
    "AllocationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAddressTransfersRequestPaginateTypeDef](./type_defs.md#describeaddresstransfersrequestpaginatetypedef)
## DescribeAddressesAttributePaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_addresses_attribute")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeAddressesAttribute.html#EC2.Paginator.DescribeAddressesAttribute)

```python
# DescribeAddressesAttributePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeAddressesAttributePaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeAddressesAttributePaginator = client.get_paginator("describe_addresses_attribute")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAddressesAttributeResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeAddressesAttributePaginator](./paginators.md#describeaddressesattributepaginator)
3. item: `AioPageIterator[DescribeAddressesAttributeResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAddressesAttributePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AllocationIds: Sequence[str] = ...,
    Attribute: AddressAttributeNameType = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeAddressesAttributeResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AddressAttributeNameType](./literals.md#addressattributenametype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeAddressesAttributeResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAddressesAttributeRequestPaginateTypeDef = {  # (1)
    "AllocationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAddressesAttributeRequestPaginateTypeDef](./type_defs.md#describeaddressesattributerequestpaginatetypedef)
## DescribeAwsNetworkPerformanceMetricSubscriptionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_aws_network_performance_metric_subscriptions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeAwsNetworkPerformanceMetricSubscriptions.html#EC2.Paginator.DescribeAwsNetworkPerformanceMetricSubscriptions)

```python
# DescribeAwsNetworkPerformanceMetricSubscriptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeAwsNetworkPerformanceMetricSubscriptionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeAwsNetworkPerformanceMetricSubscriptionsPaginator = client.get_paginator("describe_aws_network_performance_metric_subscriptions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeAwsNetworkPerformanceMetricSubscriptionsPaginator](./paginators.md#describeawsnetworkperformancemetricsubscriptionspaginator)
3. item: `AioPageIterator[DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAwsNetworkPerformanceMetricSubscriptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeAwsNetworkPerformanceMetricSubscriptionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAwsNetworkPerformanceMetricSubscriptionsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAwsNetworkPerformanceMetricSubscriptionsRequestPaginateTypeDef](./type_defs.md#describeawsnetworkperformancemetricsubscriptionsrequestpaginatetypedef)
## DescribeByoipCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_byoip_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeByoipCidrs.html#EC2.Paginator.DescribeByoipCidrs)

```python
# DescribeByoipCidrsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeByoipCidrsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeByoipCidrsPaginator = client.get_paginator("describe_byoip_cidrs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeByoipCidrsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeByoipCidrsPaginator](./paginators.md#describebyoipcidrspaginator)
3. item: `AioPageIterator[DescribeByoipCidrsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeByoipCidrsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeByoipCidrsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeByoipCidrsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeByoipCidrsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeByoipCidrsRequestPaginateTypeDef](./type_defs.md#describebyoipcidrsrequestpaginatetypedef)
## DescribeCapacityBlockExtensionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_block_extension_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityBlockExtensionHistory.html#EC2.Paginator.DescribeCapacityBlockExtensionHistory)

```python
# DescribeCapacityBlockExtensionHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityBlockExtensionHistoryPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityBlockExtensionHistoryPaginator = client.get_paginator("describe_capacity_block_extension_history")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityBlockExtensionHistoryResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityBlockExtensionHistoryPaginator](./paginators.md#describecapacityblockextensionhistorypaginator)
3. item: `AioPageIterator[DescribeCapacityBlockExtensionHistoryResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityBlockExtensionHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityReservationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityBlockExtensionHistoryResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCapacityBlockExtensionHistoryResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityBlockExtensionHistoryRequestPaginateTypeDef = {  # (1)
    "CapacityReservationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityBlockExtensionHistoryRequestPaginateTypeDef](./type_defs.md#describecapacityblockextensionhistoryrequestpaginatetypedef)
## DescribeCapacityBlockExtensionOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_block_extension_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityBlockExtensionOfferings.html#EC2.Paginator.DescribeCapacityBlockExtensionOfferings)

```python
# DescribeCapacityBlockExtensionOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityBlockExtensionOfferingsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityBlockExtensionOfferingsPaginator = client.get_paginator("describe_capacity_block_extension_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityBlockExtensionOfferingsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityBlockExtensionOfferingsPaginator](./paginators.md#describecapacityblockextensionofferingspaginator)
3. item: `AioPageIterator[DescribeCapacityBlockExtensionOfferingsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityBlockExtensionOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityBlockExtensionDurationHours: int,
    CapacityReservationId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityBlockExtensionOfferingsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeCapacityBlockExtensionOfferingsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityBlockExtensionOfferingsRequestPaginateTypeDef = {  # (1)
    "CapacityBlockExtensionDurationHours": ...,
    "CapacityReservationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityBlockExtensionOfferingsRequestPaginateTypeDef](./type_defs.md#describecapacityblockextensionofferingsrequestpaginatetypedef)
## DescribeCapacityBlockOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_block_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityBlockOfferings.html#EC2.Paginator.DescribeCapacityBlockOfferings)

```python
# DescribeCapacityBlockOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityBlockOfferingsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityBlockOfferingsPaginator = client.get_paginator("describe_capacity_block_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityBlockOfferingsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityBlockOfferingsPaginator](./paginators.md#describecapacityblockofferingspaginator)
3. item: `AioPageIterator[DescribeCapacityBlockOfferingsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityBlockOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityDurationHours: int,
    DryRun: bool = ...,
    InstanceType: str = ...,
    InstanceCount: int = ...,
    StartDateRange: TimestampTypeDef = ...,
    EndDateRange: TimestampTypeDef = ...,
    UltraserverType: str = ...,
    UltraserverCount: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityBlockOfferingsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeCapacityBlockOfferingsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityBlockOfferingsRequestPaginateTypeDef = {  # (1)
    "CapacityDurationHours": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityBlockOfferingsRequestPaginateTypeDef](./type_defs.md#describecapacityblockofferingsrequestpaginatetypedef)
## DescribeCapacityBlockStatusPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_block_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityBlockStatus.html#EC2.Paginator.DescribeCapacityBlockStatus)

```python
# DescribeCapacityBlockStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityBlockStatusPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityBlockStatusPaginator = client.get_paginator("describe_capacity_block_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityBlockStatusResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityBlockStatusPaginator](./paginators.md#describecapacityblockstatuspaginator)
3. item: `AioPageIterator[DescribeCapacityBlockStatusResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityBlockStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityBlockIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityBlockStatusResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCapacityBlockStatusResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityBlockStatusRequestPaginateTypeDef = {  # (1)
    "CapacityBlockIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityBlockStatusRequestPaginateTypeDef](./type_defs.md#describecapacityblockstatusrequestpaginatetypedef)
## DescribeCapacityBlocksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_blocks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityBlocks.html#EC2.Paginator.DescribeCapacityBlocks)

```python
# DescribeCapacityBlocksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityBlocksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityBlocksPaginator = client.get_paginator("describe_capacity_blocks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityBlocksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityBlocksPaginator](./paginators.md#describecapacityblockspaginator)
3. item: `AioPageIterator[DescribeCapacityBlocksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityBlocksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityBlockIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityBlocksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCapacityBlocksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityBlocksRequestPaginateTypeDef = {  # (1)
    "CapacityBlockIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityBlocksRequestPaginateTypeDef](./type_defs.md#describecapacityblocksrequestpaginatetypedef)
## DescribeCapacityManagerDataExportsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_manager_data_exports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityManagerDataExports.html#EC2.Paginator.DescribeCapacityManagerDataExports)

```python
# DescribeCapacityManagerDataExportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityManagerDataExportsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityManagerDataExportsPaginator = client.get_paginator("describe_capacity_manager_data_exports")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityManagerDataExportsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityManagerDataExportsPaginator](./paginators.md#describecapacitymanagerdataexportspaginator)
3. item: `AioPageIterator[DescribeCapacityManagerDataExportsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityManagerDataExportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityManagerDataExportIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityManagerDataExportsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCapacityManagerDataExportsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityManagerDataExportsRequestPaginateTypeDef = {  # (1)
    "CapacityManagerDataExportIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityManagerDataExportsRequestPaginateTypeDef](./type_defs.md#describecapacitymanagerdataexportsrequestpaginatetypedef)
## DescribeCapacityReservationBillingRequestsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_reservation_billing_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityReservationBillingRequests.html#EC2.Paginator.DescribeCapacityReservationBillingRequests)

```python
# DescribeCapacityReservationBillingRequestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityReservationBillingRequestsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityReservationBillingRequestsPaginator = client.get_paginator("describe_capacity_reservation_billing_requests")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityReservationBillingRequestsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityReservationBillingRequestsPaginator](./paginators.md#describecapacityreservationbillingrequestspaginator)
3. item: `AioPageIterator[DescribeCapacityReservationBillingRequestsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityReservationBillingRequestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Role: CallerRoleType,  # (1)
    CapacityReservationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityReservationBillingRequestsResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: CallerRoleType](./literals.md#callerroletype)
2. See `Sequence[FilterTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribeCapacityReservationBillingRequestsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityReservationBillingRequestsRequestPaginateTypeDef = {  # (1)
    "Role": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityReservationBillingRequestsRequestPaginateTypeDef](./type_defs.md#describecapacityreservationbillingrequestsrequestpaginatetypedef)
## DescribeCapacityReservationFleetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_reservation_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityReservationFleets.html#EC2.Paginator.DescribeCapacityReservationFleets)

```python
# DescribeCapacityReservationFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityReservationFleetsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityReservationFleetsPaginator = client.get_paginator("describe_capacity_reservation_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityReservationFleetsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityReservationFleetsPaginator](./paginators.md#describecapacityreservationfleetspaginator)
3. item: `AioPageIterator[DescribeCapacityReservationFleetsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityReservationFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityReservationFleetIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityReservationFleetsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCapacityReservationFleetsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityReservationFleetsRequestPaginateTypeDef = {  # (1)
    "CapacityReservationFleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityReservationFleetsRequestPaginateTypeDef](./type_defs.md#describecapacityreservationfleetsrequestpaginatetypedef)
## DescribeCapacityReservationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCapacityReservations.html#EC2.Paginator.DescribeCapacityReservations)

```python
# DescribeCapacityReservationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCapacityReservationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCapacityReservationsPaginator = client.get_paginator("describe_capacity_reservations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCapacityReservationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCapacityReservationsPaginator](./paginators.md#describecapacityreservationspaginator)
3. item: `AioPageIterator[DescribeCapacityReservationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCapacityReservationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityReservationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCapacityReservationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCapacityReservationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCapacityReservationsRequestPaginateTypeDef = {  # (1)
    "CapacityReservationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityReservationsRequestPaginateTypeDef](./type_defs.md#describecapacityreservationsrequestpaginatetypedef)
## DescribeCarrierGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_carrier_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCarrierGateways.html#EC2.Paginator.DescribeCarrierGateways)

```python
# DescribeCarrierGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCarrierGatewaysPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCarrierGatewaysPaginator = client.get_paginator("describe_carrier_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCarrierGatewaysResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCarrierGatewaysPaginator](./paginators.md#describecarriergatewayspaginator)
3. item: `AioPageIterator[DescribeCarrierGatewaysResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCarrierGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CarrierGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCarrierGatewaysResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCarrierGatewaysResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCarrierGatewaysRequestPaginateTypeDef = {  # (1)
    "CarrierGatewayIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCarrierGatewaysRequestPaginateTypeDef](./type_defs.md#describecarriergatewaysrequestpaginatetypedef)
## DescribeClassicLinkInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_classic_link_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeClassicLinkInstances.html#EC2.Paginator.DescribeClassicLinkInstances)

```python
# DescribeClassicLinkInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeClassicLinkInstancesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeClassicLinkInstancesPaginator = client.get_paginator("describe_classic_link_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClassicLinkInstancesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeClassicLinkInstancesPaginator](./paginators.md#describeclassiclinkinstancespaginator)
3. item: `AioPageIterator[DescribeClassicLinkInstancesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeClassicLinkInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    InstanceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeClassicLinkInstancesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeClassicLinkInstancesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClassicLinkInstancesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClassicLinkInstancesRequestPaginateTypeDef](./type_defs.md#describeclassiclinkinstancesrequestpaginatetypedef)
## DescribeClientVpnAuthorizationRulesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_authorization_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeClientVpnAuthorizationRules.html#EC2.Paginator.DescribeClientVpnAuthorizationRules)

```python
# DescribeClientVpnAuthorizationRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeClientVpnAuthorizationRulesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeClientVpnAuthorizationRulesPaginator = client.get_paginator("describe_client_vpn_authorization_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClientVpnAuthorizationRulesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeClientVpnAuthorizationRulesPaginator](./paginators.md#describeclientvpnauthorizationrulespaginator)
3. item: `AioPageIterator[DescribeClientVpnAuthorizationRulesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeClientVpnAuthorizationRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeClientVpnAuthorizationRulesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeClientVpnAuthorizationRulesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClientVpnAuthorizationRulesRequestPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnAuthorizationRulesRequestPaginateTypeDef](./type_defs.md#describeclientvpnauthorizationrulesrequestpaginatetypedef)
## DescribeClientVpnConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeClientVpnConnections.html#EC2.Paginator.DescribeClientVpnConnections)

```python
# DescribeClientVpnConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeClientVpnConnectionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeClientVpnConnectionsPaginator = client.get_paginator("describe_client_vpn_connections")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClientVpnConnectionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeClientVpnConnectionsPaginator](./paginators.md#describeclientvpnconnectionspaginator)
3. item: `AioPageIterator[DescribeClientVpnConnectionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeClientVpnConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeClientVpnConnectionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeClientVpnConnectionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClientVpnConnectionsRequestPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnConnectionsRequestPaginateTypeDef](./type_defs.md#describeclientvpnconnectionsrequestpaginatetypedef)
## DescribeClientVpnEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeClientVpnEndpoints.html#EC2.Paginator.DescribeClientVpnEndpoints)

```python
# DescribeClientVpnEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeClientVpnEndpointsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeClientVpnEndpointsPaginator = client.get_paginator("describe_client_vpn_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClientVpnEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeClientVpnEndpointsPaginator](./paginators.md#describeclientvpnendpointspaginator)
3. item: `AioPageIterator[DescribeClientVpnEndpointsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeClientVpnEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClientVpnEndpointIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeClientVpnEndpointsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeClientVpnEndpointsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClientVpnEndpointsRequestPaginateTypeDef = {  # (1)
    "ClientVpnEndpointIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnEndpointsRequestPaginateTypeDef](./type_defs.md#describeclientvpnendpointsrequestpaginatetypedef)
## DescribeClientVpnRoutesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeClientVpnRoutes.html#EC2.Paginator.DescribeClientVpnRoutes)

```python
# DescribeClientVpnRoutesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeClientVpnRoutesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeClientVpnRoutesPaginator = client.get_paginator("describe_client_vpn_routes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClientVpnRoutesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeClientVpnRoutesPaginator](./paginators.md#describeclientvpnroutespaginator)
3. item: `AioPageIterator[DescribeClientVpnRoutesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeClientVpnRoutesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeClientVpnRoutesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeClientVpnRoutesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClientVpnRoutesRequestPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnRoutesRequestPaginateTypeDef](./type_defs.md#describeclientvpnroutesrequestpaginatetypedef)
## DescribeClientVpnTargetNetworksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_target_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeClientVpnTargetNetworks.html#EC2.Paginator.DescribeClientVpnTargetNetworks)

```python
# DescribeClientVpnTargetNetworksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeClientVpnTargetNetworksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeClientVpnTargetNetworksPaginator = client.get_paginator("describe_client_vpn_target_networks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeClientVpnTargetNetworksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeClientVpnTargetNetworksPaginator](./paginators.md#describeclientvpntargetnetworkspaginator)
3. item: `AioPageIterator[DescribeClientVpnTargetNetworksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeClientVpnTargetNetworksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    AssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeClientVpnTargetNetworksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeClientVpnTargetNetworksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeClientVpnTargetNetworksRequestPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnTargetNetworksRequestPaginateTypeDef](./type_defs.md#describeclientvpntargetnetworksrequestpaginatetypedef)
## DescribeCoipPoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_coip_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeCoipPools.html#EC2.Paginator.DescribeCoipPools)

```python
# DescribeCoipPoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeCoipPoolsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeCoipPoolsPaginator = client.get_paginator("describe_coip_pools")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeCoipPoolsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeCoipPoolsPaginator](./paginators.md#describecoippoolspaginator)
3. item: `AioPageIterator[DescribeCoipPoolsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeCoipPoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeCoipPoolsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeCoipPoolsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeCoipPoolsRequestPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCoipPoolsRequestPaginateTypeDef](./type_defs.md#describecoippoolsrequestpaginatetypedef)
## DescribeDhcpOptionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_dhcp_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeDhcpOptions.html#EC2.Paginator.DescribeDhcpOptions)

```python
# DescribeDhcpOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeDhcpOptionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeDhcpOptionsPaginator = client.get_paginator("describe_dhcp_options")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDhcpOptionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeDhcpOptionsPaginator](./paginators.md#describedhcpoptionspaginator)
3. item: `AioPageIterator[DescribeDhcpOptionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeDhcpOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DhcpOptionsIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeDhcpOptionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeDhcpOptionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDhcpOptionsRequestPaginateTypeDef = {  # (1)
    "DhcpOptionsIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDhcpOptionsRequestPaginateTypeDef](./type_defs.md#describedhcpoptionsrequestpaginatetypedef)
## DescribeEgressOnlyInternetGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_egress_only_internet_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeEgressOnlyInternetGateways.html#EC2.Paginator.DescribeEgressOnlyInternetGateways)

```python
# DescribeEgressOnlyInternetGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeEgressOnlyInternetGatewaysPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeEgressOnlyInternetGatewaysPaginator = client.get_paginator("describe_egress_only_internet_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEgressOnlyInternetGatewaysResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeEgressOnlyInternetGatewaysPaginator](./paginators.md#describeegressonlyinternetgatewayspaginator)
3. item: `AioPageIterator[DescribeEgressOnlyInternetGatewaysResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeEgressOnlyInternetGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    EgressOnlyInternetGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeEgressOnlyInternetGatewaysResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeEgressOnlyInternetGatewaysResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEgressOnlyInternetGatewaysRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEgressOnlyInternetGatewaysRequestPaginateTypeDef](./type_defs.md#describeegressonlyinternetgatewaysrequestpaginatetypedef)
## DescribeExportImageTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_export_image_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeExportImageTasks.html#EC2.Paginator.DescribeExportImageTasks)

```python
# DescribeExportImageTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeExportImageTasksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeExportImageTasksPaginator = client.get_paginator("describe_export_image_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeExportImageTasksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeExportImageTasksPaginator](./paginators.md#describeexportimagetaskspaginator)
3. item: `AioPageIterator[DescribeExportImageTasksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeExportImageTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ExportImageTaskIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeExportImageTasksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeExportImageTasksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeExportImageTasksRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportImageTasksRequestPaginateTypeDef](./type_defs.md#describeexportimagetasksrequestpaginatetypedef)
## DescribeFastLaunchImagesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fast_launch_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeFastLaunchImages.html#EC2.Paginator.DescribeFastLaunchImages)

```python
# DescribeFastLaunchImagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeFastLaunchImagesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeFastLaunchImagesPaginator = client.get_paginator("describe_fast_launch_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFastLaunchImagesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeFastLaunchImagesPaginator](./paginators.md#describefastlaunchimagespaginator)
3. item: `AioPageIterator[DescribeFastLaunchImagesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFastLaunchImagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeFastLaunchImagesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeFastLaunchImagesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFastLaunchImagesRequestPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFastLaunchImagesRequestPaginateTypeDef](./type_defs.md#describefastlaunchimagesrequestpaginatetypedef)
## DescribeFastSnapshotRestoresPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fast_snapshot_restores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeFastSnapshotRestores.html#EC2.Paginator.DescribeFastSnapshotRestores)

```python
# DescribeFastSnapshotRestoresPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeFastSnapshotRestoresPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeFastSnapshotRestoresPaginator = client.get_paginator("describe_fast_snapshot_restores")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFastSnapshotRestoresResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeFastSnapshotRestoresPaginator](./paginators.md#describefastsnapshotrestorespaginator)
3. item: `AioPageIterator[DescribeFastSnapshotRestoresResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFastSnapshotRestoresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeFastSnapshotRestoresResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeFastSnapshotRestoresResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFastSnapshotRestoresRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFastSnapshotRestoresRequestPaginateTypeDef](./type_defs.md#describefastsnapshotrestoresrequestpaginatetypedef)
## DescribeFleetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeFleets.html#EC2.Paginator.DescribeFleets)

```python
# DescribeFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeFleetsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeFleetsPaginator = client.get_paginator("describe_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFleetsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeFleetsPaginator](./paginators.md#describefleetspaginator)
3. item: `AioPageIterator[DescribeFleetsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    FleetIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeFleetsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeFleetsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFleetsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetsRequestPaginateTypeDef](./type_defs.md#describefleetsrequestpaginatetypedef)
## DescribeFlowLogsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_flow_logs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeFlowLogs.html#EC2.Paginator.DescribeFlowLogs)

```python
# DescribeFlowLogsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeFlowLogsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeFlowLogsPaginator = client.get_paginator("describe_flow_logs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFlowLogsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeFlowLogsPaginator](./paginators.md#describeflowlogspaginator)
3. item: `AioPageIterator[DescribeFlowLogsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFlowLogsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    FlowLogIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeFlowLogsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeFlowLogsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFlowLogsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFlowLogsRequestPaginateTypeDef](./type_defs.md#describeflowlogsrequestpaginatetypedef)
## DescribeFpgaImagesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fpga_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeFpgaImages.html#EC2.Paginator.DescribeFpgaImages)

```python
# DescribeFpgaImagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeFpgaImagesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeFpgaImagesPaginator = client.get_paginator("describe_fpga_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeFpgaImagesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeFpgaImagesPaginator](./paginators.md#describefpgaimagespaginator)
3. item: `AioPageIterator[DescribeFpgaImagesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeFpgaImagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    FpgaImageIds: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeFpgaImagesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeFpgaImagesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeFpgaImagesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFpgaImagesRequestPaginateTypeDef](./type_defs.md#describefpgaimagesrequestpaginatetypedef)
## DescribeHostReservationOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_host_reservation_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeHostReservationOfferings.html#EC2.Paginator.DescribeHostReservationOfferings)

```python
# DescribeHostReservationOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeHostReservationOfferingsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeHostReservationOfferingsPaginator = client.get_paginator("describe_host_reservation_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeHostReservationOfferingsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeHostReservationOfferingsPaginator](./paginators.md#describehostreservationofferingspaginator)
3. item: `AioPageIterator[DescribeHostReservationOfferingsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeHostReservationOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxDuration: int = ...,
    MinDuration: int = ...,
    OfferingId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeHostReservationOfferingsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeHostReservationOfferingsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeHostReservationOfferingsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHostReservationOfferingsRequestPaginateTypeDef](./type_defs.md#describehostreservationofferingsrequestpaginatetypedef)
## DescribeHostReservationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_host_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeHostReservations.html#EC2.Paginator.DescribeHostReservations)

```python
# DescribeHostReservationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeHostReservationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeHostReservationsPaginator = client.get_paginator("describe_host_reservations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeHostReservationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeHostReservationsPaginator](./paginators.md#describehostreservationspaginator)
3. item: `AioPageIterator[DescribeHostReservationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeHostReservationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    HostReservationIdSet: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeHostReservationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeHostReservationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeHostReservationsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHostReservationsRequestPaginateTypeDef](./type_defs.md#describehostreservationsrequestpaginatetypedef)
## DescribeHostsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_hosts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeHosts.html#EC2.Paginator.DescribeHosts)

```python
# DescribeHostsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeHostsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeHostsPaginator = client.get_paginator("describe_hosts")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeHostsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeHostsPaginator](./paginators.md#describehostspaginator)
3. item: `AioPageIterator[DescribeHostsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeHostsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    HostIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeHostsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeHostsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeHostsRequestPaginateTypeDef = {  # (1)
    "HostIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHostsRequestPaginateTypeDef](./type_defs.md#describehostsrequestpaginatetypedef)
## DescribeIamInstanceProfileAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_iam_instance_profile_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIamInstanceProfileAssociations.html#EC2.Paginator.DescribeIamInstanceProfileAssociations)

```python
# DescribeIamInstanceProfileAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIamInstanceProfileAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIamInstanceProfileAssociationsPaginator = client.get_paginator("describe_iam_instance_profile_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIamInstanceProfileAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIamInstanceProfileAssociationsPaginator](./paginators.md#describeiaminstanceprofileassociationspaginator)
3. item: `AioPageIterator[DescribeIamInstanceProfileAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIamInstanceProfileAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIamInstanceProfileAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIamInstanceProfileAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIamInstanceProfileAssociationsRequestPaginateTypeDef = {  # (1)
    "AssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIamInstanceProfileAssociationsRequestPaginateTypeDef](./type_defs.md#describeiaminstanceprofileassociationsrequestpaginatetypedef)
## DescribeImageReferencesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_image_references")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeImageReferences.html#EC2.Paginator.DescribeImageReferences)

```python
# DescribeImageReferencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeImageReferencesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeImageReferencesPaginator = client.get_paginator("describe_image_references")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageReferencesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeImageReferencesPaginator](./paginators.md#describeimagereferencespaginator)
3. item: `AioPageIterator[DescribeImageReferencesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeImageReferencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageIds: Sequence[str],
    IncludeAllResourceTypes: bool = ...,
    ResourceTypes: Sequence[ResourceTypeRequestTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeImageReferencesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[ResourceTypeRequestTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeImageReferencesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImageReferencesRequestPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageReferencesRequestPaginateTypeDef](./type_defs.md#describeimagereferencesrequestpaginatetypedef)
## DescribeImageUsageReportEntriesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_image_usage_report_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeImageUsageReportEntries.html#EC2.Paginator.DescribeImageUsageReportEntries)

```python
# DescribeImageUsageReportEntriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeImageUsageReportEntriesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeImageUsageReportEntriesPaginator = client.get_paginator("describe_image_usage_report_entries")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageUsageReportEntriesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeImageUsageReportEntriesPaginator](./paginators.md#describeimageusagereportentriespaginator)
3. item: `AioPageIterator[DescribeImageUsageReportEntriesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeImageUsageReportEntriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    ReportIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeImageUsageReportEntriesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeImageUsageReportEntriesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImageUsageReportEntriesRequestPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageUsageReportEntriesRequestPaginateTypeDef](./type_defs.md#describeimageusagereportentriesrequestpaginatetypedef)
## DescribeImageUsageReportsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_image_usage_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeImageUsageReports.html#EC2.Paginator.DescribeImageUsageReports)

```python
# DescribeImageUsageReportsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeImageUsageReportsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeImageUsageReportsPaginator = client.get_paginator("describe_image_usage_reports")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImageUsageReportsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeImageUsageReportsPaginator](./paginators.md#describeimageusagereportspaginator)
3. item: `AioPageIterator[DescribeImageUsageReportsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeImageUsageReportsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    ReportIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeImageUsageReportsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeImageUsageReportsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImageUsageReportsRequestPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImageUsageReportsRequestPaginateTypeDef](./type_defs.md#describeimageusagereportsrequestpaginatetypedef)
## DescribeImagesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeImages.html#EC2.Paginator.DescribeImages)

```python
# DescribeImagesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeImagesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeImagesPaginator = client.get_paginator("describe_images")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImagesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeImagesPaginator](./paginators.md#describeimagespaginator)
3. item: `AioPageIterator[DescribeImagesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeImagesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ExecutableUsers: Sequence[str] = ...,
    ImageIds: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    IncludeDeprecated: bool = ...,
    IncludeDisabled: bool = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeImagesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeImagesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImagesRequestPaginateTypeDef = {  # (1)
    "ExecutableUsers": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImagesRequestPaginateTypeDef](./type_defs.md#describeimagesrequestpaginatetypedef)
## DescribeImportImageTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_import_image_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeImportImageTasks.html#EC2.Paginator.DescribeImportImageTasks)

```python
# DescribeImportImageTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeImportImageTasksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeImportImageTasksPaginator = client.get_paginator("describe_import_image_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImportImageTasksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeImportImageTasksPaginator](./paginators.md#describeimportimagetaskspaginator)
3. item: `AioPageIterator[DescribeImportImageTasksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeImportImageTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ImportTaskIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeImportImageTasksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeImportImageTasksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImportImageTasksRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImportImageTasksRequestPaginateTypeDef](./type_defs.md#describeimportimagetasksrequestpaginatetypedef)
## DescribeImportSnapshotTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_import_snapshot_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeImportSnapshotTasks.html#EC2.Paginator.DescribeImportSnapshotTasks)

```python
# DescribeImportSnapshotTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeImportSnapshotTasksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeImportSnapshotTasksPaginator = client.get_paginator("describe_import_snapshot_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeImportSnapshotTasksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeImportSnapshotTasksPaginator](./paginators.md#describeimportsnapshottaskspaginator)
3. item: `AioPageIterator[DescribeImportSnapshotTasksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeImportSnapshotTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ImportTaskIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeImportSnapshotTasksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeImportSnapshotTasksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeImportSnapshotTasksRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImportSnapshotTasksRequestPaginateTypeDef](./type_defs.md#describeimportsnapshottasksrequestpaginatetypedef)
## DescribeInstanceConnectEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_connect_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceConnectEndpoints.html#EC2.Paginator.DescribeInstanceConnectEndpoints)

```python
# DescribeInstanceConnectEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceConnectEndpointsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceConnectEndpointsPaginator = client.get_paginator("describe_instance_connect_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceConnectEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceConnectEndpointsPaginator](./paginators.md#describeinstanceconnectendpointspaginator)
3. item: `AioPageIterator[DescribeInstanceConnectEndpointsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceConnectEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    InstanceConnectEndpointIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceConnectEndpointsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInstanceConnectEndpointsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceConnectEndpointsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceConnectEndpointsRequestPaginateTypeDef](./type_defs.md#describeinstanceconnectendpointsrequestpaginatetypedef)
## DescribeInstanceCreditSpecificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_credit_specifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceCreditSpecifications.html#EC2.Paginator.DescribeInstanceCreditSpecifications)

```python
# DescribeInstanceCreditSpecificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceCreditSpecificationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceCreditSpecificationsPaginator = client.get_paginator("describe_instance_credit_specifications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceCreditSpecificationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceCreditSpecificationsPaginator](./paginators.md#describeinstancecreditspecificationspaginator)
3. item: `AioPageIterator[DescribeInstanceCreditSpecificationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceCreditSpecificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    InstanceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceCreditSpecificationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInstanceCreditSpecificationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceCreditSpecificationsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceCreditSpecificationsRequestPaginateTypeDef](./type_defs.md#describeinstancecreditspecificationsrequestpaginatetypedef)
## DescribeInstanceEventWindowsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_event_windows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceEventWindows.html#EC2.Paginator.DescribeInstanceEventWindows)

```python
# DescribeInstanceEventWindowsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceEventWindowsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceEventWindowsPaginator = client.get_paginator("describe_instance_event_windows")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceEventWindowsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceEventWindowsPaginator](./paginators.md#describeinstanceeventwindowspaginator)
3. item: `AioPageIterator[DescribeInstanceEventWindowsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceEventWindowsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    InstanceEventWindowIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceEventWindowsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInstanceEventWindowsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceEventWindowsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceEventWindowsRequestPaginateTypeDef](./type_defs.md#describeinstanceeventwindowsrequestpaginatetypedef)
## DescribeInstanceImageMetadataPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_image_metadata")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceImageMetadata.html#EC2.Paginator.DescribeInstanceImageMetadata)

```python
# DescribeInstanceImageMetadataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceImageMetadataPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceImageMetadataPaginator = client.get_paginator("describe_instance_image_metadata")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceImageMetadataResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceImageMetadataPaginator](./paginators.md#describeinstanceimagemetadatapaginator)
3. item: `AioPageIterator[DescribeInstanceImageMetadataResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceImageMetadataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceImageMetadataResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInstanceImageMetadataResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceImageMetadataRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceImageMetadataRequestPaginateTypeDef](./type_defs.md#describeinstanceimagemetadatarequestpaginatetypedef)
## DescribeInstanceStatusPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceStatus.html#EC2.Paginator.DescribeInstanceStatus)

```python
# DescribeInstanceStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceStatusPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceStatusPaginator = client.get_paginator("describe_instance_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceStatusResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceStatusPaginator](./paginators.md#describeinstancestatuspaginator)
3. item: `AioPageIterator[DescribeInstanceStatusResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeAllInstances: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceStatusResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInstanceStatusResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceStatusRequestPaginateTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceStatusRequestPaginateTypeDef](./type_defs.md#describeinstancestatusrequestpaginatetypedef)
## DescribeInstanceTopologyPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_topology")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceTopology.html#EC2.Paginator.DescribeInstanceTopology)

```python
# DescribeInstanceTopologyPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceTopologyPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceTopologyPaginator = client.get_paginator("describe_instance_topology")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceTopologyResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceTopologyPaginator](./paginators.md#describeinstancetopologypaginator)
3. item: `AioPageIterator[DescribeInstanceTopologyResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceTopologyPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    InstanceIds: Sequence[str] = ...,
    GroupNames: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceTopologyResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInstanceTopologyResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceTopologyRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceTopologyRequestPaginateTypeDef](./type_defs.md#describeinstancetopologyrequestpaginatetypedef)
## DescribeInstanceTypeOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_type_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceTypeOfferings.html#EC2.Paginator.DescribeInstanceTypeOfferings)

```python
# DescribeInstanceTypeOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceTypeOfferingsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceTypeOfferingsPaginator = client.get_paginator("describe_instance_type_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceTypeOfferingsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceTypeOfferingsPaginator](./paginators.md#describeinstancetypeofferingspaginator)
3. item: `AioPageIterator[DescribeInstanceTypeOfferingsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceTypeOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    LocationType: LocationTypeType = ...,  # (1)
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceTypeOfferingsResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype)
2. See `Sequence[FilterTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribeInstanceTypeOfferingsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceTypeOfferingsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceTypeOfferingsRequestPaginateTypeDef](./type_defs.md#describeinstancetypeofferingsrequestpaginatetypedef)
## DescribeInstanceTypesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstanceTypes.html#EC2.Paginator.DescribeInstanceTypes)

```python
# DescribeInstanceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstanceTypesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstanceTypesPaginator = client.get_paginator("describe_instance_types")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstanceTypesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstanceTypesPaginator](./paginators.md#describeinstancetypespaginator)
3. item: `AioPageIterator[DescribeInstanceTypesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstanceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    InstanceTypes: Sequence[InstanceTypeType] = ...,  # (1)
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstanceTypesResultTypeDef]:  # (4)
    ...
```

1. See `Sequence[InstanceTypeType]`
2. See `Sequence[FilterTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribeInstanceTypesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstanceTypesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceTypesRequestPaginateTypeDef](./type_defs.md#describeinstancetypesrequestpaginatetypedef)
## DescribeInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInstances.html#EC2.Paginator.DescribeInstances)

```python
# DescribeInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInstancesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInstancesPaginator = client.get_paginator("describe_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInstancesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInstancesPaginator](./paginators.md#describeinstancespaginator)
3. item: `AioPageIterator[DescribeInstancesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInstancesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInstancesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInstancesRequestPaginateTypeDef = {  # (1)
    "InstanceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesRequestPaginateTypeDef](./type_defs.md#describeinstancesrequestpaginatetypedef)
## DescribeInternetGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_internet_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeInternetGateways.html#EC2.Paginator.DescribeInternetGateways)

```python
# DescribeInternetGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeInternetGatewaysPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeInternetGatewaysPaginator = client.get_paginator("describe_internet_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeInternetGatewaysResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeInternetGatewaysPaginator](./paginators.md#describeinternetgatewayspaginator)
3. item: `AioPageIterator[DescribeInternetGatewaysResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeInternetGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    InternetGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeInternetGatewaysResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeInternetGatewaysResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeInternetGatewaysRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInternetGatewaysRequestPaginateTypeDef](./type_defs.md#describeinternetgatewaysrequestpaginatetypedef)
## DescribeIpamPoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpamPools.html#EC2.Paginator.DescribeIpamPools)

```python
# DescribeIpamPoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpamPoolsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpamPoolsPaginator = client.get_paginator("describe_ipam_pools")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpamPoolsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpamPoolsPaginator](./paginators.md#describeipampoolspaginator)
3. item: `AioPageIterator[DescribeIpamPoolsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpamPoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamPoolIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpamPoolsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpamPoolsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpamPoolsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamPoolsRequestPaginateTypeDef](./type_defs.md#describeipampoolsrequestpaginatetypedef)
## DescribeIpamPrefixListResolverTargetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_prefix_list_resolver_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpamPrefixListResolverTargets.html#EC2.Paginator.DescribeIpamPrefixListResolverTargets)

```python
# DescribeIpamPrefixListResolverTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpamPrefixListResolverTargetsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpamPrefixListResolverTargetsPaginator = client.get_paginator("describe_ipam_prefix_list_resolver_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpamPrefixListResolverTargetsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpamPrefixListResolverTargetsPaginator](./paginators.md#describeipamprefixlistresolvertargetspaginator)
3. item: `AioPageIterator[DescribeIpamPrefixListResolverTargetsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpamPrefixListResolverTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamPrefixListResolverTargetIds: Sequence[str] = ...,
    IpamPrefixListResolverId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpamPrefixListResolverTargetsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpamPrefixListResolverTargetsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpamPrefixListResolverTargetsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamPrefixListResolverTargetsRequestPaginateTypeDef](./type_defs.md#describeipamprefixlistresolvertargetsrequestpaginatetypedef)
## DescribeIpamPrefixListResolversPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_prefix_list_resolvers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpamPrefixListResolvers.html#EC2.Paginator.DescribeIpamPrefixListResolvers)

```python
# DescribeIpamPrefixListResolversPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpamPrefixListResolversPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpamPrefixListResolversPaginator = client.get_paginator("describe_ipam_prefix_list_resolvers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpamPrefixListResolversResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpamPrefixListResolversPaginator](./paginators.md#describeipamprefixlistresolverspaginator)
3. item: `AioPageIterator[DescribeIpamPrefixListResolversResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpamPrefixListResolversPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamPrefixListResolverIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpamPrefixListResolversResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpamPrefixListResolversResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpamPrefixListResolversRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamPrefixListResolversRequestPaginateTypeDef](./type_defs.md#describeipamprefixlistresolversrequestpaginatetypedef)
## DescribeIpamResourceDiscoveriesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_resource_discoveries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpamResourceDiscoveries.html#EC2.Paginator.DescribeIpamResourceDiscoveries)

```python
# DescribeIpamResourceDiscoveriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpamResourceDiscoveriesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpamResourceDiscoveriesPaginator = client.get_paginator("describe_ipam_resource_discoveries")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpamResourceDiscoveriesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpamResourceDiscoveriesPaginator](./paginators.md#describeipamresourcediscoveriespaginator)
3. item: `AioPageIterator[DescribeIpamResourceDiscoveriesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpamResourceDiscoveriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    IpamResourceDiscoveryIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpamResourceDiscoveriesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpamResourceDiscoveriesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpamResourceDiscoveriesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamResourceDiscoveriesRequestPaginateTypeDef](./type_defs.md#describeipamresourcediscoveriesrequestpaginatetypedef)
## DescribeIpamResourceDiscoveryAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_resource_discovery_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpamResourceDiscoveryAssociations.html#EC2.Paginator.DescribeIpamResourceDiscoveryAssociations)

```python
# DescribeIpamResourceDiscoveryAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpamResourceDiscoveryAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpamResourceDiscoveryAssociationsPaginator = client.get_paginator("describe_ipam_resource_discovery_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpamResourceDiscoveryAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpamResourceDiscoveryAssociationsPaginator](./paginators.md#describeipamresourcediscoveryassociationspaginator)
3. item: `AioPageIterator[DescribeIpamResourceDiscoveryAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpamResourceDiscoveryAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    IpamResourceDiscoveryAssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpamResourceDiscoveryAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpamResourceDiscoveryAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpamResourceDiscoveryAssociationsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamResourceDiscoveryAssociationsRequestPaginateTypeDef](./type_defs.md#describeipamresourcediscoveryassociationsrequestpaginatetypedef)
## DescribeIpamScopesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_scopes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpamScopes.html#EC2.Paginator.DescribeIpamScopes)

```python
# DescribeIpamScopesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpamScopesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpamScopesPaginator = client.get_paginator("describe_ipam_scopes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpamScopesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpamScopesPaginator](./paginators.md#describeipamscopespaginator)
3. item: `AioPageIterator[DescribeIpamScopesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpamScopesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamScopeIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpamScopesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpamScopesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpamScopesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamScopesRequestPaginateTypeDef](./type_defs.md#describeipamscopesrequestpaginatetypedef)
## DescribeIpamsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpams.html#EC2.Paginator.DescribeIpams)

```python
# DescribeIpamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpamsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpamsPaginator = client.get_paginator("describe_ipams")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpamsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpamsPaginator](./paginators.md#describeipamspaginator)
3. item: `AioPageIterator[DescribeIpamsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpamsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpamsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpamsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamsRequestPaginateTypeDef](./type_defs.md#describeipamsrequestpaginatetypedef)
## DescribeIpv6PoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipv6_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeIpv6Pools.html#EC2.Paginator.DescribeIpv6Pools)

```python
# DescribeIpv6PoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeIpv6PoolsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeIpv6PoolsPaginator = client.get_paginator("describe_ipv6_pools")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeIpv6PoolsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeIpv6PoolsPaginator](./paginators.md#describeipv6poolspaginator)
3. item: `AioPageIterator[DescribeIpv6PoolsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeIpv6PoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeIpv6PoolsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeIpv6PoolsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeIpv6PoolsRequestPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpv6PoolsRequestPaginateTypeDef](./type_defs.md#describeipv6poolsrequestpaginatetypedef)
## DescribeLaunchTemplateVersionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_launch_template_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLaunchTemplateVersions.html#EC2.Paginator.DescribeLaunchTemplateVersions)

```python
# DescribeLaunchTemplateVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLaunchTemplateVersionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLaunchTemplateVersionsPaginator = client.get_paginator("describe_launch_template_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLaunchTemplateVersionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLaunchTemplateVersionsPaginator](./paginators.md#describelaunchtemplateversionspaginator)
3. item: `AioPageIterator[DescribeLaunchTemplateVersionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLaunchTemplateVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    LaunchTemplateId: str = ...,
    LaunchTemplateName: str = ...,
    Versions: Sequence[str] = ...,
    MinVersion: str = ...,
    MaxVersion: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ResolveAlias: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLaunchTemplateVersionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLaunchTemplateVersionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLaunchTemplateVersionsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchTemplateVersionsRequestPaginateTypeDef](./type_defs.md#describelaunchtemplateversionsrequestpaginatetypedef)
## DescribeLaunchTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_launch_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLaunchTemplates.html#EC2.Paginator.DescribeLaunchTemplates)

```python
# DescribeLaunchTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLaunchTemplatesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLaunchTemplatesPaginator = client.get_paginator("describe_launch_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLaunchTemplatesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLaunchTemplatesPaginator](./paginators.md#describelaunchtemplatespaginator)
3. item: `AioPageIterator[DescribeLaunchTemplatesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLaunchTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    LaunchTemplateIds: Sequence[str] = ...,
    LaunchTemplateNames: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLaunchTemplatesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLaunchTemplatesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLaunchTemplatesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchTemplatesRequestPaginateTypeDef](./type_defs.md#describelaunchtemplatesrequestpaginatetypedef)
## DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_route_table_virtual_interface_group_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociations.html#EC2.Paginator.DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociations)

```python
# DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator = client.get_paginator("describe_local_gateway_route_table_virtual_interface_group_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator](./paginators.md#describelocalgatewayroutetablevirtualinterfacegroupassociationspaginator)
3. item: `AioPageIterator[DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LocalGatewayRouteTableVirtualInterfaceGroupAssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsRequestPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableVirtualInterfaceGroupAssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsRequestPaginateTypeDef](./type_defs.md#describelocalgatewayroutetablevirtualinterfacegroupassociationsrequestpaginatetypedef)
## DescribeLocalGatewayRouteTableVpcAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_route_table_vpc_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLocalGatewayRouteTableVpcAssociations.html#EC2.Paginator.DescribeLocalGatewayRouteTableVpcAssociations)

```python
# DescribeLocalGatewayRouteTableVpcAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLocalGatewayRouteTableVpcAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLocalGatewayRouteTableVpcAssociationsPaginator = client.get_paginator("describe_local_gateway_route_table_vpc_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLocalGatewayRouteTableVpcAssociationsPaginator](./paginators.md#describelocalgatewayroutetablevpcassociationspaginator)
3. item: `AioPageIterator[DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayRouteTableVpcAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LocalGatewayRouteTableVpcAssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLocalGatewayRouteTableVpcAssociationsRequestPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableVpcAssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayRouteTableVpcAssociationsRequestPaginateTypeDef](./type_defs.md#describelocalgatewayroutetablevpcassociationsrequestpaginatetypedef)
## DescribeLocalGatewayRouteTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_route_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLocalGatewayRouteTables.html#EC2.Paginator.DescribeLocalGatewayRouteTables)

```python
# DescribeLocalGatewayRouteTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLocalGatewayRouteTablesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLocalGatewayRouteTablesPaginator = client.get_paginator("describe_local_gateway_route_tables")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLocalGatewayRouteTablesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLocalGatewayRouteTablesPaginator](./paginators.md#describelocalgatewayroutetablespaginator)
3. item: `AioPageIterator[DescribeLocalGatewayRouteTablesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayRouteTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LocalGatewayRouteTableIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLocalGatewayRouteTablesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLocalGatewayRouteTablesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLocalGatewayRouteTablesRequestPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayRouteTablesRequestPaginateTypeDef](./type_defs.md#describelocalgatewayroutetablesrequestpaginatetypedef)
## DescribeLocalGatewayVirtualInterfaceGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_virtual_interface_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLocalGatewayVirtualInterfaceGroups.html#EC2.Paginator.DescribeLocalGatewayVirtualInterfaceGroups)

```python
# DescribeLocalGatewayVirtualInterfaceGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLocalGatewayVirtualInterfaceGroupsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLocalGatewayVirtualInterfaceGroupsPaginator = client.get_paginator("describe_local_gateway_virtual_interface_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLocalGatewayVirtualInterfaceGroupsPaginator](./paginators.md#describelocalgatewayvirtualinterfacegroupspaginator)
3. item: `AioPageIterator[DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayVirtualInterfaceGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LocalGatewayVirtualInterfaceGroupIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLocalGatewayVirtualInterfaceGroupsRequestPaginateTypeDef = {  # (1)
    "LocalGatewayVirtualInterfaceGroupIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayVirtualInterfaceGroupsRequestPaginateTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacegroupsrequestpaginatetypedef)
## DescribeLocalGatewayVirtualInterfacesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_virtual_interfaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLocalGatewayVirtualInterfaces.html#EC2.Paginator.DescribeLocalGatewayVirtualInterfaces)

```python
# DescribeLocalGatewayVirtualInterfacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLocalGatewayVirtualInterfacesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLocalGatewayVirtualInterfacesPaginator = client.get_paginator("describe_local_gateway_virtual_interfaces")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLocalGatewayVirtualInterfacesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLocalGatewayVirtualInterfacesPaginator](./paginators.md#describelocalgatewayvirtualinterfacespaginator)
3. item: `AioPageIterator[DescribeLocalGatewayVirtualInterfacesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayVirtualInterfacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LocalGatewayVirtualInterfaceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLocalGatewayVirtualInterfacesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLocalGatewayVirtualInterfacesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLocalGatewayVirtualInterfacesRequestPaginateTypeDef = {  # (1)
    "LocalGatewayVirtualInterfaceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayVirtualInterfacesRequestPaginateTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacesrequestpaginatetypedef)
## DescribeLocalGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeLocalGateways.html#EC2.Paginator.DescribeLocalGateways)

```python
# DescribeLocalGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeLocalGatewaysPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeLocalGatewaysPaginator = client.get_paginator("describe_local_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLocalGatewaysResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeLocalGatewaysPaginator](./paginators.md#describelocalgatewayspaginator)
3. item: `AioPageIterator[DescribeLocalGatewaysResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LocalGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeLocalGatewaysResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeLocalGatewaysResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLocalGatewaysRequestPaginateTypeDef = {  # (1)
    "LocalGatewayIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewaysRequestPaginateTypeDef](./type_defs.md#describelocalgatewaysrequestpaginatetypedef)
## DescribeMacHostsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_mac_hosts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeMacHosts.html#EC2.Paginator.DescribeMacHosts)

```python
# DescribeMacHostsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeMacHostsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeMacHostsPaginator = client.get_paginator("describe_mac_hosts")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMacHostsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeMacHostsPaginator](./paginators.md#describemachostspaginator)
3. item: `AioPageIterator[DescribeMacHostsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeMacHostsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    HostIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeMacHostsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeMacHostsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMacHostsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMacHostsRequestPaginateTypeDef](./type_defs.md#describemachostsrequestpaginatetypedef)
## DescribeMacModificationTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_mac_modification_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeMacModificationTasks.html#EC2.Paginator.DescribeMacModificationTasks)

```python
# DescribeMacModificationTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeMacModificationTasksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeMacModificationTasksPaginator = client.get_paginator("describe_mac_modification_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMacModificationTasksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeMacModificationTasksPaginator](./paginators.md#describemacmodificationtaskspaginator)
3. item: `AioPageIterator[DescribeMacModificationTasksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeMacModificationTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MacModificationTaskIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeMacModificationTasksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeMacModificationTasksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMacModificationTasksRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMacModificationTasksRequestPaginateTypeDef](./type_defs.md#describemacmodificationtasksrequestpaginatetypedef)
## DescribeManagedPrefixListsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_managed_prefix_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeManagedPrefixLists.html#EC2.Paginator.DescribeManagedPrefixLists)

```python
# DescribeManagedPrefixListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeManagedPrefixListsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeManagedPrefixListsPaginator = client.get_paginator("describe_managed_prefix_lists")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeManagedPrefixListsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeManagedPrefixListsPaginator](./paginators.md#describemanagedprefixlistspaginator)
3. item: `AioPageIterator[DescribeManagedPrefixListsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeManagedPrefixListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PrefixListIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeManagedPrefixListsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeManagedPrefixListsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeManagedPrefixListsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeManagedPrefixListsRequestPaginateTypeDef](./type_defs.md#describemanagedprefixlistsrequestpaginatetypedef)
## DescribeMovingAddressesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_moving_addresses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeMovingAddresses.html#EC2.Paginator.DescribeMovingAddresses)

```python
# DescribeMovingAddressesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeMovingAddressesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeMovingAddressesPaginator = client.get_paginator("describe_moving_addresses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMovingAddressesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeMovingAddressesPaginator](./paginators.md#describemovingaddressespaginator)
3. item: `AioPageIterator[DescribeMovingAddressesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeMovingAddressesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    PublicIps: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeMovingAddressesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeMovingAddressesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMovingAddressesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMovingAddressesRequestPaginateTypeDef](./type_defs.md#describemovingaddressesrequestpaginatetypedef)
## DescribeNatGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_nat_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNatGateways.html#EC2.Paginator.DescribeNatGateways)

```python
# DescribeNatGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNatGatewaysPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNatGatewaysPaginator = client.get_paginator("describe_nat_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNatGatewaysResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNatGatewaysPaginator](./paginators.md#describenatgatewayspaginator)
3. item: `AioPageIterator[DescribeNatGatewaysResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNatGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NatGatewayIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNatGatewaysResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNatGatewaysResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNatGatewaysRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNatGatewaysRequestPaginateTypeDef](./type_defs.md#describenatgatewaysrequestpaginatetypedef)
## DescribeNetworkAclsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_acls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNetworkAcls.html#EC2.Paginator.DescribeNetworkAcls)

```python
# DescribeNetworkAclsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNetworkAclsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNetworkAclsPaginator = client.get_paginator("describe_network_acls")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNetworkAclsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNetworkAclsPaginator](./paginators.md#describenetworkaclspaginator)
3. item: `AioPageIterator[DescribeNetworkAclsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNetworkAclsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    NetworkAclIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNetworkAclsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNetworkAclsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNetworkAclsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkAclsRequestPaginateTypeDef](./type_defs.md#describenetworkaclsrequestpaginatetypedef)
## DescribeNetworkInsightsAccessScopeAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_access_scope_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNetworkInsightsAccessScopeAnalyses.html#EC2.Paginator.DescribeNetworkInsightsAccessScopeAnalyses)

```python
# DescribeNetworkInsightsAccessScopeAnalysesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNetworkInsightsAccessScopeAnalysesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNetworkInsightsAccessScopeAnalysesPaginator = client.get_paginator("describe_network_insights_access_scope_analyses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNetworkInsightsAccessScopeAnalysesPaginator](./paginators.md#describenetworkinsightsaccessscopeanalysespaginator)
3. item: `AioPageIterator[DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsAccessScopeAnalysesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NetworkInsightsAccessScopeAnalysisIds: Sequence[str] = ...,
    NetworkInsightsAccessScopeId: str = ...,
    AnalysisStartTimeBegin: TimestampTypeDef = ...,
    AnalysisStartTimeEnd: TimestampTypeDef = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNetworkInsightsAccessScopeAnalysesRequestPaginateTypeDef = {  # (1)
    "NetworkInsightsAccessScopeAnalysisIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsAccessScopeAnalysesRequestPaginateTypeDef](./type_defs.md#describenetworkinsightsaccessscopeanalysesrequestpaginatetypedef)
## DescribeNetworkInsightsAccessScopesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_access_scopes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNetworkInsightsAccessScopes.html#EC2.Paginator.DescribeNetworkInsightsAccessScopes)

```python
# DescribeNetworkInsightsAccessScopesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNetworkInsightsAccessScopesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNetworkInsightsAccessScopesPaginator = client.get_paginator("describe_network_insights_access_scopes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNetworkInsightsAccessScopesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNetworkInsightsAccessScopesPaginator](./paginators.md#describenetworkinsightsaccessscopespaginator)
3. item: `AioPageIterator[DescribeNetworkInsightsAccessScopesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsAccessScopesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NetworkInsightsAccessScopeIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNetworkInsightsAccessScopesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNetworkInsightsAccessScopesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNetworkInsightsAccessScopesRequestPaginateTypeDef = {  # (1)
    "NetworkInsightsAccessScopeIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsAccessScopesRequestPaginateTypeDef](./type_defs.md#describenetworkinsightsaccessscopesrequestpaginatetypedef)
## DescribeNetworkInsightsAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNetworkInsightsAnalyses.html#EC2.Paginator.DescribeNetworkInsightsAnalyses)

```python
# DescribeNetworkInsightsAnalysesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNetworkInsightsAnalysesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNetworkInsightsAnalysesPaginator = client.get_paginator("describe_network_insights_analyses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNetworkInsightsAnalysesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNetworkInsightsAnalysesPaginator](./paginators.md#describenetworkinsightsanalysespaginator)
3. item: `AioPageIterator[DescribeNetworkInsightsAnalysesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsAnalysesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NetworkInsightsAnalysisIds: Sequence[str] = ...,
    NetworkInsightsPathId: str = ...,
    AnalysisStartTime: TimestampTypeDef = ...,
    AnalysisEndTime: TimestampTypeDef = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNetworkInsightsAnalysesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNetworkInsightsAnalysesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNetworkInsightsAnalysesRequestPaginateTypeDef = {  # (1)
    "NetworkInsightsAnalysisIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsAnalysesRequestPaginateTypeDef](./type_defs.md#describenetworkinsightsanalysesrequestpaginatetypedef)
## DescribeNetworkInsightsPathsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_paths")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNetworkInsightsPaths.html#EC2.Paginator.DescribeNetworkInsightsPaths)

```python
# DescribeNetworkInsightsPathsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNetworkInsightsPathsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNetworkInsightsPathsPaginator = client.get_paginator("describe_network_insights_paths")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNetworkInsightsPathsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNetworkInsightsPathsPaginator](./paginators.md#describenetworkinsightspathspaginator)
3. item: `AioPageIterator[DescribeNetworkInsightsPathsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsPathsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NetworkInsightsPathIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNetworkInsightsPathsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNetworkInsightsPathsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNetworkInsightsPathsRequestPaginateTypeDef = {  # (1)
    "NetworkInsightsPathIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsPathsRequestPaginateTypeDef](./type_defs.md#describenetworkinsightspathsrequestpaginatetypedef)
## DescribeNetworkInterfacePermissionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_interface_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNetworkInterfacePermissions.html#EC2.Paginator.DescribeNetworkInterfacePermissions)

```python
# DescribeNetworkInterfacePermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNetworkInterfacePermissionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNetworkInterfacePermissionsPaginator = client.get_paginator("describe_network_interface_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNetworkInterfacePermissionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNetworkInterfacePermissionsPaginator](./paginators.md#describenetworkinterfacepermissionspaginator)
3. item: `AioPageIterator[DescribeNetworkInterfacePermissionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNetworkInterfacePermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NetworkInterfacePermissionIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNetworkInterfacePermissionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNetworkInterfacePermissionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNetworkInterfacePermissionsRequestPaginateTypeDef = {  # (1)
    "NetworkInterfacePermissionIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInterfacePermissionsRequestPaginateTypeDef](./type_defs.md#describenetworkinterfacepermissionsrequestpaginatetypedef)
## DescribeNetworkInterfacesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_interfaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeNetworkInterfaces.html#EC2.Paginator.DescribeNetworkInterfaces)

```python
# DescribeNetworkInterfacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeNetworkInterfacesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeNetworkInterfacesPaginator = client.get_paginator("describe_network_interfaces")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeNetworkInterfacesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeNetworkInterfacesPaginator](./paginators.md#describenetworkinterfacespaginator)
3. item: `AioPageIterator[DescribeNetworkInterfacesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeNetworkInterfacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    NetworkInterfaceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeNetworkInterfacesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeNetworkInterfacesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeNetworkInterfacesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInterfacesRequestPaginateTypeDef](./type_defs.md#describenetworkinterfacesrequestpaginatetypedef)
## DescribePrefixListsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_prefix_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribePrefixLists.html#EC2.Paginator.DescribePrefixLists)

```python
# DescribePrefixListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribePrefixListsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribePrefixListsPaginator = client.get_paginator("describe_prefix_lists")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePrefixListsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribePrefixListsPaginator](./paginators.md#describeprefixlistspaginator)
3. item: `AioPageIterator[DescribePrefixListsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribePrefixListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PrefixListIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribePrefixListsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribePrefixListsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribePrefixListsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePrefixListsRequestPaginateTypeDef](./type_defs.md#describeprefixlistsrequestpaginatetypedef)
## DescribePrincipalIdFormatPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_principal_id_format")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribePrincipalIdFormat.html#EC2.Paginator.DescribePrincipalIdFormat)

```python
# DescribePrincipalIdFormatPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribePrincipalIdFormatPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribePrincipalIdFormatPaginator = client.get_paginator("describe_principal_id_format")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePrincipalIdFormatResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribePrincipalIdFormatPaginator](./paginators.md#describeprincipalidformatpaginator)
3. item: `AioPageIterator[DescribePrincipalIdFormatResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribePrincipalIdFormatPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Resources: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribePrincipalIdFormatResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribePrincipalIdFormatResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribePrincipalIdFormatRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePrincipalIdFormatRequestPaginateTypeDef](./type_defs.md#describeprincipalidformatrequestpaginatetypedef)
## DescribePublicIpv4PoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_public_ipv4_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribePublicIpv4Pools.html#EC2.Paginator.DescribePublicIpv4Pools)

```python
# DescribePublicIpv4PoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribePublicIpv4PoolsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribePublicIpv4PoolsPaginator = client.get_paginator("describe_public_ipv4_pools")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePublicIpv4PoolsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribePublicIpv4PoolsPaginator](./paginators.md#describepublicipv4poolspaginator)
3. item: `AioPageIterator[DescribePublicIpv4PoolsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribePublicIpv4PoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribePublicIpv4PoolsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribePublicIpv4PoolsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribePublicIpv4PoolsRequestPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePublicIpv4PoolsRequestPaginateTypeDef](./type_defs.md#describepublicipv4poolsrequestpaginatetypedef)
## DescribeReplaceRootVolumeTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_replace_root_volume_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeReplaceRootVolumeTasks.html#EC2.Paginator.DescribeReplaceRootVolumeTasks)

```python
# DescribeReplaceRootVolumeTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeReplaceRootVolumeTasksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeReplaceRootVolumeTasksPaginator = client.get_paginator("describe_replace_root_volume_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReplaceRootVolumeTasksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeReplaceRootVolumeTasksPaginator](./paginators.md#describereplacerootvolumetaskspaginator)
3. item: `AioPageIterator[DescribeReplaceRootVolumeTasksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeReplaceRootVolumeTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReplaceRootVolumeTaskIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeReplaceRootVolumeTasksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeReplaceRootVolumeTasksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReplaceRootVolumeTasksRequestPaginateTypeDef = {  # (1)
    "ReplaceRootVolumeTaskIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplaceRootVolumeTasksRequestPaginateTypeDef](./type_defs.md#describereplacerootvolumetasksrequestpaginatetypedef)
## DescribeReservedInstancesModificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_reserved_instances_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeReservedInstancesModifications.html#EC2.Paginator.DescribeReservedInstancesModifications)

```python
# DescribeReservedInstancesModificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeReservedInstancesModificationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeReservedInstancesModificationsPaginator = client.get_paginator("describe_reserved_instances_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedInstancesModificationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeReservedInstancesModificationsPaginator](./paginators.md#describereservedinstancesmodificationspaginator)
3. item: `AioPageIterator[DescribeReservedInstancesModificationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeReservedInstancesModificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ReservedInstancesModificationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeReservedInstancesModificationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeReservedInstancesModificationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedInstancesModificationsRequestPaginateTypeDef = {  # (1)
    "ReservedInstancesModificationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedInstancesModificationsRequestPaginateTypeDef](./type_defs.md#describereservedinstancesmodificationsrequestpaginatetypedef)
## DescribeReservedInstancesOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_reserved_instances_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeReservedInstancesOfferings.html#EC2.Paginator.DescribeReservedInstancesOfferings)

```python
# DescribeReservedInstancesOfferingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeReservedInstancesOfferingsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeReservedInstancesOfferingsPaginator = client.get_paginator("describe_reserved_instances_offerings")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeReservedInstancesOfferingsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeReservedInstancesOfferingsPaginator](./paginators.md#describereservedinstancesofferingspaginator)
3. item: `AioPageIterator[DescribeReservedInstancesOfferingsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeReservedInstancesOfferingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AvailabilityZone: str = ...,
    IncludeMarketplace: bool = ...,
    InstanceType: InstanceTypeType = ...,  # (1)
    MaxDuration: int = ...,
    MaxInstanceCount: int = ...,
    MinDuration: int = ...,
    OfferingClass: OfferingClassTypeType = ...,  # (2)
    ProductDescription: RIProductDescriptionType = ...,  # (3)
    ReservedInstancesOfferingIds: Sequence[str] = ...,
    AvailabilityZoneId: str = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (4)
    InstanceTenancy: TenancyType = ...,  # (5)
    OfferingType: OfferingTypeValuesType = ...,  # (6)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (7)
) -> aiobotocore.paginate.AioPageIterator[DescribeReservedInstancesOfferingsResultTypeDef]:  # (8)
    ...
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype)
2. See [:material-code-brackets: OfferingClassTypeType](./literals.md#offeringclasstypetype)
3. See [:material-code-brackets: RIProductDescriptionType](./literals.md#riproductdescriptiontype)
4. See `Sequence[FilterTypeDef]`
5. See [:material-code-brackets: TenancyType](./literals.md#tenancytype)
6. See [:material-code-brackets: OfferingTypeValuesType](./literals.md#offeringtypevaluestype)
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
8. See `AioPageIterator[DescribeReservedInstancesOfferingsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeReservedInstancesOfferingsRequestPaginateTypeDef = {  # (1)
    "AvailabilityZone": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedInstancesOfferingsRequestPaginateTypeDef](./type_defs.md#describereservedinstancesofferingsrequestpaginatetypedef)
## DescribeRouteServerEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_route_server_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeRouteServerEndpoints.html#EC2.Paginator.DescribeRouteServerEndpoints)

```python
# DescribeRouteServerEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeRouteServerEndpointsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeRouteServerEndpointsPaginator = client.get_paginator("describe_route_server_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRouteServerEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeRouteServerEndpointsPaginator](./paginators.md#describerouteserverendpointspaginator)
3. item: `AioPageIterator[DescribeRouteServerEndpointsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRouteServerEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RouteServerEndpointIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRouteServerEndpointsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRouteServerEndpointsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRouteServerEndpointsRequestPaginateTypeDef = {  # (1)
    "RouteServerEndpointIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRouteServerEndpointsRequestPaginateTypeDef](./type_defs.md#describerouteserverendpointsrequestpaginatetypedef)
## DescribeRouteServerPeersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_route_server_peers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeRouteServerPeers.html#EC2.Paginator.DescribeRouteServerPeers)

```python
# DescribeRouteServerPeersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeRouteServerPeersPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeRouteServerPeersPaginator = client.get_paginator("describe_route_server_peers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRouteServerPeersResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeRouteServerPeersPaginator](./paginators.md#describerouteserverpeerspaginator)
3. item: `AioPageIterator[DescribeRouteServerPeersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRouteServerPeersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RouteServerPeerIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRouteServerPeersResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRouteServerPeersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRouteServerPeersRequestPaginateTypeDef = {  # (1)
    "RouteServerPeerIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRouteServerPeersRequestPaginateTypeDef](./type_defs.md#describerouteserverpeersrequestpaginatetypedef)
## DescribeRouteServersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_route_servers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeRouteServers.html#EC2.Paginator.DescribeRouteServers)

```python
# DescribeRouteServersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeRouteServersPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeRouteServersPaginator = client.get_paginator("describe_route_servers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRouteServersResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeRouteServersPaginator](./paginators.md#describerouteserverspaginator)
3. item: `AioPageIterator[DescribeRouteServersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRouteServersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RouteServerIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRouteServersResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRouteServersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRouteServersRequestPaginateTypeDef = {  # (1)
    "RouteServerIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRouteServersRequestPaginateTypeDef](./type_defs.md#describerouteserversrequestpaginatetypedef)
## DescribeRouteTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_route_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeRouteTables.html#EC2.Paginator.DescribeRouteTables)

```python
# DescribeRouteTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeRouteTablesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeRouteTablesPaginator = client.get_paginator("describe_route_tables")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRouteTablesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeRouteTablesPaginator](./paginators.md#describeroutetablespaginator)
3. item: `AioPageIterator[DescribeRouteTablesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRouteTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    RouteTableIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRouteTablesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRouteTablesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRouteTablesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRouteTablesRequestPaginateTypeDef](./type_defs.md#describeroutetablesrequestpaginatetypedef)
## DescribeScheduledInstanceAvailabilityPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_scheduled_instance_availability")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeScheduledInstanceAvailability.html#EC2.Paginator.DescribeScheduledInstanceAvailability)

```python
# DescribeScheduledInstanceAvailabilityPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeScheduledInstanceAvailabilityPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeScheduledInstanceAvailabilityPaginator = client.get_paginator("describe_scheduled_instance_availability")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScheduledInstanceAvailabilityResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeScheduledInstanceAvailabilityPaginator](./paginators.md#describescheduledinstanceavailabilitypaginator)
3. item: `AioPageIterator[DescribeScheduledInstanceAvailabilityResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeScheduledInstanceAvailabilityPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    FirstSlotStartTimeRange: SlotDateTimeRangeRequestTypeDef,  # (1)
    Recurrence: ScheduledInstanceRecurrenceRequestTypeDef,  # (2)
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (3)
    MaxSlotDurationInHours: int = ...,
    MinSlotDurationInHours: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[DescribeScheduledInstanceAvailabilityResultTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: SlotDateTimeRangeRequestTypeDef](./type_defs.md#slotdatetimerangerequesttypedef)
2. See [:material-code-braces: ScheduledInstanceRecurrenceRequestTypeDef](./type_defs.md#scheduledinstancerecurrencerequesttypedef)
3. See `Sequence[FilterTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[DescribeScheduledInstanceAvailabilityResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScheduledInstanceAvailabilityRequestPaginateTypeDef = {  # (1)
    "FirstSlotStartTimeRange": ...,
    "Recurrence": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledInstanceAvailabilityRequestPaginateTypeDef](./type_defs.md#describescheduledinstanceavailabilityrequestpaginatetypedef)
## DescribeScheduledInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_scheduled_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeScheduledInstances.html#EC2.Paginator.DescribeScheduledInstances)

```python
# DescribeScheduledInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeScheduledInstancesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeScheduledInstancesPaginator = client.get_paginator("describe_scheduled_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeScheduledInstancesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeScheduledInstancesPaginator](./paginators.md#describescheduledinstancespaginator)
3. item: `AioPageIterator[DescribeScheduledInstancesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeScheduledInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ScheduledInstanceIds: Sequence[str] = ...,
    SlotStartTimeRange: SlotStartTimeRangeRequestTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribeScheduledInstancesResultTypeDef]:  # (4)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: SlotStartTimeRangeRequestTypeDef](./type_defs.md#slotstarttimerangerequesttypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribeScheduledInstancesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeScheduledInstancesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledInstancesRequestPaginateTypeDef](./type_defs.md#describescheduledinstancesrequestpaginatetypedef)
## DescribeSecurityGroupRulesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_security_group_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSecurityGroupRules.html#EC2.Paginator.DescribeSecurityGroupRules)

```python
# DescribeSecurityGroupRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSecurityGroupRulesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSecurityGroupRulesPaginator = client.get_paginator("describe_security_group_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSecurityGroupRulesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSecurityGroupRulesPaginator](./paginators.md#describesecuritygrouprulespaginator)
3. item: `AioPageIterator[DescribeSecurityGroupRulesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSecurityGroupRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SecurityGroupRuleIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSecurityGroupRulesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSecurityGroupRulesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSecurityGroupRulesRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityGroupRulesRequestPaginateTypeDef](./type_defs.md#describesecuritygrouprulesrequestpaginatetypedef)
## DescribeSecurityGroupVpcAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_security_group_vpc_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSecurityGroupVpcAssociations.html#EC2.Paginator.DescribeSecurityGroupVpcAssociations)

```python
# DescribeSecurityGroupVpcAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSecurityGroupVpcAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSecurityGroupVpcAssociationsPaginator = client.get_paginator("describe_security_group_vpc_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSecurityGroupVpcAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSecurityGroupVpcAssociationsPaginator](./paginators.md#describesecuritygroupvpcassociationspaginator)
3. item: `AioPageIterator[DescribeSecurityGroupVpcAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSecurityGroupVpcAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSecurityGroupVpcAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSecurityGroupVpcAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSecurityGroupVpcAssociationsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityGroupVpcAssociationsRequestPaginateTypeDef](./type_defs.md#describesecuritygroupvpcassociationsrequestpaginatetypedef)
## DescribeSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSecurityGroups.html#EC2.Paginator.DescribeSecurityGroups)

```python
# DescribeSecurityGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSecurityGroupsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSecurityGroupsPaginator = client.get_paginator("describe_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSecurityGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSecurityGroupsPaginator](./paginators.md#describesecuritygroupspaginator)
3. item: `AioPageIterator[DescribeSecurityGroupsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSecurityGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupIds: Sequence[str] = ...,
    GroupNames: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSecurityGroupsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSecurityGroupsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSecurityGroupsRequestPaginateTypeDef = {  # (1)
    "GroupIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityGroupsRequestPaginateTypeDef](./type_defs.md#describesecuritygroupsrequestpaginatetypedef)
## DescribeSnapshotTierStatusPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_snapshot_tier_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSnapshotTierStatus.html#EC2.Paginator.DescribeSnapshotTierStatus)

```python
# DescribeSnapshotTierStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSnapshotTierStatusPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSnapshotTierStatusPaginator = client.get_paginator("describe_snapshot_tier_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotTierStatusResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSnapshotTierStatusPaginator](./paginators.md#describesnapshottierstatuspaginator)
3. item: `AioPageIterator[DescribeSnapshotTierStatusResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSnapshotTierStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSnapshotTierStatusResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSnapshotTierStatusResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotTierStatusRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotTierStatusRequestPaginateTypeDef](./type_defs.md#describesnapshottierstatusrequestpaginatetypedef)
## DescribeSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSnapshots.html#EC2.Paginator.DescribeSnapshots)

```python
# DescribeSnapshotsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSnapshotsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSnapshotsPaginator = client.get_paginator("describe_snapshots")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSnapshotsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSnapshotsPaginator](./paginators.md#describesnapshotspaginator)
3. item: `AioPageIterator[DescribeSnapshotsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSnapshotsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OwnerIds: Sequence[str] = ...,
    RestorableByUserIds: Sequence[str] = ...,
    SnapshotIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSnapshotsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSnapshotsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSnapshotsRequestPaginateTypeDef = {  # (1)
    "OwnerIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestPaginateTypeDef](./type_defs.md#describesnapshotsrequestpaginatetypedef)
## DescribeSpotFleetInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_fleet_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSpotFleetInstances.html#EC2.Paginator.DescribeSpotFleetInstances)

```python
# DescribeSpotFleetInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSpotFleetInstancesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSpotFleetInstancesPaginator = client.get_paginator("describe_spot_fleet_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSpotFleetInstancesResponseTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSpotFleetInstancesPaginator](./paginators.md#describespotfleetinstancespaginator)
3. item: `AioPageIterator[DescribeSpotFleetInstancesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSpotFleetInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SpotFleetRequestId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeSpotFleetInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeSpotFleetInstancesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSpotFleetInstancesRequestPaginateTypeDef = {  # (1)
    "SpotFleetRequestId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotFleetInstancesRequestPaginateTypeDef](./type_defs.md#describespotfleetinstancesrequestpaginatetypedef)
## DescribeSpotFleetRequestsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_fleet_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSpotFleetRequests.html#EC2.Paginator.DescribeSpotFleetRequests)

```python
# DescribeSpotFleetRequestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSpotFleetRequestsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSpotFleetRequestsPaginator = client.get_paginator("describe_spot_fleet_requests")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSpotFleetRequestsResponseTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSpotFleetRequestsPaginator](./paginators.md#describespotfleetrequestspaginator)
3. item: `AioPageIterator[DescribeSpotFleetRequestsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSpotFleetRequestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    SpotFleetRequestIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeSpotFleetRequestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeSpotFleetRequestsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSpotFleetRequestsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotFleetRequestsRequestPaginateTypeDef](./type_defs.md#describespotfleetrequestsrequestpaginatetypedef)
## DescribeSpotInstanceRequestsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_instance_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSpotInstanceRequests.html#EC2.Paginator.DescribeSpotInstanceRequests)

```python
# DescribeSpotInstanceRequestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSpotInstanceRequestsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSpotInstanceRequestsPaginator = client.get_paginator("describe_spot_instance_requests")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSpotInstanceRequestsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSpotInstanceRequestsPaginator](./paginators.md#describespotinstancerequestspaginator)
3. item: `AioPageIterator[DescribeSpotInstanceRequestsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSpotInstanceRequestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    SpotInstanceRequestIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSpotInstanceRequestsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSpotInstanceRequestsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSpotInstanceRequestsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotInstanceRequestsRequestPaginateTypeDef](./type_defs.md#describespotinstancerequestsrequestpaginatetypedef)
## DescribeSpotPriceHistoryPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_price_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSpotPriceHistory.html#EC2.Paginator.DescribeSpotPriceHistory)

```python
# DescribeSpotPriceHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSpotPriceHistoryPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSpotPriceHistoryPaginator = client.get_paginator("describe_spot_price_history")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSpotPriceHistoryResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSpotPriceHistoryPaginator](./paginators.md#describespotpricehistorypaginator)
3. item: `AioPageIterator[DescribeSpotPriceHistoryResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSpotPriceHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AvailabilityZoneId: str = ...,
    DryRun: bool = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    InstanceTypes: Sequence[InstanceTypeType] = ...,  # (1)
    ProductDescriptions: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    AvailabilityZone: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribeSpotPriceHistoryResultTypeDef]:  # (4)
    ...
```

1. See `Sequence[InstanceTypeType]`
2. See `Sequence[FilterTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribeSpotPriceHistoryResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSpotPriceHistoryRequestPaginateTypeDef = {  # (1)
    "AvailabilityZoneId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotPriceHistoryRequestPaginateTypeDef](./type_defs.md#describespotpricehistoryrequestpaginatetypedef)
## DescribeStaleSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_stale_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeStaleSecurityGroups.html#EC2.Paginator.DescribeStaleSecurityGroups)

```python
# DescribeStaleSecurityGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeStaleSecurityGroupsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeStaleSecurityGroupsPaginator = client.get_paginator("describe_stale_security_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStaleSecurityGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeStaleSecurityGroupsPaginator](./paginators.md#describestalesecuritygroupspaginator)
3. item: `AioPageIterator[DescribeStaleSecurityGroupsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeStaleSecurityGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VpcId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeStaleSecurityGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeStaleSecurityGroupsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStaleSecurityGroupsRequestPaginateTypeDef = {  # (1)
    "VpcId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStaleSecurityGroupsRequestPaginateTypeDef](./type_defs.md#describestalesecuritygroupsrequestpaginatetypedef)
## DescribeStoreImageTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_store_image_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeStoreImageTasks.html#EC2.Paginator.DescribeStoreImageTasks)

```python
# DescribeStoreImageTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeStoreImageTasksPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeStoreImageTasksPaginator = client.get_paginator("describe_store_image_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeStoreImageTasksResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeStoreImageTasksPaginator](./paginators.md#describestoreimagetaskspaginator)
3. item: `AioPageIterator[DescribeStoreImageTasksResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeStoreImageTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeStoreImageTasksResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeStoreImageTasksResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeStoreImageTasksRequestPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStoreImageTasksRequestPaginateTypeDef](./type_defs.md#describestoreimagetasksrequestpaginatetypedef)
## DescribeSubnetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_subnets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeSubnets.html#EC2.Paginator.DescribeSubnets)

```python
# DescribeSubnetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeSubnetsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeSubnetsPaginator = client.get_paginator("describe_subnets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSubnetsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeSubnetsPaginator](./paginators.md#describesubnetspaginator)
3. item: `AioPageIterator[DescribeSubnetsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSubnetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SubnetIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeSubnetsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeSubnetsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSubnetsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubnetsRequestPaginateTypeDef](./type_defs.md#describesubnetsrequestpaginatetypedef)
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTags.html#EC2.Paginator.DescribeTags)

```python
# DescribeTagsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTagsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTagsPaginator = client.get_paginator("describe_tags")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTagsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTagsPaginator](./paginators.md#describetagspaginator)
3. item: `AioPageIterator[DescribeTagsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTagsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTagsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTagsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestPaginateTypeDef](./type_defs.md#describetagsrequestpaginatetypedef)
## DescribeTrafficMirrorFiltersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_traffic_mirror_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTrafficMirrorFilters.html#EC2.Paginator.DescribeTrafficMirrorFilters)

```python
# DescribeTrafficMirrorFiltersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTrafficMirrorFiltersPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTrafficMirrorFiltersPaginator = client.get_paginator("describe_traffic_mirror_filters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTrafficMirrorFiltersResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTrafficMirrorFiltersPaginator](./paginators.md#describetrafficmirrorfilterspaginator)
3. item: `AioPageIterator[DescribeTrafficMirrorFiltersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTrafficMirrorFiltersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TrafficMirrorFilterIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTrafficMirrorFiltersResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTrafficMirrorFiltersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTrafficMirrorFiltersRequestPaginateTypeDef = {  # (1)
    "TrafficMirrorFilterIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrafficMirrorFiltersRequestPaginateTypeDef](./type_defs.md#describetrafficmirrorfiltersrequestpaginatetypedef)
## DescribeTrafficMirrorSessionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_traffic_mirror_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTrafficMirrorSessions.html#EC2.Paginator.DescribeTrafficMirrorSessions)

```python
# DescribeTrafficMirrorSessionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTrafficMirrorSessionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTrafficMirrorSessionsPaginator = client.get_paginator("describe_traffic_mirror_sessions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTrafficMirrorSessionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTrafficMirrorSessionsPaginator](./paginators.md#describetrafficmirrorsessionspaginator)
3. item: `AioPageIterator[DescribeTrafficMirrorSessionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTrafficMirrorSessionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TrafficMirrorSessionIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTrafficMirrorSessionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTrafficMirrorSessionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTrafficMirrorSessionsRequestPaginateTypeDef = {  # (1)
    "TrafficMirrorSessionIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrafficMirrorSessionsRequestPaginateTypeDef](./type_defs.md#describetrafficmirrorsessionsrequestpaginatetypedef)
## DescribeTrafficMirrorTargetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_traffic_mirror_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTrafficMirrorTargets.html#EC2.Paginator.DescribeTrafficMirrorTargets)

```python
# DescribeTrafficMirrorTargetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTrafficMirrorTargetsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTrafficMirrorTargetsPaginator = client.get_paginator("describe_traffic_mirror_targets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTrafficMirrorTargetsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTrafficMirrorTargetsPaginator](./paginators.md#describetrafficmirrortargetspaginator)
3. item: `AioPageIterator[DescribeTrafficMirrorTargetsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTrafficMirrorTargetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TrafficMirrorTargetIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTrafficMirrorTargetsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTrafficMirrorTargetsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTrafficMirrorTargetsRequestPaginateTypeDef = {  # (1)
    "TrafficMirrorTargetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrafficMirrorTargetsRequestPaginateTypeDef](./type_defs.md#describetrafficmirrortargetsrequestpaginatetypedef)
## DescribeTransitGatewayAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayAttachments.html#EC2.Paginator.DescribeTransitGatewayAttachments)

```python
# DescribeTransitGatewayAttachmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayAttachmentsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayAttachmentsPaginator = client.get_paginator("describe_transit_gateway_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayAttachmentsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayAttachmentsPaginator](./paginators.md#describetransitgatewayattachmentspaginator)
3. item: `AioPageIterator[DescribeTransitGatewayAttachmentsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayAttachmentsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayAttachmentsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayAttachmentsRequestPaginateTypeDef](./type_defs.md#describetransitgatewayattachmentsrequestpaginatetypedef)
## DescribeTransitGatewayConnectPeersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_connect_peers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayConnectPeers.html#EC2.Paginator.DescribeTransitGatewayConnectPeers)

```python
# DescribeTransitGatewayConnectPeersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayConnectPeersPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayConnectPeersPaginator = client.get_paginator("describe_transit_gateway_connect_peers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayConnectPeersResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayConnectPeersPaginator](./paginators.md#describetransitgatewayconnectpeerspaginator)
3. item: `AioPageIterator[DescribeTransitGatewayConnectPeersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayConnectPeersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayConnectPeerIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayConnectPeersResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayConnectPeersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayConnectPeersRequestPaginateTypeDef = {  # (1)
    "TransitGatewayConnectPeerIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayConnectPeersRequestPaginateTypeDef](./type_defs.md#describetransitgatewayconnectpeersrequestpaginatetypedef)
## DescribeTransitGatewayConnectsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_connects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayConnects.html#EC2.Paginator.DescribeTransitGatewayConnects)

```python
# DescribeTransitGatewayConnectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayConnectsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayConnectsPaginator = client.get_paginator("describe_transit_gateway_connects")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayConnectsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayConnectsPaginator](./paginators.md#describetransitgatewayconnectspaginator)
3. item: `AioPageIterator[DescribeTransitGatewayConnectsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayConnectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayConnectsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayConnectsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayConnectsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayConnectsRequestPaginateTypeDef](./type_defs.md#describetransitgatewayconnectsrequestpaginatetypedef)
## DescribeTransitGatewayMulticastDomainsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_multicast_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayMulticastDomains.html#EC2.Paginator.DescribeTransitGatewayMulticastDomains)

```python
# DescribeTransitGatewayMulticastDomainsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayMulticastDomainsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayMulticastDomainsPaginator = client.get_paginator("describe_transit_gateway_multicast_domains")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayMulticastDomainsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayMulticastDomainsPaginator](./paginators.md#describetransitgatewaymulticastdomainspaginator)
3. item: `AioPageIterator[DescribeTransitGatewayMulticastDomainsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayMulticastDomainsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayMulticastDomainIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayMulticastDomainsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayMulticastDomainsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayMulticastDomainsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayMulticastDomainIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayMulticastDomainsRequestPaginateTypeDef](./type_defs.md#describetransitgatewaymulticastdomainsrequestpaginatetypedef)
## DescribeTransitGatewayPeeringAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_peering_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayPeeringAttachments.html#EC2.Paginator.DescribeTransitGatewayPeeringAttachments)

```python
# DescribeTransitGatewayPeeringAttachmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayPeeringAttachmentsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayPeeringAttachmentsPaginator = client.get_paginator("describe_transit_gateway_peering_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayPeeringAttachmentsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayPeeringAttachmentsPaginator](./paginators.md#describetransitgatewaypeeringattachmentspaginator)
3. item: `AioPageIterator[DescribeTransitGatewayPeeringAttachmentsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayPeeringAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayPeeringAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayPeeringAttachmentsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayPeeringAttachmentsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayPeeringAttachmentsRequestPaginateTypeDef](./type_defs.md#describetransitgatewaypeeringattachmentsrequestpaginatetypedef)
## DescribeTransitGatewayPolicyTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_policy_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayPolicyTables.html#EC2.Paginator.DescribeTransitGatewayPolicyTables)

```python
# DescribeTransitGatewayPolicyTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayPolicyTablesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayPolicyTablesPaginator = client.get_paginator("describe_transit_gateway_policy_tables")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayPolicyTablesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayPolicyTablesPaginator](./paginators.md#describetransitgatewaypolicytablespaginator)
3. item: `AioPageIterator[DescribeTransitGatewayPolicyTablesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayPolicyTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayPolicyTableIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayPolicyTablesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayPolicyTablesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayPolicyTablesRequestPaginateTypeDef = {  # (1)
    "TransitGatewayPolicyTableIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayPolicyTablesRequestPaginateTypeDef](./type_defs.md#describetransitgatewaypolicytablesrequestpaginatetypedef)
## DescribeTransitGatewayRouteTableAnnouncementsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_route_table_announcements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayRouteTableAnnouncements.html#EC2.Paginator.DescribeTransitGatewayRouteTableAnnouncements)

```python
# DescribeTransitGatewayRouteTableAnnouncementsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayRouteTableAnnouncementsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayRouteTableAnnouncementsPaginator = client.get_paginator("describe_transit_gateway_route_table_announcements")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayRouteTableAnnouncementsPaginator](./paginators.md#describetransitgatewayroutetableannouncementspaginator)
3. item: `AioPageIterator[DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayRouteTableAnnouncementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayRouteTableAnnouncementIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayRouteTableAnnouncementsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableAnnouncementIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayRouteTableAnnouncementsRequestPaginateTypeDef](./type_defs.md#describetransitgatewayroutetableannouncementsrequestpaginatetypedef)
## DescribeTransitGatewayRouteTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_route_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayRouteTables.html#EC2.Paginator.DescribeTransitGatewayRouteTables)

```python
# DescribeTransitGatewayRouteTablesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayRouteTablesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayRouteTablesPaginator = client.get_paginator("describe_transit_gateway_route_tables")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayRouteTablesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayRouteTablesPaginator](./paginators.md#describetransitgatewayroutetablespaginator)
3. item: `AioPageIterator[DescribeTransitGatewayRouteTablesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayRouteTablesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayRouteTableIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayRouteTablesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayRouteTablesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayRouteTablesRequestPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayRouteTablesRequestPaginateTypeDef](./type_defs.md#describetransitgatewayroutetablesrequestpaginatetypedef)
## DescribeTransitGatewayVpcAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_vpc_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGatewayVpcAttachments.html#EC2.Paginator.DescribeTransitGatewayVpcAttachments)

```python
# DescribeTransitGatewayVpcAttachmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewayVpcAttachmentsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewayVpcAttachmentsPaginator = client.get_paginator("describe_transit_gateway_vpc_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewayVpcAttachmentsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewayVpcAttachmentsPaginator](./paginators.md#describetransitgatewayvpcattachmentspaginator)
3. item: `AioPageIterator[DescribeTransitGatewayVpcAttachmentsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayVpcAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewayVpcAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewayVpcAttachmentsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewayVpcAttachmentsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayVpcAttachmentsRequestPaginateTypeDef](./type_defs.md#describetransitgatewayvpcattachmentsrequestpaginatetypedef)
## DescribeTransitGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTransitGateways.html#EC2.Paginator.DescribeTransitGateways)

```python
# DescribeTransitGatewaysPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTransitGatewaysPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTransitGatewaysPaginator = client.get_paginator("describe_transit_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTransitGatewaysResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTransitGatewaysPaginator](./paginators.md#describetransitgatewayspaginator)
3. item: `AioPageIterator[DescribeTransitGatewaysResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewaysPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTransitGatewaysResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTransitGatewaysResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTransitGatewaysRequestPaginateTypeDef = {  # (1)
    "TransitGatewayIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewaysRequestPaginateTypeDef](./type_defs.md#describetransitgatewaysrequestpaginatetypedef)
## DescribeTrunkInterfaceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_trunk_interface_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeTrunkInterfaceAssociations.html#EC2.Paginator.DescribeTrunkInterfaceAssociations)

```python
# DescribeTrunkInterfaceAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeTrunkInterfaceAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeTrunkInterfaceAssociationsPaginator = client.get_paginator("describe_trunk_interface_associations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeTrunkInterfaceAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeTrunkInterfaceAssociationsPaginator](./paginators.md#describetrunkinterfaceassociationspaginator)
3. item: `AioPageIterator[DescribeTrunkInterfaceAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeTrunkInterfaceAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    AssociationIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeTrunkInterfaceAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeTrunkInterfaceAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeTrunkInterfaceAssociationsRequestPaginateTypeDef = {  # (1)
    "AssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrunkInterfaceAssociationsRequestPaginateTypeDef](./type_defs.md#describetrunkinterfaceassociationsrequestpaginatetypedef)
## DescribeVerifiedAccessEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_verified_access_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVerifiedAccessEndpoints.html#EC2.Paginator.DescribeVerifiedAccessEndpoints)

```python
# DescribeVerifiedAccessEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVerifiedAccessEndpointsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVerifiedAccessEndpointsPaginator = client.get_paginator("describe_verified_access_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVerifiedAccessEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVerifiedAccessEndpointsPaginator](./paginators.md#describeverifiedaccessendpointspaginator)
3. item: `AioPageIterator[DescribeVerifiedAccessEndpointsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVerifiedAccessEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VerifiedAccessEndpointIds: Sequence[str] = ...,
    VerifiedAccessInstanceId: str = ...,
    VerifiedAccessGroupId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVerifiedAccessEndpointsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVerifiedAccessEndpointsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVerifiedAccessEndpointsRequestPaginateTypeDef = {  # (1)
    "VerifiedAccessEndpointIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVerifiedAccessEndpointsRequestPaginateTypeDef](./type_defs.md#describeverifiedaccessendpointsrequestpaginatetypedef)
## DescribeVerifiedAccessGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_verified_access_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVerifiedAccessGroups.html#EC2.Paginator.DescribeVerifiedAccessGroups)

```python
# DescribeVerifiedAccessGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVerifiedAccessGroupsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVerifiedAccessGroupsPaginator = client.get_paginator("describe_verified_access_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVerifiedAccessGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVerifiedAccessGroupsPaginator](./paginators.md#describeverifiedaccessgroupspaginator)
3. item: `AioPageIterator[DescribeVerifiedAccessGroupsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVerifiedAccessGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VerifiedAccessGroupIds: Sequence[str] = ...,
    VerifiedAccessInstanceId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVerifiedAccessGroupsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVerifiedAccessGroupsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVerifiedAccessGroupsRequestPaginateTypeDef = {  # (1)
    "VerifiedAccessGroupIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVerifiedAccessGroupsRequestPaginateTypeDef](./type_defs.md#describeverifiedaccessgroupsrequestpaginatetypedef)
## DescribeVerifiedAccessInstanceLoggingConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_verified_access_instance_logging_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVerifiedAccessInstanceLoggingConfigurations.html#EC2.Paginator.DescribeVerifiedAccessInstanceLoggingConfigurations)

```python
# DescribeVerifiedAccessInstanceLoggingConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVerifiedAccessInstanceLoggingConfigurationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVerifiedAccessInstanceLoggingConfigurationsPaginator = client.get_paginator("describe_verified_access_instance_logging_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVerifiedAccessInstanceLoggingConfigurationsPaginator](./paginators.md#describeverifiedaccessinstanceloggingconfigurationspaginator)
3. item: `AioPageIterator[DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVerifiedAccessInstanceLoggingConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VerifiedAccessInstanceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVerifiedAccessInstanceLoggingConfigurationsRequestPaginateTypeDef = {  # (1)
    "VerifiedAccessInstanceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVerifiedAccessInstanceLoggingConfigurationsRequestPaginateTypeDef](./type_defs.md#describeverifiedaccessinstanceloggingconfigurationsrequestpaginatetypedef)
## DescribeVerifiedAccessInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_verified_access_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVerifiedAccessInstances.html#EC2.Paginator.DescribeVerifiedAccessInstances)

```python
# DescribeVerifiedAccessInstancesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVerifiedAccessInstancesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVerifiedAccessInstancesPaginator = client.get_paginator("describe_verified_access_instances")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVerifiedAccessInstancesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVerifiedAccessInstancesPaginator](./paginators.md#describeverifiedaccessinstancespaginator)
3. item: `AioPageIterator[DescribeVerifiedAccessInstancesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVerifiedAccessInstancesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VerifiedAccessInstanceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVerifiedAccessInstancesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVerifiedAccessInstancesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVerifiedAccessInstancesRequestPaginateTypeDef = {  # (1)
    "VerifiedAccessInstanceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVerifiedAccessInstancesRequestPaginateTypeDef](./type_defs.md#describeverifiedaccessinstancesrequestpaginatetypedef)
## DescribeVerifiedAccessTrustProvidersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_verified_access_trust_providers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVerifiedAccessTrustProviders.html#EC2.Paginator.DescribeVerifiedAccessTrustProviders)

```python
# DescribeVerifiedAccessTrustProvidersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVerifiedAccessTrustProvidersPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVerifiedAccessTrustProvidersPaginator = client.get_paginator("describe_verified_access_trust_providers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVerifiedAccessTrustProvidersResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVerifiedAccessTrustProvidersPaginator](./paginators.md#describeverifiedaccesstrustproviderspaginator)
3. item: `AioPageIterator[DescribeVerifiedAccessTrustProvidersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVerifiedAccessTrustProvidersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VerifiedAccessTrustProviderIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVerifiedAccessTrustProvidersResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVerifiedAccessTrustProvidersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVerifiedAccessTrustProvidersRequestPaginateTypeDef = {  # (1)
    "VerifiedAccessTrustProviderIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVerifiedAccessTrustProvidersRequestPaginateTypeDef](./type_defs.md#describeverifiedaccesstrustprovidersrequestpaginatetypedef)
## DescribeVolumeStatusPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_volume_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVolumeStatus.html#EC2.Paginator.DescribeVolumeStatus)

```python
# DescribeVolumeStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVolumeStatusPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVolumeStatusPaginator = client.get_paginator("describe_volume_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVolumeStatusResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVolumeStatusPaginator](./paginators.md#describevolumestatuspaginator)
3. item: `AioPageIterator[DescribeVolumeStatusResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVolumeStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VolumeIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVolumeStatusResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVolumeStatusResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVolumeStatusRequestPaginateTypeDef = {  # (1)
    "VolumeIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVolumeStatusRequestPaginateTypeDef](./type_defs.md#describevolumestatusrequestpaginatetypedef)
## DescribeVolumesModificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_volumes_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVolumesModifications.html#EC2.Paginator.DescribeVolumesModifications)

```python
# DescribeVolumesModificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVolumesModificationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVolumesModificationsPaginator = client.get_paginator("describe_volumes_modifications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVolumesModificationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVolumesModificationsPaginator](./paginators.md#describevolumesmodificationspaginator)
3. item: `AioPageIterator[DescribeVolumesModificationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVolumesModificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    VolumeIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVolumesModificationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVolumesModificationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVolumesModificationsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesModificationsRequestPaginateTypeDef](./type_defs.md#describevolumesmodificationsrequestpaginatetypedef)
## DescribeVolumesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_volumes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVolumes.html#EC2.Paginator.DescribeVolumes)

```python
# DescribeVolumesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVolumesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVolumesPaginator = client.get_paginator("describe_volumes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVolumesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVolumesPaginator](./paginators.md#describevolumespaginator)
3. item: `AioPageIterator[DescribeVolumesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVolumesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VolumeIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVolumesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVolumesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVolumesRequestPaginateTypeDef = {  # (1)
    "VolumeIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestPaginateTypeDef](./type_defs.md#describevolumesrequestpaginatetypedef)
## DescribeVpcClassicLinkDnsSupportPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_classic_link_dns_support")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcClassicLinkDnsSupport.html#EC2.Paginator.DescribeVpcClassicLinkDnsSupport)

```python
# DescribeVpcClassicLinkDnsSupportPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcClassicLinkDnsSupportPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcClassicLinkDnsSupportPaginator = client.get_paginator("describe_vpc_classic_link_dns_support")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcClassicLinkDnsSupportResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcClassicLinkDnsSupportPaginator](./paginators.md#describevpcclassiclinkdnssupportpaginator)
3. item: `AioPageIterator[DescribeVpcClassicLinkDnsSupportResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcClassicLinkDnsSupportPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VpcIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcClassicLinkDnsSupportResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeVpcClassicLinkDnsSupportResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcClassicLinkDnsSupportRequestPaginateTypeDef = {  # (1)
    "VpcIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcClassicLinkDnsSupportRequestPaginateTypeDef](./type_defs.md#describevpcclassiclinkdnssupportrequestpaginatetypedef)
## DescribeVpcEndpointConnectionNotificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_connection_notifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcEndpointConnectionNotifications.html#EC2.Paginator.DescribeVpcEndpointConnectionNotifications)

```python
# DescribeVpcEndpointConnectionNotificationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcEndpointConnectionNotificationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcEndpointConnectionNotificationsPaginator = client.get_paginator("describe_vpc_endpoint_connection_notifications")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcEndpointConnectionNotificationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcEndpointConnectionNotificationsPaginator](./paginators.md#describevpcendpointconnectionnotificationspaginator)
3. item: `AioPageIterator[DescribeVpcEndpointConnectionNotificationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointConnectionNotificationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    ConnectionNotificationId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcEndpointConnectionNotificationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcEndpointConnectionNotificationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcEndpointConnectionNotificationsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointConnectionNotificationsRequestPaginateTypeDef](./type_defs.md#describevpcendpointconnectionnotificationsrequestpaginatetypedef)
## DescribeVpcEndpointConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcEndpointConnections.html#EC2.Paginator.DescribeVpcEndpointConnections)

```python
# DescribeVpcEndpointConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcEndpointConnectionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcEndpointConnectionsPaginator = client.get_paginator("describe_vpc_endpoint_connections")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcEndpointConnectionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcEndpointConnectionsPaginator](./paginators.md#describevpcendpointconnectionspaginator)
3. item: `AioPageIterator[DescribeVpcEndpointConnectionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcEndpointConnectionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcEndpointConnectionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcEndpointConnectionsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointConnectionsRequestPaginateTypeDef](./type_defs.md#describevpcendpointconnectionsrequestpaginatetypedef)
## DescribeVpcEndpointServiceConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_service_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcEndpointServiceConfigurations.html#EC2.Paginator.DescribeVpcEndpointServiceConfigurations)

```python
# DescribeVpcEndpointServiceConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcEndpointServiceConfigurationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcEndpointServiceConfigurationsPaginator = client.get_paginator("describe_vpc_endpoint_service_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcEndpointServiceConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcEndpointServiceConfigurationsPaginator](./paginators.md#describevpcendpointserviceconfigurationspaginator)
3. item: `AioPageIterator[DescribeVpcEndpointServiceConfigurationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointServiceConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    ServiceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcEndpointServiceConfigurationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcEndpointServiceConfigurationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcEndpointServiceConfigurationsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointServiceConfigurationsRequestPaginateTypeDef](./type_defs.md#describevpcendpointserviceconfigurationsrequestpaginatetypedef)
## DescribeVpcEndpointServicePermissionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_service_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcEndpointServicePermissions.html#EC2.Paginator.DescribeVpcEndpointServicePermissions)

```python
# DescribeVpcEndpointServicePermissionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcEndpointServicePermissionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcEndpointServicePermissionsPaginator = client.get_paginator("describe_vpc_endpoint_service_permissions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcEndpointServicePermissionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcEndpointServicePermissionsPaginator](./paginators.md#describevpcendpointservicepermissionspaginator)
3. item: `AioPageIterator[DescribeVpcEndpointServicePermissionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointServicePermissionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ServiceId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcEndpointServicePermissionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcEndpointServicePermissionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcEndpointServicePermissionsRequestPaginateTypeDef = {  # (1)
    "ServiceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointServicePermissionsRequestPaginateTypeDef](./type_defs.md#describevpcendpointservicepermissionsrequestpaginatetypedef)
## DescribeVpcEndpointServicesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcEndpointServices.html#EC2.Paginator.DescribeVpcEndpointServices)

```python
# DescribeVpcEndpointServicesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcEndpointServicesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcEndpointServicesPaginator = client.get_paginator("describe_vpc_endpoint_services")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcEndpointServicesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcEndpointServicesPaginator](./paginators.md#describevpcendpointservicespaginator)
3. item: `AioPageIterator[DescribeVpcEndpointServicesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointServicesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    ServiceNames: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ServiceRegions: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcEndpointServicesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcEndpointServicesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcEndpointServicesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointServicesRequestPaginateTypeDef](./type_defs.md#describevpcendpointservicesrequestpaginatetypedef)
## DescribeVpcEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcEndpoints.html#EC2.Paginator.DescribeVpcEndpoints)

```python
# DescribeVpcEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcEndpointsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcEndpointsPaginator = client.get_paginator("describe_vpc_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcEndpointsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcEndpointsPaginator](./paginators.md#describevpcendpointspaginator)
3. item: `AioPageIterator[DescribeVpcEndpointsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    VpcEndpointIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcEndpointsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcEndpointsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcEndpointsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointsRequestPaginateTypeDef](./type_defs.md#describevpcendpointsrequestpaginatetypedef)
## DescribeVpcPeeringConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_peering_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcPeeringConnections.html#EC2.Paginator.DescribeVpcPeeringConnections)

```python
# DescribeVpcPeeringConnectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcPeeringConnectionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcPeeringConnectionsPaginator = client.get_paginator("describe_vpc_peering_connections")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcPeeringConnectionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcPeeringConnectionsPaginator](./paginators.md#describevpcpeeringconnectionspaginator)
3. item: `AioPageIterator[DescribeVpcPeeringConnectionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcPeeringConnectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    VpcPeeringConnectionIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcPeeringConnectionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcPeeringConnectionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcPeeringConnectionsRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcPeeringConnectionsRequestPaginateTypeDef](./type_defs.md#describevpcpeeringconnectionsrequestpaginatetypedef)
## DescribeVpcsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpcs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpcs.html#EC2.Paginator.DescribeVpcs)

```python
# DescribeVpcsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpcsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpcsPaginator = client.get_paginator("describe_vpcs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpcsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpcsPaginator](./paginators.md#describevpcspaginator)
3. item: `AioPageIterator[DescribeVpcsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpcsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VpcIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpcsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpcsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpcsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcsRequestPaginateTypeDef](./type_defs.md#describevpcsrequestpaginatetypedef)
## DescribeVpnConcentratorsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpn_concentrators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/DescribeVpnConcentrators.html#EC2.Paginator.DescribeVpnConcentrators)

```python
# DescribeVpnConcentratorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import DescribeVpnConcentratorsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: DescribeVpnConcentratorsPaginator = client.get_paginator("describe_vpn_concentrators")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVpnConcentratorsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [DescribeVpnConcentratorsPaginator](./paginators.md#describevpnconcentratorspaginator)
3. item: `AioPageIterator[DescribeVpnConcentratorsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVpnConcentratorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VpnConcentratorIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVpnConcentratorsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVpnConcentratorsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVpnConcentratorsRequestPaginateTypeDef = {  # (1)
    "VpnConcentratorIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpnConcentratorsRequestPaginateTypeDef](./type_defs.md#describevpnconcentratorsrequestpaginatetypedef)
## GetAssociatedIpv6PoolCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_associated_ipv6_pool_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetAssociatedIpv6PoolCidrs.html#EC2.Paginator.GetAssociatedIpv6PoolCidrs)

```python
# GetAssociatedIpv6PoolCidrsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetAssociatedIpv6PoolCidrsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetAssociatedIpv6PoolCidrsPaginator = client.get_paginator("get_associated_ipv6_pool_cidrs")  # (2)
    async for item in paginator.paginate(...):
        item: GetAssociatedIpv6PoolCidrsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetAssociatedIpv6PoolCidrsPaginator](./paginators.md#getassociatedipv6poolcidrspaginator)
3. item: `AioPageIterator[GetAssociatedIpv6PoolCidrsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAssociatedIpv6PoolCidrsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetAssociatedIpv6PoolCidrsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetAssociatedIpv6PoolCidrsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAssociatedIpv6PoolCidrsRequestPaginateTypeDef = {  # (1)
    "PoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAssociatedIpv6PoolCidrsRequestPaginateTypeDef](./type_defs.md#getassociatedipv6poolcidrsrequestpaginatetypedef)
## GetAwsNetworkPerformanceDataPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_aws_network_performance_data")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetAwsNetworkPerformanceData.html#EC2.Paginator.GetAwsNetworkPerformanceData)

```python
# GetAwsNetworkPerformanceDataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetAwsNetworkPerformanceDataPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetAwsNetworkPerformanceDataPaginator = client.get_paginator("get_aws_network_performance_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetAwsNetworkPerformanceDataResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetAwsNetworkPerformanceDataPaginator](./paginators.md#getawsnetworkperformancedatapaginator)
3. item: `AioPageIterator[GetAwsNetworkPerformanceDataResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetAwsNetworkPerformanceDataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DataQueries: Sequence[DataQueryTypeDef] = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetAwsNetworkPerformanceDataResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[DataQueryTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetAwsNetworkPerformanceDataResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetAwsNetworkPerformanceDataRequestPaginateTypeDef = {  # (1)
    "DataQueries": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAwsNetworkPerformanceDataRequestPaginateTypeDef](./type_defs.md#getawsnetworkperformancedatarequestpaginatetypedef)
## GetCapacityManagerMetricDataPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_capacity_manager_metric_data")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetCapacityManagerMetricData.html#EC2.Paginator.GetCapacityManagerMetricData)

```python
# GetCapacityManagerMetricDataPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetCapacityManagerMetricDataPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetCapacityManagerMetricDataPaginator = client.get_paginator("get_capacity_manager_metric_data")  # (2)
    async for item in paginator.paginate(...):
        item: GetCapacityManagerMetricDataResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetCapacityManagerMetricDataPaginator](./paginators.md#getcapacitymanagermetricdatapaginator)
3. item: `AioPageIterator[GetCapacityManagerMetricDataResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetCapacityManagerMetricDataPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    MetricNames: Sequence[MetricType],  # (1)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    Period: int,
    GroupBy: Sequence[GroupByType] = ...,  # (2)
    FilterBy: Sequence[CapacityManagerConditionTypeDef] = ...,  # (3)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[GetCapacityManagerMetricDataResultTypeDef]:  # (5)
    ...
```

1. See `Sequence[MetricType]`
2. See `Sequence[GroupByType]`
3. See `Sequence[CapacityManagerConditionTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[GetCapacityManagerMetricDataResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetCapacityManagerMetricDataRequestPaginateTypeDef = {  # (1)
    "MetricNames": ...,
    "StartTime": ...,
    "EndTime": ...,
    "Period": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCapacityManagerMetricDataRequestPaginateTypeDef](./type_defs.md#getcapacitymanagermetricdatarequestpaginatetypedef)
## GetCapacityManagerMetricDimensionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_capacity_manager_metric_dimensions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetCapacityManagerMetricDimensions.html#EC2.Paginator.GetCapacityManagerMetricDimensions)

```python
# GetCapacityManagerMetricDimensionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetCapacityManagerMetricDimensionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetCapacityManagerMetricDimensionsPaginator = client.get_paginator("get_capacity_manager_metric_dimensions")  # (2)
    async for item in paginator.paginate(...):
        item: GetCapacityManagerMetricDimensionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetCapacityManagerMetricDimensionsPaginator](./paginators.md#getcapacitymanagermetricdimensionspaginator)
3. item: `AioPageIterator[GetCapacityManagerMetricDimensionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetCapacityManagerMetricDimensionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    GroupBy: Sequence[GroupByType],  # (1)
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    MetricNames: Sequence[MetricType],  # (2)
    FilterBy: Sequence[CapacityManagerConditionTypeDef] = ...,  # (3)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[GetCapacityManagerMetricDimensionsResultTypeDef]:  # (5)
    ...
```

1. See `Sequence[GroupByType]`
2. See `Sequence[MetricType]`
3. See `Sequence[CapacityManagerConditionTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[GetCapacityManagerMetricDimensionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetCapacityManagerMetricDimensionsRequestPaginateTypeDef = {  # (1)
    "GroupBy": ...,
    "StartTime": ...,
    "EndTime": ...,
    "MetricNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetCapacityManagerMetricDimensionsRequestPaginateTypeDef](./type_defs.md#getcapacitymanagermetricdimensionsrequestpaginatetypedef)
## GetGroupsForCapacityReservationPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_groups_for_capacity_reservation")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetGroupsForCapacityReservation.html#EC2.Paginator.GetGroupsForCapacityReservation)

```python
# GetGroupsForCapacityReservationPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetGroupsForCapacityReservationPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetGroupsForCapacityReservationPaginator = client.get_paginator("get_groups_for_capacity_reservation")  # (2)
    async for item in paginator.paginate(...):
        item: GetGroupsForCapacityReservationResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetGroupsForCapacityReservationPaginator](./paginators.md#getgroupsforcapacityreservationpaginator)
3. item: `AioPageIterator[GetGroupsForCapacityReservationResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetGroupsForCapacityReservationPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CapacityReservationId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetGroupsForCapacityReservationResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetGroupsForCapacityReservationResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetGroupsForCapacityReservationRequestPaginateTypeDef = {  # (1)
    "CapacityReservationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGroupsForCapacityReservationRequestPaginateTypeDef](./type_defs.md#getgroupsforcapacityreservationrequestpaginatetypedef)
## GetInstanceTypesFromInstanceRequirementsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_instance_types_from_instance_requirements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetInstanceTypesFromInstanceRequirements.html#EC2.Paginator.GetInstanceTypesFromInstanceRequirements)

```python
# GetInstanceTypesFromInstanceRequirementsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetInstanceTypesFromInstanceRequirementsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetInstanceTypesFromInstanceRequirementsPaginator = client.get_paginator("get_instance_types_from_instance_requirements")  # (2)
    async for item in paginator.paginate(...):
        item: GetInstanceTypesFromInstanceRequirementsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetInstanceTypesFromInstanceRequirementsPaginator](./paginators.md#getinstancetypesfrominstancerequirementspaginator)
3. item: `AioPageIterator[GetInstanceTypesFromInstanceRequirementsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetInstanceTypesFromInstanceRequirementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ArchitectureTypes: Sequence[ArchitectureTypeType],  # (1)
    VirtualizationTypes: Sequence[VirtualizationTypeType],  # (2)
    InstanceRequirements: InstanceRequirementsRequestTypeDef,  # (3)
    DryRun: bool = ...,
    Context: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[GetInstanceTypesFromInstanceRequirementsResultTypeDef]:  # (5)
    ...
```

1. See `Sequence[ArchitectureTypeType]`
2. See `Sequence[VirtualizationTypeType]`
3. See [:material-code-braces: InstanceRequirementsRequestTypeDef](./type_defs.md#instancerequirementsrequesttypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[GetInstanceTypesFromInstanceRequirementsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetInstanceTypesFromInstanceRequirementsRequestPaginateTypeDef = {  # (1)
    "ArchitectureTypes": ...,
    "VirtualizationTypes": ...,
    "InstanceRequirements": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInstanceTypesFromInstanceRequirementsRequestPaginateTypeDef](./type_defs.md#getinstancetypesfrominstancerequirementsrequestpaginatetypedef)
## GetIpamAddressHistoryPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_address_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamAddressHistory.html#EC2.Paginator.GetIpamAddressHistory)

```python
# GetIpamAddressHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamAddressHistoryPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamAddressHistoryPaginator = client.get_paginator("get_ipam_address_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamAddressHistoryResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamAddressHistoryPaginator](./paginators.md#getipamaddresshistorypaginator)
3. item: `AioPageIterator[GetIpamAddressHistoryResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamAddressHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Cidr: str,
    IpamScopeId: str,
    DryRun: bool = ...,
    VpcId: str = ...,
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetIpamAddressHistoryResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetIpamAddressHistoryResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamAddressHistoryRequestPaginateTypeDef = {  # (1)
    "Cidr": ...,
    "IpamScopeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamAddressHistoryRequestPaginateTypeDef](./type_defs.md#getipamaddresshistoryrequestpaginatetypedef)
## GetIpamDiscoveredAccountsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_discovered_accounts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamDiscoveredAccounts.html#EC2.Paginator.GetIpamDiscoveredAccounts)

```python
# GetIpamDiscoveredAccountsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamDiscoveredAccountsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamDiscoveredAccountsPaginator = client.get_paginator("get_ipam_discovered_accounts")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamDiscoveredAccountsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamDiscoveredAccountsPaginator](./paginators.md#getipamdiscoveredaccountspaginator)
3. item: `AioPageIterator[GetIpamDiscoveredAccountsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamDiscoveredAccountsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamResourceDiscoveryId: str,
    DiscoveryRegion: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetIpamDiscoveredAccountsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetIpamDiscoveredAccountsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamDiscoveredAccountsRequestPaginateTypeDef = {  # (1)
    "IpamResourceDiscoveryId": ...,
    "DiscoveryRegion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamDiscoveredAccountsRequestPaginateTypeDef](./type_defs.md#getipamdiscoveredaccountsrequestpaginatetypedef)
## GetIpamDiscoveredResourceCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_discovered_resource_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamDiscoveredResourceCidrs.html#EC2.Paginator.GetIpamDiscoveredResourceCidrs)

```python
# GetIpamDiscoveredResourceCidrsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamDiscoveredResourceCidrsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamDiscoveredResourceCidrsPaginator = client.get_paginator("get_ipam_discovered_resource_cidrs")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamDiscoveredResourceCidrsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamDiscoveredResourceCidrsPaginator](./paginators.md#getipamdiscoveredresourcecidrspaginator)
3. item: `AioPageIterator[GetIpamDiscoveredResourceCidrsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamDiscoveredResourceCidrsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamResourceDiscoveryId: str,
    ResourceRegion: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetIpamDiscoveredResourceCidrsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetIpamDiscoveredResourceCidrsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamDiscoveredResourceCidrsRequestPaginateTypeDef = {  # (1)
    "IpamResourceDiscoveryId": ...,
    "ResourceRegion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamDiscoveredResourceCidrsRequestPaginateTypeDef](./type_defs.md#getipamdiscoveredresourcecidrsrequestpaginatetypedef)
## GetIpamPoolAllocationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_pool_allocations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamPoolAllocations.html#EC2.Paginator.GetIpamPoolAllocations)

```python
# GetIpamPoolAllocationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamPoolAllocationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamPoolAllocationsPaginator = client.get_paginator("get_ipam_pool_allocations")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamPoolAllocationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamPoolAllocationsPaginator](./paginators.md#getipampoolallocationspaginator)
3. item: `AioPageIterator[GetIpamPoolAllocationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamPoolAllocationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamPoolId: str,
    DryRun: bool = ...,
    IpamPoolAllocationId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetIpamPoolAllocationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetIpamPoolAllocationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamPoolAllocationsRequestPaginateTypeDef = {  # (1)
    "IpamPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamPoolAllocationsRequestPaginateTypeDef](./type_defs.md#getipampoolallocationsrequestpaginatetypedef)
## GetIpamPoolCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_pool_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamPoolCidrs.html#EC2.Paginator.GetIpamPoolCidrs)

```python
# GetIpamPoolCidrsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamPoolCidrsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamPoolCidrsPaginator = client.get_paginator("get_ipam_pool_cidrs")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamPoolCidrsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamPoolCidrsPaginator](./paginators.md#getipampoolcidrspaginator)
3. item: `AioPageIterator[GetIpamPoolCidrsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamPoolCidrsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamPoolId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetIpamPoolCidrsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetIpamPoolCidrsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamPoolCidrsRequestPaginateTypeDef = {  # (1)
    "IpamPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamPoolCidrsRequestPaginateTypeDef](./type_defs.md#getipampoolcidrsrequestpaginatetypedef)
## GetIpamPrefixListResolverRulesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_prefix_list_resolver_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamPrefixListResolverRules.html#EC2.Paginator.GetIpamPrefixListResolverRules)

```python
# GetIpamPrefixListResolverRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamPrefixListResolverRulesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamPrefixListResolverRulesPaginator = client.get_paginator("get_ipam_prefix_list_resolver_rules")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamPrefixListResolverRulesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamPrefixListResolverRulesPaginator](./paginators.md#getipamprefixlistresolverrulespaginator)
3. item: `AioPageIterator[GetIpamPrefixListResolverRulesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamPrefixListResolverRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamPrefixListResolverId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetIpamPrefixListResolverRulesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetIpamPrefixListResolverRulesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamPrefixListResolverRulesRequestPaginateTypeDef = {  # (1)
    "IpamPrefixListResolverId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamPrefixListResolverRulesRequestPaginateTypeDef](./type_defs.md#getipamprefixlistresolverrulesrequestpaginatetypedef)
## GetIpamPrefixListResolverVersionEntriesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_prefix_list_resolver_version_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamPrefixListResolverVersionEntries.html#EC2.Paginator.GetIpamPrefixListResolverVersionEntries)

```python
# GetIpamPrefixListResolverVersionEntriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamPrefixListResolverVersionEntriesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamPrefixListResolverVersionEntriesPaginator = client.get_paginator("get_ipam_prefix_list_resolver_version_entries")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamPrefixListResolverVersionEntriesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamPrefixListResolverVersionEntriesPaginator](./paginators.md#getipamprefixlistresolverversionentriespaginator)
3. item: `AioPageIterator[GetIpamPrefixListResolverVersionEntriesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamPrefixListResolverVersionEntriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamPrefixListResolverId: str,
    IpamPrefixListResolverVersion: int,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetIpamPrefixListResolverVersionEntriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetIpamPrefixListResolverVersionEntriesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamPrefixListResolverVersionEntriesRequestPaginateTypeDef = {  # (1)
    "IpamPrefixListResolverId": ...,
    "IpamPrefixListResolverVersion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamPrefixListResolverVersionEntriesRequestPaginateTypeDef](./type_defs.md#getipamprefixlistresolverversionentriesrequestpaginatetypedef)
## GetIpamPrefixListResolverVersionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_prefix_list_resolver_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamPrefixListResolverVersions.html#EC2.Paginator.GetIpamPrefixListResolverVersions)

```python
# GetIpamPrefixListResolverVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamPrefixListResolverVersionsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamPrefixListResolverVersionsPaginator = client.get_paginator("get_ipam_prefix_list_resolver_versions")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamPrefixListResolverVersionsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamPrefixListResolverVersionsPaginator](./paginators.md#getipamprefixlistresolverversionspaginator)
3. item: `AioPageIterator[GetIpamPrefixListResolverVersionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamPrefixListResolverVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamPrefixListResolverId: str,
    DryRun: bool = ...,
    IpamPrefixListResolverVersions: Sequence[int] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetIpamPrefixListResolverVersionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetIpamPrefixListResolverVersionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamPrefixListResolverVersionsRequestPaginateTypeDef = {  # (1)
    "IpamPrefixListResolverId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamPrefixListResolverVersionsRequestPaginateTypeDef](./type_defs.md#getipamprefixlistresolverversionsrequestpaginatetypedef)
## GetIpamResourceCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_resource_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetIpamResourceCidrs.html#EC2.Paginator.GetIpamResourceCidrs)

```python
# GetIpamResourceCidrsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetIpamResourceCidrsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetIpamResourceCidrsPaginator = client.get_paginator("get_ipam_resource_cidrs")  # (2)
    async for item in paginator.paginate(...):
        item: GetIpamResourceCidrsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetIpamResourceCidrsPaginator](./paginators.md#getipamresourcecidrspaginator)
3. item: `AioPageIterator[GetIpamResourceCidrsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetIpamResourceCidrsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    IpamScopeId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamPoolId: str = ...,
    ResourceId: str = ...,
    ResourceType: IpamResourceTypeType = ...,  # (2)
    ResourceTag: RequestIpamResourceTagTypeDef = ...,  # (3)
    ResourceOwner: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[GetIpamResourceCidrsResultTypeDef]:  # (5)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-brackets: IpamResourceTypeType](./literals.md#ipamresourcetypetype)
3. See [:material-code-braces: RequestIpamResourceTagTypeDef](./type_defs.md#requestipamresourcetagtypedef)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[GetIpamResourceCidrsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetIpamResourceCidrsRequestPaginateTypeDef = {  # (1)
    "IpamScopeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamResourceCidrsRequestPaginateTypeDef](./type_defs.md#getipamresourcecidrsrequestpaginatetypedef)
## GetManagedPrefixListAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_managed_prefix_list_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetManagedPrefixListAssociations.html#EC2.Paginator.GetManagedPrefixListAssociations)

```python
# GetManagedPrefixListAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetManagedPrefixListAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetManagedPrefixListAssociationsPaginator = client.get_paginator("get_managed_prefix_list_associations")  # (2)
    async for item in paginator.paginate(...):
        item: GetManagedPrefixListAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetManagedPrefixListAssociationsPaginator](./paginators.md#getmanagedprefixlistassociationspaginator)
3. item: `AioPageIterator[GetManagedPrefixListAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetManagedPrefixListAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PrefixListId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetManagedPrefixListAssociationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetManagedPrefixListAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetManagedPrefixListAssociationsRequestPaginateTypeDef = {  # (1)
    "PrefixListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetManagedPrefixListAssociationsRequestPaginateTypeDef](./type_defs.md#getmanagedprefixlistassociationsrequestpaginatetypedef)
## GetManagedPrefixListEntriesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_managed_prefix_list_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetManagedPrefixListEntries.html#EC2.Paginator.GetManagedPrefixListEntries)

```python
# GetManagedPrefixListEntriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetManagedPrefixListEntriesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetManagedPrefixListEntriesPaginator = client.get_paginator("get_managed_prefix_list_entries")  # (2)
    async for item in paginator.paginate(...):
        item: GetManagedPrefixListEntriesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetManagedPrefixListEntriesPaginator](./paginators.md#getmanagedprefixlistentriespaginator)
3. item: `AioPageIterator[GetManagedPrefixListEntriesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetManagedPrefixListEntriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PrefixListId: str,
    DryRun: bool = ...,
    TargetVersion: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetManagedPrefixListEntriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetManagedPrefixListEntriesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetManagedPrefixListEntriesRequestPaginateTypeDef = {  # (1)
    "PrefixListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetManagedPrefixListEntriesRequestPaginateTypeDef](./type_defs.md#getmanagedprefixlistentriesrequestpaginatetypedef)
## GetNetworkInsightsAccessScopeAnalysisFindingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_network_insights_access_scope_analysis_findings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetNetworkInsightsAccessScopeAnalysisFindings.html#EC2.Paginator.GetNetworkInsightsAccessScopeAnalysisFindings)

```python
# GetNetworkInsightsAccessScopeAnalysisFindingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetNetworkInsightsAccessScopeAnalysisFindingsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetNetworkInsightsAccessScopeAnalysisFindingsPaginator = client.get_paginator("get_network_insights_access_scope_analysis_findings")  # (2)
    async for item in paginator.paginate(...):
        item: GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetNetworkInsightsAccessScopeAnalysisFindingsPaginator](./paginators.md#getnetworkinsightsaccessscopeanalysisfindingspaginator)
3. item: `AioPageIterator[GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetNetworkInsightsAccessScopeAnalysisFindingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    NetworkInsightsAccessScopeAnalysisId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetNetworkInsightsAccessScopeAnalysisFindingsRequestPaginateTypeDef = {  # (1)
    "NetworkInsightsAccessScopeAnalysisId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetNetworkInsightsAccessScopeAnalysisFindingsRequestPaginateTypeDef](./type_defs.md#getnetworkinsightsaccessscopeanalysisfindingsrequestpaginatetypedef)
## GetSecurityGroupsForVpcPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_security_groups_for_vpc")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetSecurityGroupsForVpc.html#EC2.Paginator.GetSecurityGroupsForVpc)

```python
# GetSecurityGroupsForVpcPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetSecurityGroupsForVpcPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetSecurityGroupsForVpcPaginator = client.get_paginator("get_security_groups_for_vpc")  # (2)
    async for item in paginator.paginate(...):
        item: GetSecurityGroupsForVpcResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetSecurityGroupsForVpcPaginator](./paginators.md#getsecuritygroupsforvpcpaginator)
3. item: `AioPageIterator[GetSecurityGroupsForVpcResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetSecurityGroupsForVpcPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VpcId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetSecurityGroupsForVpcResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetSecurityGroupsForVpcResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetSecurityGroupsForVpcRequestPaginateTypeDef = {  # (1)
    "VpcId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSecurityGroupsForVpcRequestPaginateTypeDef](./type_defs.md#getsecuritygroupsforvpcrequestpaginatetypedef)
## GetSpotPlacementScoresPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_spot_placement_scores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetSpotPlacementScores.html#EC2.Paginator.GetSpotPlacementScores)

```python
# GetSpotPlacementScoresPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetSpotPlacementScoresPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetSpotPlacementScoresPaginator = client.get_paginator("get_spot_placement_scores")  # (2)
    async for item in paginator.paginate(...):
        item: GetSpotPlacementScoresResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetSpotPlacementScoresPaginator](./paginators.md#getspotplacementscorespaginator)
3. item: `AioPageIterator[GetSpotPlacementScoresResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetSpotPlacementScoresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TargetCapacity: int,
    InstanceTypes: Sequence[str] = ...,
    TargetCapacityUnitType: TargetCapacityUnitTypeType = ...,  # (1)
    SingleAvailabilityZone: bool = ...,
    RegionNames: Sequence[str] = ...,
    InstanceRequirementsWithMetadata: InstanceRequirementsWithMetadataRequestTypeDef = ...,  # (2)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[GetSpotPlacementScoresResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: TargetCapacityUnitTypeType](./literals.md#targetcapacityunittypetype)
2. See [:material-code-braces: InstanceRequirementsWithMetadataRequestTypeDef](./type_defs.md#instancerequirementswithmetadatarequesttypedef)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[GetSpotPlacementScoresResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetSpotPlacementScoresRequestPaginateTypeDef = {  # (1)
    "TargetCapacity": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSpotPlacementScoresRequestPaginateTypeDef](./type_defs.md#getspotplacementscoresrequestpaginatetypedef)
## GetTransitGatewayAttachmentPropagationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_attachment_propagations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetTransitGatewayAttachmentPropagations.html#EC2.Paginator.GetTransitGatewayAttachmentPropagations)

```python
# GetTransitGatewayAttachmentPropagationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetTransitGatewayAttachmentPropagationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetTransitGatewayAttachmentPropagationsPaginator = client.get_paginator("get_transit_gateway_attachment_propagations")  # (2)
    async for item in paginator.paginate(...):
        item: GetTransitGatewayAttachmentPropagationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetTransitGatewayAttachmentPropagationsPaginator](./paginators.md#gettransitgatewayattachmentpropagationspaginator)
3. item: `AioPageIterator[GetTransitGatewayAttachmentPropagationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTransitGatewayAttachmentPropagationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayAttachmentId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetTransitGatewayAttachmentPropagationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetTransitGatewayAttachmentPropagationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTransitGatewayAttachmentPropagationsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayAttachmentPropagationsRequestPaginateTypeDef](./type_defs.md#gettransitgatewayattachmentpropagationsrequestpaginatetypedef)
## GetTransitGatewayMulticastDomainAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_multicast_domain_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetTransitGatewayMulticastDomainAssociations.html#EC2.Paginator.GetTransitGatewayMulticastDomainAssociations)

```python
# GetTransitGatewayMulticastDomainAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetTransitGatewayMulticastDomainAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetTransitGatewayMulticastDomainAssociationsPaginator = client.get_paginator("get_transit_gateway_multicast_domain_associations")  # (2)
    async for item in paginator.paginate(...):
        item: GetTransitGatewayMulticastDomainAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetTransitGatewayMulticastDomainAssociationsPaginator](./paginators.md#gettransitgatewaymulticastdomainassociationspaginator)
3. item: `AioPageIterator[GetTransitGatewayMulticastDomainAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTransitGatewayMulticastDomainAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayMulticastDomainId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetTransitGatewayMulticastDomainAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetTransitGatewayMulticastDomainAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTransitGatewayMulticastDomainAssociationsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayMulticastDomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayMulticastDomainAssociationsRequestPaginateTypeDef](./type_defs.md#gettransitgatewaymulticastdomainassociationsrequestpaginatetypedef)
## GetTransitGatewayPolicyTableAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_policy_table_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetTransitGatewayPolicyTableAssociations.html#EC2.Paginator.GetTransitGatewayPolicyTableAssociations)

```python
# GetTransitGatewayPolicyTableAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetTransitGatewayPolicyTableAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetTransitGatewayPolicyTableAssociationsPaginator = client.get_paginator("get_transit_gateway_policy_table_associations")  # (2)
    async for item in paginator.paginate(...):
        item: GetTransitGatewayPolicyTableAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetTransitGatewayPolicyTableAssociationsPaginator](./paginators.md#gettransitgatewaypolicytableassociationspaginator)
3. item: `AioPageIterator[GetTransitGatewayPolicyTableAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTransitGatewayPolicyTableAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayPolicyTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetTransitGatewayPolicyTableAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetTransitGatewayPolicyTableAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTransitGatewayPolicyTableAssociationsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayPolicyTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayPolicyTableAssociationsRequestPaginateTypeDef](./type_defs.md#gettransitgatewaypolicytableassociationsrequestpaginatetypedef)
## GetTransitGatewayPrefixListReferencesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_prefix_list_references")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetTransitGatewayPrefixListReferences.html#EC2.Paginator.GetTransitGatewayPrefixListReferences)

```python
# GetTransitGatewayPrefixListReferencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetTransitGatewayPrefixListReferencesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetTransitGatewayPrefixListReferencesPaginator = client.get_paginator("get_transit_gateway_prefix_list_references")  # (2)
    async for item in paginator.paginate(...):
        item: GetTransitGatewayPrefixListReferencesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetTransitGatewayPrefixListReferencesPaginator](./paginators.md#gettransitgatewayprefixlistreferencespaginator)
3. item: `AioPageIterator[GetTransitGatewayPrefixListReferencesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTransitGatewayPrefixListReferencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetTransitGatewayPrefixListReferencesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetTransitGatewayPrefixListReferencesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTransitGatewayPrefixListReferencesRequestPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayPrefixListReferencesRequestPaginateTypeDef](./type_defs.md#gettransitgatewayprefixlistreferencesrequestpaginatetypedef)
## GetTransitGatewayRouteTableAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_route_table_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetTransitGatewayRouteTableAssociations.html#EC2.Paginator.GetTransitGatewayRouteTableAssociations)

```python
# GetTransitGatewayRouteTableAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetTransitGatewayRouteTableAssociationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetTransitGatewayRouteTableAssociationsPaginator = client.get_paginator("get_transit_gateway_route_table_associations")  # (2)
    async for item in paginator.paginate(...):
        item: GetTransitGatewayRouteTableAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetTransitGatewayRouteTableAssociationsPaginator](./paginators.md#gettransitgatewayroutetableassociationspaginator)
3. item: `AioPageIterator[GetTransitGatewayRouteTableAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTransitGatewayRouteTableAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetTransitGatewayRouteTableAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetTransitGatewayRouteTableAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTransitGatewayRouteTableAssociationsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayRouteTableAssociationsRequestPaginateTypeDef](./type_defs.md#gettransitgatewayroutetableassociationsrequestpaginatetypedef)
## GetTransitGatewayRouteTablePropagationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_route_table_propagations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetTransitGatewayRouteTablePropagations.html#EC2.Paginator.GetTransitGatewayRouteTablePropagations)

```python
# GetTransitGatewayRouteTablePropagationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetTransitGatewayRouteTablePropagationsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetTransitGatewayRouteTablePropagationsPaginator = client.get_paginator("get_transit_gateway_route_table_propagations")  # (2)
    async for item in paginator.paginate(...):
        item: GetTransitGatewayRouteTablePropagationsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetTransitGatewayRouteTablePropagationsPaginator](./paginators.md#gettransitgatewayroutetablepropagationspaginator)
3. item: `AioPageIterator[GetTransitGatewayRouteTablePropagationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetTransitGatewayRouteTablePropagationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[GetTransitGatewayRouteTablePropagationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[GetTransitGatewayRouteTablePropagationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetTransitGatewayRouteTablePropagationsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayRouteTablePropagationsRequestPaginateTypeDef](./type_defs.md#gettransitgatewayroutetablepropagationsrequestpaginatetypedef)
## GetVpnConnectionDeviceTypesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_vpn_connection_device_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/GetVpnConnectionDeviceTypes.html#EC2.Paginator.GetVpnConnectionDeviceTypes)

```python
# GetVpnConnectionDeviceTypesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import GetVpnConnectionDeviceTypesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: GetVpnConnectionDeviceTypesPaginator = client.get_paginator("get_vpn_connection_device_types")  # (2)
    async for item in paginator.paginate(...):
        item: GetVpnConnectionDeviceTypesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [GetVpnConnectionDeviceTypesPaginator](./paginators.md#getvpnconnectiondevicetypespaginator)
3. item: `AioPageIterator[GetVpnConnectionDeviceTypesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python GetVpnConnectionDeviceTypesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetVpnConnectionDeviceTypesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetVpnConnectionDeviceTypesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetVpnConnectionDeviceTypesRequestPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetVpnConnectionDeviceTypesRequestPaginateTypeDef](./type_defs.md#getvpnconnectiondevicetypesrequestpaginatetypedef)
## ListImagesInRecycleBinPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("list_images_in_recycle_bin")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/ListImagesInRecycleBin.html#EC2.Paginator.ListImagesInRecycleBin)

```python
# ListImagesInRecycleBinPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import ListImagesInRecycleBinPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: ListImagesInRecycleBinPaginator = client.get_paginator("list_images_in_recycle_bin")  # (2)
    async for item in paginator.paginate(...):
        item: ListImagesInRecycleBinResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [ListImagesInRecycleBinPaginator](./paginators.md#listimagesinrecyclebinpaginator)
3. item: `AioPageIterator[ListImagesInRecycleBinResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListImagesInRecycleBinPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListImagesInRecycleBinResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListImagesInRecycleBinResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListImagesInRecycleBinRequestPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImagesInRecycleBinRequestPaginateTypeDef](./type_defs.md#listimagesinrecyclebinrequestpaginatetypedef)
## ListSnapshotsInRecycleBinPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("list_snapshots_in_recycle_bin")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/ListSnapshotsInRecycleBin.html#EC2.Paginator.ListSnapshotsInRecycleBin)

```python
# ListSnapshotsInRecycleBinPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import ListSnapshotsInRecycleBinPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: ListSnapshotsInRecycleBinPaginator = client.get_paginator("list_snapshots_in_recycle_bin")  # (2)
    async for item in paginator.paginate(...):
        item: ListSnapshotsInRecycleBinResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [ListSnapshotsInRecycleBinPaginator](./paginators.md#listsnapshotsinrecyclebinpaginator)
3. item: `AioPageIterator[ListSnapshotsInRecycleBinResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSnapshotsInRecycleBinPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SnapshotIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSnapshotsInRecycleBinResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSnapshotsInRecycleBinResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSnapshotsInRecycleBinRequestPaginateTypeDef = {  # (1)
    "SnapshotIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSnapshotsInRecycleBinRequestPaginateTypeDef](./type_defs.md#listsnapshotsinrecyclebinrequestpaginatetypedef)
## SearchLocalGatewayRoutesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("search_local_gateway_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/SearchLocalGatewayRoutes.html#EC2.Paginator.SearchLocalGatewayRoutes)

```python
# SearchLocalGatewayRoutesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import SearchLocalGatewayRoutesPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: SearchLocalGatewayRoutesPaginator = client.get_paginator("search_local_gateway_routes")  # (2)
    async for item in paginator.paginate(...):
        item: SearchLocalGatewayRoutesResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [SearchLocalGatewayRoutesPaginator](./paginators.md#searchlocalgatewayroutespaginator)
3. item: `AioPageIterator[SearchLocalGatewayRoutesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchLocalGatewayRoutesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    LocalGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchLocalGatewayRoutesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchLocalGatewayRoutesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchLocalGatewayRoutesRequestPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchLocalGatewayRoutesRequestPaginateTypeDef](./type_defs.md#searchlocalgatewayroutesrequestpaginatetypedef)
## SearchTransitGatewayMulticastGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("search_transit_gateway_multicast_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2/paginator/SearchTransitGatewayMulticastGroups.html#EC2.Paginator.SearchTransitGatewayMulticastGroups)

```python
# SearchTransitGatewayMulticastGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2.paginator import SearchTransitGatewayMulticastGroupsPaginator

session = get_session()
async with session.create_client("ec2") as client:  # (1)
    paginator: SearchTransitGatewayMulticastGroupsPaginator = client.get_paginator("search_transit_gateway_multicast_groups")  # (2)
    async for item in paginator.paginate(...):
        item: SearchTransitGatewayMulticastGroupsResultTypeDef
        print(item)  # (3)
```

1. client: [EC2Client](./client.md)
2. paginator: [SearchTransitGatewayMulticastGroupsPaginator](./paginators.md#searchtransitgatewaymulticastgroupspaginator)
3. item: `AioPageIterator[SearchTransitGatewayMulticastGroupsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchTransitGatewayMulticastGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    TransitGatewayMulticastDomainId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[SearchTransitGatewayMulticastGroupsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[FilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[SearchTransitGatewayMulticastGroupsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchTransitGatewayMulticastGroupsRequestPaginateTypeDef = {  # (1)
    "TransitGatewayMulticastDomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchTransitGatewayMulticastGroupsRequestPaginateTypeDef](./type_defs.md#searchtransitgatewaymulticastgroupsrequestpaginatetypedef)
