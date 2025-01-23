# Type definitions

> [Index](../README.md) > [EC2InstanceConnect](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#ec2instanceconnect)
    type annotations stubs module [types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).



## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## SendSSHPublicKeyRequestRequestTypeDef

```python
# SendSSHPublicKeyRequestRequestTypeDef definition

class SendSSHPublicKeyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    InstanceOSUser: str,
    SSHPublicKey: str,
    AvailabilityZone: NotRequired[str],
```

## SendSerialConsoleSSHPublicKeyRequestRequestTypeDef

```python
# SendSerialConsoleSSHPublicKeyRequestRequestTypeDef definition

class SendSerialConsoleSSHPublicKeyRequestRequestTypeDef(TypedDict):
    InstanceId: str,
    SSHPublicKey: str,
    SerialPort: NotRequired[int],
```

## SendSSHPublicKeyResponseTypeDef

```python
# SendSSHPublicKeyResponseTypeDef definition

class SendSSHPublicKeyResponseTypeDef(TypedDict):
    RequestId: str,
    Success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendSerialConsoleSSHPublicKeyResponseTypeDef

```python
# SendSerialConsoleSSHPublicKeyResponseTypeDef definition

class SendSerialConsoleSSHPublicKeyResponseTypeDef(TypedDict):
    RequestId: str,
    Success: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
