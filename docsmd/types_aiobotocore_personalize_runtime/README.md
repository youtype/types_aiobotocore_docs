# PersonalizeRuntime module

> [Index](../README.md) > PersonalizeRuntime


!!! note ""

    Auto-generated documentation for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
    type annotations stubs module [types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `PersonalizeRuntime`.

### From PyPI with pip

Install `types-aiobotocore` for `PersonalizeRuntime` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[personalize-runtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[personalize-runtime]'


# standalone installation
python -m pip install types-aiobotocore-personalize-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-personalize-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## PersonalizeRuntimeClient

Type annotations and code completion for  `#!python session.create_client("personalize-runtime")` as [PersonalizeRuntimeClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_personalize_runtime.client import PersonalizeRuntimeClient


session = get_session()
async with session.create_client("personalize-runtime") as client:
    client: PersonalizeRuntimeClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_personalize_runtime.literals import PersonalizeRuntimeServiceName

def get_value() -> PersonalizeRuntimeServiceName:
    return "personalize-runtime"
```

- [PersonalizeRuntimeServiceName](./literals.md#personalizeruntimeservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_personalize_runtime.type_defs import GetPersonalizedRankingRequestRequestTypeDef

def get_value() -> GetPersonalizedRankingRequestRequestTypeDef:
    return {
        "campaignArn": ...,
        "inputList": ...,
        "userId": ...,
    }
```

- [GetPersonalizedRankingRequestRequestTypeDef](./type_defs.md#getpersonalizedrankingrequestrequesttypedef)
- [PredictedItemTypeDef](./type_defs.md#predicteditemtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef)
- [GetPersonalizedRankingResponseTypeDef](./type_defs.md#getpersonalizedrankingresponsetypedef)
- [GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef)

