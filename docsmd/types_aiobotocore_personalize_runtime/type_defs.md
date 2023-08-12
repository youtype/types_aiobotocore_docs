# Type definitions

> [Index](../README.md) > [PersonalizeRuntime](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime)
    type annotations stubs module [types-aiobotocore-personalize-runtime](https://pypi.org/project/types-aiobotocore-personalize-runtime/).



## GetPersonalizedRankingRequestRequestTypeDef

```python
# GetPersonalizedRankingRequestRequestTypeDef definition

class GetPersonalizedRankingRequestRequestTypeDef(TypedDict):
    campaignArn: str,
    inputList: Sequence[str],
    userId: str,
    context: NotRequired[Mapping[str, str]],
    filterArn: NotRequired[str],
    filterValues: NotRequired[Mapping[str, str]],
```

## PredictedItemTypeDef

```python
# PredictedItemTypeDef definition

class PredictedItemTypeDef(TypedDict):
    itemId: NotRequired[str],
    score: NotRequired[float],
    promotionName: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## PromotionTypeDef

```python
# PromotionTypeDef definition

class PromotionTypeDef(TypedDict):
    name: NotRequired[str],
    percentPromotedItems: NotRequired[int],
    filterArn: NotRequired[str],
    filterValues: NotRequired[Mapping[str, str]],
```

## GetPersonalizedRankingResponseTypeDef

```python
# GetPersonalizedRankingResponseTypeDef definition

class GetPersonalizedRankingResponseTypeDef(TypedDict):
    personalizedRanking: List[PredictedItemTypeDef],  # (1)
    recommendationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredictedItemTypeDef](./type_defs.md#predicteditemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommendationsResponseTypeDef

```python
# GetRecommendationsResponseTypeDef definition

class GetRecommendationsResponseTypeDef(TypedDict):
    itemList: List[PredictedItemTypeDef],  # (1)
    recommendationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PredictedItemTypeDef](./type_defs.md#predicteditemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommendationsRequestRequestTypeDef

```python
# GetRecommendationsRequestRequestTypeDef definition

class GetRecommendationsRequestRequestTypeDef(TypedDict):
    campaignArn: NotRequired[str],
    itemId: NotRequired[str],
    userId: NotRequired[str],
    numResults: NotRequired[int],
    context: NotRequired[Mapping[str, str]],
    filterArn: NotRequired[str],
    filterValues: NotRequired[Mapping[str, str]],
    recommenderArn: NotRequired[str],
    promotions: NotRequired[Sequence[PromotionTypeDef]],  # (1)
```

1. See [:material-code-braces: PromotionTypeDef](./type_defs.md#promotiontypedef) 
