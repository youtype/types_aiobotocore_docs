# SSMGUIConnect module

> [Index](../README.md) > SSMGUIConnect


!!! note ""

    Auto-generated documentation for [SSMGUIConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-guiconnect.html#ssmguiconnect)
    type annotations stubs module [types-aiobotocore-ssm-guiconnect](https://pypi.org/project/types-aiobotocore-ssm-guiconnect/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SSMGUIConnect` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SSMGUIConnect` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ssm-guiconnect]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ssm-guiconnect]'

# standalone installation
python -m pip install types-aiobotocore-ssm-guiconnect
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ssm-guiconnect
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SSMGUIConnectClient

Type annotations and code completion for  `#!python session.create_client("ssm-guiconnect")` as [SSMGUIConnectClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-guiconnect.html#SSMGUIConnect.Client)

```python
# SSMGUIConnectClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_guiconnect.client import SSMGUIConnectClient


session = get_session()
async with session.create_client("ssm-guiconnect") as client:
    client: SSMGUIConnectClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# SSMGUIConnectServiceName usage example

from types_aiobotocore_ssm_guiconnect.literals import SSMGUIConnectServiceName

def get_value() -> SSMGUIConnectServiceName:
    return "ssm-guiconnect"
```

- [SSMGUIConnectServiceName](./literals.md#ssmguiconnectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [DeleteConnectionRecordingPreferencesRequestTypeDef](./type_defs.md#deleteconnectionrecordingpreferencesrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [S3BucketTypeDef](./type_defs.md#s3buckettypedef)
- [DeleteConnectionRecordingPreferencesResponseTypeDef](./type_defs.md#deleteconnectionrecordingpreferencesresponsetypedef)
- [RecordingDestinationsOutputTypeDef](./type_defs.md#recordingdestinationsoutputtypedef)
- [RecordingDestinationsTypeDef](./type_defs.md#recordingdestinationstypedef)
- [ConnectionRecordingPreferencesOutputTypeDef](./type_defs.md#connectionrecordingpreferencesoutputtypedef)
- [ConnectionRecordingPreferencesTypeDef](./type_defs.md#connectionrecordingpreferencestypedef)
- [GetConnectionRecordingPreferencesResponseTypeDef](./type_defs.md#getconnectionrecordingpreferencesresponsetypedef)
- [UpdateConnectionRecordingPreferencesResponseTypeDef](./type_defs.md#updateconnectionrecordingpreferencesresponsetypedef)
- [ConnectionRecordingPreferencesUnionTypeDef](./type_defs.md#connectionrecordingpreferencesuniontypedef)
- [UpdateConnectionRecordingPreferencesRequestTypeDef](./type_defs.md#updateconnectionrecordingpreferencesrequesttypedef)

