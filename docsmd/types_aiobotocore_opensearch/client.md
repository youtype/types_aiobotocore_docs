# OpenSearchServiceClient

> [Index](../README.md) > [OpenSearchService](./README.md) > OpenSearchServiceClient

!!! note ""

    Auto-generated documentation for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
    type annotations stubs module [types-aiobotocore-opensearch](https://pypi.org/project/types-aiobotocore-opensearch/).

## OpenSearchServiceClient

Type annotations and code completion for `#!python session.create_client("opensearch")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client)

```python
# OpenSearchServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_opensearch.client import OpenSearchServiceClient

session = get_session()
async with session.create_client("opensearch") as client:
    client: OpenSearchServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("opensearch").exceptions` structure.

```python
# OpenSearchServiceClient.exceptions usage example

async with session.create_client("opensearch") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BaseException,
        client.ClientError,
        client.ConflictException,
        client.DependencyFailureException,
        client.DisabledOperationException,
        client.InternalException,
        client.InvalidPaginationTokenException,
        client.InvalidTypeException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.SlotNotAvailableException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# OpenSearchServiceClient usage type checking example

from types_aiobotocore_opensearch.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### accept\_inbound\_connection

Allows the destination Amazon OpenSearch Service domain owner to accept an
inbound cross-cluster search connection
request.

Type annotations and code completion for `#!python session.create_client("opensearch").accept_inbound_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.accept_inbound_connection)

```python
# accept_inbound_connection method definition

await def accept_inbound_connection(
    self,
    *,
    ConnectionId: str,
) -> AcceptInboundConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AcceptInboundConnectionResponseTypeDef](./type_defs.md#acceptinboundconnectionresponsetypedef) 


```python
# accept_inbound_connection method usage example with argument unpacking

kwargs: AcceptInboundConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.accept_inbound_connection(**kwargs)
```

1. See [:material-code-braces: AcceptInboundConnectionRequestRequestTypeDef](./type_defs.md#acceptinboundconnectionrequestrequesttypedef) 

### add\_data\_source

Creates a new direct-query data source to the specified domain.

Type annotations and code completion for `#!python session.create_client("opensearch").add_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.add_data_source)

```python
# add_data_source method definition

await def add_data_source(
    self,
    *,
    DomainName: str,
    Name: str,
    DataSourceType: DataSourceTypeTypeDef,  # (1)
    Description: str = ...,
) -> AddDataSourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DataSourceTypeTypeDef](./type_defs.md#datasourcetypetypedef) 
2. See [:material-code-braces: AddDataSourceResponseTypeDef](./type_defs.md#adddatasourceresponsetypedef) 


```python
# add_data_source method usage example with argument unpacking

kwargs: AddDataSourceRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Name": ...,
    "DataSourceType": ...,
}

parent.add_data_source(**kwargs)
```

1. See [:material-code-braces: AddDataSourceRequestRequestTypeDef](./type_defs.md#adddatasourcerequestrequesttypedef) 

### add\_tags

Attaches tags to an existing Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").add_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.add_tags)

```python
# add_tags method definition

await def add_tags(
    self,
    *,
    ARN: str,
    TagList: Sequence[TagTypeDef],  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# add_tags method usage example with argument unpacking

kwargs: AddTagsRequestRequestTypeDef = {  # (1)
    "ARN": ...,
    "TagList": ...,
}

parent.add_tags(**kwargs)
```

1. See [:material-code-braces: AddTagsRequestRequestTypeDef](./type_defs.md#addtagsrequestrequesttypedef) 

### associate\_package

Associates a package with an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").associate_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.associate_package)

```python
# associate_package method definition

await def associate_package(
    self,
    *,
    PackageID: str,
    DomainName: str,
) -> AssociatePackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociatePackageResponseTypeDef](./type_defs.md#associatepackageresponsetypedef) 


```python
# associate_package method usage example with argument unpacking

kwargs: AssociatePackageRequestRequestTypeDef = {  # (1)
    "PackageID": ...,
    "DomainName": ...,
}

parent.associate_package(**kwargs)
```

1. See [:material-code-braces: AssociatePackageRequestRequestTypeDef](./type_defs.md#associatepackagerequestrequesttypedef) 

### authorize\_vpc\_endpoint\_access

Provides access to an Amazon OpenSearch Service domain through the use of an
interface VPC
endpoint.

Type annotations and code completion for `#!python session.create_client("opensearch").authorize_vpc_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.authorize_vpc_endpoint_access)

```python
# authorize_vpc_endpoint_access method definition

await def authorize_vpc_endpoint_access(
    self,
    *,
    DomainName: str,
    Account: str,
) -> AuthorizeVpcEndpointAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AuthorizeVpcEndpointAccessResponseTypeDef](./type_defs.md#authorizevpcendpointaccessresponsetypedef) 


```python
# authorize_vpc_endpoint_access method usage example with argument unpacking

kwargs: AuthorizeVpcEndpointAccessRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Account": ...,
}

parent.authorize_vpc_endpoint_access(**kwargs)
```

1. See [:material-code-braces: AuthorizeVpcEndpointAccessRequestRequestTypeDef](./type_defs.md#authorizevpcendpointaccessrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("opensearch").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_domain\_config\_change

Cancels a pending configuration change on an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").cancel_domain_config_change` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.cancel_domain_config_change)

```python
# cancel_domain_config_change method definition

await def cancel_domain_config_change(
    self,
    *,
    DomainName: str,
    DryRun: bool = ...,
) -> CancelDomainConfigChangeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelDomainConfigChangeResponseTypeDef](./type_defs.md#canceldomainconfigchangeresponsetypedef) 


```python
# cancel_domain_config_change method usage example with argument unpacking

kwargs: CancelDomainConfigChangeRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.cancel_domain_config_change(**kwargs)
```

1. See [:material-code-braces: CancelDomainConfigChangeRequestRequestTypeDef](./type_defs.md#canceldomainconfigchangerequestrequesttypedef) 

### cancel\_service\_software\_update

Cancels a scheduled service software update for an Amazon OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").cancel_service_software_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.cancel_service_software_update)

```python
# cancel_service_software_update method definition

await def cancel_service_software_update(
    self,
    *,
    DomainName: str,
) -> CancelServiceSoftwareUpdateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelServiceSoftwareUpdateResponseTypeDef](./type_defs.md#cancelservicesoftwareupdateresponsetypedef) 


```python
# cancel_service_software_update method usage example with argument unpacking

kwargs: CancelServiceSoftwareUpdateRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.cancel_service_software_update(**kwargs)
```

1. See [:material-code-braces: CancelServiceSoftwareUpdateRequestRequestTypeDef](./type_defs.md#cancelservicesoftwareupdaterequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("opensearch").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_domain

Creates an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").create_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_domain)

```python
# create_domain method definition

await def create_domain(
    self,
    *,
    DomainName: str,
    EngineVersion: str = ...,
    ClusterConfig: ClusterConfigTypeDef = ...,  # (1)
    EBSOptions: EBSOptionsTypeDef = ...,  # (2)
    AccessPolicies: str = ...,
    IPAddressType: IPAddressTypeType = ...,  # (3)
    SnapshotOptions: SnapshotOptionsTypeDef = ...,  # (4)
    VPCOptions: VPCOptionsTypeDef = ...,  # (5)
    CognitoOptions: CognitoOptionsTypeDef = ...,  # (6)
    EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,  # (7)
    NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,  # (8)
    AdvancedOptions: Mapping[str, str] = ...,
    LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,  # (9)
    DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,  # (10)
    AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,  # (11)
    TagList: Sequence[TagTypeDef] = ...,  # (12)
    AutoTuneOptions: AutoTuneOptionsInputTypeDef = ...,  # (13)
    OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,  # (14)
    SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,  # (15)
    AIMLOptions: AIMLOptionsInputTypeDef = ...,  # (16)
) -> CreateDomainResponseTypeDef:  # (17)
    ...
```

1. See [:material-code-braces: ClusterConfigTypeDef](./type_defs.md#clusterconfigtypedef) 
2. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
3. See [:material-code-brackets: IPAddressTypeType](./literals.md#ipaddresstypetype) 
4. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
5. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
6. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
7. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
8. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
9. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
10. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
11. See [:material-code-braces: AdvancedSecurityOptionsInputTypeDef](./type_defs.md#advancedsecurityoptionsinputtypedef) 
12. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
13. See [:material-code-braces: AutoTuneOptionsInputTypeDef](./type_defs.md#autotuneoptionsinputtypedef) 
14. See [:material-code-braces: OffPeakWindowOptionsTypeDef](./type_defs.md#offpeakwindowoptionstypedef) 
15. See [:material-code-braces: SoftwareUpdateOptionsTypeDef](./type_defs.md#softwareupdateoptionstypedef) 
16. See [:material-code-braces: AIMLOptionsInputTypeDef](./type_defs.md#aimloptionsinputtypedef) 
17. See [:material-code-braces: CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef) 


```python
# create_domain method usage example with argument unpacking

kwargs: CreateDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.create_domain(**kwargs)
```

1. See [:material-code-braces: CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef) 

### create\_outbound\_connection

Creates a new cross-cluster search connection from a source Amazon OpenSearch
Service domain to a destination
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").create_outbound_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_outbound_connection)

```python
# create_outbound_connection method definition

await def create_outbound_connection(
    self,
    *,
    LocalDomainInfo: DomainInformationContainerTypeDef,  # (1)
    RemoteDomainInfo: DomainInformationContainerTypeDef,  # (1)
    ConnectionAlias: str,
    ConnectionMode: ConnectionModeType = ...,  # (3)
    ConnectionProperties: ConnectionPropertiesTypeDef = ...,  # (4)
) -> CreateOutboundConnectionResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
2. See [:material-code-braces: DomainInformationContainerTypeDef](./type_defs.md#domaininformationcontainertypedef) 
3. See [:material-code-brackets: ConnectionModeType](./literals.md#connectionmodetype) 
4. See [:material-code-braces: ConnectionPropertiesTypeDef](./type_defs.md#connectionpropertiestypedef) 
5. See [:material-code-braces: CreateOutboundConnectionResponseTypeDef](./type_defs.md#createoutboundconnectionresponsetypedef) 


```python
# create_outbound_connection method usage example with argument unpacking

kwargs: CreateOutboundConnectionRequestRequestTypeDef = {  # (1)
    "LocalDomainInfo": ...,
    "RemoteDomainInfo": ...,
    "ConnectionAlias": ...,
}

parent.create_outbound_connection(**kwargs)
```

1. See [:material-code-braces: CreateOutboundConnectionRequestRequestTypeDef](./type_defs.md#createoutboundconnectionrequestrequesttypedef) 

### create\_package

Creates a package for use with Amazon OpenSearch Service domains.

Type annotations and code completion for `#!python session.create_client("opensearch").create_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_package)

```python
# create_package method definition

await def create_package(
    self,
    *,
    PackageName: str,
    PackageType: PackageTypeType,  # (1)
    PackageSource: PackageSourceTypeDef,  # (2)
    PackageDescription: str = ...,
) -> CreatePackageResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: PackageTypeType](./literals.md#packagetypetype) 
2. See [:material-code-braces: PackageSourceTypeDef](./type_defs.md#packagesourcetypedef) 
3. See [:material-code-braces: CreatePackageResponseTypeDef](./type_defs.md#createpackageresponsetypedef) 


```python
# create_package method usage example with argument unpacking

kwargs: CreatePackageRequestRequestTypeDef = {  # (1)
    "PackageName": ...,
    "PackageType": ...,
    "PackageSource": ...,
}

parent.create_package(**kwargs)
```

1. See [:material-code-braces: CreatePackageRequestRequestTypeDef](./type_defs.md#createpackagerequestrequesttypedef) 

### create\_vpc\_endpoint

Creates an Amazon OpenSearch Service-managed VPC endpoint.

Type annotations and code completion for `#!python session.create_client("opensearch").create_vpc_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.create_vpc_endpoint)

```python
# create_vpc_endpoint method definition

await def create_vpc_endpoint(
    self,
    *,
    DomainArn: str,
    VpcOptions: VPCOptionsTypeDef,  # (1)
    ClientToken: str = ...,
) -> CreateVpcEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
2. See [:material-code-braces: CreateVpcEndpointResponseTypeDef](./type_defs.md#createvpcendpointresponsetypedef) 


```python
# create_vpc_endpoint method usage example with argument unpacking

kwargs: CreateVpcEndpointRequestRequestTypeDef = {  # (1)
    "DomainArn": ...,
    "VpcOptions": ...,
}

parent.create_vpc_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateVpcEndpointRequestRequestTypeDef](./type_defs.md#createvpcendpointrequestrequesttypedef) 

### delete\_data\_source

Deletes a direct-query data source.

Type annotations and code completion for `#!python session.create_client("opensearch").delete_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.delete_data_source)

```python
# delete_data_source method definition

await def delete_data_source(
    self,
    *,
    DomainName: str,
    Name: str,
) -> DeleteDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDataSourceResponseTypeDef](./type_defs.md#deletedatasourceresponsetypedef) 


```python
# delete_data_source method usage example with argument unpacking

kwargs: DeleteDataSourceRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Name": ...,
}

parent.delete_data_source(**kwargs)
```

1. See [:material-code-braces: DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef) 

### delete\_domain

Deletes an Amazon OpenSearch Service domain and all of its data.

Type annotations and code completion for `#!python session.create_client("opensearch").delete_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.delete_domain)

```python
# delete_domain method definition

await def delete_domain(
    self,
    *,
    DomainName: str,
) -> DeleteDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteDomainResponseTypeDef](./type_defs.md#deletedomainresponsetypedef) 


```python
# delete_domain method usage example with argument unpacking

kwargs: DeleteDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.delete_domain(**kwargs)
```

1. See [:material-code-braces: DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef) 

### delete\_inbound\_connection

Allows the destination Amazon OpenSearch Service domain owner to delete an
existing inbound cross-cluster search
connection.

Type annotations and code completion for `#!python session.create_client("opensearch").delete_inbound_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.delete_inbound_connection)

```python
# delete_inbound_connection method definition

await def delete_inbound_connection(
    self,
    *,
    ConnectionId: str,
) -> DeleteInboundConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteInboundConnectionResponseTypeDef](./type_defs.md#deleteinboundconnectionresponsetypedef) 


```python
# delete_inbound_connection method usage example with argument unpacking

kwargs: DeleteInboundConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.delete_inbound_connection(**kwargs)
```

1. See [:material-code-braces: DeleteInboundConnectionRequestRequestTypeDef](./type_defs.md#deleteinboundconnectionrequestrequesttypedef) 

### delete\_outbound\_connection

Allows the source Amazon OpenSearch Service domain owner to delete an existing
outbound cross-cluster search
connection.

Type annotations and code completion for `#!python session.create_client("opensearch").delete_outbound_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.delete_outbound_connection)

```python
# delete_outbound_connection method definition

await def delete_outbound_connection(
    self,
    *,
    ConnectionId: str,
) -> DeleteOutboundConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteOutboundConnectionResponseTypeDef](./type_defs.md#deleteoutboundconnectionresponsetypedef) 


```python
# delete_outbound_connection method usage example with argument unpacking

kwargs: DeleteOutboundConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.delete_outbound_connection(**kwargs)
```

1. See [:material-code-braces: DeleteOutboundConnectionRequestRequestTypeDef](./type_defs.md#deleteoutboundconnectionrequestrequesttypedef) 

### delete\_package

Deletes an Amazon OpenSearch Service package.

Type annotations and code completion for `#!python session.create_client("opensearch").delete_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.delete_package)

```python
# delete_package method definition

await def delete_package(
    self,
    *,
    PackageID: str,
) -> DeletePackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeletePackageResponseTypeDef](./type_defs.md#deletepackageresponsetypedef) 


```python
# delete_package method usage example with argument unpacking

kwargs: DeletePackageRequestRequestTypeDef = {  # (1)
    "PackageID": ...,
}

parent.delete_package(**kwargs)
```

1. See [:material-code-braces: DeletePackageRequestRequestTypeDef](./type_defs.md#deletepackagerequestrequesttypedef) 

### delete\_vpc\_endpoint

Deletes an Amazon OpenSearch Service-managed interface VPC endpoint.

Type annotations and code completion for `#!python session.create_client("opensearch").delete_vpc_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.delete_vpc_endpoint)

```python
# delete_vpc_endpoint method definition

await def delete_vpc_endpoint(
    self,
    *,
    VpcEndpointId: str,
) -> DeleteVpcEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteVpcEndpointResponseTypeDef](./type_defs.md#deletevpcendpointresponsetypedef) 


```python
# delete_vpc_endpoint method usage example with argument unpacking

kwargs: DeleteVpcEndpointRequestRequestTypeDef = {  # (1)
    "VpcEndpointId": ...,
}

parent.delete_vpc_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteVpcEndpointRequestRequestTypeDef](./type_defs.md#deletevpcendpointrequestrequesttypedef) 

### describe\_domain

Describes the domain configuration for the specified Amazon OpenSearch Service
domain, including the domain ID, domain service endpoint, and domain
ARN.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain)

```python
# describe_domain method definition

await def describe_domain(
    self,
    *,
    DomainName: str,
) -> DescribeDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainResponseTypeDef](./type_defs.md#describedomainresponsetypedef) 


```python
# describe_domain method usage example with argument unpacking

kwargs: DescribeDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_domain(**kwargs)
```

1. See [:material-code-braces: DescribeDomainRequestRequestTypeDef](./type_defs.md#describedomainrequestrequesttypedef) 

### describe\_domain\_auto\_tunes

Returns the list of optimizations that Auto-Tune has made to an Amazon
OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_domain_auto_tunes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_auto_tunes)

```python
# describe_domain_auto_tunes method definition

await def describe_domain_auto_tunes(
    self,
    *,
    DomainName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeDomainAutoTunesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainAutoTunesResponseTypeDef](./type_defs.md#describedomainautotunesresponsetypedef) 


```python
# describe_domain_auto_tunes method usage example with argument unpacking

kwargs: DescribeDomainAutoTunesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_domain_auto_tunes(**kwargs)
```

1. See [:material-code-braces: DescribeDomainAutoTunesRequestRequestTypeDef](./type_defs.md#describedomainautotunesrequestrequesttypedef) 

### describe\_domain\_change\_progress

Returns information about the current blue/green deployment happening on an
Amazon OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_domain_change_progress` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_change_progress)

```python
# describe_domain_change_progress method definition

await def describe_domain_change_progress(
    self,
    *,
    DomainName: str,
    ChangeId: str = ...,
) -> DescribeDomainChangeProgressResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainChangeProgressResponseTypeDef](./type_defs.md#describedomainchangeprogressresponsetypedef) 


```python
# describe_domain_change_progress method usage example with argument unpacking

kwargs: DescribeDomainChangeProgressRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_domain_change_progress(**kwargs)
```

1. See [:material-code-braces: DescribeDomainChangeProgressRequestRequestTypeDef](./type_defs.md#describedomainchangeprogressrequestrequesttypedef) 

### describe\_domain\_config

Returns the configuration of an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_domain_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_config)

```python
# describe_domain_config method definition

await def describe_domain_config(
    self,
    *,
    DomainName: str,
) -> DescribeDomainConfigResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainConfigResponseTypeDef](./type_defs.md#describedomainconfigresponsetypedef) 


```python
# describe_domain_config method usage example with argument unpacking

kwargs: DescribeDomainConfigRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_domain_config(**kwargs)
```

1. See [:material-code-braces: DescribeDomainConfigRequestRequestTypeDef](./type_defs.md#describedomainconfigrequestrequesttypedef) 

### describe\_domain\_health

Returns information about domain and node health, the standby Availability
Zone, number of nodes per Availability Zone, and shard count per
node.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_domain_health` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_health)

```python
# describe_domain_health method definition

await def describe_domain_health(
    self,
    *,
    DomainName: str,
) -> DescribeDomainHealthResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainHealthResponseTypeDef](./type_defs.md#describedomainhealthresponsetypedef) 


```python
# describe_domain_health method usage example with argument unpacking

kwargs: DescribeDomainHealthRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_domain_health(**kwargs)
```

1. See [:material-code-braces: DescribeDomainHealthRequestRequestTypeDef](./type_defs.md#describedomainhealthrequestrequesttypedef) 

### describe\_domain\_nodes

Returns information about domain and nodes, including data nodes, master nodes,
ultrawarm nodes, Availability Zone(s), standby nodes, node configurations, and
node
states.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_domain_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domain_nodes)

```python
# describe_domain_nodes method definition

await def describe_domain_nodes(
    self,
    *,
    DomainName: str,
) -> DescribeDomainNodesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainNodesResponseTypeDef](./type_defs.md#describedomainnodesresponsetypedef) 


```python
# describe_domain_nodes method usage example with argument unpacking

kwargs: DescribeDomainNodesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_domain_nodes(**kwargs)
```

1. See [:material-code-braces: DescribeDomainNodesRequestRequestTypeDef](./type_defs.md#describedomainnodesrequestrequesttypedef) 

### describe\_domains

Returns domain configuration information about the specified Amazon OpenSearch
Service
domains.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_domains)

```python
# describe_domains method definition

await def describe_domains(
    self,
    *,
    DomainNames: Sequence[str],
) -> DescribeDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDomainsResponseTypeDef](./type_defs.md#describedomainsresponsetypedef) 


```python
# describe_domains method usage example with argument unpacking

kwargs: DescribeDomainsRequestRequestTypeDef = {  # (1)
    "DomainNames": ...,
}

parent.describe_domains(**kwargs)
```

1. See [:material-code-braces: DescribeDomainsRequestRequestTypeDef](./type_defs.md#describedomainsrequestrequesttypedef) 

### describe\_dry\_run\_progress

Describes the progress of a pre-update dry run analysis on an Amazon OpenSearch
Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_dry_run_progress` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_dry_run_progress)

```python
# describe_dry_run_progress method definition

await def describe_dry_run_progress(
    self,
    *,
    DomainName: str,
    DryRunId: str = ...,
    LoadDryRunConfig: bool = ...,
) -> DescribeDryRunProgressResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDryRunProgressResponseTypeDef](./type_defs.md#describedryrunprogressresponsetypedef) 


```python
# describe_dry_run_progress method usage example with argument unpacking

kwargs: DescribeDryRunProgressRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.describe_dry_run_progress(**kwargs)
```

1. See [:material-code-braces: DescribeDryRunProgressRequestRequestTypeDef](./type_defs.md#describedryrunprogressrequestrequesttypedef) 

### describe\_inbound\_connections

Lists all the inbound cross-cluster search connections for a destination
(remote) Amazon OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_inbound_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_inbound_connections)

```python
# describe_inbound_connections method definition

await def describe_inbound_connections(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeInboundConnectionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeInboundConnectionsResponseTypeDef](./type_defs.md#describeinboundconnectionsresponsetypedef) 


```python
# describe_inbound_connections method usage example with argument unpacking

kwargs: DescribeInboundConnectionsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_inbound_connections(**kwargs)
```

1. See [:material-code-braces: DescribeInboundConnectionsRequestRequestTypeDef](./type_defs.md#describeinboundconnectionsrequestrequesttypedef) 

### describe\_instance\_type\_limits

Describes the instance count, storage, and master node limits for a given
OpenSearch or Elasticsearch version and instance
type.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_instance_type_limits` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_instance_type_limits)

```python
# describe_instance_type_limits method definition

await def describe_instance_type_limits(
    self,
    *,
    InstanceType: OpenSearchPartitionInstanceTypeType,  # (1)
    EngineVersion: str,
    DomainName: str = ...,
) -> DescribeInstanceTypeLimitsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OpenSearchPartitionInstanceTypeType](./literals.md#opensearchpartitioninstancetypetype) 
2. See [:material-code-braces: DescribeInstanceTypeLimitsResponseTypeDef](./type_defs.md#describeinstancetypelimitsresponsetypedef) 


```python
# describe_instance_type_limits method usage example with argument unpacking

kwargs: DescribeInstanceTypeLimitsRequestRequestTypeDef = {  # (1)
    "InstanceType": ...,
    "EngineVersion": ...,
}

parent.describe_instance_type_limits(**kwargs)
```

1. See [:material-code-braces: DescribeInstanceTypeLimitsRequestRequestTypeDef](./type_defs.md#describeinstancetypelimitsrequestrequesttypedef) 

### describe\_outbound\_connections

Lists all the outbound cross-cluster connections for a local (source) Amazon
OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_outbound_connections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_outbound_connections)

```python
# describe_outbound_connections method definition

await def describe_outbound_connections(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeOutboundConnectionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: DescribeOutboundConnectionsResponseTypeDef](./type_defs.md#describeoutboundconnectionsresponsetypedef) 


```python
# describe_outbound_connections method usage example with argument unpacking

kwargs: DescribeOutboundConnectionsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_outbound_connections(**kwargs)
```

1. See [:material-code-braces: DescribeOutboundConnectionsRequestRequestTypeDef](./type_defs.md#describeoutboundconnectionsrequestrequesttypedef) 

### describe\_packages

Describes all packages available to OpenSearch Service.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_packages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_packages)

```python
# describe_packages method definition

await def describe_packages(
    self,
    *,
    Filters: Sequence[DescribePackagesFilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribePackagesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DescribePackagesFilterTypeDef](./type_defs.md#describepackagesfiltertypedef) 
2. See [:material-code-braces: DescribePackagesResponseTypeDef](./type_defs.md#describepackagesresponsetypedef) 


```python
# describe_packages method usage example with argument unpacking

kwargs: DescribePackagesRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.describe_packages(**kwargs)
```

1. See [:material-code-braces: DescribePackagesRequestRequestTypeDef](./type_defs.md#describepackagesrequestrequesttypedef) 

### describe\_reserved\_instance\_offerings

Describes the available Amazon OpenSearch Service Reserved Instance offerings
for a given
Region.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_reserved_instance_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_reserved_instance_offerings)

```python
# describe_reserved_instance_offerings method definition

await def describe_reserved_instance_offerings(
    self,
    *,
    ReservedInstanceOfferingId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeReservedInstanceOfferingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReservedInstanceOfferingsResponseTypeDef](./type_defs.md#describereservedinstanceofferingsresponsetypedef) 


```python
# describe_reserved_instance_offerings method usage example with argument unpacking

kwargs: DescribeReservedInstanceOfferingsRequestRequestTypeDef = {  # (1)
    "ReservedInstanceOfferingId": ...,
}

parent.describe_reserved_instance_offerings(**kwargs)
```

1. See [:material-code-braces: DescribeReservedInstanceOfferingsRequestRequestTypeDef](./type_defs.md#describereservedinstanceofferingsrequestrequesttypedef) 

### describe\_reserved\_instances

Describes the Amazon OpenSearch Service instances that you have reserved in a
given
Region.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_reserved_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_reserved_instances)

```python
# describe_reserved_instances method definition

await def describe_reserved_instances(
    self,
    *,
    ReservedInstanceId: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeReservedInstancesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReservedInstancesResponseTypeDef](./type_defs.md#describereservedinstancesresponsetypedef) 


```python
# describe_reserved_instances method usage example with argument unpacking

kwargs: DescribeReservedInstancesRequestRequestTypeDef = {  # (1)
    "ReservedInstanceId": ...,
}

parent.describe_reserved_instances(**kwargs)
```

1. See [:material-code-braces: DescribeReservedInstancesRequestRequestTypeDef](./type_defs.md#describereservedinstancesrequestrequesttypedef) 

### describe\_vpc\_endpoints

Describes one or more Amazon OpenSearch Service-managed VPC endpoints.

Type annotations and code completion for `#!python session.create_client("opensearch").describe_vpc_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.describe_vpc_endpoints)

```python
# describe_vpc_endpoints method definition

await def describe_vpc_endpoints(
    self,
    *,
    VpcEndpointIds: Sequence[str],
) -> DescribeVpcEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeVpcEndpointsResponseTypeDef](./type_defs.md#describevpcendpointsresponsetypedef) 


```python
# describe_vpc_endpoints method usage example with argument unpacking

kwargs: DescribeVpcEndpointsRequestRequestTypeDef = {  # (1)
    "VpcEndpointIds": ...,
}

parent.describe_vpc_endpoints(**kwargs)
```

1. See [:material-code-braces: DescribeVpcEndpointsRequestRequestTypeDef](./type_defs.md#describevpcendpointsrequestrequesttypedef) 

### dissociate\_package

Removes a package from the specified Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").dissociate_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.dissociate_package)

```python
# dissociate_package method definition

await def dissociate_package(
    self,
    *,
    PackageID: str,
    DomainName: str,
) -> DissociatePackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DissociatePackageResponseTypeDef](./type_defs.md#dissociatepackageresponsetypedef) 


```python
# dissociate_package method usage example with argument unpacking

kwargs: DissociatePackageRequestRequestTypeDef = {  # (1)
    "PackageID": ...,
    "DomainName": ...,
}

parent.dissociate_package(**kwargs)
```

1. See [:material-code-braces: DissociatePackageRequestRequestTypeDef](./type_defs.md#dissociatepackagerequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("opensearch").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.generate_presigned_url)

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


### get\_compatible\_versions

Returns a map of OpenSearch or Elasticsearch versions and the versions you can
upgrade them
to.

Type annotations and code completion for `#!python session.create_client("opensearch").get_compatible_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_compatible_versions)

```python
# get_compatible_versions method definition

await def get_compatible_versions(
    self,
    *,
    DomainName: str = ...,
) -> GetCompatibleVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCompatibleVersionsResponseTypeDef](./type_defs.md#getcompatibleversionsresponsetypedef) 


```python
# get_compatible_versions method usage example with argument unpacking

kwargs: GetCompatibleVersionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.get_compatible_versions(**kwargs)
```

1. See [:material-code-braces: GetCompatibleVersionsRequestRequestTypeDef](./type_defs.md#getcompatibleversionsrequestrequesttypedef) 

### get\_data\_source

Retrieves information about a direct query data source.

Type annotations and code completion for `#!python session.create_client("opensearch").get_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_data_source)

```python
# get_data_source method definition

await def get_data_source(
    self,
    *,
    DomainName: str,
    Name: str,
) -> GetDataSourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef) 


```python
# get_data_source method usage example with argument unpacking

kwargs: GetDataSourceRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Name": ...,
}

parent.get_data_source(**kwargs)
```

1. See [:material-code-braces: GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef) 

### get\_domain\_maintenance\_status

The status of the maintenance action.

Type annotations and code completion for `#!python session.create_client("opensearch").get_domain_maintenance_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_domain_maintenance_status)

```python
# get_domain_maintenance_status method definition

await def get_domain_maintenance_status(
    self,
    *,
    DomainName: str,
    MaintenanceId: str,
) -> GetDomainMaintenanceStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDomainMaintenanceStatusResponseTypeDef](./type_defs.md#getdomainmaintenancestatusresponsetypedef) 


```python
# get_domain_maintenance_status method usage example with argument unpacking

kwargs: GetDomainMaintenanceStatusRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "MaintenanceId": ...,
}

parent.get_domain_maintenance_status(**kwargs)
```

1. See [:material-code-braces: GetDomainMaintenanceStatusRequestRequestTypeDef](./type_defs.md#getdomainmaintenancestatusrequestrequesttypedef) 

### get\_package\_version\_history

Returns a list of Amazon OpenSearch Service package versions, along with their
creation time, commit message, and plugin properties (if the package is a zip
plugin
package).

Type annotations and code completion for `#!python session.create_client("opensearch").get_package_version_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_package_version_history)

```python
# get_package_version_history method definition

await def get_package_version_history(
    self,
    *,
    PackageID: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetPackageVersionHistoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetPackageVersionHistoryResponseTypeDef](./type_defs.md#getpackageversionhistoryresponsetypedef) 


```python
# get_package_version_history method usage example with argument unpacking

kwargs: GetPackageVersionHistoryRequestRequestTypeDef = {  # (1)
    "PackageID": ...,
}

parent.get_package_version_history(**kwargs)
```

1. See [:material-code-braces: GetPackageVersionHistoryRequestRequestTypeDef](./type_defs.md#getpackageversionhistoryrequestrequesttypedef) 

### get\_upgrade\_history

Retrieves the complete history of the last 10 upgrades performed on an Amazon
OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").get_upgrade_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_upgrade_history)

```python
# get_upgrade_history method definition

await def get_upgrade_history(
    self,
    *,
    DomainName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> GetUpgradeHistoryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUpgradeHistoryResponseTypeDef](./type_defs.md#getupgradehistoryresponsetypedef) 


```python
# get_upgrade_history method usage example with argument unpacking

kwargs: GetUpgradeHistoryRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.get_upgrade_history(**kwargs)
```

1. See [:material-code-braces: GetUpgradeHistoryRequestRequestTypeDef](./type_defs.md#getupgradehistoryrequestrequesttypedef) 

### get\_upgrade\_status

Returns the most recent status of the last upgrade or upgrade eligibility check
performed on an Amazon OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").get_upgrade_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.get_upgrade_status)

```python
# get_upgrade_status method definition

await def get_upgrade_status(
    self,
    *,
    DomainName: str,
) -> GetUpgradeStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetUpgradeStatusResponseTypeDef](./type_defs.md#getupgradestatusresponsetypedef) 


```python
# get_upgrade_status method usage example with argument unpacking

kwargs: GetUpgradeStatusRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.get_upgrade_status(**kwargs)
```

1. See [:material-code-braces: GetUpgradeStatusRequestRequestTypeDef](./type_defs.md#getupgradestatusrequestrequesttypedef) 

### list\_data\_sources

Lists direct-query data sources for a specific domain.

Type annotations and code completion for `#!python session.create_client("opensearch").list_data_sources` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_data_sources)

```python
# list_data_sources method definition

await def list_data_sources(
    self,
    *,
    DomainName: str,
) -> ListDataSourcesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef) 


```python
# list_data_sources method usage example with argument unpacking

kwargs: ListDataSourcesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_data_sources(**kwargs)
```

1. See [:material-code-braces: ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef) 

### list\_domain\_maintenances

A list of maintenance actions for the domain.

Type annotations and code completion for `#!python session.create_client("opensearch").list_domain_maintenances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_domain_maintenances)

```python
# list_domain_maintenances method definition

await def list_domain_maintenances(
    self,
    *,
    DomainName: str,
    Action: MaintenanceTypeType = ...,  # (1)
    Status: MaintenanceStatusType = ...,  # (2)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDomainMaintenancesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: MaintenanceTypeType](./literals.md#maintenancetypetype) 
2. See [:material-code-brackets: MaintenanceStatusType](./literals.md#maintenancestatustype) 
3. See [:material-code-braces: ListDomainMaintenancesResponseTypeDef](./type_defs.md#listdomainmaintenancesresponsetypedef) 


```python
# list_domain_maintenances method usage example with argument unpacking

kwargs: ListDomainMaintenancesRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_domain_maintenances(**kwargs)
```

1. See [:material-code-braces: ListDomainMaintenancesRequestRequestTypeDef](./type_defs.md#listdomainmaintenancesrequestrequesttypedef) 

### list\_domain\_names

Returns the names of all Amazon OpenSearch Service domains owned by the current
user in the active
Region.

Type annotations and code completion for `#!python session.create_client("opensearch").list_domain_names` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_domain_names)

```python
# list_domain_names method definition

await def list_domain_names(
    self,
    *,
    EngineType: EngineTypeType = ...,  # (1)
) -> ListDomainNamesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EngineTypeType](./literals.md#enginetypetype) 
2. See [:material-code-braces: ListDomainNamesResponseTypeDef](./type_defs.md#listdomainnamesresponsetypedef) 


```python
# list_domain_names method usage example with argument unpacking

kwargs: ListDomainNamesRequestRequestTypeDef = {  # (1)
    "EngineType": ...,
}

parent.list_domain_names(**kwargs)
```

1. See [:material-code-braces: ListDomainNamesRequestRequestTypeDef](./type_defs.md#listdomainnamesrequestrequesttypedef) 

### list\_domains\_for\_package

Lists all Amazon OpenSearch Service domains associated with a given package.

Type annotations and code completion for `#!python session.create_client("opensearch").list_domains_for_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_domains_for_package)

```python
# list_domains_for_package method definition

await def list_domains_for_package(
    self,
    *,
    PackageID: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDomainsForPackageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainsForPackageResponseTypeDef](./type_defs.md#listdomainsforpackageresponsetypedef) 


```python
# list_domains_for_package method usage example with argument unpacking

kwargs: ListDomainsForPackageRequestRequestTypeDef = {  # (1)
    "PackageID": ...,
}

parent.list_domains_for_package(**kwargs)
```

1. See [:material-code-braces: ListDomainsForPackageRequestRequestTypeDef](./type_defs.md#listdomainsforpackagerequestrequesttypedef) 

### list\_instance\_type\_details

Lists all instance types and available features for a given OpenSearch or
Elasticsearch
version.

Type annotations and code completion for `#!python session.create_client("opensearch").list_instance_type_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_instance_type_details)

```python
# list_instance_type_details method definition

await def list_instance_type_details(
    self,
    *,
    EngineVersion: str,
    DomainName: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    RetrieveAZs: bool = ...,
    InstanceType: str = ...,
) -> ListInstanceTypeDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInstanceTypeDetailsResponseTypeDef](./type_defs.md#listinstancetypedetailsresponsetypedef) 


```python
# list_instance_type_details method usage example with argument unpacking

kwargs: ListInstanceTypeDetailsRequestRequestTypeDef = {  # (1)
    "EngineVersion": ...,
}

parent.list_instance_type_details(**kwargs)
```

1. See [:material-code-braces: ListInstanceTypeDetailsRequestRequestTypeDef](./type_defs.md#listinstancetypedetailsrequestrequesttypedef) 

### list\_packages\_for\_domain

Lists all packages associated with an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").list_packages_for_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_packages_for_domain)

```python
# list_packages_for_domain method definition

await def list_packages_for_domain(
    self,
    *,
    DomainName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPackagesForDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPackagesForDomainResponseTypeDef](./type_defs.md#listpackagesfordomainresponsetypedef) 


```python
# list_packages_for_domain method usage example with argument unpacking

kwargs: ListPackagesForDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_packages_for_domain(**kwargs)
```

1. See [:material-code-braces: ListPackagesForDomainRequestRequestTypeDef](./type_defs.md#listpackagesfordomainrequestrequesttypedef) 

### list\_scheduled\_actions

Retrieves a list of configuration changes that are scheduled for a domain.

Type annotations and code completion for `#!python session.create_client("opensearch").list_scheduled_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_scheduled_actions)

```python
# list_scheduled_actions method definition

await def list_scheduled_actions(
    self,
    *,
    DomainName: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListScheduledActionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListScheduledActionsResponseTypeDef](./type_defs.md#listscheduledactionsresponsetypedef) 


```python
# list_scheduled_actions method usage example with argument unpacking

kwargs: ListScheduledActionsRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_scheduled_actions(**kwargs)
```

1. See [:material-code-braces: ListScheduledActionsRequestRequestTypeDef](./type_defs.md#listscheduledactionsrequestrequesttypedef) 

### list\_tags

Returns all resource tags for an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").list_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_tags)

```python
# list_tags method definition

await def list_tags(
    self,
    *,
    ARN: str,
) -> ListTagsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python
# list_tags method usage example with argument unpacking

kwargs: ListTagsRequestRequestTypeDef = {  # (1)
    "ARN": ...,
}

parent.list_tags(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestRequestTypeDef](./type_defs.md#listtagsrequestrequesttypedef) 

### list\_versions

Lists all versions of OpenSearch and Elasticsearch that Amazon OpenSearch
Service
supports.

Type annotations and code completion for `#!python session.create_client("opensearch").list_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_versions)

```python
# list_versions method definition

await def list_versions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVersionsResponseTypeDef](./type_defs.md#listversionsresponsetypedef) 


```python
# list_versions method usage example with argument unpacking

kwargs: ListVersionsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_versions(**kwargs)
```

1. See [:material-code-braces: ListVersionsRequestRequestTypeDef](./type_defs.md#listversionsrequestrequesttypedef) 

### list\_vpc\_endpoint\_access

Retrieves information about each Amazon Web Services principal that is allowed
to access a given Amazon OpenSearch Service domain through the use of an
interface VPC
endpoint.

Type annotations and code completion for `#!python session.create_client("opensearch").list_vpc_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_vpc_endpoint_access)

```python
# list_vpc_endpoint_access method definition

await def list_vpc_endpoint_access(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
) -> ListVpcEndpointAccessResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVpcEndpointAccessResponseTypeDef](./type_defs.md#listvpcendpointaccessresponsetypedef) 


```python
# list_vpc_endpoint_access method usage example with argument unpacking

kwargs: ListVpcEndpointAccessRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_vpc_endpoint_access(**kwargs)
```

1. See [:material-code-braces: ListVpcEndpointAccessRequestRequestTypeDef](./type_defs.md#listvpcendpointaccessrequestrequesttypedef) 

### list\_vpc\_endpoints

Retrieves all Amazon OpenSearch Service-managed VPC endpoints in the current
Amazon Web Services account and
Region.

Type annotations and code completion for `#!python session.create_client("opensearch").list_vpc_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_vpc_endpoints)

```python
# list_vpc_endpoints method definition

await def list_vpc_endpoints(
    self,
    *,
    NextToken: str = ...,
) -> ListVpcEndpointsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVpcEndpointsResponseTypeDef](./type_defs.md#listvpcendpointsresponsetypedef) 


```python
# list_vpc_endpoints method usage example with argument unpacking

kwargs: ListVpcEndpointsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_vpc_endpoints(**kwargs)
```

1. See [:material-code-braces: ListVpcEndpointsRequestRequestTypeDef](./type_defs.md#listvpcendpointsrequestrequesttypedef) 

### list\_vpc\_endpoints\_for\_domain

Retrieves all Amazon OpenSearch Service-managed VPC endpoints associated with a
particular
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").list_vpc_endpoints_for_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.list_vpc_endpoints_for_domain)

```python
# list_vpc_endpoints_for_domain method definition

await def list_vpc_endpoints_for_domain(
    self,
    *,
    DomainName: str,
    NextToken: str = ...,
) -> ListVpcEndpointsForDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVpcEndpointsForDomainResponseTypeDef](./type_defs.md#listvpcendpointsfordomainresponsetypedef) 


```python
# list_vpc_endpoints_for_domain method usage example with argument unpacking

kwargs: ListVpcEndpointsForDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.list_vpc_endpoints_for_domain(**kwargs)
```

1. See [:material-code-braces: ListVpcEndpointsForDomainRequestRequestTypeDef](./type_defs.md#listvpcendpointsfordomainrequestrequesttypedef) 

### purchase\_reserved\_instance\_offering

Allows you to purchase Amazon OpenSearch Service Reserved Instances.

Type annotations and code completion for `#!python session.create_client("opensearch").purchase_reserved_instance_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.purchase_reserved_instance_offering)

```python
# purchase_reserved_instance_offering method definition

await def purchase_reserved_instance_offering(
    self,
    *,
    ReservedInstanceOfferingId: str,
    ReservationName: str,
    InstanceCount: int = ...,
) -> PurchaseReservedInstanceOfferingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PurchaseReservedInstanceOfferingResponseTypeDef](./type_defs.md#purchasereservedinstanceofferingresponsetypedef) 


```python
# purchase_reserved_instance_offering method usage example with argument unpacking

kwargs: PurchaseReservedInstanceOfferingRequestRequestTypeDef = {  # (1)
    "ReservedInstanceOfferingId": ...,
    "ReservationName": ...,
}

parent.purchase_reserved_instance_offering(**kwargs)
```

1. See [:material-code-braces: PurchaseReservedInstanceOfferingRequestRequestTypeDef](./type_defs.md#purchasereservedinstanceofferingrequestrequesttypedef) 

### reject\_inbound\_connection

Allows the remote Amazon OpenSearch Service domain owner to reject an inbound
cross-cluster connection
request.

Type annotations and code completion for `#!python session.create_client("opensearch").reject_inbound_connection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.reject_inbound_connection)

```python
# reject_inbound_connection method definition

await def reject_inbound_connection(
    self,
    *,
    ConnectionId: str,
) -> RejectInboundConnectionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RejectInboundConnectionResponseTypeDef](./type_defs.md#rejectinboundconnectionresponsetypedef) 


```python
# reject_inbound_connection method usage example with argument unpacking

kwargs: RejectInboundConnectionRequestRequestTypeDef = {  # (1)
    "ConnectionId": ...,
}

parent.reject_inbound_connection(**kwargs)
```

1. See [:material-code-braces: RejectInboundConnectionRequestRequestTypeDef](./type_defs.md#rejectinboundconnectionrequestrequesttypedef) 

### remove\_tags

Removes the specified set of tags from an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").remove_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.remove_tags)

```python
# remove_tags method definition

await def remove_tags(
    self,
    *,
    ARN: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# remove_tags method usage example with argument unpacking

kwargs: RemoveTagsRequestRequestTypeDef = {  # (1)
    "ARN": ...,
    "TagKeys": ...,
}

parent.remove_tags(**kwargs)
```

1. See [:material-code-braces: RemoveTagsRequestRequestTypeDef](./type_defs.md#removetagsrequestrequesttypedef) 

### revoke\_vpc\_endpoint\_access

Revokes access to an Amazon OpenSearch Service domain that was provided through
an interface VPC
endpoint.

Type annotations and code completion for `#!python session.create_client("opensearch").revoke_vpc_endpoint_access` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.revoke_vpc_endpoint_access)

```python
# revoke_vpc_endpoint_access method definition

await def revoke_vpc_endpoint_access(
    self,
    *,
    DomainName: str,
    Account: str,
) -> Dict[str, Any]:
    ...
```



```python
# revoke_vpc_endpoint_access method usage example with argument unpacking

kwargs: RevokeVpcEndpointAccessRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Account": ...,
}

parent.revoke_vpc_endpoint_access(**kwargs)
```

1. See [:material-code-braces: RevokeVpcEndpointAccessRequestRequestTypeDef](./type_defs.md#revokevpcendpointaccessrequestrequesttypedef) 

### start\_domain\_maintenance

Starts the node maintenance process on the data node.

Type annotations and code completion for `#!python session.create_client("opensearch").start_domain_maintenance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.start_domain_maintenance)

```python
# start_domain_maintenance method definition

await def start_domain_maintenance(
    self,
    *,
    DomainName: str,
    Action: MaintenanceTypeType,  # (1)
    NodeId: str = ...,
) -> StartDomainMaintenanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: MaintenanceTypeType](./literals.md#maintenancetypetype) 
2. See [:material-code-braces: StartDomainMaintenanceResponseTypeDef](./type_defs.md#startdomainmaintenanceresponsetypedef) 


```python
# start_domain_maintenance method usage example with argument unpacking

kwargs: StartDomainMaintenanceRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Action": ...,
}

parent.start_domain_maintenance(**kwargs)
```

1. See [:material-code-braces: StartDomainMaintenanceRequestRequestTypeDef](./type_defs.md#startdomainmaintenancerequestrequesttypedef) 

### start\_service\_software\_update

Schedules a service software update for an Amazon OpenSearch Service domain.

Type annotations and code completion for `#!python session.create_client("opensearch").start_service_software_update` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.start_service_software_update)

```python
# start_service_software_update method definition

await def start_service_software_update(
    self,
    *,
    DomainName: str,
    ScheduleAt: ScheduleAtType = ...,  # (1)
    DesiredStartTime: int = ...,
) -> StartServiceSoftwareUpdateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ScheduleAtType](./literals.md#scheduleattype) 
2. See [:material-code-braces: StartServiceSoftwareUpdateResponseTypeDef](./type_defs.md#startservicesoftwareupdateresponsetypedef) 


```python
# start_service_software_update method usage example with argument unpacking

kwargs: StartServiceSoftwareUpdateRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.start_service_software_update(**kwargs)
```

1. See [:material-code-braces: StartServiceSoftwareUpdateRequestRequestTypeDef](./type_defs.md#startservicesoftwareupdaterequestrequesttypedef) 

### update\_data\_source

Updates a direct-query data source.

Type annotations and code completion for `#!python session.create_client("opensearch").update_data_source` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_data_source)

```python
# update_data_source method definition

await def update_data_source(
    self,
    *,
    DomainName: str,
    Name: str,
    DataSourceType: DataSourceTypeTypeDef,  # (1)
    Description: str = ...,
    Status: DataSourceStatusType = ...,  # (2)
) -> UpdateDataSourceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: DataSourceTypeTypeDef](./type_defs.md#datasourcetypetypedef) 
2. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
3. See [:material-code-braces: UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef) 


```python
# update_data_source method usage example with argument unpacking

kwargs: UpdateDataSourceRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "Name": ...,
    "DataSourceType": ...,
}

parent.update_data_source(**kwargs)
```

1. See [:material-code-braces: UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef) 

### update\_domain\_config

Modifies the cluster configuration of the specified Amazon OpenSearch Service
domain.

Type annotations and code completion for `#!python session.create_client("opensearch").update_domain_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_domain_config)

```python
# update_domain_config method definition

await def update_domain_config(
    self,
    *,
    DomainName: str,
    ClusterConfig: ClusterConfigTypeDef = ...,  # (1)
    EBSOptions: EBSOptionsTypeDef = ...,  # (2)
    SnapshotOptions: SnapshotOptionsTypeDef = ...,  # (3)
    VPCOptions: VPCOptionsTypeDef = ...,  # (4)
    CognitoOptions: CognitoOptionsTypeDef = ...,  # (5)
    AdvancedOptions: Mapping[str, str] = ...,
    AccessPolicies: str = ...,
    IPAddressType: IPAddressTypeType = ...,  # (6)
    LogPublishingOptions: Mapping[LogTypeType, LogPublishingOptionTypeDef] = ...,  # (7)
    EncryptionAtRestOptions: EncryptionAtRestOptionsTypeDef = ...,  # (8)
    DomainEndpointOptions: DomainEndpointOptionsTypeDef = ...,  # (9)
    NodeToNodeEncryptionOptions: NodeToNodeEncryptionOptionsTypeDef = ...,  # (10)
    AdvancedSecurityOptions: AdvancedSecurityOptionsInputTypeDef = ...,  # (11)
    AutoTuneOptions: AutoTuneOptionsTypeDef = ...,  # (12)
    DryRun: bool = ...,
    DryRunMode: DryRunModeType = ...,  # (13)
    OffPeakWindowOptions: OffPeakWindowOptionsTypeDef = ...,  # (14)
    SoftwareUpdateOptions: SoftwareUpdateOptionsTypeDef = ...,  # (15)
    AIMLOptions: AIMLOptionsInputTypeDef = ...,  # (16)
) -> UpdateDomainConfigResponseTypeDef:  # (17)
    ...
```

1. See [:material-code-braces: ClusterConfigTypeDef](./type_defs.md#clusterconfigtypedef) 
2. See [:material-code-braces: EBSOptionsTypeDef](./type_defs.md#ebsoptionstypedef) 
3. See [:material-code-braces: SnapshotOptionsTypeDef](./type_defs.md#snapshotoptionstypedef) 
4. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
5. See [:material-code-braces: CognitoOptionsTypeDef](./type_defs.md#cognitooptionstypedef) 
6. See [:material-code-brackets: IPAddressTypeType](./literals.md#ipaddresstypetype) 
7. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) [:material-code-braces: LogPublishingOptionTypeDef](./type_defs.md#logpublishingoptiontypedef) 
8. See [:material-code-braces: EncryptionAtRestOptionsTypeDef](./type_defs.md#encryptionatrestoptionstypedef) 
9. See [:material-code-braces: DomainEndpointOptionsTypeDef](./type_defs.md#domainendpointoptionstypedef) 
10. See [:material-code-braces: NodeToNodeEncryptionOptionsTypeDef](./type_defs.md#nodetonodeencryptionoptionstypedef) 
11. See [:material-code-braces: AdvancedSecurityOptionsInputTypeDef](./type_defs.md#advancedsecurityoptionsinputtypedef) 
12. See [:material-code-braces: AutoTuneOptionsTypeDef](./type_defs.md#autotuneoptionstypedef) 
13. See [:material-code-brackets: DryRunModeType](./literals.md#dryrunmodetype) 
14. See [:material-code-braces: OffPeakWindowOptionsTypeDef](./type_defs.md#offpeakwindowoptionstypedef) 
15. See [:material-code-braces: SoftwareUpdateOptionsTypeDef](./type_defs.md#softwareupdateoptionstypedef) 
16. See [:material-code-braces: AIMLOptionsInputTypeDef](./type_defs.md#aimloptionsinputtypedef) 
17. See [:material-code-braces: UpdateDomainConfigResponseTypeDef](./type_defs.md#updatedomainconfigresponsetypedef) 


```python
# update_domain_config method usage example with argument unpacking

kwargs: UpdateDomainConfigRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
}

parent.update_domain_config(**kwargs)
```

1. See [:material-code-braces: UpdateDomainConfigRequestRequestTypeDef](./type_defs.md#updatedomainconfigrequestrequesttypedef) 

### update\_package

Updates a package for use with Amazon OpenSearch Service domains.

Type annotations and code completion for `#!python session.create_client("opensearch").update_package` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_package)

```python
# update_package method definition

await def update_package(
    self,
    *,
    PackageID: str,
    PackageSource: PackageSourceTypeDef,  # (1)
    PackageDescription: str = ...,
    CommitMessage: str = ...,
) -> UpdatePackageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PackageSourceTypeDef](./type_defs.md#packagesourcetypedef) 
2. See [:material-code-braces: UpdatePackageResponseTypeDef](./type_defs.md#updatepackageresponsetypedef) 


```python
# update_package method usage example with argument unpacking

kwargs: UpdatePackageRequestRequestTypeDef = {  # (1)
    "PackageID": ...,
    "PackageSource": ...,
}

parent.update_package(**kwargs)
```

1. See [:material-code-braces: UpdatePackageRequestRequestTypeDef](./type_defs.md#updatepackagerequestrequesttypedef) 

### update\_scheduled\_action

Reschedules a planned domain configuration change for a later time.

Type annotations and code completion for `#!python session.create_client("opensearch").update_scheduled_action` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_scheduled_action)

```python
# update_scheduled_action method definition

await def update_scheduled_action(
    self,
    *,
    DomainName: str,
    ActionID: str,
    ActionType: ActionTypeType,  # (1)
    ScheduleAt: ScheduleAtType,  # (2)
    DesiredStartTime: int = ...,
) -> UpdateScheduledActionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ActionTypeType](./literals.md#actiontypetype) 
2. See [:material-code-brackets: ScheduleAtType](./literals.md#scheduleattype) 
3. See [:material-code-braces: UpdateScheduledActionResponseTypeDef](./type_defs.md#updatescheduledactionresponsetypedef) 


```python
# update_scheduled_action method usage example with argument unpacking

kwargs: UpdateScheduledActionRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "ActionID": ...,
    "ActionType": ...,
    "ScheduleAt": ...,
}

parent.update_scheduled_action(**kwargs)
```

1. See [:material-code-braces: UpdateScheduledActionRequestRequestTypeDef](./type_defs.md#updatescheduledactionrequestrequesttypedef) 

### update\_vpc\_endpoint

Modifies an Amazon OpenSearch Service-managed interface VPC endpoint.

Type annotations and code completion for `#!python session.create_client("opensearch").update_vpc_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.update_vpc_endpoint)

```python
# update_vpc_endpoint method definition

await def update_vpc_endpoint(
    self,
    *,
    VpcEndpointId: str,
    VpcOptions: VPCOptionsTypeDef,  # (1)
) -> UpdateVpcEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: VPCOptionsTypeDef](./type_defs.md#vpcoptionstypedef) 
2. See [:material-code-braces: UpdateVpcEndpointResponseTypeDef](./type_defs.md#updatevpcendpointresponsetypedef) 


```python
# update_vpc_endpoint method usage example with argument unpacking

kwargs: UpdateVpcEndpointRequestRequestTypeDef = {  # (1)
    "VpcEndpointId": ...,
    "VpcOptions": ...,
}

parent.update_vpc_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateVpcEndpointRequestRequestTypeDef](./type_defs.md#updatevpcendpointrequestrequesttypedef) 

### upgrade\_domain

Allows you to either upgrade your Amazon OpenSearch Service domain or perform
an upgrade eligibility check to a compatible version of OpenSearch or
Elasticsearch.

Type annotations and code completion for `#!python session.create_client("opensearch").upgrade_domain` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.upgrade_domain)

```python
# upgrade_domain method definition

await def upgrade_domain(
    self,
    *,
    DomainName: str,
    TargetVersion: str,
    PerformCheckOnly: bool = ...,
    AdvancedOptions: Mapping[str, str] = ...,
) -> UpgradeDomainResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpgradeDomainResponseTypeDef](./type_defs.md#upgradedomainresponsetypedef) 


```python
# upgrade_domain method usage example with argument unpacking

kwargs: UpgradeDomainRequestRequestTypeDef = {  # (1)
    "DomainName": ...,
    "TargetVersion": ...,
}

parent.upgrade_domain(**kwargs)
```

1. See [:material-code-braces: UpgradeDomainRequestRequestTypeDef](./type_defs.md#upgradedomainrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("opensearch").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "OpenSearchServiceClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("opensearch").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService.Client.__aexit__)

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





