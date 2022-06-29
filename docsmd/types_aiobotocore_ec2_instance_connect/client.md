# EC2InstanceConnectClient

> [Index](../README.md) > [EC2InstanceConnect](./README.md) > EC2InstanceConnectClient

!!! note ""

    Auto-generated documentation for [EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
    type annotations stubs module [types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).

## EC2InstanceConnectClient

Type annotations and code completion for `#!python session.create_client("ec2-instance-connect")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_ec2_instance_connect.client import EC2InstanceConnectClient

session = get_session()
async with session.create_client("ec2-instance-connect") as client:
    client: EC2InstanceConnectClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("ec2-instance-connect").exceptions` structure.

```python title="Usage example"
async with session.create_client("ec2-instance-connect") as client:
    try:
        do_something(client)
    except (
            client.AuthException,
        client.ClientError,
        client.EC2InstanceNotFoundException,
        client.EC2InstanceStateInvalidException,
        client.EC2InstanceTypeInvalidException,
        client.InvalidArgsException,
        client.SerialConsoleAccessDisabledException,
        client.SerialConsoleSessionLimitExceededException,
        client.SerialConsoleSessionUnavailableException,
        client.ServiceException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_ec2_instance_connect.client import Exceptions

def handle_error(exc: Exceptions.AuthException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("ec2-instance-connect").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("ec2-instance-connect").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("ec2-instance-connect").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### send\_serial\_console\_ssh\_public\_key

Pushes an SSH public key to the specified EC2 instance.

Type annotations and code completion for `#!python session.create_client("ec2-instance-connect").send_serial_console_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.send_serial_console_ssh_public_key)

```python title="Method definition"
await def send_serial_console_ssh_public_key(
    self,
    *,
    InstanceId: str,
    SSHPublicKey: str,
    SerialPort: int = ...,
) -> SendSerialConsoleSSHPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendSerialConsoleSSHPublicKeyResponseTypeDef](./type_defs.md#sendserialconsolesshpublickeyresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SendSerialConsoleSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "SSHPublicKey": ...,
}

parent.send_serial_console_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: SendSerialConsoleSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendserialconsolesshpublickeyrequestrequesttypedef) 

### send\_ssh\_public\_key

Pushes an SSH public key to the specified EC2 instance for use by the specified
user.

Type annotations and code completion for `#!python session.create_client("ec2-instance-connect").send_ssh_public_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.send_ssh_public_key)

```python title="Method definition"
await def send_ssh_public_key(
    self,
    *,
    InstanceId: str,
    InstanceOSUser: str,
    SSHPublicKey: str,
    AvailabilityZone: str = ...,
) -> SendSSHPublicKeyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SendSSHPublicKeyResponseTypeDef](./type_defs.md#sendsshpublickeyresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: SendSSHPublicKeyRequestRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "InstanceOSUser": ...,
    "SSHPublicKey": ...,
}

parent.send_ssh_public_key(**kwargs)
```

1. See [:material-code-braces: SendSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendsshpublickeyrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("ec2-instance-connect").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> EC2InstanceConnectClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("ec2-instance-connect").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```





