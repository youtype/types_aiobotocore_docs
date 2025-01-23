# Type definitions

> [Index](../README.md) > [PrivateCAConnectorforSCEP](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [PrivateCAConnectorforSCEP](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep.html#privatecaconnectorforscep)
    type annotations stubs module [types-aiobotocore-pca-connector-scep](https://pypi.org/project/types-aiobotocore-pca-connector-scep/).



## ChallengeMetadataSummaryTypeDef

```python
# ChallengeMetadataSummaryTypeDef definition

class ChallengeMetadataSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    ConnectorArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

## ChallengeMetadataTypeDef

```python
# ChallengeMetadataTypeDef definition

class ChallengeMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
    ConnectorArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

## ChallengeTypeDef

```python
# ChallengeTypeDef definition

class ChallengeTypeDef(TypedDict):
    Arn: NotRequired[str],
    ConnectorArn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    Password: NotRequired[str],
```

## OpenIdConfigurationTypeDef

```python
# OpenIdConfigurationTypeDef definition

class OpenIdConfigurationTypeDef(TypedDict):
    Issuer: NotRequired[str],
    Subject: NotRequired[str],
    Audience: NotRequired[str],
```

## CreateChallengeRequestRequestTypeDef

```python
# CreateChallengeRequestRequestTypeDef definition

class CreateChallengeRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
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

## DeleteChallengeRequestRequestTypeDef

```python
# DeleteChallengeRequestRequestTypeDef definition

class DeleteChallengeRequestRequestTypeDef(TypedDict):
    ChallengeArn: str,
```

## DeleteConnectorRequestRequestTypeDef

```python
# DeleteConnectorRequestRequestTypeDef definition

class DeleteConnectorRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
```

## GetChallengeMetadataRequestRequestTypeDef

```python
# GetChallengeMetadataRequestRequestTypeDef definition

class GetChallengeMetadataRequestRequestTypeDef(TypedDict):
    ChallengeArn: str,
```

## GetChallengePasswordRequestRequestTypeDef

```python
# GetChallengePasswordRequestRequestTypeDef definition

class GetChallengePasswordRequestRequestTypeDef(TypedDict):
    ChallengeArn: str,
```

## GetConnectorRequestRequestTypeDef

```python
# GetConnectorRequestRequestTypeDef definition

class GetConnectorRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
```

## IntuneConfigurationTypeDef

```python
# IntuneConfigurationTypeDef definition

class IntuneConfigurationTypeDef(TypedDict):
    AzureApplicationId: str,
    Domain: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChallengeMetadataRequestRequestTypeDef

```python
# ListChallengeMetadataRequestRequestTypeDef definition

class ListChallengeMetadataRequestRequestTypeDef(TypedDict):
    ConnectorArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConnectorsRequestRequestTypeDef

```python
# ListConnectorsRequestRequestTypeDef definition

class ListConnectorsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## CreateChallengeResponseTypeDef

```python
# CreateChallengeResponseTypeDef definition

class CreateChallengeResponseTypeDef(TypedDict):
    Challenge: ChallengeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChallengeTypeDef](./type_defs.md#challengetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectorResponseTypeDef

```python
# CreateConnectorResponseTypeDef definition

class CreateConnectorResponseTypeDef(TypedDict):
    ConnectorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChallengeMetadataResponseTypeDef

```python
# GetChallengeMetadataResponseTypeDef definition

class GetChallengeMetadataResponseTypeDef(TypedDict):
    ChallengeMetadata: ChallengeMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChallengeMetadataTypeDef](./type_defs.md#challengemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChallengePasswordResponseTypeDef

```python
# GetChallengePasswordResponseTypeDef definition

class GetChallengePasswordResponseTypeDef(TypedDict):
    Password: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChallengeMetadataResponseTypeDef

```python
# ListChallengeMetadataResponseTypeDef definition

class ListChallengeMetadataResponseTypeDef(TypedDict):
    Challenges: List[ChallengeMetadataSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ChallengeMetadataSummaryTypeDef](./type_defs.md#challengemetadatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MobileDeviceManagementTypeDef

```python
# MobileDeviceManagementTypeDef definition

class MobileDeviceManagementTypeDef(TypedDict):
    Intune: NotRequired[IntuneConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: IntuneConfigurationTypeDef](./type_defs.md#intuneconfigurationtypedef) 
## ListChallengeMetadataRequestPaginateTypeDef

```python
# ListChallengeMetadataRequestPaginateTypeDef definition

class ListChallengeMetadataRequestPaginateTypeDef(TypedDict):
    ConnectorArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectorsRequestPaginateTypeDef

```python
# ListConnectorsRequestPaginateTypeDef definition

class ListConnectorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ConnectorSummaryTypeDef

```python
# ConnectorSummaryTypeDef definition

class ConnectorSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CertificateAuthorityArn: NotRequired[str],
    Type: NotRequired[ConnectorTypeType],  # (1)
    MobileDeviceManagement: NotRequired[MobileDeviceManagementTypeDef],  # (2)
    OpenIdConfiguration: NotRequired[OpenIdConfigurationTypeDef],  # (3)
    Status: NotRequired[ConnectorStatusType],  # (4)
    StatusReason: NotRequired[ConnectorStatusReasonType],  # (5)
    Endpoint: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-braces: MobileDeviceManagementTypeDef](./type_defs.md#mobiledevicemanagementtypedef) 
3. See [:material-code-braces: OpenIdConfigurationTypeDef](./type_defs.md#openidconfigurationtypedef) 
4. See [:material-code-brackets: ConnectorStatusType](./literals.md#connectorstatustype) 
5. See [:material-code-brackets: ConnectorStatusReasonType](./literals.md#connectorstatusreasontype) 
## ConnectorTypeDef

```python
# ConnectorTypeDef definition

class ConnectorTypeDef(TypedDict):
    Arn: NotRequired[str],
    CertificateAuthorityArn: NotRequired[str],
    Type: NotRequired[ConnectorTypeType],  # (1)
    MobileDeviceManagement: NotRequired[MobileDeviceManagementTypeDef],  # (2)
    OpenIdConfiguration: NotRequired[OpenIdConfigurationTypeDef],  # (3)
    Status: NotRequired[ConnectorStatusType],  # (4)
    StatusReason: NotRequired[ConnectorStatusReasonType],  # (5)
    Endpoint: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ConnectorTypeType](./literals.md#connectortypetype) 
2. See [:material-code-braces: MobileDeviceManagementTypeDef](./type_defs.md#mobiledevicemanagementtypedef) 
3. See [:material-code-braces: OpenIdConfigurationTypeDef](./type_defs.md#openidconfigurationtypedef) 
4. See [:material-code-brackets: ConnectorStatusType](./literals.md#connectorstatustype) 
5. See [:material-code-brackets: ConnectorStatusReasonType](./literals.md#connectorstatusreasontype) 
## CreateConnectorRequestRequestTypeDef

```python
# CreateConnectorRequestRequestTypeDef definition

class CreateConnectorRequestRequestTypeDef(TypedDict):
    CertificateAuthorityArn: str,
    MobileDeviceManagement: NotRequired[MobileDeviceManagementTypeDef],  # (1)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MobileDeviceManagementTypeDef](./type_defs.md#mobiledevicemanagementtypedef) 
## ListConnectorsResponseTypeDef

```python
# ListConnectorsResponseTypeDef definition

class ListConnectorsResponseTypeDef(TypedDict):
    Connectors: List[ConnectorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectorSummaryTypeDef](./type_defs.md#connectorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectorResponseTypeDef

```python
# GetConnectorResponseTypeDef definition

class GetConnectorResponseTypeDef(TypedDict):
    Connector: ConnectorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectorTypeDef](./type_defs.md#connectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
