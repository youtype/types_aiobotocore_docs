# EC2InstanceConnect module

> [Index](../README.md) > EC2InstanceConnect


!!! note ""

    Auto-generated documentation for [EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#ec2instanceconnect)
    type annotations stubs module [types-aiobotocore-ec2-instance-connect](https://pypi.org/project/types-aiobotocore-ec2-instance-connect/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `EC2InstanceConnect` service.
1. Use provided commands to install generated packages.



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

```python
# EC2InstanceConnectClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ec2_instance_connect.client import EC2InstanceConnectClient


session = get_session()
async with session.create_client("ec2-instance-connect") as client:
    client: EC2InstanceConnectClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# EC2InstanceConnectServiceName usage example

from types_aiobotocore_ec2_instance_connect.literals import EC2InstanceConnectServiceName

def get_value() -> EC2InstanceConnectServiceName:
    return "ec2-instance-connect"
```

- [EC2InstanceConnectServiceName](./literals.md#ec2instanceconnectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SendSSHPublicKeyRequestTypeDef](./type_defs.md#sendsshpublickeyrequesttypedef)
- [SendSerialConsoleSSHPublicKeyRequestTypeDef](./type_defs.md#sendserialconsolesshpublickeyrequesttypedef)
- [SendSSHPublicKeyResponseTypeDef](./type_defs.md#sendsshpublickeyresponsetypedef)
- [SendSerialConsoleSSHPublicKeyResponseTypeDef](./type_defs.md#sendserialconsolesshpublickeyresponsetypedef)

