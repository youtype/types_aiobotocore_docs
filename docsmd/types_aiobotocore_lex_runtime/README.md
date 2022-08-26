# LexRuntimeService module

> [Index](../README.md) > LexRuntimeService


!!! note ""

    Auto-generated documentation for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
    type annotations stubs module [types-aiobotocore-lex-runtime](https://pypi.org/project/types-aiobotocore-lex-runtime/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `LexRuntimeService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[lex-runtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[lex-runtime]'


# standalone installation
python -m pip install types-aiobotocore-lex-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lex-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LexRuntimeServiceClient

Type annotations and code completion for  `#!python session.create_client("lex-runtime")` as [LexRuntimeServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient


session = get_session()
async with session.create_client("lex-runtime") as client:
    client: LexRuntimeServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_lex_runtime.literals import ConfirmationStatusType

def get_value() -> ConfirmationStatusType:
    return "Confirmed"
```

- [ConfirmationStatusType](./literals.md#confirmationstatustype)
- [ContentTypeType](./literals.md#contenttypetype)
- [DialogActionTypeType](./literals.md#dialogactiontypetype)
- [DialogStateType](./literals.md#dialogstatetype)
- [FulfillmentStateType](./literals.md#fulfillmentstatetype)
- [MessageFormatTypeType](./literals.md#messageformattypetype)
- [LexRuntimeServiceServiceName](./literals.md#lexruntimeserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef

def get_value() -> ActiveContextTimeToLiveTypeDef:
    return {
        "timeToLiveInSeconds": ...,
    }
```

- [ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef)
- [ButtonTypeDef](./type_defs.md#buttontypedef)
- [DeleteSessionRequestRequestTypeDef](./type_defs.md#deletesessionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DialogActionTypeDef](./type_defs.md#dialogactiontypedef)
- [GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef)
- [IntentSummaryTypeDef](./type_defs.md#intentsummarytypedef)
- [IntentConfidenceTypeDef](./type_defs.md#intentconfidencetypedef)
- [PostContentRequestRequestTypeDef](./type_defs.md#postcontentrequestrequesttypedef)
- [SentimentResponseTypeDef](./type_defs.md#sentimentresponsetypedef)
- [ActiveContextTypeDef](./type_defs.md#activecontexttypedef)
- [GenericAttachmentTypeDef](./type_defs.md#genericattachmenttypedef)
- [DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef)
- [PostContentResponseTypeDef](./type_defs.md#postcontentresponsetypedef)
- [PutSessionResponseTypeDef](./type_defs.md#putsessionresponsetypedef)
- [PredictedIntentTypeDef](./type_defs.md#predictedintenttypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [PostTextRequestRequestTypeDef](./type_defs.md#posttextrequestrequesttypedef)
- [PutSessionRequestRequestTypeDef](./type_defs.md#putsessionrequestrequesttypedef)
- [ResponseCardTypeDef](./type_defs.md#responsecardtypedef)
- [PostTextResponseTypeDef](./type_defs.md#posttextresponsetypedef)

