# OpsWorksCMClient

> [Index](../README.md) > [OpsWorksCM](./README.md) > OpsWorksCMClient

!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#opsworkscm)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

## OpsWorksCMClient

Type annotations and code completion for `#!python session.create_client("opsworkscm")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client)

```python
# OpsWorksCMClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_opsworkscm.client import OpsWorksCMClient

session = get_session()
async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("opsworkscm").exceptions` structure.

```python
# OpsWorksCMClient.exceptions usage example

async with session.create_client("opsworkscm") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InvalidNextTokenException,
        client.InvalidStateException,
        client.LimitExceededException,
        client.ResourceAlreadyExistsException,
        client.ResourceNotFoundException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# OpsWorksCMClient usage type checking example

from types_aiobotocore_opsworkscm.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("opsworkscm").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("opsworkscm").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/generate_presigned_url.html)

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


### associate\_node

Associates a new node with the server.

Type annotations and code completion for `#!python session.create_client("opsworkscm").associate_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/associate_node.html)

```python
# associate_node method definition

await def associate_node(
    self,
    *,
    ServerName: str,
    NodeName: str,
    EngineAttributes: Sequence[EngineAttributeTypeDef],  # (1)
) -> AssociateNodeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-braces: AssociateNodeResponseTypeDef](./type_defs.md#associatenoderesponsetypedef) 


```python
# associate_node method usage example with argument unpacking

kwargs: AssociateNodeRequestTypeDef = {  # (1)
    "ServerName": ...,
    "NodeName": ...,
    "EngineAttributes": ...,
}

parent.associate_node(**kwargs)
```

1. See [:material-code-braces: AssociateNodeRequestTypeDef](./type_defs.md#associatenoderequesttypedef) 

### create\_backup

Creates an application-level backup of a server.

Type annotations and code completion for `#!python session.create_client("opsworkscm").create_backup` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/create_backup.html)

```python
# create_backup method definition

await def create_backup(
    self,
    *,
    ServerName: str,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> CreateBackupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateBackupResponseTypeDef](./type_defs.md#createbackupresponsetypedef) 


```python
# create_backup method usage example with argument unpacking

kwargs: CreateBackupRequestTypeDef = {  # (1)
    "ServerName": ...,
}

parent.create_backup(**kwargs)
```

1. See [:material-code-braces: CreateBackupRequestTypeDef](./type_defs.md#createbackuprequesttypedef) 

### create\_server

Creates and immedately starts a new server.

Type annotations and code completion for `#!python session.create_client("opsworkscm").create_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/create_server.html)

```python
# create_server method definition

await def create_server(
    self,
    *,
    Engine: str,
    ServerName: str,
    InstanceProfileArn: str,
    InstanceType: str,
    ServiceRoleArn: str,
    AssociatePublicIpAddress: bool = ...,
    CustomDomain: str = ...,
    CustomCertificate: str = ...,
    CustomPrivateKey: str = ...,
    DisableAutomatedBackup: bool = ...,
    EngineModel: str = ...,
    EngineVersion: str = ...,
    EngineAttributes: Sequence[EngineAttributeTypeDef] = ...,  # (1)
    BackupRetentionCount: int = ...,
    KeyPair: str = ...,
    PreferredMaintenanceWindow: str = ...,
    PreferredBackupWindow: str = ...,
    SecurityGroupIds: Sequence[str] = ...,
    SubnetIds: Sequence[str] = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    BackupId: str = ...,
) -> CreateServerResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateServerResponseTypeDef](./type_defs.md#createserverresponsetypedef) 


```python
# create_server method usage example with argument unpacking

kwargs: CreateServerRequestTypeDef = {  # (1)
    "Engine": ...,
    "ServerName": ...,
    "InstanceProfileArn": ...,
    "InstanceType": ...,
    "ServiceRoleArn": ...,
}

parent.create_server(**kwargs)
```

1. See [:material-code-braces: CreateServerRequestTypeDef](./type_defs.md#createserverrequesttypedef) 

### delete\_backup

Deletes a backup.

Type annotations and code completion for `#!python session.create_client("opsworkscm").delete_backup` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/delete_backup.html)

```python
# delete_backup method definition

await def delete_backup(
    self,
    *,
    BackupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_backup method usage example with argument unpacking

kwargs: DeleteBackupRequestTypeDef = {  # (1)
    "BackupId": ...,
}

parent.delete_backup(**kwargs)
```

1. See [:material-code-braces: DeleteBackupRequestTypeDef](./type_defs.md#deletebackuprequesttypedef) 

### delete\_server

Deletes the server and the underlying AWS CloudFormation stacks (including the
server's EC2 instance).

Type annotations and code completion for `#!python session.create_client("opsworkscm").delete_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/delete_server.html)

```python
# delete_server method definition

await def delete_server(
    self,
    *,
    ServerName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_server method usage example with argument unpacking

kwargs: DeleteServerRequestTypeDef = {  # (1)
    "ServerName": ...,
}

parent.delete_server(**kwargs)
```

1. See [:material-code-braces: DeleteServerRequestTypeDef](./type_defs.md#deleteserverrequesttypedef) 

### describe\_account\_attributes

Describes your OpsWorks-CM account attributes.

Type annotations and code completion for `#!python session.create_client("opsworkscm").describe_account_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/describe_account_attributes.html)

```python
# describe_account_attributes method definition

await def describe_account_attributes(
    self,
) -> DescribeAccountAttributesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountAttributesResponseTypeDef](./type_defs.md#describeaccountattributesresponsetypedef) 

### describe\_backups

Describes backups.

Type annotations and code completion for `#!python session.create_client("opsworkscm").describe_backups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/describe_backups.html)

```python
# describe_backups method definition

await def describe_backups(
    self,
    *,
    BackupId: str = ...,
    ServerName: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeBackupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef) 


```python
# describe_backups method usage example with argument unpacking

kwargs: DescribeBackupsRequestTypeDef = {  # (1)
    "BackupId": ...,
}

parent.describe_backups(**kwargs)
```

1. See [:material-code-braces: DescribeBackupsRequestTypeDef](./type_defs.md#describebackupsrequesttypedef) 

### describe\_events

Describes events for a specified server.

Type annotations and code completion for `#!python session.create_client("opsworkscm").describe_events` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/describe_events.html)

```python
# describe_events method definition

await def describe_events(
    self,
    *,
    ServerName: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeEventsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python
# describe_events method usage example with argument unpacking

kwargs: DescribeEventsRequestTypeDef = {  # (1)
    "ServerName": ...,
}

parent.describe_events(**kwargs)
```

1. See [:material-code-braces: DescribeEventsRequestTypeDef](./type_defs.md#describeeventsrequesttypedef) 

### describe\_node\_association\_status

Returns the current status of an existing association or disassociation request.

Type annotations and code completion for `#!python session.create_client("opsworkscm").describe_node_association_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/describe_node_association_status.html)

```python
# describe_node_association_status method definition

await def describe_node_association_status(
    self,
    *,
    NodeAssociationStatusToken: str,
    ServerName: str,
) -> DescribeNodeAssociationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNodeAssociationStatusResponseTypeDef](./type_defs.md#describenodeassociationstatusresponsetypedef) 


```python
# describe_node_association_status method usage example with argument unpacking

kwargs: DescribeNodeAssociationStatusRequestTypeDef = {  # (1)
    "NodeAssociationStatusToken": ...,
    "ServerName": ...,
}

parent.describe_node_association_status(**kwargs)
```

1. See [:material-code-braces: DescribeNodeAssociationStatusRequestTypeDef](./type_defs.md#describenodeassociationstatusrequesttypedef) 

### describe\_servers

Lists all configuration management servers that are identified with your
account.

Type annotations and code completion for `#!python session.create_client("opsworkscm").describe_servers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/describe_servers.html)

```python
# describe_servers method definition

await def describe_servers(
    self,
    *,
    ServerName: str = ...,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> DescribeServersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServersResponseTypeDef](./type_defs.md#describeserversresponsetypedef) 


```python
# describe_servers method usage example with argument unpacking

kwargs: DescribeServersRequestTypeDef = {  # (1)
    "ServerName": ...,
}

parent.describe_servers(**kwargs)
```

1. See [:material-code-braces: DescribeServersRequestTypeDef](./type_defs.md#describeserversrequesttypedef) 

### disassociate\_node

Disassociates a node from an AWS OpsWorks CM server, and removes the node from
the server's managed nodes.

Type annotations and code completion for `#!python session.create_client("opsworkscm").disassociate_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/disassociate_node.html)

```python
# disassociate_node method definition

await def disassociate_node(
    self,
    *,
    ServerName: str,
    NodeName: str,
    EngineAttributes: Sequence[EngineAttributeTypeDef] = ...,  # (1)
) -> DisassociateNodeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-braces: DisassociateNodeResponseTypeDef](./type_defs.md#disassociatenoderesponsetypedef) 


```python
# disassociate_node method usage example with argument unpacking

kwargs: DisassociateNodeRequestTypeDef = {  # (1)
    "ServerName": ...,
    "NodeName": ...,
}

parent.disassociate_node(**kwargs)
```

1. See [:material-code-braces: DisassociateNodeRequestTypeDef](./type_defs.md#disassociatenoderequesttypedef) 

### export\_server\_engine\_attribute

Exports a specified server engine attribute as a base64-encoded string.

Type annotations and code completion for `#!python session.create_client("opsworkscm").export_server_engine_attribute` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/export_server_engine_attribute.html)

```python
# export_server_engine_attribute method definition

await def export_server_engine_attribute(
    self,
    *,
    ExportAttributeName: str,
    ServerName: str,
    InputAttributes: Sequence[EngineAttributeTypeDef] = ...,  # (1)
) -> ExportServerEngineAttributeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-braces: ExportServerEngineAttributeResponseTypeDef](./type_defs.md#exportserverengineattributeresponsetypedef) 


```python
# export_server_engine_attribute method usage example with argument unpacking

kwargs: ExportServerEngineAttributeRequestTypeDef = {  # (1)
    "ExportAttributeName": ...,
    "ServerName": ...,
}

parent.export_server_engine_attribute(**kwargs)
```

1. See [:material-code-braces: ExportServerEngineAttributeRequestTypeDef](./type_defs.md#exportserverengineattributerequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags that are applied to the specified AWS OpsWorks for Chef
Automate or AWS OpsWorks for Puppet Enterprise servers or backups.

Type annotations and code completion for `#!python session.create_client("opsworkscm").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### restore\_server

Restores a backup to a server that is in a <code>CONNECTION_LOST</code>,
<code>HEALTHY</code>, <code>RUNNING</code>, <code>UNHEALTHY</code>, or
<code>TERMINATED</code> state.

Type annotations and code completion for `#!python session.create_client("opsworkscm").restore_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/restore_server.html)

```python
# restore_server method definition

await def restore_server(
    self,
    *,
    BackupId: str,
    ServerName: str,
    InstanceType: str = ...,
    KeyPair: str = ...,
) -> RestoreServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RestoreServerResponseTypeDef](./type_defs.md#restoreserverresponsetypedef) 


```python
# restore_server method usage example with argument unpacking

kwargs: RestoreServerRequestTypeDef = {  # (1)
    "BackupId": ...,
    "ServerName": ...,
}

parent.restore_server(**kwargs)
```

1. See [:material-code-braces: RestoreServerRequestTypeDef](./type_defs.md#restoreserverrequesttypedef) 

### start\_maintenance

Manually starts server maintenance.

Type annotations and code completion for `#!python session.create_client("opsworkscm").start_maintenance` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/start_maintenance.html)

```python
# start_maintenance method definition

await def start_maintenance(
    self,
    *,
    ServerName: str,
    EngineAttributes: Sequence[EngineAttributeTypeDef] = ...,  # (1)
) -> StartMaintenanceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngineAttributeTypeDef](./type_defs.md#engineattributetypedef) 
2. See [:material-code-braces: StartMaintenanceResponseTypeDef](./type_defs.md#startmaintenanceresponsetypedef) 


```python
# start_maintenance method usage example with argument unpacking

kwargs: StartMaintenanceRequestTypeDef = {  # (1)
    "ServerName": ...,
}

parent.start_maintenance(**kwargs)
```

1. See [:material-code-braces: StartMaintenanceRequestTypeDef](./type_defs.md#startmaintenancerequesttypedef) 

### tag\_resource

Applies tags to an AWS OpsWorks for Chef Automate or AWS OpsWorks for Puppet
Enterprise server, or to server backups.

Type annotations and code completion for `#!python session.create_client("opsworkscm").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes specified tags from an AWS OpsWorks-CM server or backup.

Type annotations and code completion for `#!python session.create_client("opsworkscm").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/untag_resource.html)

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

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_server

Updates settings for a server.

Type annotations and code completion for `#!python session.create_client("opsworkscm").update_server` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/update_server.html)

```python
# update_server method definition

await def update_server(
    self,
    *,
    ServerName: str,
    DisableAutomatedBackup: bool = ...,
    BackupRetentionCount: int = ...,
    PreferredMaintenanceWindow: str = ...,
    PreferredBackupWindow: str = ...,
) -> UpdateServerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServerResponseTypeDef](./type_defs.md#updateserverresponsetypedef) 


```python
# update_server method usage example with argument unpacking

kwargs: UpdateServerRequestTypeDef = {  # (1)
    "ServerName": ...,
}

parent.update_server(**kwargs)
```

1. See [:material-code-braces: UpdateServerRequestTypeDef](./type_defs.md#updateserverrequesttypedef) 

### update\_server\_engine\_attributes

Updates engine-specific attributes on a specified server.

Type annotations and code completion for `#!python session.create_client("opsworkscm").update_server_engine_attributes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm/client/update_server_engine_attributes.html)

```python
# update_server_engine_attributes method definition

await def update_server_engine_attributes(
    self,
    *,
    ServerName: str,
    AttributeName: str,
    AttributeValue: str = ...,
) -> UpdateServerEngineAttributesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateServerEngineAttributesResponseTypeDef](./type_defs.md#updateserverengineattributesresponsetypedef) 


```python
# update_server_engine_attributes method usage example with argument unpacking

kwargs: UpdateServerEngineAttributesRequestTypeDef = {  # (1)
    "ServerName": ...,
    "AttributeName": ...,
}

parent.update_server_engine_attributes(**kwargs)
```

1. See [:material-code-braces: UpdateServerEngineAttributesRequestTypeDef](./type_defs.md#updateserverengineattributesrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("opsworkscm").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("opsworkscm").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client)

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

Type annotations and code completion for `#!python session.create_client("opsworkscm").get_paginator` method with overloads.

- `client.get_paginator("describe_backups")` -> [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
- `client.get_paginator("describe_events")` -> [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- `client.get_paginator("describe_servers")` -> [DescribeServersPaginator](./paginators.md#describeserverspaginator)
- `client.get_paginator("list_tags_for_resource")` -> [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("opsworkscm").get_waiter` method with overloads.

- `client.get_waiter("node_associated")` -> [NodeAssociatedWaiter](./waiters.md#nodeassociatedwaiter)

