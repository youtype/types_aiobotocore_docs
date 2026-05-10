# EVSClient

> [Index](../README.md) > [EVS](./README.md) > EVSClient

!!! note ""

    Auto-generated documentation for [EVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs.html#evs)
    type annotations stubs module [types-aiobotocore-evs](https://pypi.org/project/types-aiobotocore-evs/).

## EVSClient

Type annotations and code completion for `#!python session.create_client("evs")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs.html#EVS.Client)

```python
# EVSClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_evs.client import EVSClient

session = get_session()
async with session.create_client("evs") as client:
    client: EVSClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("evs").exceptions` structure.

```python
# EVSClient.exceptions usage example

async with session.create_client("evs") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.TagPolicyException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# EVSClient usage type checking example

from types_aiobotocore_evs.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("evs").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("evs").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/generate_presigned_url.html)

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


### associate\_eip\_to\_vlan

Associates an Elastic IP address with a public HCX VLAN.

Type annotations and code completion for `#!python session.create_client("evs").associate_eip_to_vlan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/associate_eip_to_vlan.html)

```python
# associate_eip_to_vlan method definition

await def associate_eip_to_vlan(
    self,
    *,
    environmentId: str,
    vlanName: str,
    allocationId: str,
    clientToken: str = ...,
) -> AssociateEipToVlanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateEipToVlanResponseTypeDef](./type_defs.md#associateeiptovlanresponsetypedef)


```python
# associate_eip_to_vlan method usage example with argument unpacking

kwargs: AssociateEipToVlanRequestTypeDef = {  # (1)
    "environmentId": ...,
    "vlanName": ...,
    "allocationId": ...,
}

parent.associate_eip_to_vlan(**kwargs)
```

1. See [:material-code-braces: AssociateEipToVlanRequestTypeDef](./type_defs.md#associateeiptovlanrequesttypedef)

### create\_entitlement

Creates a Windows Server License entitlement for virtual machines in an Amazon
EVS environment using the provided vCenter Server connector.

Type annotations and code completion for `#!python session.create_client("evs").create_entitlement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/create_entitlement.html)

```python
# create_entitlement method definition

await def create_entitlement(
    self,
    *,
    environmentId: str,
    connectorId: str,
    entitlementType: EntitlementTypeType,  # (1)
    vmIds: Sequence[str],
    clientToken: str = ...,
) -> CreateEntitlementResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EntitlementTypeType](./literals.md#entitlementtypetype)
2. See [:material-code-braces: CreateEntitlementResponseTypeDef](./type_defs.md#createentitlementresponsetypedef)


```python
# create_entitlement method usage example with argument unpacking

kwargs: CreateEntitlementRequestTypeDef = {  # (1)
    "environmentId": ...,
    "connectorId": ...,
    "entitlementType": ...,
    "vmIds": ...,
}

parent.create_entitlement(**kwargs)
```

1. See [:material-code-braces: CreateEntitlementRequestTypeDef](./type_defs.md#createentitlementrequesttypedef)

### create\_environment

Creates an Amazon EVS environment that runs VCF software, such as SDDC Manager,
NSX Manager, and vCenter Server.

Type annotations and code completion for `#!python session.create_client("evs").create_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/create_environment.html)

```python
# create_environment method definition

await def create_environment(
    self,
    *,
    vpcId: str,
    serviceAccessSubnetId: str,
    vcfVersion: VcfVersionType,  # (1)
    termsAccepted: bool,
    licenseInfo: Sequence[LicenseInfoTypeDef],  # (2)
    initialVlans: InitialVlansTypeDef,  # (3)
    hosts: Sequence[HostInfoForCreateTypeDef],  # (4)
    connectivityInfo: ConnectivityInfoUnionTypeDef,  # (5)
    vcfHostnames: VcfHostnamesTypeDef,  # (6)
    siteId: str,
    clientToken: str = ...,
    environmentName: str = ...,
    kmsKeyId: str = ...,
    tags: Mapping[str, str] = ...,
    serviceAccessSecurityGroups: ServiceAccessSecurityGroupsUnionTypeDef = ...,  # (7)
) -> CreateEnvironmentResponseTypeDef:  # (8)
    ...
```

1. See [:material-code-brackets: VcfVersionType](./literals.md#vcfversiontype)
2. See `Sequence[LicenseInfoTypeDef]`
3. See [:material-code-braces: InitialVlansTypeDef](./type_defs.md#initialvlanstypedef)
4. See `Sequence[HostInfoForCreateTypeDef]`
5. See [:material-code-braces: ConnectivityInfoUnionTypeDef](#connectivityinfouniontypedef)
6. See [:material-code-braces: VcfHostnamesTypeDef](./type_defs.md#vcfhostnamestypedef)
7. See [:material-code-braces: ServiceAccessSecurityGroupsUnionTypeDef](#serviceaccesssecuritygroupsuniontypedef)
8. See [:material-code-braces: CreateEnvironmentResponseTypeDef](./type_defs.md#createenvironmentresponsetypedef)


```python
# create_environment method usage example with argument unpacking

kwargs: CreateEnvironmentRequestTypeDef = {  # (1)
    "vpcId": ...,
    "serviceAccessSubnetId": ...,
    "vcfVersion": ...,
    "termsAccepted": ...,
    "licenseInfo": ...,
    "initialVlans": ...,
    "hosts": ...,
    "connectivityInfo": ...,
    "vcfHostnames": ...,
    "siteId": ...,
}

parent.create_environment(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentRequestTypeDef](./type_defs.md#createenvironmentrequesttypedef)

### create\_environment\_connector

Creates a connector for an Amazon EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").create_environment_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/create_environment_connector.html)

```python
# create_environment_connector method definition

await def create_environment_connector(
    self,
    *,
    environmentId: str,
    type: ConnectorTypeType,  # (1)
    applianceFqdn: str,
    secretIdentifier: str,
    clientToken: str = ...,
) -> CreateEnvironmentConnectorResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype)
2. See [:material-code-braces: CreateEnvironmentConnectorResponseTypeDef](./type_defs.md#createenvironmentconnectorresponsetypedef)


```python
# create_environment_connector method usage example with argument unpacking

kwargs: CreateEnvironmentConnectorRequestTypeDef = {  # (1)
    "environmentId": ...,
    "type": ...,
    "applianceFqdn": ...,
    "secretIdentifier": ...,
}

parent.create_environment_connector(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentConnectorRequestTypeDef](./type_defs.md#createenvironmentconnectorrequesttypedef)

### create\_environment\_host

Creates an ESX host and adds it to an Amazon EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").create_environment_host` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/create_environment_host.html)

```python
# create_environment_host method definition

await def create_environment_host(
    self,
    *,
    environmentId: str,
    host: HostInfoForCreateTypeDef,  # (1)
    clientToken: str = ...,
    esxVersion: str = ...,
) -> CreateEnvironmentHostResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HostInfoForCreateTypeDef](./type_defs.md#hostinfoforcreatetypedef)
2. See [:material-code-braces: CreateEnvironmentHostResponseTypeDef](./type_defs.md#createenvironmenthostresponsetypedef)


```python
# create_environment_host method usage example with argument unpacking

kwargs: CreateEnvironmentHostRequestTypeDef = {  # (1)
    "environmentId": ...,
    "host": ...,
}

parent.create_environment_host(**kwargs)
```

1. See [:material-code-braces: CreateEnvironmentHostRequestTypeDef](./type_defs.md#createenvironmenthostrequesttypedef)

### delete\_entitlement

Deletes a Windows Server License entitlement for virtual machines in an Amazon
EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").delete_entitlement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/delete_entitlement.html)

```python
# delete_entitlement method definition

await def delete_entitlement(
    self,
    *,
    environmentId: str,
    connectorId: str,
    entitlementType: EntitlementTypeType,  # (1)
    vmIds: Sequence[str],
    clientToken: str = ...,
) -> DeleteEntitlementResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EntitlementTypeType](./literals.md#entitlementtypetype)
2. See [:material-code-braces: DeleteEntitlementResponseTypeDef](./type_defs.md#deleteentitlementresponsetypedef)


```python
# delete_entitlement method usage example with argument unpacking

kwargs: DeleteEntitlementRequestTypeDef = {  # (1)
    "environmentId": ...,
    "connectorId": ...,
    "entitlementType": ...,
    "vmIds": ...,
}

parent.delete_entitlement(**kwargs)
```

1. See [:material-code-braces: DeleteEntitlementRequestTypeDef](./type_defs.md#deleteentitlementrequesttypedef)

### delete\_environment

Deletes an Amazon EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").delete_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/delete_environment.html)

```python
# delete_environment method definition

await def delete_environment(
    self,
    *,
    environmentId: str,
    clientToken: str = ...,
) -> DeleteEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEnvironmentResponseTypeDef](./type_defs.md#deleteenvironmentresponsetypedef)


```python
# delete_environment method usage example with argument unpacking

kwargs: DeleteEnvironmentRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.delete_environment(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentRequestTypeDef](./type_defs.md#deleteenvironmentrequesttypedef)

### delete\_environment\_connector

Deletes a connector from an Amazon EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").delete_environment_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/delete_environment_connector.html)

```python
# delete_environment_connector method definition

await def delete_environment_connector(
    self,
    *,
    environmentId: str,
    connectorId: str,
    clientToken: str = ...,
) -> DeleteEnvironmentConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEnvironmentConnectorResponseTypeDef](./type_defs.md#deleteenvironmentconnectorresponsetypedef)


```python
# delete_environment_connector method usage example with argument unpacking

kwargs: DeleteEnvironmentConnectorRequestTypeDef = {  # (1)
    "environmentId": ...,
    "connectorId": ...,
}

parent.delete_environment_connector(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentConnectorRequestTypeDef](./type_defs.md#deleteenvironmentconnectorrequesttypedef)

### delete\_environment\_host

Deletes a host from an Amazon EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").delete_environment_host` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/delete_environment_host.html)

```python
# delete_environment_host method definition

await def delete_environment_host(
    self,
    *,
    environmentId: str,
    hostName: str,
    clientToken: str = ...,
) -> DeleteEnvironmentHostResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteEnvironmentHostResponseTypeDef](./type_defs.md#deleteenvironmenthostresponsetypedef)


```python
# delete_environment_host method usage example with argument unpacking

kwargs: DeleteEnvironmentHostRequestTypeDef = {  # (1)
    "environmentId": ...,
    "hostName": ...,
}

parent.delete_environment_host(**kwargs)
```

1. See [:material-code-braces: DeleteEnvironmentHostRequestTypeDef](./type_defs.md#deleteenvironmenthostrequesttypedef)

### disassociate\_eip\_from\_vlan

Disassociates an Elastic IP address from a public HCX VLAN.

Type annotations and code completion for `#!python session.create_client("evs").disassociate_eip_from_vlan` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/disassociate_eip_from_vlan.html)

```python
# disassociate_eip_from_vlan method definition

await def disassociate_eip_from_vlan(
    self,
    *,
    environmentId: str,
    vlanName: str,
    associationId: str,
    clientToken: str = ...,
) -> DisassociateEipFromVlanResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateEipFromVlanResponseTypeDef](./type_defs.md#disassociateeipfromvlanresponsetypedef)


```python
# disassociate_eip_from_vlan method usage example with argument unpacking

kwargs: DisassociateEipFromVlanRequestTypeDef = {  # (1)
    "environmentId": ...,
    "vlanName": ...,
    "associationId": ...,
}

parent.disassociate_eip_from_vlan(**kwargs)
```

1. See [:material-code-braces: DisassociateEipFromVlanRequestTypeDef](./type_defs.md#disassociateeipfromvlanrequesttypedef)

### get\_environment

Returns a description of the specified environment.

Type annotations and code completion for `#!python session.create_client("evs").get_environment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/get_environment.html)

```python
# get_environment method definition

await def get_environment(
    self,
    *,
    environmentId: str,
) -> GetEnvironmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef)


```python
# get_environment method usage example with argument unpacking

kwargs: GetEnvironmentRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.get_environment(**kwargs)
```

1. See [:material-code-braces: GetEnvironmentRequestTypeDef](./type_defs.md#getenvironmentrequesttypedef)

### get\_versions

Returns information about VCF versions, ESX versions and EC2 instance types
provided by Amazon EVS.

Type annotations and code completion for `#!python session.create_client("evs").get_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/get_versions.html)

```python
# get_versions method definition

await def get_versions(
    self,
) -> GetVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVersionsResponseTypeDef](./type_defs.md#getversionsresponsetypedef)



### list\_environment\_connectors

Lists the connectors within an environment.

Type annotations and code completion for `#!python session.create_client("evs").list_environment_connectors` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/list_environment_connectors.html)

```python
# list_environment_connectors method definition

await def list_environment_connectors(
    self,
    *,
    environmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEnvironmentConnectorsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentConnectorsResponseTypeDef](./type_defs.md#listenvironmentconnectorsresponsetypedef)


```python
# list_environment_connectors method usage example with argument unpacking

kwargs: ListEnvironmentConnectorsRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.list_environment_connectors(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentConnectorsRequestTypeDef](./type_defs.md#listenvironmentconnectorsrequesttypedef)

### list\_environment\_hosts

List the hosts within an environment.

Type annotations and code completion for `#!python session.create_client("evs").list_environment_hosts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/list_environment_hosts.html)

```python
# list_environment_hosts method definition

await def list_environment_hosts(
    self,
    *,
    environmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEnvironmentHostsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentHostsResponseTypeDef](./type_defs.md#listenvironmenthostsresponsetypedef)


```python
# list_environment_hosts method usage example with argument unpacking

kwargs: ListEnvironmentHostsRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.list_environment_hosts(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentHostsRequestTypeDef](./type_defs.md#listenvironmenthostsrequesttypedef)

### list\_environment\_vlans

Lists environment VLANs that are associated with the specified environment.

Type annotations and code completion for `#!python session.create_client("evs").list_environment_vlans` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/list_environment_vlans.html)

```python
# list_environment_vlans method definition

await def list_environment_vlans(
    self,
    *,
    environmentId: str,
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListEnvironmentVlansResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEnvironmentVlansResponseTypeDef](./type_defs.md#listenvironmentvlansresponsetypedef)


```python
# list_environment_vlans method usage example with argument unpacking

kwargs: ListEnvironmentVlansRequestTypeDef = {  # (1)
    "environmentId": ...,
}

parent.list_environment_vlans(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentVlansRequestTypeDef](./type_defs.md#listenvironmentvlansrequesttypedef)

### list\_environments

Lists the Amazon EVS environments in your Amazon Web Services account in the
specified Amazon Web Services Region.

Type annotations and code completion for `#!python session.create_client("evs").list_environments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/list_environments.html)

```python
# list_environments method definition

await def list_environments(
    self,
    *,
    nextToken: str = ...,
    maxResults: int = ...,
    state: Sequence[EnvironmentStateType] = ...,  # (1)
) -> ListEnvironmentsResponseTypeDef:  # (2)
    ...
```

1. See `Sequence[EnvironmentStateType]`
2. See [:material-code-braces: ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef)


```python
# list_environments method usage example with argument unpacking

kwargs: ListEnvironmentsRequestTypeDef = {  # (1)
    "nextToken": ...,
}

parent.list_environments(**kwargs)
```

1. See [:material-code-braces: ListEnvironmentsRequestTypeDef](./type_defs.md#listenvironmentsrequesttypedef)

### list\_tags\_for\_resource

Lists the tags for an Amazon EVS resource.

Type annotations and code completion for `#!python session.create_client("evs").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/list_tags_for_resource.html)

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

### list\_vm\_entitlements

Lists the Windows Server License entitlements for virtual machines in an Amazon
EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").list_vm_entitlements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/list_vm_entitlements.html)

```python
# list_vm_entitlements method definition

await def list_vm_entitlements(
    self,
    *,
    environmentId: str,
    connectorId: str,
    entitlementType: EntitlementTypeType,  # (1)
    nextToken: str = ...,
    maxResults: int = ...,
) -> ListVmEntitlementsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EntitlementTypeType](./literals.md#entitlementtypetype)
2. See [:material-code-braces: ListVmEntitlementsResponseTypeDef](./type_defs.md#listvmentitlementsresponsetypedef)


```python
# list_vm_entitlements method usage example with argument unpacking

kwargs: ListVmEntitlementsRequestTypeDef = {  # (1)
    "environmentId": ...,
    "connectorId": ...,
    "entitlementType": ...,
}

parent.list_vm_entitlements(**kwargs)
```

1. See [:material-code-braces: ListVmEntitlementsRequestTypeDef](./type_defs.md#listvmentitlementsrequesttypedef)

### tag\_resource

Associates the specified tags to an Amazon EVS resource with the specified
<code>resourceArn</code>.

Type annotations and code completion for `#!python session.create_client("evs").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> dict[str, Any]:
    ...
```

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

Deletes specified tags from an Amazon EVS resource.

Type annotations and code completion for `#!python session.create_client("evs").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> dict[str, Any]:
    ...
```

```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)

### update\_environment\_connector

Updates a connector for an Amazon EVS environment.

Type annotations and code completion for `#!python session.create_client("evs").update_environment_connector` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs/client/update_environment_connector.html)

```python
# update_environment_connector method definition

await def update_environment_connector(
    self,
    *,
    environmentId: str,
    connectorId: str,
    clientToken: str = ...,
    applianceFqdn: str = ...,
    secretIdentifier: str = ...,
) -> UpdateEnvironmentConnectorResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEnvironmentConnectorResponseTypeDef](./type_defs.md#updateenvironmentconnectorresponsetypedef)


```python
# update_environment_connector method usage example with argument unpacking

kwargs: UpdateEnvironmentConnectorRequestTypeDef = {  # (1)
    "environmentId": ...,
    "connectorId": ...,
}

parent.update_environment_connector(**kwargs)
```

1. See [:material-code-braces: UpdateEnvironmentConnectorRequestTypeDef](./type_defs.md#updateenvironmentconnectorrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("evs").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs.html#EVS.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("evs").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs.html#EVS.Client)

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

Type annotations and code completion for `#!python session.create_client("evs").get_paginator` method with overloads.

- `client.get_paginator("list_environment_connectors")` -> [ListEnvironmentConnectorsPaginator](./paginators.md#listenvironmentconnectorspaginator)
- `client.get_paginator("list_environment_hosts")` -> [ListEnvironmentHostsPaginator](./paginators.md#listenvironmenthostspaginator)
- `client.get_paginator("list_environment_vlans")` -> [ListEnvironmentVlansPaginator](./paginators.md#listenvironmentvlanspaginator)
- `client.get_paginator("list_environments")` -> [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)
- `client.get_paginator("list_vm_entitlements")` -> [ListVmEntitlementsPaginator](./paginators.md#listvmentitlementspaginator)



