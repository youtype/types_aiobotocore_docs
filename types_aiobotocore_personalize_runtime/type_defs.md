<a id="typed-dictionaries-for-aiobotocore-personalizeruntime-module"></a>

# Typed dictionaries for aiobotocore PersonalizeRuntime module

> [Index](..) > [PersonalizeRuntime](.) > Typed dictionaries

Auto-generated documentation for
[PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
type annotations stubs module
[types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).

- [Typed dictionaries for aiobotocore PersonalizeRuntime module](#typed-dictionaries-for-aiobotocore-personalizeruntime-module)
  - [GetPersonalizedRankingRequestRequestTypeDef](#getpersonalizedrankingrequestrequesttypedef)
  - [GetPersonalizedRankingResponseTypeDef](#getpersonalizedrankingresponsetypedef)
  - [GetRecommendationsRequestRequestTypeDef](#getrecommendationsrequestrequesttypedef)
  - [GetRecommendationsResponseTypeDef](#getrecommendationsresponsetypedef)
  - [PredictedItemTypeDef](#predicteditemtypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)

<a id="getpersonalizedrankingrequestrequesttypedef"></a>

## GetPersonalizedRankingRequestRequestTypeDef

```python
from types_aiobotocore_personalize_runtime.type_defs import GetPersonalizedRankingRequestRequestTypeDef
```

Required fields:

- `campaignArn`: `str`
- `inputList`: `Sequence`\[`str`\]
- `userId`: `str`

Optional fields:

- `context`: `Mapping`\[`str`, `str`\]
- `filterArn`: `str`
- `filterValues`: `Mapping`\[`str`, `str`\]

<a id="getpersonalizedrankingresponsetypedef"></a>

## GetPersonalizedRankingResponseTypeDef

```python
from types_aiobotocore_personalize_runtime.type_defs import GetPersonalizedRankingResponseTypeDef
```

Required fields:

- `personalizedRanking`:
  `List`\[[PredictedItemTypeDef](./type_defs.md#predicteditemtypedef)\]
- `recommendationId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="getrecommendationsrequestrequesttypedef"></a>

## GetRecommendationsRequestRequestTypeDef

```python
from types_aiobotocore_personalize_runtime.type_defs import GetRecommendationsRequestRequestTypeDef
```

Optional fields:

- `campaignArn`: `str`
- `itemId`: `str`
- `userId`: `str`
- `numResults`: `int`
- `context`: `Mapping`\[`str`, `str`\]
- `filterArn`: `str`
- `filterValues`: `Mapping`\[`str`, `str`\]
- `recommenderArn`: `str`

<a id="getrecommendationsresponsetypedef"></a>

## GetRecommendationsResponseTypeDef

```python
from types_aiobotocore_personalize_runtime.type_defs import GetRecommendationsResponseTypeDef
```

Required fields:

- `itemList`:
  `List`\[[PredictedItemTypeDef](./type_defs.md#predicteditemtypedef)\]
- `recommendationId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="predicteditemtypedef"></a>

## PredictedItemTypeDef

```python
from types_aiobotocore_personalize_runtime.type_defs import PredictedItemTypeDef
```

Optional fields:

- `itemId`: `str`
- `score`: `float`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_personalize_runtime.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`
