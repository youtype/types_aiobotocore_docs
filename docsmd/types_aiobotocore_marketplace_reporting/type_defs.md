# Type definitions

> [Index](../README.md) > [MarketplaceReportingService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceReportingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#marketplacereportingservice)
    type annotations stubs module [types-aiobotocore-marketplace-reporting](https://pypi.org/project/types-aiobotocore-marketplace-reporting/).



## GetBuyerDashboardInputRequestTypeDef

```python
# GetBuyerDashboardInputRequestTypeDef definition

class GetBuyerDashboardInputRequestTypeDef(TypedDict):
    dashboardIdentifier: str,
    embeddingDomains: Sequence[str],
```

## ResponseMetadataTypeDef

```python
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
# GetBuyerDashboardOutputTypeDef definition

class GetBuyerDashboardOutputTypeDef(TypedDict):
    embedUrl: str,
    dashboardIdentifier: str,
    embeddingDomains: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
