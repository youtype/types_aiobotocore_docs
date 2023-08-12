# LexRuntimeV2 module

> [Index](../README.md) > LexRuntimeV2


!!! note ""

    Auto-generated documentation for [LexRuntimeV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
    type annotations stubs module [types-aiobotocore-lexv2-runtime](https://pypi.org/project/types-aiobotocore-lexv2-runtime/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `LexRuntimeV2` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[lexv2-runtime]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[lexv2-runtime]'


# standalone installation
python -m pip install types-aiobotocore-lexv2-runtime
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-lexv2-runtime
```

## Usage

Code samples can be found in [Examples](./usage.md).

## LexRuntimeV2Client

Type annotations and code completion for  `#!python session.create_client("lexv2-runtime")` as [LexRuntimeV2Client](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client)

```python
# LexRuntimeV2Client usage example

from aiobotocore.session import get_session

from types_aiobotocore_lexv2_runtime.client import LexRuntimeV2Client


session = get_session()
async with session.create_client("lexv2-runtime") as client:
    client: LexRuntimeV2Client
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ConfirmationStateType usage example

from types_aiobotocore_lexv2_runtime.literals import ConfirmationStateType

def get_value() -> ConfirmationStateType:
    return "Confirmed"
```

- [ConfirmationStateType](./literals.md#confirmationstatetype)
- [DialogActionTypeType](./literals.md#dialogactiontypetype)
- [IntentStateType](./literals.md#intentstatetype)
- [MessageContentTypeType](./literals.md#messagecontenttypetype)
- [SentimentTypeType](./literals.md#sentimenttypetype)
- [ShapeType](./literals.md#shapetype)
- [StyleTypeType](./literals.md#styletypetype)
- [LexRuntimeV2ServiceName](./literals.md#lexruntimev2servicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ActiveContextTimeToLiveTypeDef](./type_defs.md#activecontexttimetolivetypedef)
- [BlobTypeDef](./type_defs.md#blobtypedef)
- [ButtonTypeDef](./type_defs.md#buttontypedef)
- [ConfidenceScoreTypeDef](./type_defs.md#confidencescoretypedef)
- [DeleteSessionRequestRequestTypeDef](./type_defs.md#deletesessionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DialogActionTypeDef](./type_defs.md#dialogactiontypedef)
- [ElicitSubSlotTypeDef](./type_defs.md#elicitsubslottypedef)
- [GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef)
- [IntentTypeDef](./type_defs.md#intenttypedef)
- [RecognizedBotMemberTypeDef](./type_defs.md#recognizedbotmembertypedef)
- [RuntimeHintValueTypeDef](./type_defs.md#runtimehintvaluetypedef)
- [RuntimeHintsTypeDef](./type_defs.md#runtimehintstypedef)
- [SentimentScoreTypeDef](./type_defs.md#sentimentscoretypedef)
- [ValueTypeDef](./type_defs.md#valuetypedef)
- [ActiveContextTypeDef](./type_defs.md#activecontexttypedef)
- [RecognizeUtteranceRequestRequestTypeDef](./type_defs.md#recognizeutterancerequestrequesttypedef)
- [ImageResponseCardTypeDef](./type_defs.md#imageresponsecardtypedef)
- [DeleteSessionResponseTypeDef](./type_defs.md#deletesessionresponsetypedef)
- [PutSessionResponseTypeDef](./type_defs.md#putsessionresponsetypedef)
- [RecognizeUtteranceResponseTypeDef](./type_defs.md#recognizeutteranceresponsetypedef)
- [RuntimeHintDetailsTypeDef](./type_defs.md#runtimehintdetailstypedef)
- [SentimentResponseTypeDef](./type_defs.md#sentimentresponsetypedef)
- [SlotTypeDef](./type_defs.md#slottypedef)
- [SessionStateTypeDef](./type_defs.md#sessionstatetypedef)
- [MessageTypeDef](./type_defs.md#messagetypedef)
- [InterpretationTypeDef](./type_defs.md#interpretationtypedef)
- [RecognizeTextRequestRequestTypeDef](./type_defs.md#recognizetextrequestrequesttypedef)
- [PutSessionRequestRequestTypeDef](./type_defs.md#putsessionrequestrequesttypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [RecognizeTextResponseTypeDef](./type_defs.md#recognizetextresponsetypedef)

