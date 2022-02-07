<a id="type-annotations-for-aiobotocore-ec2instanceconnect-module"></a>

# Type annotations for aiobotocore EC2InstanceConnect module

> [Index](..) > EC2InstanceConnect

Auto-generated documentation for
[EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
type annotations stubs module
[types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[ec2-instance-connect]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ec2-instance-connect]'

# standalone installation
pip install types-aiobotocore-ec2-instance-connect
```

- [Type annotations for aiobotocore EC2InstanceConnect module](#type-annotations-for-aiobotocore-ec2instanceconnect-module)
  - [EC2InstanceConnectClient](#ec2instanceconnectclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="ec2instanceconnectclient"></a>

## EC2InstanceConnectClient

Type annotations for `session.create_client("ec2-instance-connect")` as
[EC2InstanceConnectClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_ec2_instance_connect.client import EC2InstanceConnectClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [send_serial_console_ssh_public_key](./client.md#send_serial_console_ssh_public_key)
- [send_ssh_public_key](./client.md#send_ssh_public_key)

<a id="exceptions"></a>

### Exceptions

EC2InstanceConnectClient [exceptions](./client.md#exceptions)

- AuthException
- ClientError
- EC2InstanceNotFoundException
- EC2InstanceTypeInvalidException
- InvalidArgsException
- SerialConsoleAccessDisabledException
- SerialConsoleSessionLimitExceededException
- SerialConsoleSessionUnavailableException
- ServiceException
- ThrottlingException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_ec2_instance_connect.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_ec2_instance_connect.type_defs import ResponseMetadataTypeDef, ...
```

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SendSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendsshpublickeyrequestrequesttypedef)
- [SendSSHPublicKeyResponseTypeDef](./type_defs.md#sendsshpublickeyresponsetypedef)
- [SendSerialConsoleSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendserialconsolesshpublickeyrequestrequesttypedef)
- [SendSerialConsoleSSHPublicKeyResponseTypeDef](./type_defs.md#sendserialconsolesshpublickeyresponsetypedef)
