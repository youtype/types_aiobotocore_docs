<a id="typed-dictionaries-for-aiobotocore-ec2instanceconnect-module"></a>

# Typed dictionaries for aiobotocore EC2InstanceConnect module

> [Index](../README.md) > [EC2InstanceConnect](./README.md) > Typed
> dictionaries

Auto-generated documentation for
[EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
type annotations stubs module
[types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).

- [Typed dictionaries for aiobotocore EC2InstanceConnect module](#typed-dictionaries-for-aiobotocore-ec2instanceconnect-module)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [SendSSHPublicKeyRequestRequestTypeDef](#sendsshpublickeyrequestrequesttypedef)
  - [SendSSHPublicKeyResponseTypeDef](#sendsshpublickeyresponsetypedef)
  - [SendSerialConsoleSSHPublicKeyRequestRequestTypeDef](#sendserialconsolesshpublickeyrequestrequesttypedef)
  - [SendSerialConsoleSSHPublicKeyResponseTypeDef](#sendserialconsolesshpublickeyresponsetypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_ec2_instance_connect.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="sendsshpublickeyrequestrequesttypedef"></a>

## SendSSHPublicKeyRequestRequestTypeDef

```python
from types_aiobotocore_ec2_instance_connect.type_defs import SendSSHPublicKeyRequestRequestTypeDef
```

Required fields:

- `InstanceId`: `str`
- `InstanceOSUser`: `str`
- `SSHPublicKey`: `str`

Optional fields:

- `AvailabilityZone`: `str`

<a id="sendsshpublickeyresponsetypedef"></a>

## SendSSHPublicKeyResponseTypeDef

```python
from types_aiobotocore_ec2_instance_connect.type_defs import SendSSHPublicKeyResponseTypeDef
```

Required fields:

- `RequestId`: `str`
- `Success`: `bool`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="sendserialconsolesshpublickeyrequestrequesttypedef"></a>

## SendSerialConsoleSSHPublicKeyRequestRequestTypeDef

```python
from types_aiobotocore_ec2_instance_connect.type_defs import SendSerialConsoleSSHPublicKeyRequestRequestTypeDef
```

Required fields:

- `InstanceId`: `str`
- `SSHPublicKey`: `str`

Optional fields:

- `SerialPort`: `int`

<a id="sendserialconsolesshpublickeyresponsetypedef"></a>

## SendSerialConsoleSSHPublicKeyResponseTypeDef

```python
from types_aiobotocore_ec2_instance_connect.type_defs import SendSerialConsoleSSHPublicKeyResponseTypeDef
```

Required fields:

- `RequestId`: `str`
- `Success`: `bool`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
