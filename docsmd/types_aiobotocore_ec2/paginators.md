# Paginators

> [Index](../README.md) > [EC2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2)
    type annotations stubs module [types-aiobotocore-ec2](https://pypi.org/project/types-aiobotocore-ec2/).

## DescribeAddressesAttributePaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_addresses_attribute")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeAddressesAttribute)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeAddressesAttributeResultTypeDef](./type_defs.md#describeaddressesattributeresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAddressesAttributePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AllocationIds: Sequence[str] = ...,
    Attribute: AddressAttributeNameType = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeAddressesAttributeResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AddressAttributeNameType](./literals.md#addressattributenametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAddressesAttributeResultTypeDef](./type_defs.md#describeaddressesattributeresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeAddressesAttributeRequestDescribeAddressesAttributePaginateTypeDef = {  # (1)
    "AllocationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAddressesAttributeRequestDescribeAddressesAttributePaginateTypeDef](./type_defs.md#describeaddressesattributerequestdescribeaddressesattributepaginatetypedef) 
## DescribeByoipCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_byoip_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeByoipCidrs)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeByoipCidrsResultTypeDef](./type_defs.md#describebyoipcidrsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeByoipCidrsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeByoipCidrsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeByoipCidrsResultTypeDef](./type_defs.md#describebyoipcidrsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeByoipCidrsRequestDescribeByoipCidrsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeByoipCidrsRequestDescribeByoipCidrsPaginateTypeDef](./type_defs.md#describebyoipcidrsrequestdescribebyoipcidrspaginatetypedef) 
## DescribeCapacityReservationFleetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_reservation_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeCapacityReservationFleets)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeCapacityReservationFleetsResultTypeDef](./type_defs.md#describecapacityreservationfleetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCapacityReservationFleetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CapacityReservationFleetIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeCapacityReservationFleetsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeCapacityReservationFleetsResultTypeDef](./type_defs.md#describecapacityreservationfleetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCapacityReservationFleetsRequestDescribeCapacityReservationFleetsPaginateTypeDef = {  # (1)
    "CapacityReservationFleetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityReservationFleetsRequestDescribeCapacityReservationFleetsPaginateTypeDef](./type_defs.md#describecapacityreservationfleetsrequestdescribecapacityreservationfleetspaginatetypedef) 
## DescribeCapacityReservationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_capacity_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeCapacityReservations)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeCapacityReservationsResultTypeDef](./type_defs.md#describecapacityreservationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCapacityReservationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CapacityReservationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeCapacityReservationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeCapacityReservationsResultTypeDef](./type_defs.md#describecapacityreservationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCapacityReservationsRequestDescribeCapacityReservationsPaginateTypeDef = {  # (1)
    "CapacityReservationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCapacityReservationsRequestDescribeCapacityReservationsPaginateTypeDef](./type_defs.md#describecapacityreservationsrequestdescribecapacityreservationspaginatetypedef) 
## DescribeCarrierGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_carrier_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeCarrierGateways)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeCarrierGatewaysResultTypeDef](./type_defs.md#describecarriergatewaysresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCarrierGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CarrierGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeCarrierGatewaysResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeCarrierGatewaysResultTypeDef](./type_defs.md#describecarriergatewaysresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCarrierGatewaysRequestDescribeCarrierGatewaysPaginateTypeDef = {  # (1)
    "CarrierGatewayIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCarrierGatewaysRequestDescribeCarrierGatewaysPaginateTypeDef](./type_defs.md#describecarriergatewaysrequestdescribecarriergatewayspaginatetypedef) 
## DescribeClassicLinkInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_classic_link_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeClassicLinkInstances)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeClassicLinkInstancesResultTypeDef](./type_defs.md#describeclassiclinkinstancesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClassicLinkInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    InstanceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeClassicLinkInstancesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeClassicLinkInstancesResultTypeDef](./type_defs.md#describeclassiclinkinstancesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClassicLinkInstancesRequestDescribeClassicLinkInstancesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClassicLinkInstancesRequestDescribeClassicLinkInstancesPaginateTypeDef](./type_defs.md#describeclassiclinkinstancesrequestdescribeclassiclinkinstancespaginatetypedef) 
## DescribeClientVpnAuthorizationRulesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_authorization_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeClientVpnAuthorizationRules)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeClientVpnAuthorizationRulesResultTypeDef](./type_defs.md#describeclientvpnauthorizationrulesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClientVpnAuthorizationRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeClientVpnAuthorizationRulesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeClientVpnAuthorizationRulesResultTypeDef](./type_defs.md#describeclientvpnauthorizationrulesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClientVpnAuthorizationRulesRequestDescribeClientVpnAuthorizationRulesPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnAuthorizationRulesRequestDescribeClientVpnAuthorizationRulesPaginateTypeDef](./type_defs.md#describeclientvpnauthorizationrulesrequestdescribeclientvpnauthorizationrulespaginatetypedef) 
## DescribeClientVpnConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeClientVpnConnections)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeClientVpnConnectionsResultTypeDef](./type_defs.md#describeclientvpnconnectionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClientVpnConnectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeClientVpnConnectionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeClientVpnConnectionsResultTypeDef](./type_defs.md#describeclientvpnconnectionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClientVpnConnectionsRequestDescribeClientVpnConnectionsPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnConnectionsRequestDescribeClientVpnConnectionsPaginateTypeDef](./type_defs.md#describeclientvpnconnectionsrequestdescribeclientvpnconnectionspaginatetypedef) 
## DescribeClientVpnEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeClientVpnEndpoints)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeClientVpnEndpointsResultTypeDef](./type_defs.md#describeclientvpnendpointsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClientVpnEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClientVpnEndpointIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeClientVpnEndpointsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeClientVpnEndpointsResultTypeDef](./type_defs.md#describeclientvpnendpointsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClientVpnEndpointsRequestDescribeClientVpnEndpointsPaginateTypeDef = {  # (1)
    "ClientVpnEndpointIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnEndpointsRequestDescribeClientVpnEndpointsPaginateTypeDef](./type_defs.md#describeclientvpnendpointsrequestdescribeclientvpnendpointspaginatetypedef) 
## DescribeClientVpnRoutesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeClientVpnRoutes)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeClientVpnRoutesResultTypeDef](./type_defs.md#describeclientvpnroutesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClientVpnRoutesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeClientVpnRoutesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeClientVpnRoutesResultTypeDef](./type_defs.md#describeclientvpnroutesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClientVpnRoutesRequestDescribeClientVpnRoutesPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnRoutesRequestDescribeClientVpnRoutesPaginateTypeDef](./type_defs.md#describeclientvpnroutesrequestdescribeclientvpnroutespaginatetypedef) 
## DescribeClientVpnTargetNetworksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_client_vpn_target_networks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeClientVpnTargetNetworks)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeClientVpnTargetNetworksResultTypeDef](./type_defs.md#describeclientvpntargetnetworksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeClientVpnTargetNetworksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClientVpnEndpointId: str,
    AssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeClientVpnTargetNetworksResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeClientVpnTargetNetworksResultTypeDef](./type_defs.md#describeclientvpntargetnetworksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClientVpnTargetNetworksRequestDescribeClientVpnTargetNetworksPaginateTypeDef = {  # (1)
    "ClientVpnEndpointId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClientVpnTargetNetworksRequestDescribeClientVpnTargetNetworksPaginateTypeDef](./type_defs.md#describeclientvpntargetnetworksrequestdescribeclientvpntargetnetworkspaginatetypedef) 
## DescribeCoipPoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_coip_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeCoipPools)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeCoipPoolsResultTypeDef](./type_defs.md#describecoippoolsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeCoipPoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeCoipPoolsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeCoipPoolsResultTypeDef](./type_defs.md#describecoippoolsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeCoipPoolsRequestDescribeCoipPoolsPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeCoipPoolsRequestDescribeCoipPoolsPaginateTypeDef](./type_defs.md#describecoippoolsrequestdescribecoippoolspaginatetypedef) 
## DescribeDhcpOptionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_dhcp_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeDhcpOptions)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeDhcpOptionsResultTypeDef](./type_defs.md#describedhcpoptionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDhcpOptionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DhcpOptionsIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeDhcpOptionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeDhcpOptionsResultTypeDef](./type_defs.md#describedhcpoptionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDhcpOptionsRequestDescribeDhcpOptionsPaginateTypeDef = {  # (1)
    "DhcpOptionsIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDhcpOptionsRequestDescribeDhcpOptionsPaginateTypeDef](./type_defs.md#describedhcpoptionsrequestdescribedhcpoptionspaginatetypedef) 
## DescribeEgressOnlyInternetGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_egress_only_internet_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeEgressOnlyInternetGateways)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeEgressOnlyInternetGatewaysResultTypeDef](./type_defs.md#describeegressonlyinternetgatewaysresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEgressOnlyInternetGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    EgressOnlyInternetGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEgressOnlyInternetGatewaysResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEgressOnlyInternetGatewaysResultTypeDef](./type_defs.md#describeegressonlyinternetgatewaysresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEgressOnlyInternetGatewaysRequestDescribeEgressOnlyInternetGatewaysPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEgressOnlyInternetGatewaysRequestDescribeEgressOnlyInternetGatewaysPaginateTypeDef](./type_defs.md#describeegressonlyinternetgatewaysrequestdescribeegressonlyinternetgatewayspaginatetypedef) 
## DescribeExportImageTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_export_image_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeExportImageTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeExportImageTasksResultTypeDef](./type_defs.md#describeexportimagetasksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeExportImageTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ExportImageTaskIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeExportImageTasksResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeExportImageTasksResultTypeDef](./type_defs.md#describeexportimagetasksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeExportImageTasksRequestDescribeExportImageTasksPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportImageTasksRequestDescribeExportImageTasksPaginateTypeDef](./type_defs.md#describeexportimagetasksrequestdescribeexportimagetaskspaginatetypedef) 
## DescribeFastLaunchImagesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fast_launch_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeFastLaunchImages)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeFastLaunchImagesResultTypeDef](./type_defs.md#describefastlaunchimagesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFastLaunchImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeFastLaunchImagesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeFastLaunchImagesResultTypeDef](./type_defs.md#describefastlaunchimagesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFastLaunchImagesRequestDescribeFastLaunchImagesPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFastLaunchImagesRequestDescribeFastLaunchImagesPaginateTypeDef](./type_defs.md#describefastlaunchimagesrequestdescribefastlaunchimagespaginatetypedef) 
## DescribeFastSnapshotRestoresPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fast_snapshot_restores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeFastSnapshotRestores)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeFastSnapshotRestoresResultTypeDef](./type_defs.md#describefastsnapshotrestoresresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFastSnapshotRestoresPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeFastSnapshotRestoresResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeFastSnapshotRestoresResultTypeDef](./type_defs.md#describefastsnapshotrestoresresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFastSnapshotRestoresRequestDescribeFastSnapshotRestoresPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFastSnapshotRestoresRequestDescribeFastSnapshotRestoresPaginateTypeDef](./type_defs.md#describefastsnapshotrestoresrequestdescribefastsnapshotrestorespaginatetypedef) 
## DescribeFleetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeFleets)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeFleetsResultTypeDef](./type_defs.md#describefleetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFleetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    FleetIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeFleetsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeFleetsResultTypeDef](./type_defs.md#describefleetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFleetsRequestDescribeFleetsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFleetsRequestDescribeFleetsPaginateTypeDef](./type_defs.md#describefleetsrequestdescribefleetspaginatetypedef) 
## DescribeFlowLogsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_flow_logs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeFlowLogs)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeFlowLogsResultTypeDef](./type_defs.md#describeflowlogsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFlowLogsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    FlowLogIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeFlowLogsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeFlowLogsResultTypeDef](./type_defs.md#describeflowlogsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFlowLogsRequestDescribeFlowLogsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFlowLogsRequestDescribeFlowLogsPaginateTypeDef](./type_defs.md#describeflowlogsrequestdescribeflowlogspaginatetypedef) 
## DescribeFpgaImagesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_fpga_images")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeFpgaImages)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeFpgaImagesResultTypeDef](./type_defs.md#describefpgaimagesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeFpgaImagesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    FpgaImageIds: Sequence[str] = ...,
    Owners: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeFpgaImagesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeFpgaImagesResultTypeDef](./type_defs.md#describefpgaimagesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeFpgaImagesRequestDescribeFpgaImagesPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeFpgaImagesRequestDescribeFpgaImagesPaginateTypeDef](./type_defs.md#describefpgaimagesrequestdescribefpgaimagespaginatetypedef) 
## DescribeHostReservationOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_host_reservation_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeHostReservationOfferings)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeHostReservationOfferingsResultTypeDef](./type_defs.md#describehostreservationofferingsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeHostReservationOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxDuration: int = ...,
    MinDuration: int = ...,
    OfferingId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeHostReservationOfferingsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeHostReservationOfferingsResultTypeDef](./type_defs.md#describehostreservationofferingsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeHostReservationOfferingsRequestDescribeHostReservationOfferingsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHostReservationOfferingsRequestDescribeHostReservationOfferingsPaginateTypeDef](./type_defs.md#describehostreservationofferingsrequestdescribehostreservationofferingspaginatetypedef) 
## DescribeHostReservationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_host_reservations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeHostReservations)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeHostReservationsResultTypeDef](./type_defs.md#describehostreservationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeHostReservationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    HostReservationIdSet: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeHostReservationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeHostReservationsResultTypeDef](./type_defs.md#describehostreservationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeHostReservationsRequestDescribeHostReservationsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHostReservationsRequestDescribeHostReservationsPaginateTypeDef](./type_defs.md#describehostreservationsrequestdescribehostreservationspaginatetypedef) 
## DescribeHostsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_hosts")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeHosts)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeHostsResultTypeDef](./type_defs.md#describehostsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeHostsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    HostIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeHostsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeHostsResultTypeDef](./type_defs.md#describehostsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeHostsRequestDescribeHostsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeHostsRequestDescribeHostsPaginateTypeDef](./type_defs.md#describehostsrequestdescribehostspaginatetypedef) 
## DescribeIamInstanceProfileAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_iam_instance_profile_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeIamInstanceProfileAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeIamInstanceProfileAssociationsResultTypeDef](./type_defs.md#describeiaminstanceprofileassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIamInstanceProfileAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeIamInstanceProfileAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeIamInstanceProfileAssociationsResultTypeDef](./type_defs.md#describeiaminstanceprofileassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeIamInstanceProfileAssociationsRequestDescribeIamInstanceProfileAssociationsPaginateTypeDef = {  # (1)
    "AssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIamInstanceProfileAssociationsRequestDescribeIamInstanceProfileAssociationsPaginateTypeDef](./type_defs.md#describeiaminstanceprofileassociationsrequestdescribeiaminstanceprofileassociationspaginatetypedef) 
## DescribeImportImageTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_import_image_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeImportImageTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeImportImageTasksResultTypeDef](./type_defs.md#describeimportimagetasksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImportImageTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ImportTaskIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeImportImageTasksResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImportImageTasksResultTypeDef](./type_defs.md#describeimportimagetasksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImportImageTasksRequestDescribeImportImageTasksPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImportImageTasksRequestDescribeImportImageTasksPaginateTypeDef](./type_defs.md#describeimportimagetasksrequestdescribeimportimagetaskspaginatetypedef) 
## DescribeImportSnapshotTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_import_snapshot_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeImportSnapshotTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeImportSnapshotTasksResultTypeDef](./type_defs.md#describeimportsnapshottasksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeImportSnapshotTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ImportTaskIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeImportSnapshotTasksResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeImportSnapshotTasksResultTypeDef](./type_defs.md#describeimportsnapshottasksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeImportSnapshotTasksRequestDescribeImportSnapshotTasksPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeImportSnapshotTasksRequestDescribeImportSnapshotTasksPaginateTypeDef](./type_defs.md#describeimportsnapshottasksrequestdescribeimportsnapshottaskspaginatetypedef) 
## DescribeInstanceCreditSpecificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_credit_specifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeInstanceCreditSpecifications)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeInstanceCreditSpecificationsResultTypeDef](./type_defs.md#describeinstancecreditspecificationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInstanceCreditSpecificationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    InstanceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeInstanceCreditSpecificationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeInstanceCreditSpecificationsResultTypeDef](./type_defs.md#describeinstancecreditspecificationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInstanceCreditSpecificationsRequestDescribeInstanceCreditSpecificationsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceCreditSpecificationsRequestDescribeInstanceCreditSpecificationsPaginateTypeDef](./type_defs.md#describeinstancecreditspecificationsrequestdescribeinstancecreditspecificationspaginatetypedef) 
## DescribeInstanceEventWindowsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_event_windows")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeInstanceEventWindows)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeInstanceEventWindowsResultTypeDef](./type_defs.md#describeinstanceeventwindowsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInstanceEventWindowsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    InstanceEventWindowIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeInstanceEventWindowsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeInstanceEventWindowsResultTypeDef](./type_defs.md#describeinstanceeventwindowsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInstanceEventWindowsRequestDescribeInstanceEventWindowsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceEventWindowsRequestDescribeInstanceEventWindowsPaginateTypeDef](./type_defs.md#describeinstanceeventwindowsrequestdescribeinstanceeventwindowspaginatetypedef) 
## DescribeInstanceStatusPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeInstanceStatus)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeInstanceStatusResultTypeDef](./type_defs.md#describeinstancestatusresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInstanceStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    IncludeAllInstances: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeInstanceStatusResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeInstanceStatusResultTypeDef](./type_defs.md#describeinstancestatusresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInstanceStatusRequestDescribeInstanceStatusPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceStatusRequestDescribeInstanceStatusPaginateTypeDef](./type_defs.md#describeinstancestatusrequestdescribeinstancestatuspaginatetypedef) 
## DescribeInstanceTypeOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_type_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeInstanceTypeOfferings)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeInstanceTypeOfferingsResultTypeDef](./type_defs.md#describeinstancetypeofferingsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInstanceTypeOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    LocationType: LocationTypeType = ...,  # (1)
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeInstanceTypeOfferingsResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: LocationTypeType](./literals.md#locationtypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeInstanceTypeOfferingsResultTypeDef](./type_defs.md#describeinstancetypeofferingsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInstanceTypeOfferingsRequestDescribeInstanceTypeOfferingsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceTypeOfferingsRequestDescribeInstanceTypeOfferingsPaginateTypeDef](./type_defs.md#describeinstancetypeofferingsrequestdescribeinstancetypeofferingspaginatetypedef) 
## DescribeInstanceTypesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instance_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeInstanceTypes)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeInstanceTypesResultTypeDef](./type_defs.md#describeinstancetypesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInstanceTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    InstanceTypes: Sequence[InstanceTypeType] = ...,  # (1)
    Filters: Sequence[FilterTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeInstanceTypesResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
2. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeInstanceTypesResultTypeDef](./type_defs.md#describeinstancetypesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInstanceTypesRequestDescribeInstanceTypesPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceTypesRequestDescribeInstanceTypesPaginateTypeDef](./type_defs.md#describeinstancetypesrequestdescribeinstancetypespaginatetypedef) 
## DescribeInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeInstances)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeInstancesResultTypeDef](./type_defs.md#describeinstancesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    InstanceIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeInstancesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeInstancesResultTypeDef](./type_defs.md#describeinstancesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInstancesRequestDescribeInstancesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInstancesRequestDescribeInstancesPaginateTypeDef](./type_defs.md#describeinstancesrequestdescribeinstancespaginatetypedef) 
## DescribeInternetGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_internet_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeInternetGateways)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeInternetGatewaysResultTypeDef](./type_defs.md#describeinternetgatewaysresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeInternetGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    InternetGatewayIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeInternetGatewaysResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeInternetGatewaysResultTypeDef](./type_defs.md#describeinternetgatewaysresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeInternetGatewaysRequestDescribeInternetGatewaysPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeInternetGatewaysRequestDescribeInternetGatewaysPaginateTypeDef](./type_defs.md#describeinternetgatewaysrequestdescribeinternetgatewayspaginatetypedef) 
## DescribeIpamPoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeIpamPools)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeIpamPoolsResultTypeDef](./type_defs.md#describeipampoolsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIpamPoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamPoolIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeIpamPoolsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeIpamPoolsResultTypeDef](./type_defs.md#describeipampoolsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeIpamPoolsRequestDescribeIpamPoolsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamPoolsRequestDescribeIpamPoolsPaginateTypeDef](./type_defs.md#describeipampoolsrequestdescribeipampoolspaginatetypedef) 
## DescribeIpamScopesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipam_scopes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeIpamScopes)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeIpamScopesResultTypeDef](./type_defs.md#describeipamscopesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIpamScopesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamScopeIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeIpamScopesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeIpamScopesResultTypeDef](./type_defs.md#describeipamscopesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeIpamScopesRequestDescribeIpamScopesPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamScopesRequestDescribeIpamScopesPaginateTypeDef](./type_defs.md#describeipamscopesrequestdescribeipamscopespaginatetypedef) 
## DescribeIpamsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeIpams)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeIpamsResultTypeDef](./type_defs.md#describeipamsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIpamsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IpamIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeIpamsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeIpamsResultTypeDef](./type_defs.md#describeipamsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeIpamsRequestDescribeIpamsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpamsRequestDescribeIpamsPaginateTypeDef](./type_defs.md#describeipamsrequestdescribeipamspaginatetypedef) 
## DescribeIpv6PoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_ipv6_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeIpv6Pools)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeIpv6PoolsResultTypeDef](./type_defs.md#describeipv6poolsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeIpv6PoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeIpv6PoolsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeIpv6PoolsResultTypeDef](./type_defs.md#describeipv6poolsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeIpv6PoolsRequestDescribeIpv6PoolsPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeIpv6PoolsRequestDescribeIpv6PoolsPaginateTypeDef](./type_defs.md#describeipv6poolsrequestdescribeipv6poolspaginatetypedef) 
## DescribeLaunchTemplateVersionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_launch_template_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLaunchTemplateVersions)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLaunchTemplateVersionsResultTypeDef](./type_defs.md#describelaunchtemplateversionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLaunchTemplateVersionsPaginator.paginate` method.

```python title="Method definition"
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
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLaunchTemplateVersionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLaunchTemplateVersionsResultTypeDef](./type_defs.md#describelaunchtemplateversionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLaunchTemplateVersionsRequestDescribeLaunchTemplateVersionsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchTemplateVersionsRequestDescribeLaunchTemplateVersionsPaginateTypeDef](./type_defs.md#describelaunchtemplateversionsrequestdescribelaunchtemplateversionspaginatetypedef) 
## DescribeLaunchTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_launch_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLaunchTemplates)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLaunchTemplatesResultTypeDef](./type_defs.md#describelaunchtemplatesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLaunchTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    LaunchTemplateIds: Sequence[str] = ...,
    LaunchTemplateNames: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLaunchTemplatesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLaunchTemplatesResultTypeDef](./type_defs.md#describelaunchtemplatesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLaunchTemplatesRequestDescribeLaunchTemplatesPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLaunchTemplatesRequestDescribeLaunchTemplatesPaginateTypeDef](./type_defs.md#describelaunchtemplatesrequestdescribelaunchtemplatespaginatetypedef) 
## DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_route_table_virtual_interface_group_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef](./type_defs.md#describelocalgatewayroutetablevirtualinterfacegroupassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LocalGatewayRouteTableVirtualInterfaceGroupAssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsResultTypeDef](./type_defs.md#describelocalgatewayroutetablevirtualinterfacegroupassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsRequestDescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableVirtualInterfaceGroupAssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsRequestDescribeLocalGatewayRouteTableVirtualInterfaceGroupAssociationsPaginateTypeDef](./type_defs.md#describelocalgatewayroutetablevirtualinterfacegroupassociationsrequestdescribelocalgatewayroutetablevirtualinterfacegroupassociationspaginatetypedef) 
## DescribeLocalGatewayRouteTableVpcAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_route_table_vpc_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLocalGatewayRouteTableVpcAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef](./type_defs.md#describelocalgatewayroutetablevpcassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayRouteTableVpcAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LocalGatewayRouteTableVpcAssociationIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLocalGatewayRouteTableVpcAssociationsResultTypeDef](./type_defs.md#describelocalgatewayroutetablevpcassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLocalGatewayRouteTableVpcAssociationsRequestDescribeLocalGatewayRouteTableVpcAssociationsPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableVpcAssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayRouteTableVpcAssociationsRequestDescribeLocalGatewayRouteTableVpcAssociationsPaginateTypeDef](./type_defs.md#describelocalgatewayroutetablevpcassociationsrequestdescribelocalgatewayroutetablevpcassociationspaginatetypedef) 
## DescribeLocalGatewayRouteTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_route_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLocalGatewayRouteTables)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLocalGatewayRouteTablesResultTypeDef](./type_defs.md#describelocalgatewayroutetablesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayRouteTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LocalGatewayRouteTableIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLocalGatewayRouteTablesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLocalGatewayRouteTablesResultTypeDef](./type_defs.md#describelocalgatewayroutetablesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLocalGatewayRouteTablesRequestDescribeLocalGatewayRouteTablesPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayRouteTablesRequestDescribeLocalGatewayRouteTablesPaginateTypeDef](./type_defs.md#describelocalgatewayroutetablesrequestdescribelocalgatewayroutetablespaginatetypedef) 
## DescribeLocalGatewayVirtualInterfaceGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_virtual_interface_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLocalGatewayVirtualInterfaceGroups)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacegroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayVirtualInterfaceGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LocalGatewayVirtualInterfaceGroupIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLocalGatewayVirtualInterfaceGroupsResultTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacegroupsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLocalGatewayVirtualInterfaceGroupsRequestDescribeLocalGatewayVirtualInterfaceGroupsPaginateTypeDef = {  # (1)
    "LocalGatewayVirtualInterfaceGroupIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayVirtualInterfaceGroupsRequestDescribeLocalGatewayVirtualInterfaceGroupsPaginateTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacegroupsrequestdescribelocalgatewayvirtualinterfacegroupspaginatetypedef) 
## DescribeLocalGatewayVirtualInterfacesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateway_virtual_interfaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLocalGatewayVirtualInterfaces)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLocalGatewayVirtualInterfacesResultTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewayVirtualInterfacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LocalGatewayVirtualInterfaceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLocalGatewayVirtualInterfacesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLocalGatewayVirtualInterfacesResultTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLocalGatewayVirtualInterfacesRequestDescribeLocalGatewayVirtualInterfacesPaginateTypeDef = {  # (1)
    "LocalGatewayVirtualInterfaceIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewayVirtualInterfacesRequestDescribeLocalGatewayVirtualInterfacesPaginateTypeDef](./type_defs.md#describelocalgatewayvirtualinterfacesrequestdescribelocalgatewayvirtualinterfacespaginatetypedef) 
## DescribeLocalGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_local_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeLocalGateways)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeLocalGatewaysResultTypeDef](./type_defs.md#describelocalgatewaysresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLocalGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LocalGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeLocalGatewaysResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLocalGatewaysResultTypeDef](./type_defs.md#describelocalgatewaysresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeLocalGatewaysRequestDescribeLocalGatewaysPaginateTypeDef = {  # (1)
    "LocalGatewayIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLocalGatewaysRequestDescribeLocalGatewaysPaginateTypeDef](./type_defs.md#describelocalgatewaysrequestdescribelocalgatewayspaginatetypedef) 
## DescribeManagedPrefixListsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_managed_prefix_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeManagedPrefixLists)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeManagedPrefixListsResultTypeDef](./type_defs.md#describemanagedprefixlistsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeManagedPrefixListsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PrefixListIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeManagedPrefixListsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeManagedPrefixListsResultTypeDef](./type_defs.md#describemanagedprefixlistsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeManagedPrefixListsRequestDescribeManagedPrefixListsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeManagedPrefixListsRequestDescribeManagedPrefixListsPaginateTypeDef](./type_defs.md#describemanagedprefixlistsrequestdescribemanagedprefixlistspaginatetypedef) 
## DescribeMovingAddressesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_moving_addresses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeMovingAddresses)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeMovingAddressesResultTypeDef](./type_defs.md#describemovingaddressesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeMovingAddressesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PublicIps: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeMovingAddressesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeMovingAddressesResultTypeDef](./type_defs.md#describemovingaddressesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeMovingAddressesRequestDescribeMovingAddressesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMovingAddressesRequestDescribeMovingAddressesPaginateTypeDef](./type_defs.md#describemovingaddressesrequestdescribemovingaddressespaginatetypedef) 
## DescribeNatGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_nat_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNatGateways)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNatGatewaysResultTypeDef](./type_defs.md#describenatgatewaysresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNatGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    NatGatewayIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNatGatewaysResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNatGatewaysResultTypeDef](./type_defs.md#describenatgatewaysresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNatGatewaysRequestDescribeNatGatewaysPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNatGatewaysRequestDescribeNatGatewaysPaginateTypeDef](./type_defs.md#describenatgatewaysrequestdescribenatgatewayspaginatetypedef) 
## DescribeNetworkAclsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_acls")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNetworkAcls)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNetworkAclsResultTypeDef](./type_defs.md#describenetworkaclsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNetworkAclsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    NetworkAclIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNetworkAclsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNetworkAclsResultTypeDef](./type_defs.md#describenetworkaclsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNetworkAclsRequestDescribeNetworkAclsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkAclsRequestDescribeNetworkAclsPaginateTypeDef](./type_defs.md#describenetworkaclsrequestdescribenetworkaclspaginatetypedef) 
## DescribeNetworkInsightsAccessScopeAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_access_scope_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNetworkInsightsAccessScopeAnalyses)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef](./type_defs.md#describenetworkinsightsaccessscopeanalysesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsAccessScopeAnalysesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    NetworkInsightsAccessScopeAnalysisIds: Sequence[str] = ...,
    NetworkInsightsAccessScopeId: str = ...,
    AnalysisStartTimeBegin: Union[datetime, str] = ...,
    AnalysisStartTimeEnd: Union[datetime, str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNetworkInsightsAccessScopeAnalysesResultTypeDef](./type_defs.md#describenetworkinsightsaccessscopeanalysesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNetworkInsightsAccessScopeAnalysesRequestDescribeNetworkInsightsAccessScopeAnalysesPaginateTypeDef = {  # (1)
    "NetworkInsightsAccessScopeAnalysisIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsAccessScopeAnalysesRequestDescribeNetworkInsightsAccessScopeAnalysesPaginateTypeDef](./type_defs.md#describenetworkinsightsaccessscopeanalysesrequestdescribenetworkinsightsaccessscopeanalysespaginatetypedef) 
## DescribeNetworkInsightsAccessScopesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_access_scopes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNetworkInsightsAccessScopes)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNetworkInsightsAccessScopesResultTypeDef](./type_defs.md#describenetworkinsightsaccessscopesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsAccessScopesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    NetworkInsightsAccessScopeIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNetworkInsightsAccessScopesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNetworkInsightsAccessScopesResultTypeDef](./type_defs.md#describenetworkinsightsaccessscopesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNetworkInsightsAccessScopesRequestDescribeNetworkInsightsAccessScopesPaginateTypeDef = {  # (1)
    "NetworkInsightsAccessScopeIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsAccessScopesRequestDescribeNetworkInsightsAccessScopesPaginateTypeDef](./type_defs.md#describenetworkinsightsaccessscopesrequestdescribenetworkinsightsaccessscopespaginatetypedef) 
## DescribeNetworkInsightsAnalysesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_analyses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNetworkInsightsAnalyses)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNetworkInsightsAnalysesResultTypeDef](./type_defs.md#describenetworkinsightsanalysesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsAnalysesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    NetworkInsightsAnalysisIds: Sequence[str] = ...,
    NetworkInsightsPathId: str = ...,
    AnalysisStartTime: Union[datetime, str] = ...,
    AnalysisEndTime: Union[datetime, str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNetworkInsightsAnalysesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNetworkInsightsAnalysesResultTypeDef](./type_defs.md#describenetworkinsightsanalysesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNetworkInsightsAnalysesRequestDescribeNetworkInsightsAnalysesPaginateTypeDef = {  # (1)
    "NetworkInsightsAnalysisIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsAnalysesRequestDescribeNetworkInsightsAnalysesPaginateTypeDef](./type_defs.md#describenetworkinsightsanalysesrequestdescribenetworkinsightsanalysespaginatetypedef) 
## DescribeNetworkInsightsPathsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_insights_paths")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNetworkInsightsPaths)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNetworkInsightsPathsResultTypeDef](./type_defs.md#describenetworkinsightspathsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNetworkInsightsPathsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    NetworkInsightsPathIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNetworkInsightsPathsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNetworkInsightsPathsResultTypeDef](./type_defs.md#describenetworkinsightspathsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNetworkInsightsPathsRequestDescribeNetworkInsightsPathsPaginateTypeDef = {  # (1)
    "NetworkInsightsPathIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInsightsPathsRequestDescribeNetworkInsightsPathsPaginateTypeDef](./type_defs.md#describenetworkinsightspathsrequestdescribenetworkinsightspathspaginatetypedef) 
## DescribeNetworkInterfacePermissionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_interface_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNetworkInterfacePermissions)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNetworkInterfacePermissionsResultTypeDef](./type_defs.md#describenetworkinterfacepermissionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNetworkInterfacePermissionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    NetworkInterfacePermissionIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNetworkInterfacePermissionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNetworkInterfacePermissionsResultTypeDef](./type_defs.md#describenetworkinterfacepermissionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNetworkInterfacePermissionsRequestDescribeNetworkInterfacePermissionsPaginateTypeDef = {  # (1)
    "NetworkInterfacePermissionIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInterfacePermissionsRequestDescribeNetworkInterfacePermissionsPaginateTypeDef](./type_defs.md#describenetworkinterfacepermissionsrequestdescribenetworkinterfacepermissionspaginatetypedef) 
## DescribeNetworkInterfacesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_network_interfaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeNetworkInterfaces)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeNetworkInterfacesResultTypeDef](./type_defs.md#describenetworkinterfacesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeNetworkInterfacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    NetworkInterfaceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeNetworkInterfacesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeNetworkInterfacesResultTypeDef](./type_defs.md#describenetworkinterfacesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeNetworkInterfacesRequestDescribeNetworkInterfacesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkInterfacesRequestDescribeNetworkInterfacesPaginateTypeDef](./type_defs.md#describenetworkinterfacesrequestdescribenetworkinterfacespaginatetypedef) 
## DescribePrefixListsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_prefix_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribePrefixLists)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribePrefixListsResultTypeDef](./type_defs.md#describeprefixlistsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribePrefixListsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PrefixListIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribePrefixListsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribePrefixListsResultTypeDef](./type_defs.md#describeprefixlistsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePrefixListsRequestDescribePrefixListsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePrefixListsRequestDescribePrefixListsPaginateTypeDef](./type_defs.md#describeprefixlistsrequestdescribeprefixlistspaginatetypedef) 
## DescribePrincipalIdFormatPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_principal_id_format")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribePrincipalIdFormat)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribePrincipalIdFormatResultTypeDef](./type_defs.md#describeprincipalidformatresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribePrincipalIdFormatPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Resources: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribePrincipalIdFormatResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribePrincipalIdFormatResultTypeDef](./type_defs.md#describeprincipalidformatresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePrincipalIdFormatRequestDescribePrincipalIdFormatPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePrincipalIdFormatRequestDescribePrincipalIdFormatPaginateTypeDef](./type_defs.md#describeprincipalidformatrequestdescribeprincipalidformatpaginatetypedef) 
## DescribePublicIpv4PoolsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_public_ipv4_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribePublicIpv4Pools)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribePublicIpv4PoolsResultTypeDef](./type_defs.md#describepublicipv4poolsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribePublicIpv4PoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribePublicIpv4PoolsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribePublicIpv4PoolsResultTypeDef](./type_defs.md#describepublicipv4poolsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribePublicIpv4PoolsRequestDescribePublicIpv4PoolsPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePublicIpv4PoolsRequestDescribePublicIpv4PoolsPaginateTypeDef](./type_defs.md#describepublicipv4poolsrequestdescribepublicipv4poolspaginatetypedef) 
## DescribeReplaceRootVolumeTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_replace_root_volume_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeReplaceRootVolumeTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeReplaceRootVolumeTasksResultTypeDef](./type_defs.md#describereplacerootvolumetasksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReplaceRootVolumeTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ReplaceRootVolumeTaskIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeReplaceRootVolumeTasksResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReplaceRootVolumeTasksResultTypeDef](./type_defs.md#describereplacerootvolumetasksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReplaceRootVolumeTasksRequestDescribeReplaceRootVolumeTasksPaginateTypeDef = {  # (1)
    "ReplaceRootVolumeTaskIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReplaceRootVolumeTasksRequestDescribeReplaceRootVolumeTasksPaginateTypeDef](./type_defs.md#describereplacerootvolumetasksrequestdescribereplacerootvolumetaskspaginatetypedef) 
## DescribeReservedInstancesModificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_reserved_instances_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeReservedInstancesModifications)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeReservedInstancesModificationsResultTypeDef](./type_defs.md#describereservedinstancesmodificationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedInstancesModificationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ReservedInstancesModificationIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeReservedInstancesModificationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeReservedInstancesModificationsResultTypeDef](./type_defs.md#describereservedinstancesmodificationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedInstancesModificationsRequestDescribeReservedInstancesModificationsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedInstancesModificationsRequestDescribeReservedInstancesModificationsPaginateTypeDef](./type_defs.md#describereservedinstancesmodificationsrequestdescribereservedinstancesmodificationspaginatetypedef) 
## DescribeReservedInstancesOfferingsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_reserved_instances_offerings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeReservedInstancesOfferings)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeReservedInstancesOfferingsResultTypeDef](./type_defs.md#describereservedinstancesofferingsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeReservedInstancesOfferingsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AvailabilityZone: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    IncludeMarketplace: bool = ...,
    InstanceType: InstanceTypeType = ...,  # (2)
    MaxDuration: int = ...,
    MaxInstanceCount: int = ...,
    MinDuration: int = ...,
    OfferingClass: OfferingClassTypeType = ...,  # (3)
    ProductDescription: RIProductDescriptionType = ...,  # (4)
    ReservedInstancesOfferingIds: Sequence[str] = ...,
    DryRun: bool = ...,
    InstanceTenancy: TenancyType = ...,  # (5)
    OfferingType: OfferingTypeValuesType = ...,  # (6)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (7)
) -> AsyncIterator[DescribeReservedInstancesOfferingsResultTypeDef]:  # (8)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-brackets: OfferingClassTypeType](./literals.md#offeringclasstypetype) 
4. See [:material-code-brackets: RIProductDescriptionType](./literals.md#riproductdescriptiontype) 
5. See [:material-code-brackets: TenancyType](./literals.md#tenancytype) 
6. See [:material-code-brackets: OfferingTypeValuesType](./literals.md#offeringtypevaluestype) 
7. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
8. See [:material-code-braces: DescribeReservedInstancesOfferingsResultTypeDef](./type_defs.md#describereservedinstancesofferingsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeReservedInstancesOfferingsRequestDescribeReservedInstancesOfferingsPaginateTypeDef = {  # (1)
    "AvailabilityZone": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeReservedInstancesOfferingsRequestDescribeReservedInstancesOfferingsPaginateTypeDef](./type_defs.md#describereservedinstancesofferingsrequestdescribereservedinstancesofferingspaginatetypedef) 
## DescribeRouteTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_route_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeRouteTables)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeRouteTablesResultTypeDef](./type_defs.md#describeroutetablesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRouteTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    RouteTableIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeRouteTablesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRouteTablesResultTypeDef](./type_defs.md#describeroutetablesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeRouteTablesRequestDescribeRouteTablesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRouteTablesRequestDescribeRouteTablesPaginateTypeDef](./type_defs.md#describeroutetablesrequestdescriberoutetablespaginatetypedef) 
## DescribeScheduledInstanceAvailabilityPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_scheduled_instance_availability")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeScheduledInstanceAvailability)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeScheduledInstanceAvailabilityResultTypeDef](./type_defs.md#describescheduledinstanceavailabilityresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScheduledInstanceAvailabilityPaginator.paginate` method.

```python title="Method definition"
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
) -> AsyncIterator[DescribeScheduledInstanceAvailabilityResultTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: SlotDateTimeRangeRequestTypeDef](./type_defs.md#slotdatetimerangerequesttypedef) 
2. See [:material-code-braces: ScheduledInstanceRecurrenceRequestTypeDef](./type_defs.md#scheduledinstancerecurrencerequesttypedef) 
3. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: DescribeScheduledInstanceAvailabilityResultTypeDef](./type_defs.md#describescheduledinstanceavailabilityresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeScheduledInstanceAvailabilityRequestDescribeScheduledInstanceAvailabilityPaginateTypeDef = {  # (1)
    "FirstSlotStartTimeRange": ...,
    "Recurrence": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledInstanceAvailabilityRequestDescribeScheduledInstanceAvailabilityPaginateTypeDef](./type_defs.md#describescheduledinstanceavailabilityrequestdescribescheduledinstanceavailabilitypaginatetypedef) 
## DescribeScheduledInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_scheduled_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeScheduledInstances)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeScheduledInstancesResultTypeDef](./type_defs.md#describescheduledinstancesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeScheduledInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    ScheduledInstanceIds: Sequence[str] = ...,
    SlotStartTimeRange: SlotStartTimeRangeRequestTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeScheduledInstancesResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SlotStartTimeRangeRequestTypeDef](./type_defs.md#slotstarttimerangerequesttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeScheduledInstancesResultTypeDef](./type_defs.md#describescheduledinstancesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeScheduledInstancesRequestDescribeScheduledInstancesPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeScheduledInstancesRequestDescribeScheduledInstancesPaginateTypeDef](./type_defs.md#describescheduledinstancesrequestdescribescheduledinstancespaginatetypedef) 
## DescribeSecurityGroupRulesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_security_group_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSecurityGroupRules)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSecurityGroupRulesResultTypeDef](./type_defs.md#describesecuritygrouprulesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSecurityGroupRulesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SecurityGroupRuleIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSecurityGroupRulesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSecurityGroupRulesResultTypeDef](./type_defs.md#describesecuritygrouprulesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSecurityGroupRulesRequestDescribeSecurityGroupRulesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityGroupRulesRequestDescribeSecurityGroupRulesPaginateTypeDef](./type_defs.md#describesecuritygrouprulesrequestdescribesecuritygrouprulespaginatetypedef) 
## DescribeSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSecurityGroups)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSecurityGroupsResultTypeDef](./type_defs.md#describesecuritygroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSecurityGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    GroupIds: Sequence[str] = ...,
    GroupNames: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSecurityGroupsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSecurityGroupsResultTypeDef](./type_defs.md#describesecuritygroupsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSecurityGroupsRequestDescribeSecurityGroupsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSecurityGroupsRequestDescribeSecurityGroupsPaginateTypeDef](./type_defs.md#describesecuritygroupsrequestdescribesecuritygroupspaginatetypedef) 
## DescribeSnapshotTierStatusPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_snapshot_tier_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSnapshotTierStatus)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSnapshotTierStatusResultTypeDef](./type_defs.md#describesnapshottierstatusresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotTierStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSnapshotTierStatusResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSnapshotTierStatusResultTypeDef](./type_defs.md#describesnapshottierstatusresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSnapshotTierStatusRequestDescribeSnapshotTierStatusPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotTierStatusRequestDescribeSnapshotTierStatusPaginateTypeDef](./type_defs.md#describesnapshottierstatusrequestdescribesnapshottierstatuspaginatetypedef) 
## DescribeSnapshotsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_snapshots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSnapshots)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSnapshotsResultTypeDef](./type_defs.md#describesnapshotsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSnapshotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    OwnerIds: Sequence[str] = ...,
    RestorableByUserIds: Sequence[str] = ...,
    SnapshotIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSnapshotsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSnapshotsResultTypeDef](./type_defs.md#describesnapshotsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSnapshotsRequestDescribeSnapshotsPaginateTypeDef](./type_defs.md#describesnapshotsrequestdescribesnapshotspaginatetypedef) 
## DescribeSpotFleetInstancesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_fleet_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotFleetInstances)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSpotFleetInstancesResponseTypeDef](./type_defs.md#describespotfleetinstancesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSpotFleetInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SpotFleetRequestId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSpotFleetInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSpotFleetInstancesResponseTypeDef](./type_defs.md#describespotfleetinstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSpotFleetInstancesRequestDescribeSpotFleetInstancesPaginateTypeDef = {  # (1)
    "SpotFleetRequestId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotFleetInstancesRequestDescribeSpotFleetInstancesPaginateTypeDef](./type_defs.md#describespotfleetinstancesrequestdescribespotfleetinstancespaginatetypedef) 
## DescribeSpotFleetRequestsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_fleet_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotFleetRequests)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSpotFleetRequestsResponseTypeDef](./type_defs.md#describespotfleetrequestsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSpotFleetRequestsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    SpotFleetRequestIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSpotFleetRequestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSpotFleetRequestsResponseTypeDef](./type_defs.md#describespotfleetrequestsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSpotFleetRequestsRequestDescribeSpotFleetRequestsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotFleetRequestsRequestDescribeSpotFleetRequestsPaginateTypeDef](./type_defs.md#describespotfleetrequestsrequestdescribespotfleetrequestspaginatetypedef) 
## DescribeSpotInstanceRequestsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_instance_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotInstanceRequests)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSpotInstanceRequestsResultTypeDef](./type_defs.md#describespotinstancerequestsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSpotInstanceRequestsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    SpotInstanceRequestIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSpotInstanceRequestsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSpotInstanceRequestsResultTypeDef](./type_defs.md#describespotinstancerequestsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSpotInstanceRequestsRequestDescribeSpotInstanceRequestsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotInstanceRequestsRequestDescribeSpotInstanceRequestsPaginateTypeDef](./type_defs.md#describespotinstancerequestsrequestdescribespotinstancerequestspaginatetypedef) 
## DescribeSpotPriceHistoryPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_spot_price_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotPriceHistory)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSpotPriceHistoryResultTypeDef](./type_defs.md#describespotpricehistoryresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSpotPriceHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    AvailabilityZone: str = ...,
    DryRun: bool = ...,
    EndTime: Union[datetime, str] = ...,
    InstanceTypes: Sequence[InstanceTypeType] = ...,  # (2)
    ProductDescriptions: Sequence[str] = ...,
    StartTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[DescribeSpotPriceHistoryResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: InstanceTypeType](./literals.md#instancetypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeSpotPriceHistoryResultTypeDef](./type_defs.md#describespotpricehistoryresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSpotPriceHistoryRequestDescribeSpotPriceHistoryPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpotPriceHistoryRequestDescribeSpotPriceHistoryPaginateTypeDef](./type_defs.md#describespotpricehistoryrequestdescribespotpricehistorypaginatetypedef) 
## DescribeStaleSecurityGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_stale_security_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeStaleSecurityGroups)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeStaleSecurityGroupsResultTypeDef](./type_defs.md#describestalesecuritygroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStaleSecurityGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    VpcId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeStaleSecurityGroupsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeStaleSecurityGroupsResultTypeDef](./type_defs.md#describestalesecuritygroupsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeStaleSecurityGroupsRequestDescribeStaleSecurityGroupsPaginateTypeDef = {  # (1)
    "VpcId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStaleSecurityGroupsRequestDescribeStaleSecurityGroupsPaginateTypeDef](./type_defs.md#describestalesecuritygroupsrequestdescribestalesecuritygroupspaginatetypedef) 
## DescribeStoreImageTasksPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_store_image_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeStoreImageTasks)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeStoreImageTasksResultTypeDef](./type_defs.md#describestoreimagetasksresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeStoreImageTasksPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeStoreImageTasksResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeStoreImageTasksResultTypeDef](./type_defs.md#describestoreimagetasksresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeStoreImageTasksRequestDescribeStoreImageTasksPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeStoreImageTasksRequestDescribeStoreImageTasksPaginateTypeDef](./type_defs.md#describestoreimagetasksrequestdescribestoreimagetaskspaginatetypedef) 
## DescribeSubnetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_subnets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSubnets)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeSubnetsResultTypeDef](./type_defs.md#describesubnetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSubnetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    SubnetIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeSubnetsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeSubnetsResultTypeDef](./type_defs.md#describesubnetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSubnetsRequestDescribeSubnetsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubnetsRequestDescribeSubnetsPaginateTypeDef](./type_defs.md#describesubnetsrequestdescribesubnetspaginatetypedef) 
## DescribeTagsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTags)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTagsResultTypeDef](./type_defs.md#describetagsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTagsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTagsResultTypeDef](./type_defs.md#describetagsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTagsRequestDescribeTagsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTagsRequestDescribeTagsPaginateTypeDef](./type_defs.md#describetagsrequestdescribetagspaginatetypedef) 
## DescribeTrafficMirrorFiltersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_traffic_mirror_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTrafficMirrorFilters)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTrafficMirrorFiltersResultTypeDef](./type_defs.md#describetrafficmirrorfiltersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTrafficMirrorFiltersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TrafficMirrorFilterIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTrafficMirrorFiltersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTrafficMirrorFiltersResultTypeDef](./type_defs.md#describetrafficmirrorfiltersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTrafficMirrorFiltersRequestDescribeTrafficMirrorFiltersPaginateTypeDef = {  # (1)
    "TrafficMirrorFilterIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrafficMirrorFiltersRequestDescribeTrafficMirrorFiltersPaginateTypeDef](./type_defs.md#describetrafficmirrorfiltersrequestdescribetrafficmirrorfilterspaginatetypedef) 
## DescribeTrafficMirrorSessionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_traffic_mirror_sessions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTrafficMirrorSessions)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTrafficMirrorSessionsResultTypeDef](./type_defs.md#describetrafficmirrorsessionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTrafficMirrorSessionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TrafficMirrorSessionIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTrafficMirrorSessionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTrafficMirrorSessionsResultTypeDef](./type_defs.md#describetrafficmirrorsessionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTrafficMirrorSessionsRequestDescribeTrafficMirrorSessionsPaginateTypeDef = {  # (1)
    "TrafficMirrorSessionIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrafficMirrorSessionsRequestDescribeTrafficMirrorSessionsPaginateTypeDef](./type_defs.md#describetrafficmirrorsessionsrequestdescribetrafficmirrorsessionspaginatetypedef) 
## DescribeTrafficMirrorTargetsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_traffic_mirror_targets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTrafficMirrorTargets)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTrafficMirrorTargetsResultTypeDef](./type_defs.md#describetrafficmirrortargetsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTrafficMirrorTargetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TrafficMirrorTargetIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTrafficMirrorTargetsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTrafficMirrorTargetsResultTypeDef](./type_defs.md#describetrafficmirrortargetsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTrafficMirrorTargetsRequestDescribeTrafficMirrorTargetsPaginateTypeDef = {  # (1)
    "TrafficMirrorTargetIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrafficMirrorTargetsRequestDescribeTrafficMirrorTargetsPaginateTypeDef](./type_defs.md#describetrafficmirrortargetsrequestdescribetrafficmirrortargetspaginatetypedef) 
## DescribeTransitGatewayAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayAttachments)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayAttachmentsResultTypeDef](./type_defs.md#describetransitgatewayattachmentsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayAttachmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayAttachmentsResultTypeDef](./type_defs.md#describetransitgatewayattachmentsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayAttachmentsRequestDescribeTransitGatewayAttachmentsPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayAttachmentsRequestDescribeTransitGatewayAttachmentsPaginateTypeDef](./type_defs.md#describetransitgatewayattachmentsrequestdescribetransitgatewayattachmentspaginatetypedef) 
## DescribeTransitGatewayConnectPeersPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_connect_peers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayConnectPeers)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayConnectPeersResultTypeDef](./type_defs.md#describetransitgatewayconnectpeersresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayConnectPeersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayConnectPeerIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayConnectPeersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayConnectPeersResultTypeDef](./type_defs.md#describetransitgatewayconnectpeersresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayConnectPeersRequestDescribeTransitGatewayConnectPeersPaginateTypeDef = {  # (1)
    "TransitGatewayConnectPeerIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayConnectPeersRequestDescribeTransitGatewayConnectPeersPaginateTypeDef](./type_defs.md#describetransitgatewayconnectpeersrequestdescribetransitgatewayconnectpeerspaginatetypedef) 
## DescribeTransitGatewayConnectsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_connects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayConnects)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayConnectsResultTypeDef](./type_defs.md#describetransitgatewayconnectsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayConnectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayConnectsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayConnectsResultTypeDef](./type_defs.md#describetransitgatewayconnectsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayConnectsRequestDescribeTransitGatewayConnectsPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayConnectsRequestDescribeTransitGatewayConnectsPaginateTypeDef](./type_defs.md#describetransitgatewayconnectsrequestdescribetransitgatewayconnectspaginatetypedef) 
## DescribeTransitGatewayMulticastDomainsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_multicast_domains")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayMulticastDomains)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayMulticastDomainsResultTypeDef](./type_defs.md#describetransitgatewaymulticastdomainsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayMulticastDomainsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayMulticastDomainIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayMulticastDomainsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayMulticastDomainsResultTypeDef](./type_defs.md#describetransitgatewaymulticastdomainsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayMulticastDomainsRequestDescribeTransitGatewayMulticastDomainsPaginateTypeDef = {  # (1)
    "TransitGatewayMulticastDomainIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayMulticastDomainsRequestDescribeTransitGatewayMulticastDomainsPaginateTypeDef](./type_defs.md#describetransitgatewaymulticastdomainsrequestdescribetransitgatewaymulticastdomainspaginatetypedef) 
## DescribeTransitGatewayPeeringAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_peering_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayPeeringAttachments)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayPeeringAttachmentsResultTypeDef](./type_defs.md#describetransitgatewaypeeringattachmentsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayPeeringAttachmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayPeeringAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayPeeringAttachmentsResultTypeDef](./type_defs.md#describetransitgatewaypeeringattachmentsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayPeeringAttachmentsRequestDescribeTransitGatewayPeeringAttachmentsPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayPeeringAttachmentsRequestDescribeTransitGatewayPeeringAttachmentsPaginateTypeDef](./type_defs.md#describetransitgatewaypeeringattachmentsrequestdescribetransitgatewaypeeringattachmentspaginatetypedef) 
## DescribeTransitGatewayPolicyTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_policy_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayPolicyTables)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayPolicyTablesResultTypeDef](./type_defs.md#describetransitgatewaypolicytablesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayPolicyTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayPolicyTableIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayPolicyTablesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayPolicyTablesResultTypeDef](./type_defs.md#describetransitgatewaypolicytablesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayPolicyTablesRequestDescribeTransitGatewayPolicyTablesPaginateTypeDef = {  # (1)
    "TransitGatewayPolicyTableIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayPolicyTablesRequestDescribeTransitGatewayPolicyTablesPaginateTypeDef](./type_defs.md#describetransitgatewaypolicytablesrequestdescribetransitgatewaypolicytablespaginatetypedef) 
## DescribeTransitGatewayRouteTableAnnouncementsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_route_table_announcements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayRouteTableAnnouncements)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef](./type_defs.md#describetransitgatewayroutetableannouncementsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayRouteTableAnnouncementsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayRouteTableAnnouncementIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayRouteTableAnnouncementsResultTypeDef](./type_defs.md#describetransitgatewayroutetableannouncementsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayRouteTableAnnouncementsRequestDescribeTransitGatewayRouteTableAnnouncementsPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableAnnouncementIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayRouteTableAnnouncementsRequestDescribeTransitGatewayRouteTableAnnouncementsPaginateTypeDef](./type_defs.md#describetransitgatewayroutetableannouncementsrequestdescribetransitgatewayroutetableannouncementspaginatetypedef) 
## DescribeTransitGatewayRouteTablesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_route_tables")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayRouteTables)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayRouteTablesResultTypeDef](./type_defs.md#describetransitgatewayroutetablesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayRouteTablesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayRouteTableIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayRouteTablesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayRouteTablesResultTypeDef](./type_defs.md#describetransitgatewayroutetablesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayRouteTablesRequestDescribeTransitGatewayRouteTablesPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayRouteTablesRequestDescribeTransitGatewayRouteTablesPaginateTypeDef](./type_defs.md#describetransitgatewayroutetablesrequestdescribetransitgatewayroutetablespaginatetypedef) 
## DescribeTransitGatewayVpcAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateway_vpc_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGatewayVpcAttachments)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewayVpcAttachmentsResultTypeDef](./type_defs.md#describetransitgatewayvpcattachmentsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewayVpcAttachmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewayVpcAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewayVpcAttachmentsResultTypeDef](./type_defs.md#describetransitgatewayvpcattachmentsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewayVpcAttachmentsRequestDescribeTransitGatewayVpcAttachmentsPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewayVpcAttachmentsRequestDescribeTransitGatewayVpcAttachmentsPaginateTypeDef](./type_defs.md#describetransitgatewayvpcattachmentsrequestdescribetransitgatewayvpcattachmentspaginatetypedef) 
## DescribeTransitGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_transit_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTransitGateways)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTransitGatewaysResultTypeDef](./type_defs.md#describetransitgatewaysresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTransitGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTransitGatewaysResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTransitGatewaysResultTypeDef](./type_defs.md#describetransitgatewaysresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTransitGatewaysRequestDescribeTransitGatewaysPaginateTypeDef = {  # (1)
    "TransitGatewayIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTransitGatewaysRequestDescribeTransitGatewaysPaginateTypeDef](./type_defs.md#describetransitgatewaysrequestdescribetransitgatewayspaginatetypedef) 
## DescribeTrunkInterfaceAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_trunk_interface_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeTrunkInterfaceAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeTrunkInterfaceAssociationsResultTypeDef](./type_defs.md#describetrunkinterfaceassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeTrunkInterfaceAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    AssociationIds: Sequence[str] = ...,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeTrunkInterfaceAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeTrunkInterfaceAssociationsResultTypeDef](./type_defs.md#describetrunkinterfaceassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeTrunkInterfaceAssociationsRequestDescribeTrunkInterfaceAssociationsPaginateTypeDef = {  # (1)
    "AssociationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeTrunkInterfaceAssociationsRequestDescribeTrunkInterfaceAssociationsPaginateTypeDef](./type_defs.md#describetrunkinterfaceassociationsrequestdescribetrunkinterfaceassociationspaginatetypedef) 
## DescribeVolumeStatusPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_volume_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVolumeStatus)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVolumeStatusResultTypeDef](./type_defs.md#describevolumestatusresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVolumeStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VolumeIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVolumeStatusResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVolumeStatusResultTypeDef](./type_defs.md#describevolumestatusresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVolumeStatusRequestDescribeVolumeStatusPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVolumeStatusRequestDescribeVolumeStatusPaginateTypeDef](./type_defs.md#describevolumestatusrequestdescribevolumestatuspaginatetypedef) 
## DescribeVolumesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_volumes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVolumes)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVolumesResultTypeDef](./type_defs.md#describevolumesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVolumesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VolumeIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVolumesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVolumesResultTypeDef](./type_defs.md#describevolumesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVolumesRequestDescribeVolumesPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesRequestDescribeVolumesPaginateTypeDef](./type_defs.md#describevolumesrequestdescribevolumespaginatetypedef) 
## DescribeVolumesModificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_volumes_modifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVolumesModifications)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVolumesModificationsResultTypeDef](./type_defs.md#describevolumesmodificationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVolumesModificationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    VolumeIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVolumesModificationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVolumesModificationsResultTypeDef](./type_defs.md#describevolumesmodificationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVolumesModificationsRequestDescribeVolumesModificationsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVolumesModificationsRequestDescribeVolumesModificationsPaginateTypeDef](./type_defs.md#describevolumesmodificationsrequestdescribevolumesmodificationspaginatetypedef) 
## DescribeVpcClassicLinkDnsSupportPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_classic_link_dns_support")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcClassicLinkDnsSupport)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcClassicLinkDnsSupportResultTypeDef](./type_defs.md#describevpcclassiclinkdnssupportresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcClassicLinkDnsSupportPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    VpcIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeVpcClassicLinkDnsSupportResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeVpcClassicLinkDnsSupportResultTypeDef](./type_defs.md#describevpcclassiclinkdnssupportresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcClassicLinkDnsSupportRequestDescribeVpcClassicLinkDnsSupportPaginateTypeDef = {  # (1)
    "VpcIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcClassicLinkDnsSupportRequestDescribeVpcClassicLinkDnsSupportPaginateTypeDef](./type_defs.md#describevpcclassiclinkdnssupportrequestdescribevpcclassiclinkdnssupportpaginatetypedef) 
## DescribeVpcEndpointConnectionNotificationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_connection_notifications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcEndpointConnectionNotifications)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcEndpointConnectionNotificationsResultTypeDef](./type_defs.md#describevpcendpointconnectionnotificationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointConnectionNotificationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    ConnectionNotificationId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcEndpointConnectionNotificationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcEndpointConnectionNotificationsResultTypeDef](./type_defs.md#describevpcendpointconnectionnotificationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcEndpointConnectionNotificationsRequestDescribeVpcEndpointConnectionNotificationsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointConnectionNotificationsRequestDescribeVpcEndpointConnectionNotificationsPaginateTypeDef](./type_defs.md#describevpcendpointconnectionnotificationsrequestdescribevpcendpointconnectionnotificationspaginatetypedef) 
## DescribeVpcEndpointConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcEndpointConnections)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcEndpointConnectionsResultTypeDef](./type_defs.md#describevpcendpointconnectionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointConnectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcEndpointConnectionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcEndpointConnectionsResultTypeDef](./type_defs.md#describevpcendpointconnectionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcEndpointConnectionsRequestDescribeVpcEndpointConnectionsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointConnectionsRequestDescribeVpcEndpointConnectionsPaginateTypeDef](./type_defs.md#describevpcendpointconnectionsrequestdescribevpcendpointconnectionspaginatetypedef) 
## DescribeVpcEndpointServiceConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_service_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcEndpointServiceConfigurations)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcEndpointServiceConfigurationsResultTypeDef](./type_defs.md#describevpcendpointserviceconfigurationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointServiceConfigurationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    ServiceIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcEndpointServiceConfigurationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcEndpointServiceConfigurationsResultTypeDef](./type_defs.md#describevpcendpointserviceconfigurationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcEndpointServiceConfigurationsRequestDescribeVpcEndpointServiceConfigurationsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointServiceConfigurationsRequestDescribeVpcEndpointServiceConfigurationsPaginateTypeDef](./type_defs.md#describevpcendpointserviceconfigurationsrequestdescribevpcendpointserviceconfigurationspaginatetypedef) 
## DescribeVpcEndpointServicePermissionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_service_permissions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcEndpointServicePermissions)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcEndpointServicePermissionsResultTypeDef](./type_defs.md#describevpcendpointservicepermissionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointServicePermissionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ServiceId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcEndpointServicePermissionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcEndpointServicePermissionsResultTypeDef](./type_defs.md#describevpcendpointservicepermissionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcEndpointServicePermissionsRequestDescribeVpcEndpointServicePermissionsPaginateTypeDef = {  # (1)
    "ServiceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointServicePermissionsRequestDescribeVpcEndpointServicePermissionsPaginateTypeDef](./type_defs.md#describevpcendpointservicepermissionsrequestdescribevpcendpointservicepermissionspaginatetypedef) 
## DescribeVpcEndpointServicesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoint_services")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcEndpointServices)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcEndpointServicesResultTypeDef](./type_defs.md#describevpcendpointservicesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointServicesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    ServiceNames: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcEndpointServicesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcEndpointServicesResultTypeDef](./type_defs.md#describevpcendpointservicesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcEndpointServicesRequestDescribeVpcEndpointServicesPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointServicesRequestDescribeVpcEndpointServicesPaginateTypeDef](./type_defs.md#describevpcendpointservicesrequestdescribevpcendpointservicespaginatetypedef) 
## DescribeVpcEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcEndpoints)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcEndpointsResultTypeDef](./type_defs.md#describevpcendpointsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcEndpointsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    VpcEndpointIds: Sequence[str] = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcEndpointsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcEndpointsResultTypeDef](./type_defs.md#describevpcendpointsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcEndpointsRequestDescribeVpcEndpointsPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointsRequestDescribeVpcEndpointsPaginateTypeDef](./type_defs.md#describevpcendpointsrequestdescribevpcendpointspaginatetypedef) 
## DescribeVpcPeeringConnectionsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpc_peering_connections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcPeeringConnections)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcPeeringConnectionsResultTypeDef](./type_defs.md#describevpcpeeringconnectionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcPeeringConnectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    VpcPeeringConnectionIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcPeeringConnectionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcPeeringConnectionsResultTypeDef](./type_defs.md#describevpcpeeringconnectionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcPeeringConnectionsRequestDescribeVpcPeeringConnectionsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcPeeringConnectionsRequestDescribeVpcPeeringConnectionsPaginateTypeDef](./type_defs.md#describevpcpeeringconnectionsrequestdescribevpcpeeringconnectionspaginatetypedef) 
## DescribeVpcsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("describe_vpcs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeVpcs)

```python title="Usage example"
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
3. item: [:material-code-braces: DescribeVpcsResultTypeDef](./type_defs.md#describevpcsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeVpcsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    VpcIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeVpcsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVpcsResultTypeDef](./type_defs.md#describevpcsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVpcsRequestDescribeVpcsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVpcsRequestDescribeVpcsPaginateTypeDef](./type_defs.md#describevpcsrequestdescribevpcspaginatetypedef) 
## GetAssociatedIpv6PoolCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_associated_ipv6_pool_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetAssociatedIpv6PoolCidrs)

```python title="Usage example"
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
3. item: [:material-code-braces: GetAssociatedIpv6PoolCidrsResultTypeDef](./type_defs.md#getassociatedipv6poolcidrsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetAssociatedIpv6PoolCidrsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PoolId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetAssociatedIpv6PoolCidrsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetAssociatedIpv6PoolCidrsResultTypeDef](./type_defs.md#getassociatedipv6poolcidrsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetAssociatedIpv6PoolCidrsRequestGetAssociatedIpv6PoolCidrsPaginateTypeDef = {  # (1)
    "PoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAssociatedIpv6PoolCidrsRequestGetAssociatedIpv6PoolCidrsPaginateTypeDef](./type_defs.md#getassociatedipv6poolcidrsrequestgetassociatedipv6poolcidrspaginatetypedef) 
## GetGroupsForCapacityReservationPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_groups_for_capacity_reservation")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetGroupsForCapacityReservation)

```python title="Usage example"
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
3. item: [:material-code-braces: GetGroupsForCapacityReservationResultTypeDef](./type_defs.md#getgroupsforcapacityreservationresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetGroupsForCapacityReservationPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CapacityReservationId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetGroupsForCapacityReservationResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetGroupsForCapacityReservationResultTypeDef](./type_defs.md#getgroupsforcapacityreservationresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetGroupsForCapacityReservationRequestGetGroupsForCapacityReservationPaginateTypeDef = {  # (1)
    "CapacityReservationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetGroupsForCapacityReservationRequestGetGroupsForCapacityReservationPaginateTypeDef](./type_defs.md#getgroupsforcapacityreservationrequestgetgroupsforcapacityreservationpaginatetypedef) 
## GetInstanceTypesFromInstanceRequirementsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_instance_types_from_instance_requirements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetInstanceTypesFromInstanceRequirements)

```python title="Usage example"
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
3. item: [:material-code-braces: GetInstanceTypesFromInstanceRequirementsResultTypeDef](./type_defs.md#getinstancetypesfrominstancerequirementsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetInstanceTypesFromInstanceRequirementsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ArchitectureTypes: Sequence[ArchitectureTypeType],  # (1)
    VirtualizationTypes: Sequence[VirtualizationTypeType],  # (2)
    InstanceRequirements: InstanceRequirementsRequestTypeDef,  # (3)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> AsyncIterator[GetInstanceTypesFromInstanceRequirementsResultTypeDef]:  # (5)
    ...
```

1. See [:material-code-brackets: ArchitectureTypeType](./literals.md#architecturetypetype) 
2. See [:material-code-brackets: VirtualizationTypeType](./literals.md#virtualizationtypetype) 
3. See [:material-code-braces: InstanceRequirementsRequestTypeDef](./type_defs.md#instancerequirementsrequesttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetInstanceTypesFromInstanceRequirementsResultTypeDef](./type_defs.md#getinstancetypesfrominstancerequirementsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef = {  # (1)
    "ArchitectureTypes": ...,
    "VirtualizationTypes": ...,
    "InstanceRequirements": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef](./type_defs.md#getinstancetypesfrominstancerequirementsrequestgetinstancetypesfrominstancerequirementspaginatetypedef) 
## GetIpamAddressHistoryPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_address_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetIpamAddressHistory)

```python title="Usage example"
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
3. item: [:material-code-braces: GetIpamAddressHistoryResultTypeDef](./type_defs.md#getipamaddresshistoryresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetIpamAddressHistoryPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    Cidr: str,
    IpamScopeId: str,
    DryRun: bool = ...,
    VpcId: str = ...,
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetIpamAddressHistoryResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetIpamAddressHistoryResultTypeDef](./type_defs.md#getipamaddresshistoryresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetIpamAddressHistoryRequestGetIpamAddressHistoryPaginateTypeDef = {  # (1)
    "Cidr": ...,
    "IpamScopeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamAddressHistoryRequestGetIpamAddressHistoryPaginateTypeDef](./type_defs.md#getipamaddresshistoryrequestgetipamaddresshistorypaginatetypedef) 
## GetIpamPoolAllocationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_pool_allocations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetIpamPoolAllocations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetIpamPoolAllocationsResultTypeDef](./type_defs.md#getipampoolallocationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetIpamPoolAllocationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    IpamPoolId: str,
    DryRun: bool = ...,
    IpamPoolAllocationId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetIpamPoolAllocationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetIpamPoolAllocationsResultTypeDef](./type_defs.md#getipampoolallocationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetIpamPoolAllocationsRequestGetIpamPoolAllocationsPaginateTypeDef = {  # (1)
    "IpamPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamPoolAllocationsRequestGetIpamPoolAllocationsPaginateTypeDef](./type_defs.md#getipampoolallocationsrequestgetipampoolallocationspaginatetypedef) 
## GetIpamPoolCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_pool_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetIpamPoolCidrs)

```python title="Usage example"
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
3. item: [:material-code-braces: GetIpamPoolCidrsResultTypeDef](./type_defs.md#getipampoolcidrsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetIpamPoolCidrsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    IpamPoolId: str,
    DryRun: bool = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetIpamPoolCidrsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetIpamPoolCidrsResultTypeDef](./type_defs.md#getipampoolcidrsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetIpamPoolCidrsRequestGetIpamPoolCidrsPaginateTypeDef = {  # (1)
    "IpamPoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamPoolCidrsRequestGetIpamPoolCidrsPaginateTypeDef](./type_defs.md#getipampoolcidrsrequestgetipampoolcidrspaginatetypedef) 
## GetIpamResourceCidrsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_ipam_resource_cidrs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetIpamResourceCidrs)

```python title="Usage example"
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
3. item: [:material-code-braces: GetIpamResourceCidrsResultTypeDef](./type_defs.md#getipamresourcecidrsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetIpamResourceCidrsPaginator.paginate` method.

```python title="Method definition"
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
) -> AsyncIterator[GetIpamResourceCidrsResultTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: IpamResourceTypeType](./literals.md#ipamresourcetypetype) 
3. See [:material-code-braces: RequestIpamResourceTagTypeDef](./type_defs.md#requestipamresourcetagtypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: GetIpamResourceCidrsResultTypeDef](./type_defs.md#getipamresourcecidrsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetIpamResourceCidrsRequestGetIpamResourceCidrsPaginateTypeDef = {  # (1)
    "IpamScopeId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIpamResourceCidrsRequestGetIpamResourceCidrsPaginateTypeDef](./type_defs.md#getipamresourcecidrsrequestgetipamresourcecidrspaginatetypedef) 
## GetManagedPrefixListAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_managed_prefix_list_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetManagedPrefixListAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetManagedPrefixListAssociationsResultTypeDef](./type_defs.md#getmanagedprefixlistassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetManagedPrefixListAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PrefixListId: str,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetManagedPrefixListAssociationsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetManagedPrefixListAssociationsResultTypeDef](./type_defs.md#getmanagedprefixlistassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetManagedPrefixListAssociationsRequestGetManagedPrefixListAssociationsPaginateTypeDef = {  # (1)
    "PrefixListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetManagedPrefixListAssociationsRequestGetManagedPrefixListAssociationsPaginateTypeDef](./type_defs.md#getmanagedprefixlistassociationsrequestgetmanagedprefixlistassociationspaginatetypedef) 
## GetManagedPrefixListEntriesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_managed_prefix_list_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetManagedPrefixListEntries)

```python title="Usage example"
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
3. item: [:material-code-braces: GetManagedPrefixListEntriesResultTypeDef](./type_defs.md#getmanagedprefixlistentriesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetManagedPrefixListEntriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PrefixListId: str,
    DryRun: bool = ...,
    TargetVersion: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetManagedPrefixListEntriesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetManagedPrefixListEntriesResultTypeDef](./type_defs.md#getmanagedprefixlistentriesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetManagedPrefixListEntriesRequestGetManagedPrefixListEntriesPaginateTypeDef = {  # (1)
    "PrefixListId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetManagedPrefixListEntriesRequestGetManagedPrefixListEntriesPaginateTypeDef](./type_defs.md#getmanagedprefixlistentriesrequestgetmanagedprefixlistentriespaginatetypedef) 
## GetSpotPlacementScoresPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_spot_placement_scores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetSpotPlacementScores)

```python title="Usage example"
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
3. item: [:material-code-braces: GetSpotPlacementScoresResultTypeDef](./type_defs.md#getspotplacementscoresresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetSpotPlacementScoresPaginator.paginate` method.

```python title="Method definition"
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
) -> AsyncIterator[GetSpotPlacementScoresResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: TargetCapacityUnitTypeType](./literals.md#targetcapacityunittypetype) 
2. See [:material-code-braces: InstanceRequirementsWithMetadataRequestTypeDef](./type_defs.md#instancerequirementswithmetadatarequesttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetSpotPlacementScoresResultTypeDef](./type_defs.md#getspotplacementscoresresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef = {  # (1)
    "TargetCapacity": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef](./type_defs.md#getspotplacementscoresrequestgetspotplacementscorespaginatetypedef) 
## GetTransitGatewayAttachmentPropagationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_attachment_propagations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetTransitGatewayAttachmentPropagations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetTransitGatewayAttachmentPropagationsResultTypeDef](./type_defs.md#gettransitgatewayattachmentpropagationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTransitGatewayAttachmentPropagationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayAttachmentId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetTransitGatewayAttachmentPropagationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetTransitGatewayAttachmentPropagationsResultTypeDef](./type_defs.md#gettransitgatewayattachmentpropagationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayAttachmentPropagationsRequestGetTransitGatewayAttachmentPropagationsPaginateTypeDef = {  # (1)
    "TransitGatewayAttachmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayAttachmentPropagationsRequestGetTransitGatewayAttachmentPropagationsPaginateTypeDef](./type_defs.md#gettransitgatewayattachmentpropagationsrequestgettransitgatewayattachmentpropagationspaginatetypedef) 
## GetTransitGatewayMulticastDomainAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_multicast_domain_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetTransitGatewayMulticastDomainAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetTransitGatewayMulticastDomainAssociationsResultTypeDef](./type_defs.md#gettransitgatewaymulticastdomainassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTransitGatewayMulticastDomainAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayMulticastDomainId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetTransitGatewayMulticastDomainAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetTransitGatewayMulticastDomainAssociationsResultTypeDef](./type_defs.md#gettransitgatewaymulticastdomainassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayMulticastDomainAssociationsRequestGetTransitGatewayMulticastDomainAssociationsPaginateTypeDef = {  # (1)
    "TransitGatewayMulticastDomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayMulticastDomainAssociationsRequestGetTransitGatewayMulticastDomainAssociationsPaginateTypeDef](./type_defs.md#gettransitgatewaymulticastdomainassociationsrequestgettransitgatewaymulticastdomainassociationspaginatetypedef) 
## GetTransitGatewayPolicyTableAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_policy_table_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetTransitGatewayPolicyTableAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetTransitGatewayPolicyTableAssociationsResultTypeDef](./type_defs.md#gettransitgatewaypolicytableassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTransitGatewayPolicyTableAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayPolicyTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetTransitGatewayPolicyTableAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetTransitGatewayPolicyTableAssociationsResultTypeDef](./type_defs.md#gettransitgatewaypolicytableassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayPolicyTableAssociationsRequestGetTransitGatewayPolicyTableAssociationsPaginateTypeDef = {  # (1)
    "TransitGatewayPolicyTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayPolicyTableAssociationsRequestGetTransitGatewayPolicyTableAssociationsPaginateTypeDef](./type_defs.md#gettransitgatewaypolicytableassociationsrequestgettransitgatewaypolicytableassociationspaginatetypedef) 
## GetTransitGatewayPrefixListReferencesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_prefix_list_references")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetTransitGatewayPrefixListReferences)

```python title="Usage example"
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
3. item: [:material-code-braces: GetTransitGatewayPrefixListReferencesResultTypeDef](./type_defs.md#gettransitgatewayprefixlistreferencesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTransitGatewayPrefixListReferencesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetTransitGatewayPrefixListReferencesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetTransitGatewayPrefixListReferencesResultTypeDef](./type_defs.md#gettransitgatewayprefixlistreferencesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayPrefixListReferencesRequestGetTransitGatewayPrefixListReferencesPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayPrefixListReferencesRequestGetTransitGatewayPrefixListReferencesPaginateTypeDef](./type_defs.md#gettransitgatewayprefixlistreferencesrequestgettransitgatewayprefixlistreferencespaginatetypedef) 
## GetTransitGatewayRouteTableAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_route_table_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetTransitGatewayRouteTableAssociations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetTransitGatewayRouteTableAssociationsResultTypeDef](./type_defs.md#gettransitgatewayroutetableassociationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTransitGatewayRouteTableAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetTransitGatewayRouteTableAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetTransitGatewayRouteTableAssociationsResultTypeDef](./type_defs.md#gettransitgatewayroutetableassociationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayRouteTableAssociationsRequestGetTransitGatewayRouteTableAssociationsPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayRouteTableAssociationsRequestGetTransitGatewayRouteTableAssociationsPaginateTypeDef](./type_defs.md#gettransitgatewayroutetableassociationsrequestgettransitgatewayroutetableassociationspaginatetypedef) 
## GetTransitGatewayRouteTablePropagationsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_transit_gateway_route_table_propagations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetTransitGatewayRouteTablePropagations)

```python title="Usage example"
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
3. item: [:material-code-braces: GetTransitGatewayRouteTablePropagationsResultTypeDef](./type_defs.md#gettransitgatewayroutetablepropagationsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetTransitGatewayRouteTablePropagationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[GetTransitGatewayRouteTablePropagationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetTransitGatewayRouteTablePropagationsResultTypeDef](./type_defs.md#gettransitgatewayroutetablepropagationsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetTransitGatewayRouteTablePropagationsRequestGetTransitGatewayRouteTablePropagationsPaginateTypeDef = {  # (1)
    "TransitGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetTransitGatewayRouteTablePropagationsRequestGetTransitGatewayRouteTablePropagationsPaginateTypeDef](./type_defs.md#gettransitgatewayroutetablepropagationsrequestgettransitgatewayroutetablepropagationspaginatetypedef) 
## GetVpnConnectionDeviceTypesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("get_vpn_connection_device_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.GetVpnConnectionDeviceTypes)

```python title="Usage example"
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
3. item: [:material-code-braces: GetVpnConnectionDeviceTypesResultTypeDef](./type_defs.md#getvpnconnectiondevicetypesresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetVpnConnectionDeviceTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetVpnConnectionDeviceTypesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetVpnConnectionDeviceTypesResultTypeDef](./type_defs.md#getvpnconnectiondevicetypesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetVpnConnectionDeviceTypesRequestGetVpnConnectionDeviceTypesPaginateTypeDef = {  # (1)
    "DryRun": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetVpnConnectionDeviceTypesRequestGetVpnConnectionDeviceTypesPaginateTypeDef](./type_defs.md#getvpnconnectiondevicetypesrequestgetvpnconnectiondevicetypespaginatetypedef) 
## ListImagesInRecycleBinPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("list_images_in_recycle_bin")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.ListImagesInRecycleBin)

```python title="Usage example"
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
3. item: [:material-code-braces: ListImagesInRecycleBinResultTypeDef](./type_defs.md#listimagesinrecyclebinresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListImagesInRecycleBinPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ImageIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListImagesInRecycleBinResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListImagesInRecycleBinResultTypeDef](./type_defs.md#listimagesinrecyclebinresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListImagesInRecycleBinRequestListImagesInRecycleBinPaginateTypeDef = {  # (1)
    "ImageIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImagesInRecycleBinRequestListImagesInRecycleBinPaginateTypeDef](./type_defs.md#listimagesinrecyclebinrequestlistimagesinrecyclebinpaginatetypedef) 
## ListSnapshotsInRecycleBinPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("list_snapshots_in_recycle_bin")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.ListSnapshotsInRecycleBin)

```python title="Usage example"
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
3. item: [:material-code-braces: ListSnapshotsInRecycleBinResultTypeDef](./type_defs.md#listsnapshotsinrecyclebinresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListSnapshotsInRecycleBinPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SnapshotIds: Sequence[str] = ...,
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSnapshotsInRecycleBinResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSnapshotsInRecycleBinResultTypeDef](./type_defs.md#listsnapshotsinrecyclebinresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListSnapshotsInRecycleBinRequestListSnapshotsInRecycleBinPaginateTypeDef = {  # (1)
    "SnapshotIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSnapshotsInRecycleBinRequestListSnapshotsInRecycleBinPaginateTypeDef](./type_defs.md#listsnapshotsinrecyclebinrequestlistsnapshotsinrecyclebinpaginatetypedef) 
## SearchLocalGatewayRoutesPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("search_local_gateway_routes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.SearchLocalGatewayRoutes)

```python title="Usage example"
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
3. item: [:material-code-braces: SearchLocalGatewayRoutesResultTypeDef](./type_defs.md#searchlocalgatewayroutesresulttypedef) 


### paginate

Type annotations and code completion for `#!python SearchLocalGatewayRoutesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    LocalGatewayRouteTableId: str,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchLocalGatewayRoutesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchLocalGatewayRoutesResultTypeDef](./type_defs.md#searchlocalgatewayroutesresulttypedef) 


```python title="Usage example with kwargs"
kwargs: SearchLocalGatewayRoutesRequestSearchLocalGatewayRoutesPaginateTypeDef = {  # (1)
    "LocalGatewayRouteTableId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchLocalGatewayRoutesRequestSearchLocalGatewayRoutesPaginateTypeDef](./type_defs.md#searchlocalgatewayroutesrequestsearchlocalgatewayroutespaginatetypedef) 
## SearchTransitGatewayMulticastGroupsPaginator

Type annotations and code completion for `#!python session.create_client("ec2").get_paginator("search_transit_gateway_multicast_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.SearchTransitGatewayMulticastGroups)

```python title="Usage example"
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
3. item: [:material-code-braces: SearchTransitGatewayMulticastGroupsResultTypeDef](./type_defs.md#searchtransitgatewaymulticastgroupsresulttypedef) 


### paginate

Type annotations and code completion for `#!python SearchTransitGatewayMulticastGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    TransitGatewayMulticastDomainId: str = ...,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    DryRun: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[SearchTransitGatewayMulticastGroupsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchTransitGatewayMulticastGroupsResultTypeDef](./type_defs.md#searchtransitgatewaymulticastgroupsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: SearchTransitGatewayMulticastGroupsRequestSearchTransitGatewayMulticastGroupsPaginateTypeDef = {  # (1)
    "TransitGatewayMulticastDomainId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchTransitGatewayMulticastGroupsRequestSearchTransitGatewayMulticastGroupsPaginateTypeDef](./type_defs.md#searchtransitgatewaymulticastgroupsrequestsearchtransitgatewaymulticastgroupspaginatetypedef) 
