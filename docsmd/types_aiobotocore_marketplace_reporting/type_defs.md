# Type definitions

> [Index](../README.md) > [MarketplaceReportingService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceReportingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#marketplacereportingservice)
    type annotations stubs module [types-aiobotocore-marketplace-reporting](https://pypi.org/project/types-aiobotocore-marketplace-reporting/).



## GetBuyerDashboardInputTypeDef

```python
# GetBuyerDashboardInputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_reporting.type_defs import GetBuyerDashboardInputTypeDef


def get_value() -> GetBuyerDashboardInputTypeDef:
    return {
        "dashboardIdentifier": ...,
    }


# GetBuyerDashboardInputTypeDef definition

class GetBuyerDashboardInputTypeDef(TypedDict):
    dashboardIdentifier: str,
    embeddingDomains: Sequence[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_marketplace_reporting.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## GetBuyerDashboardOutputTypeDef

```python
# GetBuyerDashboardOutputTypeDef TypedDict usage example

from types_aiobotocore_marketplace_reporting.type_defs import GetBuyerDashboardOutputTypeDef


def get_value() -> GetBuyerDashboardOutputTypeDef:
    return {
        "embedUrl": ...,
    }


# GetBuyerDashboardOutputTypeDef definition

class GetBuyerDashboardOutputTypeDef(TypedDict):
    embedUrl: str,
    dashboardIdentifier: str,
    embeddingDomains: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
