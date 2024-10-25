# VPCLatticeClient

> [Index](../README.md) > [VPCLattice](./README.md) > VPCLatticeClient

!!! note ""

    Auto-generated documentation for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
    type annotations stubs module [types-aiobotocore-vpc-lattice](https://pypi.org/project/types-aiobotocore-vpc-lattice/).

## VPCLatticeClient

Type annotations and code completion for `#!python session.create_client("vpc-lattice")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client)

```python
# VPCLatticeClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_vpc_lattice.client import VPCLatticeClient

session = get_session()
async with session.create_client("vpc-lattice") as client:
    client: VPCLatticeClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("vpc-lattice").exceptions` structure.

```python
# VPCLatticeClient.exceptions usage example

async with session.create_client("vpc-lattice") as client:
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
# VPCLatticeClient usage type checking example

from types_aiobotocore_vpc_lattice.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### batch\_update\_rule

Updates the listener rules in a batch.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").batch_update_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.batch_update_rule)

```python
# batch_update_rule method definition

await def batch_update_rule(
    self,
    *,
    listenerIdentifier: str,
    rules: Sequence[RuleUpdateTypeDef],  # (1)
    serviceIdentifier: str,
) -> BatchUpdateRuleResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuleUpdateTypeDef](./type_defs.md#ruleupdatetypedef) 
2. See [:material-code-braces: BatchUpdateRuleResponseTypeDef](./type_defs.md#batchupdateruleresponsetypedef) 


```python
# batch_update_rule method usage example with argument unpacking

kwargs: BatchUpdateRuleRequestRequestTypeDef = {  # (1)
    "listenerIdentifier": ...,
    "rules": ...,
    "serviceIdentifier": ...,
}

parent.batch_update_rule(**kwargs)
```

1. See [:material-code-braces: BatchUpdateRuleRequestRequestTypeDef](./type_defs.md#batchupdaterulerequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_access\_log\_subscription

Enables access logs to be sent to Amazon CloudWatch, Amazon S3, and Amazon
Kinesis Data
Firehose.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_access_log_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)

```python
# create_access_log_subscription method definition

await def create_access_log_subscription(
    self,
    *,
    destinationArn: str,
    resourceIdentifier: str,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateAccessLogSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateAccessLogSubscriptionResponseTypeDef](./type_defs.md#createaccesslogsubscriptionresponsetypedef) 


```python
# create_access_log_subscription method usage example with argument unpacking

kwargs: CreateAccessLogSubscriptionRequestRequestTypeDef = {  # (1)
    "destinationArn": ...,
    "resourceIdentifier": ...,
}

parent.create_access_log_subscription(**kwargs)
```

1. See [:material-code-braces: CreateAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#createaccesslogsubscriptionrequestrequesttypedef) 

### create\_listener

Creates a listener for a service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)

```python
# create_listener method definition

await def create_listener(
    self,
    *,
    defaultAction: RuleActionTypeDef,  # (1)
    name: str,
    protocol: ListenerProtocolType,  # (2)
    serviceIdentifier: str,
    clientToken: str = ...,
    port: int = ...,
    tags: Mapping[str, str] = ...,
) -> CreateListenerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-brackets: ListenerProtocolType](./literals.md#listenerprotocoltype) 
3. See [:material-code-braces: CreateListenerResponseTypeDef](./type_defs.md#createlistenerresponsetypedef) 


```python
# create_listener method usage example with argument unpacking

kwargs: CreateListenerRequestRequestTypeDef = {  # (1)
    "defaultAction": ...,
    "name": ...,
    "protocol": ...,
    "serviceIdentifier": ...,
}

parent.create_listener(**kwargs)
```

1. See [:material-code-braces: CreateListenerRequestRequestTypeDef](./type_defs.md#createlistenerrequestrequesttypedef) 

### create\_rule

Creates a listener rule.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_rule)

```python
# create_rule method definition

await def create_rule(
    self,
    *,
    action: RuleActionTypeDef,  # (1)
    listenerIdentifier: str,
    match: RuleMatchTypeDef,  # (2)
    name: str,
    priority: int,
    serviceIdentifier: str,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateRuleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) 
3. See [:material-code-braces: CreateRuleResponseTypeDef](./type_defs.md#createruleresponsetypedef) 


```python
# create_rule method usage example with argument unpacking

kwargs: CreateRuleRequestRequestTypeDef = {  # (1)
    "action": ...,
    "listenerIdentifier": ...,
    "match": ...,
    "name": ...,
    "priority": ...,
    "serviceIdentifier": ...,
}

parent.create_rule(**kwargs)
```

1. See [:material-code-braces: CreateRuleRequestRequestTypeDef](./type_defs.md#createrulerequestrequesttypedef) 

### create\_service

Creates a service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service)

```python
# create_service method definition

await def create_service(
    self,
    *,
    name: str,
    authType: AuthTypeType = ...,  # (1)
    certificateArn: str = ...,
    clientToken: str = ...,
    customDomainName: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateServiceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: CreateServiceResponseTypeDef](./type_defs.md#createserviceresponsetypedef) 


```python
# create_service method usage example with argument unpacking

kwargs: CreateServiceRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_service(**kwargs)
```

1. See [:material-code-braces: CreateServiceRequestRequestTypeDef](./type_defs.md#createservicerequestrequesttypedef) 

### create\_service\_network

Creates a service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_service_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network)

```python
# create_service_network method definition

await def create_service_network(
    self,
    *,
    name: str,
    authType: AuthTypeType = ...,  # (1)
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateServiceNetworkResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: CreateServiceNetworkResponseTypeDef](./type_defs.md#createservicenetworkresponsetypedef) 


```python
# create_service_network method usage example with argument unpacking

kwargs: CreateServiceNetworkRequestRequestTypeDef = {  # (1)
    "name": ...,
}

parent.create_service_network(**kwargs)
```

1. See [:material-code-braces: CreateServiceNetworkRequestRequestTypeDef](./type_defs.md#createservicenetworkrequestrequesttypedef) 

### create\_service\_network\_service\_association

Associates a service with a service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_service_network_service_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_service_association)

```python
# create_service_network_service_association method definition

await def create_service_network_service_association(
    self,
    *,
    serviceIdentifier: str,
    serviceNetworkIdentifier: str,
    clientToken: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateServiceNetworkServiceAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#createservicenetworkserviceassociationresponsetypedef) 


```python
# create_service_network_service_association method usage example with argument unpacking

kwargs: CreateServiceNetworkServiceAssociationRequestRequestTypeDef = {  # (1)
    "serviceIdentifier": ...,
    "serviceNetworkIdentifier": ...,
}

parent.create_service_network_service_association(**kwargs)
```

1. See [:material-code-braces: CreateServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#createservicenetworkserviceassociationrequestrequesttypedef) 

### create\_service\_network\_vpc\_association

Associates a VPC with a service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_service_network_vpc_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_service_network_vpc_association)

```python
# create_service_network_vpc_association method definition

await def create_service_network_vpc_association(
    self,
    *,
    serviceNetworkIdentifier: str,
    vpcIdentifier: str,
    clientToken: str = ...,
    securityGroupIds: Sequence[str] = ...,
    tags: Mapping[str, str] = ...,
) -> CreateServiceNetworkVpcAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#createservicenetworkvpcassociationresponsetypedef) 


```python
# create_service_network_vpc_association method usage example with argument unpacking

kwargs: CreateServiceNetworkVpcAssociationRequestRequestTypeDef = {  # (1)
    "serviceNetworkIdentifier": ...,
    "vpcIdentifier": ...,
}

parent.create_service_network_vpc_association(**kwargs)
```

1. See [:material-code-braces: CreateServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#createservicenetworkvpcassociationrequestrequesttypedef) 

### create\_target\_group

Creates a target group.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").create_target_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_target_group)

```python
# create_target_group method definition

await def create_target_group(
    self,
    *,
    name: str,
    type: TargetGroupTypeType,  # (1)
    clientToken: str = ...,
    config: TargetGroupConfigTypeDef = ...,  # (2)
    tags: Mapping[str, str] = ...,
) -> CreateTargetGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
2. See [:material-code-braces: TargetGroupConfigTypeDef](./type_defs.md#targetgroupconfigtypedef) 
3. See [:material-code-braces: CreateTargetGroupResponseTypeDef](./type_defs.md#createtargetgroupresponsetypedef) 


```python
# create_target_group method usage example with argument unpacking

kwargs: CreateTargetGroupRequestRequestTypeDef = {  # (1)
    "name": ...,
    "type": ...,
}

parent.create_target_group(**kwargs)
```

1. See [:material-code-braces: CreateTargetGroupRequestRequestTypeDef](./type_defs.md#createtargetgrouprequestrequesttypedef) 

### delete\_access\_log\_subscription

Deletes the specified access log subscription.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_access_log_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_access_log_subscription)

```python
# delete_access_log_subscription method definition

await def delete_access_log_subscription(
    self,
    *,
    accessLogSubscriptionIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_access_log_subscription method usage example with argument unpacking

kwargs: DeleteAccessLogSubscriptionRequestRequestTypeDef = {  # (1)
    "accessLogSubscriptionIdentifier": ...,
}

parent.delete_access_log_subscription(**kwargs)
```

1. See [:material-code-braces: DeleteAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#deleteaccesslogsubscriptionrequestrequesttypedef) 

### delete\_auth\_policy

Deletes the specified auth policy.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_auth_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_auth_policy)

```python
# delete_auth_policy method definition

await def delete_auth_policy(
    self,
    *,
    resourceIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_auth_policy method usage example with argument unpacking

kwargs: DeleteAuthPolicyRequestRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.delete_auth_policy(**kwargs)
```

1. See [:material-code-braces: DeleteAuthPolicyRequestRequestTypeDef](./type_defs.md#deleteauthpolicyrequestrequesttypedef) 

### delete\_listener

Deletes the specified listener.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_listener)

```python
# delete_listener method definition

await def delete_listener(
    self,
    *,
    listenerIdentifier: str,
    serviceIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_listener method usage example with argument unpacking

kwargs: DeleteListenerRequestRequestTypeDef = {  # (1)
    "listenerIdentifier": ...,
    "serviceIdentifier": ...,
}

parent.delete_listener(**kwargs)
```

1. See [:material-code-braces: DeleteListenerRequestRequestTypeDef](./type_defs.md#deletelistenerrequestrequesttypedef) 

### delete\_resource\_policy

Deletes the specified resource policy.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_resource_policy)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    resourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### delete\_rule

Deletes a listener rule.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_rule)

```python
# delete_rule method definition

await def delete_rule(
    self,
    *,
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_rule method usage example with argument unpacking

kwargs: DeleteRuleRequestRequestTypeDef = {  # (1)
    "listenerIdentifier": ...,
    "ruleIdentifier": ...,
    "serviceIdentifier": ...,
}

parent.delete_rule(**kwargs)
```

1. See [:material-code-braces: DeleteRuleRequestRequestTypeDef](./type_defs.md#deleterulerequestrequesttypedef) 

### delete\_service

Deletes a service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service)

```python
# delete_service method definition

await def delete_service(
    self,
    *,
    serviceIdentifier: str,
) -> DeleteServiceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceResponseTypeDef](./type_defs.md#deleteserviceresponsetypedef) 


```python
# delete_service method usage example with argument unpacking

kwargs: DeleteServiceRequestRequestTypeDef = {  # (1)
    "serviceIdentifier": ...,
}

parent.delete_service(**kwargs)
```

1. See [:material-code-braces: DeleteServiceRequestRequestTypeDef](./type_defs.md#deleteservicerequestrequesttypedef) 

### delete\_service\_network

Deletes a service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_service_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network)

```python
# delete_service_network method definition

await def delete_service_network(
    self,
    *,
    serviceNetworkIdentifier: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_service_network method usage example with argument unpacking

kwargs: DeleteServiceNetworkRequestRequestTypeDef = {  # (1)
    "serviceNetworkIdentifier": ...,
}

parent.delete_service_network(**kwargs)
```

1. See [:material-code-braces: DeleteServiceNetworkRequestRequestTypeDef](./type_defs.md#deleteservicenetworkrequestrequesttypedef) 

### delete\_service\_network\_service\_association

Deletes the association between a specified service and the specific service
network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_service_network_service_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network_service_association)

```python
# delete_service_network_service_association method definition

await def delete_service_network_service_association(
    self,
    *,
    serviceNetworkServiceAssociationIdentifier: str,
) -> DeleteServiceNetworkServiceAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#deleteservicenetworkserviceassociationresponsetypedef) 


```python
# delete_service_network_service_association method usage example with argument unpacking

kwargs: DeleteServiceNetworkServiceAssociationRequestRequestTypeDef = {  # (1)
    "serviceNetworkServiceAssociationIdentifier": ...,
}

parent.delete_service_network_service_association(**kwargs)
```

1. See [:material-code-braces: DeleteServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#deleteservicenetworkserviceassociationrequestrequesttypedef) 

### delete\_service\_network\_vpc\_association

Disassociates the VPC from the service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_service_network_vpc_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_service_network_vpc_association)

```python
# delete_service_network_vpc_association method definition

await def delete_service_network_vpc_association(
    self,
    *,
    serviceNetworkVpcAssociationIdentifier: str,
) -> DeleteServiceNetworkVpcAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#deleteservicenetworkvpcassociationresponsetypedef) 


```python
# delete_service_network_vpc_association method usage example with argument unpacking

kwargs: DeleteServiceNetworkVpcAssociationRequestRequestTypeDef = {  # (1)
    "serviceNetworkVpcAssociationIdentifier": ...,
}

parent.delete_service_network_vpc_association(**kwargs)
```

1. See [:material-code-braces: DeleteServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#deleteservicenetworkvpcassociationrequestrequesttypedef) 

### delete\_target\_group

Deletes a target group.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").delete_target_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.delete_target_group)

```python
# delete_target_group method definition

await def delete_target_group(
    self,
    *,
    targetGroupIdentifier: str,
) -> DeleteTargetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteTargetGroupResponseTypeDef](./type_defs.md#deletetargetgroupresponsetypedef) 


```python
# delete_target_group method usage example with argument unpacking

kwargs: DeleteTargetGroupRequestRequestTypeDef = {  # (1)
    "targetGroupIdentifier": ...,
}

parent.delete_target_group(**kwargs)
```

1. See [:material-code-braces: DeleteTargetGroupRequestRequestTypeDef](./type_defs.md#deletetargetgrouprequestrequesttypedef) 

### deregister\_targets

Deregisters the specified targets from the specified target group.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").deregister_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.deregister_targets)

```python
# deregister_targets method definition

await def deregister_targets(
    self,
    *,
    targetGroupIdentifier: str,
    targets: Sequence[TargetTypeDef],  # (1)
) -> DeregisterTargetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: DeregisterTargetsResponseTypeDef](./type_defs.md#deregistertargetsresponsetypedef) 


```python
# deregister_targets method usage example with argument unpacking

kwargs: DeregisterTargetsRequestRequestTypeDef = {  # (1)
    "targetGroupIdentifier": ...,
    "targets": ...,
}

parent.deregister_targets(**kwargs)
```

1. See [:material-code-braces: DeregisterTargetsRequestRequestTypeDef](./type_defs.md#deregistertargetsrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.generate_presigned_url)

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


### get\_access\_log\_subscription

Retrieves information about the specified access log subscription.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_access_log_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_access_log_subscription)

```python
# get_access_log_subscription method definition

await def get_access_log_subscription(
    self,
    *,
    accessLogSubscriptionIdentifier: str,
) -> GetAccessLogSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessLogSubscriptionResponseTypeDef](./type_defs.md#getaccesslogsubscriptionresponsetypedef) 


```python
# get_access_log_subscription method usage example with argument unpacking

kwargs: GetAccessLogSubscriptionRequestRequestTypeDef = {  # (1)
    "accessLogSubscriptionIdentifier": ...,
}

parent.get_access_log_subscription(**kwargs)
```

1. See [:material-code-braces: GetAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#getaccesslogsubscriptionrequestrequesttypedef) 

### get\_auth\_policy

Retrieves information about the auth policy for the specified service or
service
network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_auth_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_auth_policy)

```python
# get_auth_policy method definition

await def get_auth_policy(
    self,
    *,
    resourceIdentifier: str,
) -> GetAuthPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAuthPolicyResponseTypeDef](./type_defs.md#getauthpolicyresponsetypedef) 


```python
# get_auth_policy method usage example with argument unpacking

kwargs: GetAuthPolicyRequestRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.get_auth_policy(**kwargs)
```

1. See [:material-code-braces: GetAuthPolicyRequestRequestTypeDef](./type_defs.md#getauthpolicyrequestrequesttypedef) 

### get\_listener

Retrieves information about the specified listener for the specified service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_listener)

```python
# get_listener method definition

await def get_listener(
    self,
    *,
    listenerIdentifier: str,
    serviceIdentifier: str,
) -> GetListenerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetListenerResponseTypeDef](./type_defs.md#getlistenerresponsetypedef) 


```python
# get_listener method usage example with argument unpacking

kwargs: GetListenerRequestRequestTypeDef = {  # (1)
    "listenerIdentifier": ...,
    "serviceIdentifier": ...,
}

parent.get_listener(**kwargs)
```

1. See [:material-code-braces: GetListenerRequestRequestTypeDef](./type_defs.md#getlistenerrequestrequesttypedef) 

### get\_resource\_policy

Retrieves information about the resource policy.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_resource_policy)

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

kwargs: GetResourcePolicyRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.get_resource_policy(**kwargs)
```

1. See [:material-code-braces: GetResourcePolicyRequestRequestTypeDef](./type_defs.md#getresourcepolicyrequestrequesttypedef) 

### get\_rule

Retrieves information about listener rules.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_rule)

```python
# get_rule method definition

await def get_rule(
    self,
    *,
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
) -> GetRuleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRuleResponseTypeDef](./type_defs.md#getruleresponsetypedef) 


```python
# get_rule method usage example with argument unpacking

kwargs: GetRuleRequestRequestTypeDef = {  # (1)
    "listenerIdentifier": ...,
    "ruleIdentifier": ...,
    "serviceIdentifier": ...,
}

parent.get_rule(**kwargs)
```

1. See [:material-code-braces: GetRuleRequestRequestTypeDef](./type_defs.md#getrulerequestrequesttypedef) 

### get\_service

Retrieves information about the specified service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service)

```python
# get_service method definition

await def get_service(
    self,
    *,
    serviceIdentifier: str,
) -> GetServiceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceResponseTypeDef](./type_defs.md#getserviceresponsetypedef) 


```python
# get_service method usage example with argument unpacking

kwargs: GetServiceRequestRequestTypeDef = {  # (1)
    "serviceIdentifier": ...,
}

parent.get_service(**kwargs)
```

1. See [:material-code-braces: GetServiceRequestRequestTypeDef](./type_defs.md#getservicerequestrequesttypedef) 

### get\_service\_network

Retrieves information about the specified service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_service_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network)

```python
# get_service_network method definition

await def get_service_network(
    self,
    *,
    serviceNetworkIdentifier: str,
) -> GetServiceNetworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceNetworkResponseTypeDef](./type_defs.md#getservicenetworkresponsetypedef) 


```python
# get_service_network method usage example with argument unpacking

kwargs: GetServiceNetworkRequestRequestTypeDef = {  # (1)
    "serviceNetworkIdentifier": ...,
}

parent.get_service_network(**kwargs)
```

1. See [:material-code-braces: GetServiceNetworkRequestRequestTypeDef](./type_defs.md#getservicenetworkrequestrequesttypedef) 

### get\_service\_network\_service\_association

Retrieves information about the specified association between a service network
and a
service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_service_network_service_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network_service_association)

```python
# get_service_network_service_association method definition

await def get_service_network_service_association(
    self,
    *,
    serviceNetworkServiceAssociationIdentifier: str,
) -> GetServiceNetworkServiceAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceNetworkServiceAssociationResponseTypeDef](./type_defs.md#getservicenetworkserviceassociationresponsetypedef) 


```python
# get_service_network_service_association method usage example with argument unpacking

kwargs: GetServiceNetworkServiceAssociationRequestRequestTypeDef = {  # (1)
    "serviceNetworkServiceAssociationIdentifier": ...,
}

parent.get_service_network_service_association(**kwargs)
```

1. See [:material-code-braces: GetServiceNetworkServiceAssociationRequestRequestTypeDef](./type_defs.md#getservicenetworkserviceassociationrequestrequesttypedef) 

### get\_service\_network\_vpc\_association

Retrieves information about the association between a service network and a VPC.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_service_network_vpc_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_service_network_vpc_association)

```python
# get_service_network_vpc_association method definition

await def get_service_network_vpc_association(
    self,
    *,
    serviceNetworkVpcAssociationIdentifier: str,
) -> GetServiceNetworkVpcAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#getservicenetworkvpcassociationresponsetypedef) 


```python
# get_service_network_vpc_association method usage example with argument unpacking

kwargs: GetServiceNetworkVpcAssociationRequestRequestTypeDef = {  # (1)
    "serviceNetworkVpcAssociationIdentifier": ...,
}

parent.get_service_network_vpc_association(**kwargs)
```

1. See [:material-code-braces: GetServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#getservicenetworkvpcassociationrequestrequesttypedef) 

### get\_target\_group

Retrieves information about the specified target group.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_target_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.get_target_group)

```python
# get_target_group method definition

await def get_target_group(
    self,
    *,
    targetGroupIdentifier: str,
) -> GetTargetGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTargetGroupResponseTypeDef](./type_defs.md#gettargetgroupresponsetypedef) 


```python
# get_target_group method usage example with argument unpacking

kwargs: GetTargetGroupRequestRequestTypeDef = {  # (1)
    "targetGroupIdentifier": ...,
}

parent.get_target_group(**kwargs)
```

1. See [:material-code-braces: GetTargetGroupRequestRequestTypeDef](./type_defs.md#gettargetgrouprequestrequesttypedef) 

### list\_access\_log\_subscriptions

Lists all access log subscriptions for the specified service network or service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_access_log_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_access_log_subscriptions)

```python
# list_access_log_subscriptions method definition

await def list_access_log_subscriptions(
    self,
    *,
    resourceIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListAccessLogSubscriptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAccessLogSubscriptionsResponseTypeDef](./type_defs.md#listaccesslogsubscriptionsresponsetypedef) 


```python
# list_access_log_subscriptions method usage example with argument unpacking

kwargs: ListAccessLogSubscriptionsRequestRequestTypeDef = {  # (1)
    "resourceIdentifier": ...,
}

parent.list_access_log_subscriptions(**kwargs)
```

1. See [:material-code-braces: ListAccessLogSubscriptionsRequestRequestTypeDef](./type_defs.md#listaccesslogsubscriptionsrequestrequesttypedef) 

### list\_listeners

Lists the listeners for the specified service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_listeners` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_listeners)

```python
# list_listeners method definition

await def list_listeners(
    self,
    *,
    serviceIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListListenersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListListenersResponseTypeDef](./type_defs.md#listlistenersresponsetypedef) 


```python
# list_listeners method usage example with argument unpacking

kwargs: ListListenersRequestRequestTypeDef = {  # (1)
    "serviceIdentifier": ...,
}

parent.list_listeners(**kwargs)
```

1. See [:material-code-braces: ListListenersRequestRequestTypeDef](./type_defs.md#listlistenersrequestrequesttypedef) 

### list\_rules

Lists the rules for the listener.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_rules` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_rules)

```python
# list_rules method definition

await def list_rules(
    self,
    *,
    listenerIdentifier: str,
    serviceIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListRulesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef) 


```python
# list_rules method usage example with argument unpacking

kwargs: ListRulesRequestRequestTypeDef = {  # (1)
    "listenerIdentifier": ...,
    "serviceIdentifier": ...,
}

parent.list_rules(**kwargs)
```

1. See [:material-code-braces: ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef) 

### list\_service\_network\_service\_associations

Lists the associations between the service network and the service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_service_network_service_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_service_associations)

```python
# list_service_network_service_associations method definition

await def list_service_network_service_associations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    serviceIdentifier: str = ...,
    serviceNetworkIdentifier: str = ...,
) -> ListServiceNetworkServiceAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceNetworkServiceAssociationsResponseTypeDef](./type_defs.md#listservicenetworkserviceassociationsresponsetypedef) 


```python
# list_service_network_service_associations method usage example with argument unpacking

kwargs: ListServiceNetworkServiceAssociationsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_service_network_service_associations(**kwargs)
```

1. See [:material-code-braces: ListServiceNetworkServiceAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkserviceassociationsrequestrequesttypedef) 

### list\_service\_network\_vpc\_associations

Lists the service network and VPC associations.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_service_network_vpc_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_network_vpc_associations)

```python
# list_service_network_vpc_associations method definition

await def list_service_network_vpc_associations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    serviceNetworkIdentifier: str = ...,
    vpcIdentifier: str = ...,
) -> ListServiceNetworkVpcAssociationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceNetworkVpcAssociationsResponseTypeDef](./type_defs.md#listservicenetworkvpcassociationsresponsetypedef) 


```python
# list_service_network_vpc_associations method usage example with argument unpacking

kwargs: ListServiceNetworkVpcAssociationsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_service_network_vpc_associations(**kwargs)
```

1. See [:material-code-braces: ListServiceNetworkVpcAssociationsRequestRequestTypeDef](./type_defs.md#listservicenetworkvpcassociationsrequestrequesttypedef) 

### list\_service\_networks

Lists the service networks owned by the caller account or shared with the
caller
account.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_service_networks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_service_networks)

```python
# list_service_networks method definition

await def list_service_networks(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListServiceNetworksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceNetworksResponseTypeDef](./type_defs.md#listservicenetworksresponsetypedef) 


```python
# list_service_networks method usage example with argument unpacking

kwargs: ListServiceNetworksRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_service_networks(**kwargs)
```

1. See [:material-code-braces: ListServiceNetworksRequestRequestTypeDef](./type_defs.md#listservicenetworksrequestrequesttypedef) 

### list\_services

Lists the services owned by the caller account or shared with the caller
account.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_services)

```python
# list_services method definition

await def list_services(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListServicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServicesResponseTypeDef](./type_defs.md#listservicesresponsetypedef) 


```python
# list_services method usage example with argument unpacking

kwargs: ListServicesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_services(**kwargs)
```

1. See [:material-code-braces: ListServicesRequestRequestTypeDef](./type_defs.md#listservicesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags for the specified resource.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_tags_for_resource)

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

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_target\_groups

Lists your target groups.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_target_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_target_groups)

```python
# list_target_groups method definition

await def list_target_groups(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    targetGroupType: TargetGroupTypeType = ...,  # (1)
    vpcIdentifier: str = ...,
) -> ListTargetGroupsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: TargetGroupTypeType](./literals.md#targetgrouptypetype) 
2. See [:material-code-braces: ListTargetGroupsResponseTypeDef](./type_defs.md#listtargetgroupsresponsetypedef) 


```python
# list_target_groups method usage example with argument unpacking

kwargs: ListTargetGroupsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_target_groups(**kwargs)
```

1. See [:material-code-braces: ListTargetGroupsRequestRequestTypeDef](./type_defs.md#listtargetgroupsrequestrequesttypedef) 

### list\_targets

Lists the targets for the target group.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").list_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.list_targets)

```python
# list_targets method definition

await def list_targets(
    self,
    *,
    targetGroupIdentifier: str,
    maxResults: int = ...,
    nextToken: str = ...,
    targets: Sequence[TargetTypeDef] = ...,  # (1)
) -> ListTargetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: ListTargetsResponseTypeDef](./type_defs.md#listtargetsresponsetypedef) 


```python
# list_targets method usage example with argument unpacking

kwargs: ListTargetsRequestRequestTypeDef = {  # (1)
    "targetGroupIdentifier": ...,
}

parent.list_targets(**kwargs)
```

1. See [:material-code-braces: ListTargetsRequestRequestTypeDef](./type_defs.md#listtargetsrequestrequesttypedef) 

### put\_auth\_policy

Creates or updates the auth policy.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").put_auth_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.put_auth_policy)

```python
# put_auth_policy method definition

await def put_auth_policy(
    self,
    *,
    policy: str,
    resourceIdentifier: str,
) -> PutAuthPolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutAuthPolicyResponseTypeDef](./type_defs.md#putauthpolicyresponsetypedef) 


```python
# put_auth_policy method usage example with argument unpacking

kwargs: PutAuthPolicyRequestRequestTypeDef = {  # (1)
    "policy": ...,
    "resourceIdentifier": ...,
}

parent.put_auth_policy(**kwargs)
```

1. See [:material-code-braces: PutAuthPolicyRequestRequestTypeDef](./type_defs.md#putauthpolicyrequestrequesttypedef) 

### put\_resource\_policy

Attaches a resource-based permission policy to a service or service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.put_resource_policy)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    policy: str,
    resourceArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "policy": ...,
    "resourceArn": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### register\_targets

Registers the targets with the target group.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").register_targets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.register_targets)

```python
# register_targets method definition

await def register_targets(
    self,
    *,
    targetGroupIdentifier: str,
    targets: Sequence[TargetTypeDef],  # (1)
) -> RegisterTargetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
2. See [:material-code-braces: RegisterTargetsResponseTypeDef](./type_defs.md#registertargetsresponsetypedef) 


```python
# register_targets method usage example with argument unpacking

kwargs: RegisterTargetsRequestRequestTypeDef = {  # (1)
    "targetGroupIdentifier": ...,
    "targets": ...,
}

parent.register_targets(**kwargs)
```

1. See [:material-code-braces: RegisterTargetsRequestRequestTypeDef](./type_defs.md#registertargetsrequestrequesttypedef) 

### tag\_resource

Adds the specified tags to the specified resource.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes the specified tags from the specified resource.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_access\_log\_subscription

Updates the specified access log subscription.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").update_access_log_subscription` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)

```python
# update_access_log_subscription method definition

await def update_access_log_subscription(
    self,
    *,
    accessLogSubscriptionIdentifier: str,
    destinationArn: str,
) -> UpdateAccessLogSubscriptionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateAccessLogSubscriptionResponseTypeDef](./type_defs.md#updateaccesslogsubscriptionresponsetypedef) 


```python
# update_access_log_subscription method usage example with argument unpacking

kwargs: UpdateAccessLogSubscriptionRequestRequestTypeDef = {  # (1)
    "accessLogSubscriptionIdentifier": ...,
    "destinationArn": ...,
}

parent.update_access_log_subscription(**kwargs)
```

1. See [:material-code-braces: UpdateAccessLogSubscriptionRequestRequestTypeDef](./type_defs.md#updateaccesslogsubscriptionrequestrequesttypedef) 

### update\_listener

Updates the specified listener for the specified service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").update_listener` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)

```python
# update_listener method definition

await def update_listener(
    self,
    *,
    defaultAction: RuleActionTypeDef,  # (1)
    listenerIdentifier: str,
    serviceIdentifier: str,
) -> UpdateListenerResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: UpdateListenerResponseTypeDef](./type_defs.md#updatelistenerresponsetypedef) 


```python
# update_listener method usage example with argument unpacking

kwargs: UpdateListenerRequestRequestTypeDef = {  # (1)
    "defaultAction": ...,
    "listenerIdentifier": ...,
    "serviceIdentifier": ...,
}

parent.update_listener(**kwargs)
```

1. See [:material-code-braces: UpdateListenerRequestRequestTypeDef](./type_defs.md#updatelistenerrequestrequesttypedef) 

### update\_rule

Updates a rule for the listener.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").update_rule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)

```python
# update_rule method definition

await def update_rule(
    self,
    *,
    listenerIdentifier: str,
    ruleIdentifier: str,
    serviceIdentifier: str,
    action: RuleActionTypeDef = ...,  # (1)
    match: RuleMatchTypeDef = ...,  # (2)
    priority: int = ...,
) -> UpdateRuleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: RuleActionTypeDef](./type_defs.md#ruleactiontypedef) 
2. See [:material-code-braces: RuleMatchTypeDef](./type_defs.md#rulematchtypedef) 
3. See [:material-code-braces: UpdateRuleResponseTypeDef](./type_defs.md#updateruleresponsetypedef) 


```python
# update_rule method usage example with argument unpacking

kwargs: UpdateRuleRequestRequestTypeDef = {  # (1)
    "listenerIdentifier": ...,
    "ruleIdentifier": ...,
    "serviceIdentifier": ...,
}

parent.update_rule(**kwargs)
```

1. See [:material-code-braces: UpdateRuleRequestRequestTypeDef](./type_defs.md#updaterulerequestrequesttypedef) 

### update\_service

Updates the specified service.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").update_service` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service)

```python
# update_service method definition

await def update_service(
    self,
    *,
    serviceIdentifier: str,
    authType: AuthTypeType = ...,  # (1)
    certificateArn: str = ...,
) -> UpdateServiceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: UpdateServiceResponseTypeDef](./type_defs.md#updateserviceresponsetypedef) 


```python
# update_service method usage example with argument unpacking

kwargs: UpdateServiceRequestRequestTypeDef = {  # (1)
    "serviceIdentifier": ...,
}

parent.update_service(**kwargs)
```

1. See [:material-code-braces: UpdateServiceRequestRequestTypeDef](./type_defs.md#updateservicerequestrequesttypedef) 

### update\_service\_network

Updates the specified service network.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").update_service_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service_network)

```python
# update_service_network method definition

await def update_service_network(
    self,
    *,
    authType: AuthTypeType,  # (1)
    serviceNetworkIdentifier: str,
) -> UpdateServiceNetworkResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-braces: UpdateServiceNetworkResponseTypeDef](./type_defs.md#updateservicenetworkresponsetypedef) 


```python
# update_service_network method usage example with argument unpacking

kwargs: UpdateServiceNetworkRequestRequestTypeDef = {  # (1)
    "authType": ...,
    "serviceNetworkIdentifier": ...,
}

parent.update_service_network(**kwargs)
```

1. See [:material-code-braces: UpdateServiceNetworkRequestRequestTypeDef](./type_defs.md#updateservicenetworkrequestrequesttypedef) 

### update\_service\_network\_vpc\_association

Updates the service network and VPC association.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").update_service_network_vpc_association` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_service_network_vpc_association)

```python
# update_service_network_vpc_association method definition

await def update_service_network_vpc_association(
    self,
    *,
    securityGroupIds: Sequence[str],
    serviceNetworkVpcAssociationIdentifier: str,
) -> UpdateServiceNetworkVpcAssociationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServiceNetworkVpcAssociationResponseTypeDef](./type_defs.md#updateservicenetworkvpcassociationresponsetypedef) 


```python
# update_service_network_vpc_association method usage example with argument unpacking

kwargs: UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = {  # (1)
    "securityGroupIds": ...,
    "serviceNetworkVpcAssociationIdentifier": ...,
}

parent.update_service_network_vpc_association(**kwargs)
```

1. See [:material-code-braces: UpdateServiceNetworkVpcAssociationRequestRequestTypeDef](./type_defs.md#updateservicenetworkvpcassociationrequestrequesttypedef) 

### update\_target\_group

Updates the specified target group.

Type annotations and code completion for `#!python session.create_client("vpc-lattice").update_target_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_target_group)

```python
# update_target_group method definition

await def update_target_group(
    self,
    *,
    healthCheck: HealthCheckConfigTypeDef,  # (1)
    targetGroupIdentifier: str,
) -> UpdateTargetGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
2. See [:material-code-braces: UpdateTargetGroupResponseTypeDef](./type_defs.md#updatetargetgroupresponsetypedef) 


```python
# update_target_group method usage example with argument unpacking

kwargs: UpdateTargetGroupRequestRequestTypeDef = {  # (1)
    "healthCheck": ...,
    "targetGroupIdentifier": ...,
}

parent.update_target_group(**kwargs)
```

1. See [:material-code-braces: UpdateTargetGroupRequestRequestTypeDef](./type_defs.md#updatetargetgrouprequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("vpc-lattice").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "VPCLatticeClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("vpc-lattice").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("vpc-lattice").get_paginator` method with overloads.

- `client.get_paginator("list_access_log_subscriptions")` -> [ListAccessLogSubscriptionsPaginator](./paginators.md#listaccesslogsubscriptionspaginator)
- `client.get_paginator("list_listeners")` -> [ListListenersPaginator](./paginators.md#listlistenerspaginator)
- `client.get_paginator("list_rules")` -> [ListRulesPaginator](./paginators.md#listrulespaginator)
- `client.get_paginator("list_service_network_service_associations")` -> [ListServiceNetworkServiceAssociationsPaginator](./paginators.md#listservicenetworkserviceassociationspaginator)
- `client.get_paginator("list_service_network_vpc_associations")` -> [ListServiceNetworkVpcAssociationsPaginator](./paginators.md#listservicenetworkvpcassociationspaginator)
- `client.get_paginator("list_service_networks")` -> [ListServiceNetworksPaginator](./paginators.md#listservicenetworkspaginator)
- `client.get_paginator("list_services")` -> [ListServicesPaginator](./paginators.md#listservicespaginator)
- `client.get_paginator("list_target_groups")` -> [ListTargetGroupsPaginator](./paginators.md#listtargetgroupspaginator)
- `client.get_paginator("list_targets")` -> [ListTargetsPaginator](./paginators.md#listtargetspaginator)



