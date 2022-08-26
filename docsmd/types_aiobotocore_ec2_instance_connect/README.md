# EC2InstanceConnect module

> [Index](../README.md) > EC2InstanceConnect


!!! note ""

    Auto-generated documentation for [EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect)
    type annotations stubs module [types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `EC2InstanceConnect` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ec2-instance-connect]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ec2-instance-connect]'


# standalone installation
python -m pip install types-aiobotocore-ec2-instance-connect
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ec2-instance-connect
```

## Usage

Code samples can be found in [Examples](./usage.md).

## EC2InstanceConnectClient

Type annotations and code completion for  `#!python session.create_client("ec2-instance-connect")` as [EC2InstanceConnectClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#EC2InstanceConnect.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ec2_instance_connect.client import EC2InstanceConnectClient


session = get_session()
async with session.create_client("ec2-instance-connect") as client:
    client: EC2InstanceConnectClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_ec2_instance_connect.literals import EC2InstanceConnectServiceName

def get_value() -> EC2InstanceConnectServiceName:
    return "ec2-instance-connect"
```

- [EC2InstanceConnectServiceName](./literals.md#ec2instanceconnectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_ec2_instance_connect.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SendSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendsshpublickeyrequestrequesttypedef)
- [SendSerialConsoleSSHPublicKeyRequestRequestTypeDef](./type_defs.md#sendserialconsolesshpublickeyrequestrequesttypedef)
- [SendSSHPublicKeyResponseTypeDef](./type_defs.md#sendsshpublickeyresponsetypedef)
- [SendSerialConsoleSSHPublicKeyResponseTypeDef](./type_defs.md#sendserialconsolesshpublickeyresponsetypedef)

