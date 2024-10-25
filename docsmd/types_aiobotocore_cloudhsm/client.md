# CloudHSMClient

> [Index](../README.md) > [CloudHSM](./README.md) > CloudHSMClient

!!! note ""

    Auto-generated documentation for [CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
    type annotations stubs module [types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).

## CloudHSMClient

Type annotations and code completion for `#!python session.create_client("cloudhsm")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client)

```python
# CloudHSMClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cloudhsm.client import CloudHSMClient

session = get_session()
async with session.create_client("cloudhsm") as client:
    client: CloudHSMClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudhsm").exceptions` structure.

```python
# CloudHSMClient.exceptions usage example

async with session.create_client("cloudhsm") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.CloudHsmInternalException,
        client.CloudHsmServiceException,
        client.InvalidRequestException,
    ) as e:
        print(e)
```

```python
# CloudHSMClient usage type checking example

from types_aiobotocore_cloudhsm.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### add\_tags\_to\_resource

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").add_tags_to_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.add_tags_to_resource)

```python
# add_tags_to_resource method definition

await def add_tags_to_resource(
    self,
    *,
    ResourceArn: str,
    TagList: Sequence[TagTypeDef],  # (1)
) -> AddTagsToResourceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: AddTagsToResourceResponseTypeDef](./type_defs.md#addtagstoresourceresponsetypedef) 


```python
# add_tags_to_resource method usage example with argument unpacking

kwargs: AddTagsToResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagList": ...,
}

parent.add_tags_to_resource(**kwargs)
```

1. See [:material-code-braces: AddTagsToResourceRequestRequestTypeDef](./type_defs.md#addtagstoresourcerequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cloudhsm").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("cloudhsm").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").create_hapg` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_hapg)

```python
# create_hapg method definition

await def create_hapg(
    self,
    *,
    Label: str,
) -> CreateHapgResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateHapgResponseTypeDef](./type_defs.md#createhapgresponsetypedef) 


```python
# create_hapg method usage example with argument unpacking

kwargs: CreateHapgRequestRequestTypeDef = {  # (1)
    "Label": ...,
}

parent.create_hapg(**kwargs)
```

1. See [:material-code-braces: CreateHapgRequestRequestTypeDef](./type_defs.md#createhapgrequestrequesttypedef) 

### create\_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").create_hsm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_hsm)

```python
# create_hsm method definition

await def create_hsm(
    self,
    *,
    SubnetId: str,
    SshKey: str,
    IamRoleArn: str,
    SubscriptionType: SubscriptionTypeType,  # (1)
    EniIp: str = ...,
    ExternalId: str = ...,
    ClientToken: str = ...,
    SyslogIp: str = ...,
) -> CreateHsmResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SubscriptionTypeType](./literals.md#subscriptiontypetype) 
2. See [:material-code-braces: CreateHsmResponseTypeDef](./type_defs.md#createhsmresponsetypedef) 


```python
# create_hsm method usage example with argument unpacking

kwargs: CreateHsmRequestRequestTypeDef = {  # (1)
    "SubnetId": ...,
    "SshKey": ...,
    "IamRoleArn": ...,
    "SubscriptionType": ...,
}

parent.create_hsm(**kwargs)
```

1. See [:material-code-braces: CreateHsmRequestRequestTypeDef](./type_defs.md#createhsmrequestrequesttypedef) 

### create\_luna\_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").create_luna_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_luna_client)

```python
# create_luna_client method definition

await def create_luna_client(
    self,
    *,
    Certificate: str,
    Label: str = ...,
) -> CreateLunaClientResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateLunaClientResponseTypeDef](./type_defs.md#createlunaclientresponsetypedef) 


```python
# create_luna_client method usage example with argument unpacking

kwargs: CreateLunaClientRequestRequestTypeDef = {  # (1)
    "Certificate": ...,
}

parent.create_luna_client(**kwargs)
```

1. See [:material-code-braces: CreateLunaClientRequestRequestTypeDef](./type_defs.md#createlunaclientrequestrequesttypedef) 

### delete\_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").delete_hapg` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.delete_hapg)

```python
# delete_hapg method definition

await def delete_hapg(
    self,
    *,
    HapgArn: str,
) -> DeleteHapgResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteHapgResponseTypeDef](./type_defs.md#deletehapgresponsetypedef) 


```python
# delete_hapg method usage example with argument unpacking

kwargs: DeleteHapgRequestRequestTypeDef = {  # (1)
    "HapgArn": ...,
}

parent.delete_hapg(**kwargs)
```

1. See [:material-code-braces: DeleteHapgRequestRequestTypeDef](./type_defs.md#deletehapgrequestrequesttypedef) 

### delete\_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").delete_hsm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.delete_hsm)

```python
# delete_hsm method definition

await def delete_hsm(
    self,
    *,
    HsmArn: str,
) -> DeleteHsmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteHsmResponseTypeDef](./type_defs.md#deletehsmresponsetypedef) 


```python
# delete_hsm method usage example with argument unpacking

kwargs: DeleteHsmRequestRequestTypeDef = {  # (1)
    "HsmArn": ...,
}

parent.delete_hsm(**kwargs)
```

1. See [:material-code-braces: DeleteHsmRequestRequestTypeDef](./type_defs.md#deletehsmrequestrequesttypedef) 

### delete\_luna\_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").delete_luna_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.delete_luna_client)

```python
# delete_luna_client method definition

await def delete_luna_client(
    self,
    *,
    ClientArn: str,
) -> DeleteLunaClientResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteLunaClientResponseTypeDef](./type_defs.md#deletelunaclientresponsetypedef) 


```python
# delete_luna_client method usage example with argument unpacking

kwargs: DeleteLunaClientRequestRequestTypeDef = {  # (1)
    "ClientArn": ...,
}

parent.delete_luna_client(**kwargs)
```

1. See [:material-code-braces: DeleteLunaClientRequestRequestTypeDef](./type_defs.md#deletelunaclientrequestrequesttypedef) 

### describe\_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").describe_hapg` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.describe_hapg)

```python
# describe_hapg method definition

await def describe_hapg(
    self,
    *,
    HapgArn: str,
) -> DescribeHapgResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHapgResponseTypeDef](./type_defs.md#describehapgresponsetypedef) 


```python
# describe_hapg method usage example with argument unpacking

kwargs: DescribeHapgRequestRequestTypeDef = {  # (1)
    "HapgArn": ...,
}

parent.describe_hapg(**kwargs)
```

1. See [:material-code-braces: DescribeHapgRequestRequestTypeDef](./type_defs.md#describehapgrequestrequesttypedef) 

### describe\_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").describe_hsm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.describe_hsm)

```python
# describe_hsm method definition

await def describe_hsm(
    self,
    *,
    HsmArn: str = ...,
    HsmSerialNumber: str = ...,
) -> DescribeHsmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeHsmResponseTypeDef](./type_defs.md#describehsmresponsetypedef) 


```python
# describe_hsm method usage example with argument unpacking

kwargs: DescribeHsmRequestRequestTypeDef = {  # (1)
    "HsmArn": ...,
}

parent.describe_hsm(**kwargs)
```

1. See [:material-code-braces: DescribeHsmRequestRequestTypeDef](./type_defs.md#describehsmrequestrequesttypedef) 

### describe\_luna\_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").describe_luna_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.describe_luna_client)

```python
# describe_luna_client method definition

await def describe_luna_client(
    self,
    *,
    ClientArn: str = ...,
    CertificateFingerprint: str = ...,
) -> DescribeLunaClientResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeLunaClientResponseTypeDef](./type_defs.md#describelunaclientresponsetypedef) 


```python
# describe_luna_client method usage example with argument unpacking

kwargs: DescribeLunaClientRequestRequestTypeDef = {  # (1)
    "ClientArn": ...,
}

parent.describe_luna_client(**kwargs)
```

1. See [:material-code-braces: DescribeLunaClientRequestRequestTypeDef](./type_defs.md#describelunaclientrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cloudhsm").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.generate_presigned_url)

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


### get\_config

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.get_config)

```python
# get_config method definition

await def get_config(
    self,
    *,
    ClientArn: str,
    ClientVersion: ClientVersionType,  # (1)
    HapgList: Sequence[str],
) -> GetConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ClientVersionType](./literals.md#clientversiontype) 
2. See [:material-code-braces: GetConfigResponseTypeDef](./type_defs.md#getconfigresponsetypedef) 


```python
# get_config method usage example with argument unpacking

kwargs: GetConfigRequestRequestTypeDef = {  # (1)
    "ClientArn": ...,
    "ClientVersion": ...,
    "HapgList": ...,
}

parent.get_config(**kwargs)
```

1. See [:material-code-braces: GetConfigRequestRequestTypeDef](./type_defs.md#getconfigrequestrequesttypedef) 

### list\_available\_zones

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").list_available_zones` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_available_zones)

```python
# list_available_zones method definition

await def list_available_zones(
    self,
) -> ListAvailableZonesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListAvailableZonesResponseTypeDef](./type_defs.md#listavailablezonesresponsetypedef) 

### list\_hapgs

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").list_hapgs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_hapgs)

```python
# list_hapgs method definition

await def list_hapgs(
    self,
    *,
    NextToken: str = ...,
) -> ListHapgsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef) 


```python
# list_hapgs method usage example with argument unpacking

kwargs: ListHapgsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_hapgs(**kwargs)
```

1. See [:material-code-braces: ListHapgsRequestRequestTypeDef](./type_defs.md#listhapgsrequestrequesttypedef) 

### list\_hsms

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").list_hsms` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_hsms)

```python
# list_hsms method definition

await def list_hsms(
    self,
    *,
    NextToken: str = ...,
) -> ListHsmsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListHsmsResponseTypeDef](./type_defs.md#listhsmsresponsetypedef) 


```python
# list_hsms method usage example with argument unpacking

kwargs: ListHsmsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_hsms(**kwargs)
```

1. See [:material-code-braces: ListHsmsRequestRequestTypeDef](./type_defs.md#listhsmsrequestrequesttypedef) 

### list\_luna\_clients

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").list_luna_clients` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_luna_clients)

```python
# list_luna_clients method definition

await def list_luna_clients(
    self,
    *,
    NextToken: str = ...,
) -> ListLunaClientsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListLunaClientsResponseTypeDef](./type_defs.md#listlunaclientsresponsetypedef) 


```python
# list_luna_clients method usage example with argument unpacking

kwargs: ListLunaClientsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_luna_clients(**kwargs)
```

1. See [:material-code-braces: ListLunaClientsRequestRequestTypeDef](./type_defs.md#listlunaclientsrequestrequesttypedef) 

### list\_tags\_for\_resource

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_tags_for_resource)

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

### modify\_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").modify_hapg` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_hapg)

```python
# modify_hapg method definition

await def modify_hapg(
    self,
    *,
    HapgArn: str,
    Label: str = ...,
    PartitionSerialList: Sequence[str] = ...,
) -> ModifyHapgResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyHapgResponseTypeDef](./type_defs.md#modifyhapgresponsetypedef) 


```python
# modify_hapg method usage example with argument unpacking

kwargs: ModifyHapgRequestRequestTypeDef = {  # (1)
    "HapgArn": ...,
}

parent.modify_hapg(**kwargs)
```

1. See [:material-code-braces: ModifyHapgRequestRequestTypeDef](./type_defs.md#modifyhapgrequestrequesttypedef) 

### modify\_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").modify_hsm` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_hsm)

```python
# modify_hsm method definition

await def modify_hsm(
    self,
    *,
    HsmArn: str,
    SubnetId: str = ...,
    EniIp: str = ...,
    IamRoleArn: str = ...,
    ExternalId: str = ...,
    SyslogIp: str = ...,
) -> ModifyHsmResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyHsmResponseTypeDef](./type_defs.md#modifyhsmresponsetypedef) 


```python
# modify_hsm method usage example with argument unpacking

kwargs: ModifyHsmRequestRequestTypeDef = {  # (1)
    "HsmArn": ...,
}

parent.modify_hsm(**kwargs)
```

1. See [:material-code-braces: ModifyHsmRequestRequestTypeDef](./type_defs.md#modifyhsmrequestrequesttypedef) 

### modify\_luna\_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").modify_luna_client` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_luna_client)

```python
# modify_luna_client method definition

await def modify_luna_client(
    self,
    *,
    ClientArn: str,
    Certificate: str,
) -> ModifyLunaClientResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ModifyLunaClientResponseTypeDef](./type_defs.md#modifylunaclientresponsetypedef) 


```python
# modify_luna_client method usage example with argument unpacking

kwargs: ModifyLunaClientRequestRequestTypeDef = {  # (1)
    "ClientArn": ...,
    "Certificate": ...,
}

parent.modify_luna_client(**kwargs)
```

1. See [:material-code-braces: ModifyLunaClientRequestRequestTypeDef](./type_defs.md#modifylunaclientrequestrequesttypedef) 

### remove\_tags\_from\_resource

This is documentation for **AWS CloudHSM Classic**.

Type annotations and code completion for `#!python session.create_client("cloudhsm").remove_tags_from_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.remove_tags_from_resource)

```python
# remove_tags_from_resource method definition

await def remove_tags_from_resource(
    self,
    *,
    ResourceArn: str,
    TagKeyList: Sequence[str],
) -> RemoveTagsFromResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RemoveTagsFromResourceResponseTypeDef](./type_defs.md#removetagsfromresourceresponsetypedef) 


```python
# remove_tags_from_resource method usage example with argument unpacking

kwargs: RemoveTagsFromResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeyList": ...,
}

parent.remove_tags_from_resource(**kwargs)
```

1. See [:material-code-braces: RemoveTagsFromResourceRequestRequestTypeDef](./type_defs.md#removetagsfromresourcerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudhsm").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "CloudHSMClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudhsm").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("cloudhsm").get_paginator` method with overloads.

- `client.get_paginator("list_hapgs")` -> [ListHapgsPaginator](./paginators.md#listhapgspaginator)
- `client.get_paginator("list_hsms")` -> [ListHsmsPaginator](./paginators.md#listhsmspaginator)
- `client.get_paginator("list_luna_clients")` -> [ListLunaClientsPaginator](./paginators.md#listlunaclientspaginator)



