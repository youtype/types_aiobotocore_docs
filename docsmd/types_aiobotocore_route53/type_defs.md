# Type definitions

> [Index](../README.md) > [Route53](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
    type annotations stubs module [types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

## ResourceRecordSetUnionTypeDef

```python
# ResourceRecordSetUnionTypeDef definition

ResourceRecordSetUnionTypeDef = Union[
    ResourceRecordSetTypeDef,  # (1)
    ResourceRecordSetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceRecordSetTypeDef](./type_defs.md#resourcerecordsettypedef) 
2. See [:material-code-braces: ResourceRecordSetOutputTypeDef](./type_defs.md#resourcerecordsetoutputtypedef) 



## AccountLimitTypeDef

```python
# AccountLimitTypeDef definition

class AccountLimitTypeDef(TypedDict):
    Type: AccountLimitTypeType,  # (1)
    Value: int,
```

1. See [:material-code-brackets: AccountLimitTypeType](./literals.md#accountlimittypetype) 
## ActivateKeySigningKeyRequestRequestTypeDef

```python
# ActivateKeySigningKeyRequestRequestTypeDef definition

class ActivateKeySigningKeyRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    Name: str,
```

## ChangeInfoTypeDef

```python
# ChangeInfoTypeDef definition

class ChangeInfoTypeDef(TypedDict):
    Id: str,
    Status: ChangeStatusType,  # (1)
    SubmittedAt: datetime,
    Comment: NotRequired[str],
```

1. See [:material-code-brackets: ChangeStatusType](./literals.md#changestatustype) 
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

## AlarmIdentifierTypeDef

```python
# AlarmIdentifierTypeDef definition

class AlarmIdentifierTypeDef(TypedDict):
    Region: CloudWatchRegionType,  # (1)
    Name: str,
```

1. See [:material-code-brackets: CloudWatchRegionType](./literals.md#cloudwatchregiontype) 
## AliasTargetTypeDef

```python
# AliasTargetTypeDef definition

class AliasTargetTypeDef(TypedDict):
    HostedZoneId: str,
    DNSName: str,
    EvaluateTargetHealth: bool,
```

## VPCTypeDef

```python
# VPCTypeDef definition

class VPCTypeDef(TypedDict):
    VPCRegion: NotRequired[VPCRegionType],  # (1)
    VPCId: NotRequired[str],
```

1. See [:material-code-brackets: VPCRegionType](./literals.md#vpcregiontype) 
## CidrCollectionChangeTypeDef

```python
# CidrCollectionChangeTypeDef definition

class CidrCollectionChangeTypeDef(TypedDict):
    LocationName: str,
    Action: CidrCollectionChangeActionType,  # (1)
    CidrList: Sequence[str],
```

1. See [:material-code-brackets: CidrCollectionChangeActionType](./literals.md#cidrcollectionchangeactiontype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## CidrBlockSummaryTypeDef

```python
# CidrBlockSummaryTypeDef definition

class CidrBlockSummaryTypeDef(TypedDict):
    CidrBlock: NotRequired[str],
    LocationName: NotRequired[str],
```

## CidrCollectionTypeDef

```python
# CidrCollectionTypeDef definition

class CidrCollectionTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[int],
```

## CidrRoutingConfigTypeDef

```python
# CidrRoutingConfigTypeDef definition

class CidrRoutingConfigTypeDef(TypedDict):
    CollectionId: str,
    LocationName: str,
```

## DimensionTypeDef

```python
# DimensionTypeDef definition

class DimensionTypeDef(TypedDict):
    Name: str,
    Value: str,
```

## CollectionSummaryTypeDef

```python
# CollectionSummaryTypeDef definition

class CollectionSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Version: NotRequired[int],
```

## CoordinatesTypeDef

```python
# CoordinatesTypeDef definition

class CoordinatesTypeDef(TypedDict):
    Latitude: str,
    Longitude: str,
```

## CreateCidrCollectionRequestRequestTypeDef

```python
# CreateCidrCollectionRequestRequestTypeDef definition

class CreateCidrCollectionRequestRequestTypeDef(TypedDict):
    Name: str,
    CallerReference: str,
```

## HostedZoneConfigTypeDef

```python
# HostedZoneConfigTypeDef definition

class HostedZoneConfigTypeDef(TypedDict):
    Comment: NotRequired[str],
    PrivateZone: NotRequired[bool],
```

## DelegationSetTypeDef

```python
# DelegationSetTypeDef definition

class DelegationSetTypeDef(TypedDict):
    NameServers: List[str],
    Id: NotRequired[str],
    CallerReference: NotRequired[str],
```

## CreateKeySigningKeyRequestRequestTypeDef

```python
# CreateKeySigningKeyRequestRequestTypeDef definition

class CreateKeySigningKeyRequestRequestTypeDef(TypedDict):
    CallerReference: str,
    HostedZoneId: str,
    KeyManagementServiceArn: str,
    Name: str,
    Status: str,
```

## KeySigningKeyTypeDef

```python
# KeySigningKeyTypeDef definition

class KeySigningKeyTypeDef(TypedDict):
    Name: NotRequired[str],
    KmsArn: NotRequired[str],
    Flag: NotRequired[int],
    SigningAlgorithmMnemonic: NotRequired[str],
    SigningAlgorithmType: NotRequired[int],
    DigestAlgorithmMnemonic: NotRequired[str],
    DigestAlgorithmType: NotRequired[int],
    KeyTag: NotRequired[int],
    DigestValue: NotRequired[str],
    PublicKey: NotRequired[str],
    DSRecord: NotRequired[str],
    DNSKEYRecord: NotRequired[str],
    Status: NotRequired[str],
    StatusMessage: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    LastModifiedDate: NotRequired[datetime],
```

## CreateQueryLoggingConfigRequestRequestTypeDef

```python
# CreateQueryLoggingConfigRequestRequestTypeDef definition

class CreateQueryLoggingConfigRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    CloudWatchLogsLogGroupArn: str,
```

## QueryLoggingConfigTypeDef

```python
# QueryLoggingConfigTypeDef definition

class QueryLoggingConfigTypeDef(TypedDict):
    Id: str,
    HostedZoneId: str,
    CloudWatchLogsLogGroupArn: str,
```

## CreateReusableDelegationSetRequestRequestTypeDef

```python
# CreateReusableDelegationSetRequestRequestTypeDef definition

class CreateReusableDelegationSetRequestRequestTypeDef(TypedDict):
    CallerReference: str,
    HostedZoneId: NotRequired[str],
```

## CreateTrafficPolicyInstanceRequestRequestTypeDef

```python
# CreateTrafficPolicyInstanceRequestRequestTypeDef definition

class CreateTrafficPolicyInstanceRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    Name: str,
    TTL: int,
    TrafficPolicyId: str,
    TrafficPolicyVersion: int,
```

## TrafficPolicyInstanceTypeDef

```python
# TrafficPolicyInstanceTypeDef definition

class TrafficPolicyInstanceTypeDef(TypedDict):
    Id: str,
    HostedZoneId: str,
    Name: str,
    TTL: int,
    State: str,
    Message: str,
    TrafficPolicyId: str,
    TrafficPolicyVersion: int,
    TrafficPolicyType: RRTypeType,  # (1)
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## CreateTrafficPolicyRequestRequestTypeDef

```python
# CreateTrafficPolicyRequestRequestTypeDef definition

class CreateTrafficPolicyRequestRequestTypeDef(TypedDict):
    Name: str,
    Document: str,
    Comment: NotRequired[str],
```

## TrafficPolicyTypeDef

```python
# TrafficPolicyTypeDef definition

class TrafficPolicyTypeDef(TypedDict):
    Id: str,
    Version: int,
    Name: str,
    Type: RRTypeType,  # (1)
    Document: str,
    Comment: NotRequired[str],
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## CreateTrafficPolicyVersionRequestRequestTypeDef

```python
# CreateTrafficPolicyVersionRequestRequestTypeDef definition

class CreateTrafficPolicyVersionRequestRequestTypeDef(TypedDict):
    Id: str,
    Document: str,
    Comment: NotRequired[str],
```

## DNSSECStatusTypeDef

```python
# DNSSECStatusTypeDef definition

class DNSSECStatusTypeDef(TypedDict):
    ServeSignature: NotRequired[str],
    StatusMessage: NotRequired[str],
```

## DeactivateKeySigningKeyRequestRequestTypeDef

```python
# DeactivateKeySigningKeyRequestRequestTypeDef definition

class DeactivateKeySigningKeyRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    Name: str,
```

## DeleteCidrCollectionRequestRequestTypeDef

```python
# DeleteCidrCollectionRequestRequestTypeDef definition

class DeleteCidrCollectionRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteHealthCheckRequestRequestTypeDef

```python
# DeleteHealthCheckRequestRequestTypeDef definition

class DeleteHealthCheckRequestRequestTypeDef(TypedDict):
    HealthCheckId: str,
```

## DeleteHostedZoneRequestRequestTypeDef

```python
# DeleteHostedZoneRequestRequestTypeDef definition

class DeleteHostedZoneRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteKeySigningKeyRequestRequestTypeDef

```python
# DeleteKeySigningKeyRequestRequestTypeDef definition

class DeleteKeySigningKeyRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    Name: str,
```

## DeleteQueryLoggingConfigRequestRequestTypeDef

```python
# DeleteQueryLoggingConfigRequestRequestTypeDef definition

class DeleteQueryLoggingConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteReusableDelegationSetRequestRequestTypeDef

```python
# DeleteReusableDelegationSetRequestRequestTypeDef definition

class DeleteReusableDelegationSetRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteTrafficPolicyInstanceRequestRequestTypeDef

```python
# DeleteTrafficPolicyInstanceRequestRequestTypeDef definition

class DeleteTrafficPolicyInstanceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeleteTrafficPolicyRequestRequestTypeDef

```python
# DeleteTrafficPolicyRequestRequestTypeDef definition

class DeleteTrafficPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
    Version: int,
```

## DisableHostedZoneDNSSECRequestRequestTypeDef

```python
# DisableHostedZoneDNSSECRequestRequestTypeDef definition

class DisableHostedZoneDNSSECRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
```

## EnableHostedZoneDNSSECRequestRequestTypeDef

```python
# EnableHostedZoneDNSSECRequestRequestTypeDef definition

class EnableHostedZoneDNSSECRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
```

## GeoLocationDetailsTypeDef

```python
# GeoLocationDetailsTypeDef definition

class GeoLocationDetailsTypeDef(TypedDict):
    ContinentCode: NotRequired[str],
    ContinentName: NotRequired[str],
    CountryCode: NotRequired[str],
    CountryName: NotRequired[str],
    SubdivisionCode: NotRequired[str],
    SubdivisionName: NotRequired[str],
```

## GeoLocationTypeDef

```python
# GeoLocationTypeDef definition

class GeoLocationTypeDef(TypedDict):
    ContinentCode: NotRequired[str],
    CountryCode: NotRequired[str],
    SubdivisionCode: NotRequired[str],
```

## GetAccountLimitRequestRequestTypeDef

```python
# GetAccountLimitRequestRequestTypeDef definition

class GetAccountLimitRequestRequestTypeDef(TypedDict):
    Type: AccountLimitTypeType,  # (1)
```

1. See [:material-code-brackets: AccountLimitTypeType](./literals.md#accountlimittypetype) 
## GetChangeRequestRequestTypeDef

```python
# GetChangeRequestRequestTypeDef definition

class GetChangeRequestRequestTypeDef(TypedDict):
    Id: str,
```

## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetDNSSECRequestRequestTypeDef

```python
# GetDNSSECRequestRequestTypeDef definition

class GetDNSSECRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
```

## GetGeoLocationRequestRequestTypeDef

```python
# GetGeoLocationRequestRequestTypeDef definition

class GetGeoLocationRequestRequestTypeDef(TypedDict):
    ContinentCode: NotRequired[str],
    CountryCode: NotRequired[str],
    SubdivisionCode: NotRequired[str],
```

## GetHealthCheckLastFailureReasonRequestRequestTypeDef

```python
# GetHealthCheckLastFailureReasonRequestRequestTypeDef definition

class GetHealthCheckLastFailureReasonRequestRequestTypeDef(TypedDict):
    HealthCheckId: str,
```

## GetHealthCheckRequestRequestTypeDef

```python
# GetHealthCheckRequestRequestTypeDef definition

class GetHealthCheckRequestRequestTypeDef(TypedDict):
    HealthCheckId: str,
```

## GetHealthCheckStatusRequestRequestTypeDef

```python
# GetHealthCheckStatusRequestRequestTypeDef definition

class GetHealthCheckStatusRequestRequestTypeDef(TypedDict):
    HealthCheckId: str,
```

## GetHostedZoneLimitRequestRequestTypeDef

```python
# GetHostedZoneLimitRequestRequestTypeDef definition

class GetHostedZoneLimitRequestRequestTypeDef(TypedDict):
    Type: HostedZoneLimitTypeType,  # (1)
    HostedZoneId: str,
```

1. See [:material-code-brackets: HostedZoneLimitTypeType](./literals.md#hostedzonelimittypetype) 
## HostedZoneLimitTypeDef

```python
# HostedZoneLimitTypeDef definition

class HostedZoneLimitTypeDef(TypedDict):
    Type: HostedZoneLimitTypeType,  # (1)
    Value: int,
```

1. See [:material-code-brackets: HostedZoneLimitTypeType](./literals.md#hostedzonelimittypetype) 
## GetHostedZoneRequestRequestTypeDef

```python
# GetHostedZoneRequestRequestTypeDef definition

class GetHostedZoneRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetQueryLoggingConfigRequestRequestTypeDef

```python
# GetQueryLoggingConfigRequestRequestTypeDef definition

class GetQueryLoggingConfigRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetReusableDelegationSetLimitRequestRequestTypeDef

```python
# GetReusableDelegationSetLimitRequestRequestTypeDef definition

class GetReusableDelegationSetLimitRequestRequestTypeDef(TypedDict):
    Type: ReusableDelegationSetLimitTypeType,  # (1)
    DelegationSetId: str,
```

1. See [:material-code-brackets: ReusableDelegationSetLimitTypeType](./literals.md#reusabledelegationsetlimittypetype) 
## ReusableDelegationSetLimitTypeDef

```python
# ReusableDelegationSetLimitTypeDef definition

class ReusableDelegationSetLimitTypeDef(TypedDict):
    Type: ReusableDelegationSetLimitTypeType,  # (1)
    Value: int,
```

1. See [:material-code-brackets: ReusableDelegationSetLimitTypeType](./literals.md#reusabledelegationsetlimittypetype) 
## GetReusableDelegationSetRequestRequestTypeDef

```python
# GetReusableDelegationSetRequestRequestTypeDef definition

class GetReusableDelegationSetRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetTrafficPolicyInstanceRequestRequestTypeDef

```python
# GetTrafficPolicyInstanceRequestRequestTypeDef definition

class GetTrafficPolicyInstanceRequestRequestTypeDef(TypedDict):
    Id: str,
```

## GetTrafficPolicyRequestRequestTypeDef

```python
# GetTrafficPolicyRequestRequestTypeDef definition

class GetTrafficPolicyRequestRequestTypeDef(TypedDict):
    Id: str,
    Version: int,
```

## StatusReportTypeDef

```python
# StatusReportTypeDef definition

class StatusReportTypeDef(TypedDict):
    Status: NotRequired[str],
    CheckedTime: NotRequired[datetime],
```

## LinkedServiceTypeDef

```python
# LinkedServiceTypeDef definition

class LinkedServiceTypeDef(TypedDict):
    ServicePrincipal: NotRequired[str],
    Description: NotRequired[str],
```

## HostedZoneOwnerTypeDef

```python
# HostedZoneOwnerTypeDef definition

class HostedZoneOwnerTypeDef(TypedDict):
    OwningAccount: NotRequired[str],
    OwningService: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCidrBlocksRequestRequestTypeDef

```python
# ListCidrBlocksRequestRequestTypeDef definition

class ListCidrBlocksRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    LocationName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[str],
```

## ListCidrCollectionsRequestRequestTypeDef

```python
# ListCidrCollectionsRequestRequestTypeDef definition

class ListCidrCollectionsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[str],
```

## ListCidrLocationsRequestRequestTypeDef

```python
# ListCidrLocationsRequestRequestTypeDef definition

class ListCidrLocationsRequestRequestTypeDef(TypedDict):
    CollectionId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[str],
```

## LocationSummaryTypeDef

```python
# LocationSummaryTypeDef definition

class LocationSummaryTypeDef(TypedDict):
    LocationName: NotRequired[str],
```

## ListGeoLocationsRequestRequestTypeDef

```python
# ListGeoLocationsRequestRequestTypeDef definition

class ListGeoLocationsRequestRequestTypeDef(TypedDict):
    StartContinentCode: NotRequired[str],
    StartCountryCode: NotRequired[str],
    StartSubdivisionCode: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListHealthChecksRequestRequestTypeDef

```python
# ListHealthChecksRequestRequestTypeDef definition

class ListHealthChecksRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListHostedZonesByNameRequestRequestTypeDef

```python
# ListHostedZonesByNameRequestRequestTypeDef definition

class ListHostedZonesByNameRequestRequestTypeDef(TypedDict):
    DNSName: NotRequired[str],
    HostedZoneId: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListHostedZonesByVPCRequestRequestTypeDef

```python
# ListHostedZonesByVPCRequestRequestTypeDef definition

class ListHostedZonesByVPCRequestRequestTypeDef(TypedDict):
    VPCId: str,
    VPCRegion: VPCRegionType,  # (1)
    MaxItems: NotRequired[str],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: VPCRegionType](./literals.md#vpcregiontype) 
## ListHostedZonesRequestRequestTypeDef

```python
# ListHostedZonesRequestRequestTypeDef definition

class ListHostedZonesRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
    DelegationSetId: NotRequired[str],
    HostedZoneType: NotRequired[HostedZoneTypeType],  # (1)
```

1. See [:material-code-brackets: HostedZoneTypeType](./literals.md#hostedzonetypetype) 
## ListQueryLoggingConfigsRequestRequestTypeDef

```python
# ListQueryLoggingConfigsRequestRequestTypeDef definition

class ListQueryLoggingConfigsRequestRequestTypeDef(TypedDict):
    HostedZoneId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[str],
```

## ListResourceRecordSetsRequestRequestTypeDef

```python
# ListResourceRecordSetsRequestRequestTypeDef definition

class ListResourceRecordSetsRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    StartRecordName: NotRequired[str],
    StartRecordType: NotRequired[RRTypeType],  # (1)
    StartRecordIdentifier: NotRequired[str],
    MaxItems: NotRequired[str],
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## ListReusableDelegationSetsRequestRequestTypeDef

```python
# ListReusableDelegationSetsRequestRequestTypeDef definition

class ListReusableDelegationSetsRequestRequestTypeDef(TypedDict):
    Marker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceType: TagResourceTypeType,  # (1)
    ResourceId: str,
```

1. See [:material-code-brackets: TagResourceTypeType](./literals.md#tagresourcetypetype) 
## ListTagsForResourcesRequestRequestTypeDef

```python
# ListTagsForResourcesRequestRequestTypeDef definition

class ListTagsForResourcesRequestRequestTypeDef(TypedDict):
    ResourceType: TagResourceTypeType,  # (1)
    ResourceIds: Sequence[str],
```

1. See [:material-code-brackets: TagResourceTypeType](./literals.md#tagresourcetypetype) 
## ListTrafficPoliciesRequestRequestTypeDef

```python
# ListTrafficPoliciesRequestRequestTypeDef definition

class ListTrafficPoliciesRequestRequestTypeDef(TypedDict):
    TrafficPolicyIdMarker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## TrafficPolicySummaryTypeDef

```python
# TrafficPolicySummaryTypeDef definition

class TrafficPolicySummaryTypeDef(TypedDict):
    Id: str,
    Name: str,
    Type: RRTypeType,  # (1)
    LatestVersion: int,
    TrafficPolicyCount: int,
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef

```python
# ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef definition

class ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    TrafficPolicyInstanceNameMarker: NotRequired[str],
    TrafficPolicyInstanceTypeMarker: NotRequired[RRTypeType],  # (1)
    MaxItems: NotRequired[str],
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef

```python
# ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef definition

class ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef(TypedDict):
    TrafficPolicyId: str,
    TrafficPolicyVersion: int,
    HostedZoneIdMarker: NotRequired[str],
    TrafficPolicyInstanceNameMarker: NotRequired[str],
    TrafficPolicyInstanceTypeMarker: NotRequired[RRTypeType],  # (1)
    MaxItems: NotRequired[str],
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## ListTrafficPolicyInstancesRequestRequestTypeDef

```python
# ListTrafficPolicyInstancesRequestRequestTypeDef definition

class ListTrafficPolicyInstancesRequestRequestTypeDef(TypedDict):
    HostedZoneIdMarker: NotRequired[str],
    TrafficPolicyInstanceNameMarker: NotRequired[str],
    TrafficPolicyInstanceTypeMarker: NotRequired[RRTypeType],  # (1)
    MaxItems: NotRequired[str],
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## ListTrafficPolicyVersionsRequestRequestTypeDef

```python
# ListTrafficPolicyVersionsRequestRequestTypeDef definition

class ListTrafficPolicyVersionsRequestRequestTypeDef(TypedDict):
    Id: str,
    TrafficPolicyVersionMarker: NotRequired[str],
    MaxItems: NotRequired[str],
```

## ListVPCAssociationAuthorizationsRequestRequestTypeDef

```python
# ListVPCAssociationAuthorizationsRequestRequestTypeDef definition

class ListVPCAssociationAuthorizationsRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[str],
```

## ResourceRecordTypeDef

```python
# ResourceRecordTypeDef definition

class ResourceRecordTypeDef(TypedDict):
    Value: str,
```

## TestDNSAnswerRequestRequestTypeDef

```python
# TestDNSAnswerRequestRequestTypeDef definition

class TestDNSAnswerRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    RecordName: str,
    RecordType: RRTypeType,  # (1)
    ResolverIP: NotRequired[str],
    EDNS0ClientSubnetIP: NotRequired[str],
    EDNS0ClientSubnetMask: NotRequired[str],
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
## UpdateHostedZoneCommentRequestRequestTypeDef

```python
# UpdateHostedZoneCommentRequestRequestTypeDef definition

class UpdateHostedZoneCommentRequestRequestTypeDef(TypedDict):
    Id: str,
    Comment: NotRequired[str],
```

## UpdateTrafficPolicyCommentRequestRequestTypeDef

```python
# UpdateTrafficPolicyCommentRequestRequestTypeDef definition

class UpdateTrafficPolicyCommentRequestRequestTypeDef(TypedDict):
    Id: str,
    Version: int,
    Comment: str,
```

## UpdateTrafficPolicyInstanceRequestRequestTypeDef

```python
# UpdateTrafficPolicyInstanceRequestRequestTypeDef definition

class UpdateTrafficPolicyInstanceRequestRequestTypeDef(TypedDict):
    Id: str,
    TTL: int,
    TrafficPolicyId: str,
    TrafficPolicyVersion: int,
```

## ActivateKeySigningKeyResponseTypeDef

```python
# ActivateKeySigningKeyResponseTypeDef definition

class ActivateKeySigningKeyResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateVPCWithHostedZoneResponseTypeDef

```python
# AssociateVPCWithHostedZoneResponseTypeDef definition

class AssociateVPCWithHostedZoneResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeCidrCollectionResponseTypeDef

```python
# ChangeCidrCollectionResponseTypeDef definition

class ChangeCidrCollectionResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeResourceRecordSetsResponseTypeDef

```python
# ChangeResourceRecordSetsResponseTypeDef definition

class ChangeResourceRecordSetsResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeactivateKeySigningKeyResponseTypeDef

```python
# DeactivateKeySigningKeyResponseTypeDef definition

class DeactivateKeySigningKeyResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteHostedZoneResponseTypeDef

```python
# DeleteHostedZoneResponseTypeDef definition

class DeleteHostedZoneResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKeySigningKeyResponseTypeDef

```python
# DeleteKeySigningKeyResponseTypeDef definition

class DeleteKeySigningKeyResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisableHostedZoneDNSSECResponseTypeDef

```python
# DisableHostedZoneDNSSECResponseTypeDef definition

class DisableHostedZoneDNSSECResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateVPCFromHostedZoneResponseTypeDef

```python
# DisassociateVPCFromHostedZoneResponseTypeDef definition

class DisassociateVPCFromHostedZoneResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableHostedZoneDNSSECResponseTypeDef

```python
# EnableHostedZoneDNSSECResponseTypeDef definition

class EnableHostedZoneDNSSECResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountLimitResponseTypeDef

```python
# GetAccountLimitResponseTypeDef definition

class GetAccountLimitResponseTypeDef(TypedDict):
    Limit: AccountLimitTypeDef,  # (1)
    Count: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountLimitTypeDef](./type_defs.md#accountlimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChangeResponseTypeDef

```python
# GetChangeResponseTypeDef definition

class GetChangeResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCheckerIpRangesResponseTypeDef

```python
# GetCheckerIpRangesResponseTypeDef definition

class GetCheckerIpRangesResponseTypeDef(TypedDict):
    CheckerIpRanges: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHealthCheckCountResponseTypeDef

```python
# GetHealthCheckCountResponseTypeDef definition

class GetHealthCheckCountResponseTypeDef(TypedDict):
    HealthCheckCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHostedZoneCountResponseTypeDef

```python
# GetHostedZoneCountResponseTypeDef definition

class GetHostedZoneCountResponseTypeDef(TypedDict):
    HostedZoneCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrafficPolicyInstanceCountResponseTypeDef

```python
# GetTrafficPolicyInstanceCountResponseTypeDef definition

class GetTrafficPolicyInstanceCountResponseTypeDef(TypedDict):
    TrafficPolicyInstanceCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TestDNSAnswerResponseTypeDef

```python
# TestDNSAnswerResponseTypeDef definition

class TestDNSAnswerResponseTypeDef(TypedDict):
    Nameserver: str,
    RecordName: str,
    RecordType: RRTypeType,  # (1)
    RecordData: List[str],
    ResponseCode: str,
    Protocol: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HealthCheckConfigOutputTypeDef

```python
# HealthCheckConfigOutputTypeDef definition

class HealthCheckConfigOutputTypeDef(TypedDict):
    Type: HealthCheckTypeType,  # (1)
    IPAddress: NotRequired[str],
    Port: NotRequired[int],
    ResourcePath: NotRequired[str],
    FullyQualifiedDomainName: NotRequired[str],
    SearchString: NotRequired[str],
    RequestInterval: NotRequired[int],
    FailureThreshold: NotRequired[int],
    MeasureLatency: NotRequired[bool],
    Inverted: NotRequired[bool],
    Disabled: NotRequired[bool],
    HealthThreshold: NotRequired[int],
    ChildHealthChecks: NotRequired[List[str]],
    EnableSNI: NotRequired[bool],
    Regions: NotRequired[List[HealthCheckRegionType]],  # (2)
    AlarmIdentifier: NotRequired[AlarmIdentifierTypeDef],  # (3)
    InsufficientDataHealthStatus: NotRequired[InsufficientDataHealthStatusType],  # (4)
    RoutingControlArn: NotRequired[str],
```

1. See [:material-code-brackets: HealthCheckTypeType](./literals.md#healthchecktypetype) 
2. See [:material-code-brackets: HealthCheckRegionType](./literals.md#healthcheckregiontype) 
3. See [:material-code-braces: AlarmIdentifierTypeDef](./type_defs.md#alarmidentifiertypedef) 
4. See [:material-code-brackets: InsufficientDataHealthStatusType](./literals.md#insufficientdatahealthstatustype) 
## HealthCheckConfigTypeDef

```python
# HealthCheckConfigTypeDef definition

class HealthCheckConfigTypeDef(TypedDict):
    Type: HealthCheckTypeType,  # (1)
    IPAddress: NotRequired[str],
    Port: NotRequired[int],
    ResourcePath: NotRequired[str],
    FullyQualifiedDomainName: NotRequired[str],
    SearchString: NotRequired[str],
    RequestInterval: NotRequired[int],
    FailureThreshold: NotRequired[int],
    MeasureLatency: NotRequired[bool],
    Inverted: NotRequired[bool],
    Disabled: NotRequired[bool],
    HealthThreshold: NotRequired[int],
    ChildHealthChecks: NotRequired[Sequence[str]],
    EnableSNI: NotRequired[bool],
    Regions: NotRequired[Sequence[HealthCheckRegionType]],  # (2)
    AlarmIdentifier: NotRequired[AlarmIdentifierTypeDef],  # (3)
    InsufficientDataHealthStatus: NotRequired[InsufficientDataHealthStatusType],  # (4)
    RoutingControlArn: NotRequired[str],
```

1. See [:material-code-brackets: HealthCheckTypeType](./literals.md#healthchecktypetype) 
2. See [:material-code-brackets: HealthCheckRegionType](./literals.md#healthcheckregiontype) 
3. See [:material-code-braces: AlarmIdentifierTypeDef](./type_defs.md#alarmidentifiertypedef) 
4. See [:material-code-brackets: InsufficientDataHealthStatusType](./literals.md#insufficientdatahealthstatustype) 
## UpdateHealthCheckRequestRequestTypeDef

```python
# UpdateHealthCheckRequestRequestTypeDef definition

class UpdateHealthCheckRequestRequestTypeDef(TypedDict):
    HealthCheckId: str,
    HealthCheckVersion: NotRequired[int],
    IPAddress: NotRequired[str],
    Port: NotRequired[int],
    ResourcePath: NotRequired[str],
    FullyQualifiedDomainName: NotRequired[str],
    SearchString: NotRequired[str],
    FailureThreshold: NotRequired[int],
    Inverted: NotRequired[bool],
    Disabled: NotRequired[bool],
    HealthThreshold: NotRequired[int],
    ChildHealthChecks: NotRequired[Sequence[str]],
    EnableSNI: NotRequired[bool],
    Regions: NotRequired[Sequence[HealthCheckRegionType]],  # (1)
    AlarmIdentifier: NotRequired[AlarmIdentifierTypeDef],  # (2)
    InsufficientDataHealthStatus: NotRequired[InsufficientDataHealthStatusType],  # (3)
    ResetElements: NotRequired[Sequence[ResettableElementNameType]],  # (4)
```

1. See [:material-code-brackets: HealthCheckRegionType](./literals.md#healthcheckregiontype) 
2. See [:material-code-braces: AlarmIdentifierTypeDef](./type_defs.md#alarmidentifiertypedef) 
3. See [:material-code-brackets: InsufficientDataHealthStatusType](./literals.md#insufficientdatahealthstatustype) 
4. See [:material-code-brackets: ResettableElementNameType](./literals.md#resettableelementnametype) 
## AssociateVPCWithHostedZoneRequestRequestTypeDef

```python
# AssociateVPCWithHostedZoneRequestRequestTypeDef definition

class AssociateVPCWithHostedZoneRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    VPC: VPCTypeDef,  # (1)
    Comment: NotRequired[str],
```

1. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
## CreateVPCAssociationAuthorizationRequestRequestTypeDef

```python
# CreateVPCAssociationAuthorizationRequestRequestTypeDef definition

class CreateVPCAssociationAuthorizationRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    VPC: VPCTypeDef,  # (1)
```

1. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
## CreateVPCAssociationAuthorizationResponseTypeDef

```python
# CreateVPCAssociationAuthorizationResponseTypeDef definition

class CreateVPCAssociationAuthorizationResponseTypeDef(TypedDict):
    HostedZoneId: str,
    VPC: VPCTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVPCAssociationAuthorizationRequestRequestTypeDef

```python
# DeleteVPCAssociationAuthorizationRequestRequestTypeDef definition

class DeleteVPCAssociationAuthorizationRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    VPC: VPCTypeDef,  # (1)
```

1. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
## DisassociateVPCFromHostedZoneRequestRequestTypeDef

```python
# DisassociateVPCFromHostedZoneRequestRequestTypeDef definition

class DisassociateVPCFromHostedZoneRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    VPC: VPCTypeDef,  # (1)
    Comment: NotRequired[str],
```

1. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
## ListVPCAssociationAuthorizationsResponseTypeDef

```python
# ListVPCAssociationAuthorizationsResponseTypeDef definition

class ListVPCAssociationAuthorizationsResponseTypeDef(TypedDict):
    HostedZoneId: str,
    VPCs: List[VPCTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeCidrCollectionRequestRequestTypeDef

```python
# ChangeCidrCollectionRequestRequestTypeDef definition

class ChangeCidrCollectionRequestRequestTypeDef(TypedDict):
    Id: str,
    Changes: Sequence[CidrCollectionChangeTypeDef],  # (1)
    CollectionVersion: NotRequired[int],
```

1. See [:material-code-braces: CidrCollectionChangeTypeDef](./type_defs.md#cidrcollectionchangetypedef) 
## ChangeTagsForResourceRequestRequestTypeDef

```python
# ChangeTagsForResourceRequestRequestTypeDef definition

class ChangeTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceType: TagResourceTypeType,  # (1)
    ResourceId: str,
    AddTags: NotRequired[Sequence[TagTypeDef]],  # (2)
    RemoveTagKeys: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: TagResourceTypeType](./literals.md#tagresourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceTagSetTypeDef

```python
# ResourceTagSetTypeDef definition

class ResourceTagSetTypeDef(TypedDict):
    ResourceType: NotRequired[TagResourceTypeType],  # (1)
    ResourceId: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: TagResourceTypeType](./literals.md#tagresourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListCidrBlocksResponseTypeDef

```python
# ListCidrBlocksResponseTypeDef definition

class ListCidrBlocksResponseTypeDef(TypedDict):
    CidrBlocks: List[CidrBlockSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CidrBlockSummaryTypeDef](./type_defs.md#cidrblocksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCidrCollectionResponseTypeDef

```python
# CreateCidrCollectionResponseTypeDef definition

class CreateCidrCollectionResponseTypeDef(TypedDict):
    Collection: CidrCollectionTypeDef,  # (1)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CidrCollectionTypeDef](./type_defs.md#cidrcollectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloudWatchAlarmConfigurationTypeDef

```python
# CloudWatchAlarmConfigurationTypeDef definition

class CloudWatchAlarmConfigurationTypeDef(TypedDict):
    EvaluationPeriods: int,
    Threshold: float,
    ComparisonOperator: ComparisonOperatorType,  # (1)
    Period: int,
    MetricName: str,
    Namespace: str,
    Statistic: StatisticType,  # (2)
    Dimensions: NotRequired[List[DimensionTypeDef]],  # (3)
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
2. See [:material-code-brackets: StatisticType](./literals.md#statistictype) 
3. See [:material-code-braces: DimensionTypeDef](./type_defs.md#dimensiontypedef) 
## ListCidrCollectionsResponseTypeDef

```python
# ListCidrCollectionsResponseTypeDef definition

class ListCidrCollectionsResponseTypeDef(TypedDict):
    CidrCollections: List[CollectionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CollectionSummaryTypeDef](./type_defs.md#collectionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GeoProximityLocationTypeDef

```python
# GeoProximityLocationTypeDef definition

class GeoProximityLocationTypeDef(TypedDict):
    AWSRegion: NotRequired[str],
    LocalZoneGroup: NotRequired[str],
    Coordinates: NotRequired[CoordinatesTypeDef],  # (1)
    Bias: NotRequired[int],
```

1. See [:material-code-braces: CoordinatesTypeDef](./type_defs.md#coordinatestypedef) 
## CreateHostedZoneRequestRequestTypeDef

```python
# CreateHostedZoneRequestRequestTypeDef definition

class CreateHostedZoneRequestRequestTypeDef(TypedDict):
    Name: str,
    CallerReference: str,
    VPC: NotRequired[VPCTypeDef],  # (1)
    HostedZoneConfig: NotRequired[HostedZoneConfigTypeDef],  # (2)
    DelegationSetId: NotRequired[str],
```

1. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
2. See [:material-code-braces: HostedZoneConfigTypeDef](./type_defs.md#hostedzoneconfigtypedef) 
## CreateReusableDelegationSetResponseTypeDef

```python
# CreateReusableDelegationSetResponseTypeDef definition

class CreateReusableDelegationSetResponseTypeDef(TypedDict):
    DelegationSet: DelegationSetTypeDef,  # (1)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DelegationSetTypeDef](./type_defs.md#delegationsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReusableDelegationSetResponseTypeDef

```python
# GetReusableDelegationSetResponseTypeDef definition

class GetReusableDelegationSetResponseTypeDef(TypedDict):
    DelegationSet: DelegationSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DelegationSetTypeDef](./type_defs.md#delegationsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReusableDelegationSetsResponseTypeDef

```python
# ListReusableDelegationSetsResponseTypeDef definition

class ListReusableDelegationSetsResponseTypeDef(TypedDict):
    DelegationSets: List[DelegationSetTypeDef],  # (1)
    Marker: str,
    IsTruncated: bool,
    NextMarker: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DelegationSetTypeDef](./type_defs.md#delegationsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateKeySigningKeyResponseTypeDef

```python
# CreateKeySigningKeyResponseTypeDef definition

class CreateKeySigningKeyResponseTypeDef(TypedDict):
    ChangeInfo: ChangeInfoTypeDef,  # (1)
    KeySigningKey: KeySigningKeyTypeDef,  # (2)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
2. See [:material-code-braces: KeySigningKeyTypeDef](./type_defs.md#keysigningkeytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQueryLoggingConfigResponseTypeDef

```python
# CreateQueryLoggingConfigResponseTypeDef definition

class CreateQueryLoggingConfigResponseTypeDef(TypedDict):
    QueryLoggingConfig: QueryLoggingConfigTypeDef,  # (1)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryLoggingConfigTypeDef](./type_defs.md#queryloggingconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryLoggingConfigResponseTypeDef

```python
# GetQueryLoggingConfigResponseTypeDef definition

class GetQueryLoggingConfigResponseTypeDef(TypedDict):
    QueryLoggingConfig: QueryLoggingConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryLoggingConfigTypeDef](./type_defs.md#queryloggingconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueryLoggingConfigsResponseTypeDef

```python
# ListQueryLoggingConfigsResponseTypeDef definition

class ListQueryLoggingConfigsResponseTypeDef(TypedDict):
    QueryLoggingConfigs: List[QueryLoggingConfigTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QueryLoggingConfigTypeDef](./type_defs.md#queryloggingconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrafficPolicyInstanceResponseTypeDef

```python
# CreateTrafficPolicyInstanceResponseTypeDef definition

class CreateTrafficPolicyInstanceResponseTypeDef(TypedDict):
    TrafficPolicyInstance: TrafficPolicyInstanceTypeDef,  # (1)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyInstanceTypeDef](./type_defs.md#trafficpolicyinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrafficPolicyInstanceResponseTypeDef

```python
# GetTrafficPolicyInstanceResponseTypeDef definition

class GetTrafficPolicyInstanceResponseTypeDef(TypedDict):
    TrafficPolicyInstance: TrafficPolicyInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyInstanceTypeDef](./type_defs.md#trafficpolicyinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficPolicyInstancesByHostedZoneResponseTypeDef

```python
# ListTrafficPolicyInstancesByHostedZoneResponseTypeDef definition

class ListTrafficPolicyInstancesByHostedZoneResponseTypeDef(TypedDict):
    TrafficPolicyInstances: List[TrafficPolicyInstanceTypeDef],  # (1)
    TrafficPolicyInstanceNameMarker: str,
    TrafficPolicyInstanceTypeMarker: RRTypeType,  # (2)
    IsTruncated: bool,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TrafficPolicyInstanceTypeDef](./type_defs.md#trafficpolicyinstancetypedef) 
2. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficPolicyInstancesByPolicyResponseTypeDef

```python
# ListTrafficPolicyInstancesByPolicyResponseTypeDef definition

class ListTrafficPolicyInstancesByPolicyResponseTypeDef(TypedDict):
    TrafficPolicyInstances: List[TrafficPolicyInstanceTypeDef],  # (1)
    HostedZoneIdMarker: str,
    TrafficPolicyInstanceNameMarker: str,
    TrafficPolicyInstanceTypeMarker: RRTypeType,  # (2)
    IsTruncated: bool,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TrafficPolicyInstanceTypeDef](./type_defs.md#trafficpolicyinstancetypedef) 
2. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficPolicyInstancesResponseTypeDef

```python
# ListTrafficPolicyInstancesResponseTypeDef definition

class ListTrafficPolicyInstancesResponseTypeDef(TypedDict):
    TrafficPolicyInstances: List[TrafficPolicyInstanceTypeDef],  # (1)
    HostedZoneIdMarker: str,
    TrafficPolicyInstanceNameMarker: str,
    TrafficPolicyInstanceTypeMarker: RRTypeType,  # (2)
    IsTruncated: bool,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: TrafficPolicyInstanceTypeDef](./type_defs.md#trafficpolicyinstancetypedef) 
2. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrafficPolicyInstanceResponseTypeDef

```python
# UpdateTrafficPolicyInstanceResponseTypeDef definition

class UpdateTrafficPolicyInstanceResponseTypeDef(TypedDict):
    TrafficPolicyInstance: TrafficPolicyInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyInstanceTypeDef](./type_defs.md#trafficpolicyinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrafficPolicyResponseTypeDef

```python
# CreateTrafficPolicyResponseTypeDef definition

class CreateTrafficPolicyResponseTypeDef(TypedDict):
    TrafficPolicy: TrafficPolicyTypeDef,  # (1)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyTypeDef](./type_defs.md#trafficpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTrafficPolicyVersionResponseTypeDef

```python
# CreateTrafficPolicyVersionResponseTypeDef definition

class CreateTrafficPolicyVersionResponseTypeDef(TypedDict):
    TrafficPolicy: TrafficPolicyTypeDef,  # (1)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyTypeDef](./type_defs.md#trafficpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTrafficPolicyResponseTypeDef

```python
# GetTrafficPolicyResponseTypeDef definition

class GetTrafficPolicyResponseTypeDef(TypedDict):
    TrafficPolicy: TrafficPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyTypeDef](./type_defs.md#trafficpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficPolicyVersionsResponseTypeDef

```python
# ListTrafficPolicyVersionsResponseTypeDef definition

class ListTrafficPolicyVersionsResponseTypeDef(TypedDict):
    TrafficPolicies: List[TrafficPolicyTypeDef],  # (1)
    IsTruncated: bool,
    TrafficPolicyVersionMarker: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyTypeDef](./type_defs.md#trafficpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTrafficPolicyCommentResponseTypeDef

```python
# UpdateTrafficPolicyCommentResponseTypeDef definition

class UpdateTrafficPolicyCommentResponseTypeDef(TypedDict):
    TrafficPolicy: TrafficPolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicyTypeDef](./type_defs.md#trafficpolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDNSSECResponseTypeDef

```python
# GetDNSSECResponseTypeDef definition

class GetDNSSECResponseTypeDef(TypedDict):
    Status: DNSSECStatusTypeDef,  # (1)
    KeySigningKeys: List[KeySigningKeyTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DNSSECStatusTypeDef](./type_defs.md#dnssecstatustypedef) 
2. See [:material-code-braces: KeySigningKeyTypeDef](./type_defs.md#keysigningkeytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGeoLocationResponseTypeDef

```python
# GetGeoLocationResponseTypeDef definition

class GetGeoLocationResponseTypeDef(TypedDict):
    GeoLocationDetails: GeoLocationDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoLocationDetailsTypeDef](./type_defs.md#geolocationdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGeoLocationsResponseTypeDef

```python
# ListGeoLocationsResponseTypeDef definition

class ListGeoLocationsResponseTypeDef(TypedDict):
    GeoLocationDetailsList: List[GeoLocationDetailsTypeDef],  # (1)
    IsTruncated: bool,
    NextContinentCode: str,
    NextCountryCode: str,
    NextSubdivisionCode: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeoLocationDetailsTypeDef](./type_defs.md#geolocationdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChangeRequestResourceRecordSetsChangedWaitTypeDef

```python
# GetChangeRequestResourceRecordSetsChangedWaitTypeDef definition

class GetChangeRequestResourceRecordSetsChangedWaitTypeDef(TypedDict):
    Id: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetHostedZoneLimitResponseTypeDef

```python
# GetHostedZoneLimitResponseTypeDef definition

class GetHostedZoneLimitResponseTypeDef(TypedDict):
    Limit: HostedZoneLimitTypeDef,  # (1)
    Count: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HostedZoneLimitTypeDef](./type_defs.md#hostedzonelimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReusableDelegationSetLimitResponseTypeDef

```python
# GetReusableDelegationSetLimitResponseTypeDef definition

class GetReusableDelegationSetLimitResponseTypeDef(TypedDict):
    Limit: ReusableDelegationSetLimitTypeDef,  # (1)
    Count: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReusableDelegationSetLimitTypeDef](./type_defs.md#reusabledelegationsetlimittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HealthCheckObservationTypeDef

```python
# HealthCheckObservationTypeDef definition

class HealthCheckObservationTypeDef(TypedDict):
    Region: NotRequired[HealthCheckRegionType],  # (1)
    IPAddress: NotRequired[str],
    StatusReport: NotRequired[StatusReportTypeDef],  # (2)
```

1. See [:material-code-brackets: HealthCheckRegionType](./literals.md#healthcheckregiontype) 
2. See [:material-code-braces: StatusReportTypeDef](./type_defs.md#statusreporttypedef) 
## HostedZoneTypeDef

```python
# HostedZoneTypeDef definition

class HostedZoneTypeDef(TypedDict):
    Id: str,
    Name: str,
    CallerReference: str,
    Config: NotRequired[HostedZoneConfigTypeDef],  # (1)
    ResourceRecordSetCount: NotRequired[int],
    LinkedService: NotRequired[LinkedServiceTypeDef],  # (2)
```

1. See [:material-code-braces: HostedZoneConfigTypeDef](./type_defs.md#hostedzoneconfigtypedef) 
2. See [:material-code-braces: LinkedServiceTypeDef](./type_defs.md#linkedservicetypedef) 
## HostedZoneSummaryTypeDef

```python
# HostedZoneSummaryTypeDef definition

class HostedZoneSummaryTypeDef(TypedDict):
    HostedZoneId: str,
    Name: str,
    Owner: HostedZoneOwnerTypeDef,  # (1)
```

1. See [:material-code-braces: HostedZoneOwnerTypeDef](./type_defs.md#hostedzoneownertypedef) 
## ListCidrBlocksRequestListCidrBlocksPaginateTypeDef

```python
# ListCidrBlocksRequestListCidrBlocksPaginateTypeDef definition

class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(TypedDict):
    CollectionId: str,
    LocationName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef

```python
# ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef definition

class ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCidrLocationsRequestListCidrLocationsPaginateTypeDef

```python
# ListCidrLocationsRequestListCidrLocationsPaginateTypeDef definition

class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(TypedDict):
    CollectionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHealthChecksRequestListHealthChecksPaginateTypeDef

```python
# ListHealthChecksRequestListHealthChecksPaginateTypeDef definition

class ListHealthChecksRequestListHealthChecksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHostedZonesRequestListHostedZonesPaginateTypeDef

```python
# ListHostedZonesRequestListHostedZonesPaginateTypeDef definition

class ListHostedZonesRequestListHostedZonesPaginateTypeDef(TypedDict):
    DelegationSetId: NotRequired[str],
    HostedZoneType: NotRequired[HostedZoneTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: HostedZoneTypeType](./literals.md#hostedzonetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef

```python
# ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef definition

class ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef(TypedDict):
    HostedZoneId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef

```python
# ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef definition

class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(TypedDict):
    HostedZoneId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef

```python
# ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef definition

class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(TypedDict):
    HostedZoneId: str,
    MaxResults: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCidrLocationsResponseTypeDef

```python
# ListCidrLocationsResponseTypeDef definition

class ListCidrLocationsResponseTypeDef(TypedDict):
    CidrLocations: List[LocationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LocationSummaryTypeDef](./type_defs.md#locationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTrafficPoliciesResponseTypeDef

```python
# ListTrafficPoliciesResponseTypeDef definition

class ListTrafficPoliciesResponseTypeDef(TypedDict):
    TrafficPolicySummaries: List[TrafficPolicySummaryTypeDef],  # (1)
    IsTruncated: bool,
    TrafficPolicyIdMarker: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TrafficPolicySummaryTypeDef](./type_defs.md#trafficpolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHealthCheckRequestRequestTypeDef

```python
# CreateHealthCheckRequestRequestTypeDef definition

class CreateHealthCheckRequestRequestTypeDef(TypedDict):
    CallerReference: str,
    HealthCheckConfig: HealthCheckConfigTypeDef,  # (1)
```

1. See [:material-code-braces: HealthCheckConfigTypeDef](./type_defs.md#healthcheckconfigtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceTagSet: ResourceTagSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagSetTypeDef](./type_defs.md#resourcetagsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourcesResponseTypeDef

```python
# ListTagsForResourcesResponseTypeDef definition

class ListTagsForResourcesResponseTypeDef(TypedDict):
    ResourceTagSets: List[ResourceTagSetTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTagSetTypeDef](./type_defs.md#resourcetagsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HealthCheckTypeDef

```python
# HealthCheckTypeDef definition

class HealthCheckTypeDef(TypedDict):
    Id: str,
    CallerReference: str,
    HealthCheckConfig: HealthCheckConfigOutputTypeDef,  # (2)
    HealthCheckVersion: int,
    LinkedService: NotRequired[LinkedServiceTypeDef],  # (1)
    CloudWatchAlarmConfiguration: NotRequired[CloudWatchAlarmConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: LinkedServiceTypeDef](./type_defs.md#linkedservicetypedef) 
2. See [:material-code-braces: HealthCheckConfigOutputTypeDef](./type_defs.md#healthcheckconfigoutputtypedef) 
3. See [:material-code-braces: CloudWatchAlarmConfigurationTypeDef](./type_defs.md#cloudwatchalarmconfigurationtypedef) 
## ResourceRecordSetOutputTypeDef

```python
# ResourceRecordSetOutputTypeDef definition

class ResourceRecordSetOutputTypeDef(TypedDict):
    Name: str,
    Type: RRTypeType,  # (1)
    SetIdentifier: NotRequired[str],
    Weight: NotRequired[int],
    Region: NotRequired[ResourceRecordSetRegionType],  # (2)
    GeoLocation: NotRequired[GeoLocationTypeDef],  # (3)
    Failover: NotRequired[ResourceRecordSetFailoverType],  # (4)
    MultiValueAnswer: NotRequired[bool],
    TTL: NotRequired[int],
    ResourceRecords: NotRequired[List[ResourceRecordTypeDef]],  # (5)
    AliasTarget: NotRequired[AliasTargetTypeDef],  # (6)
    HealthCheckId: NotRequired[str],
    TrafficPolicyInstanceId: NotRequired[str],
    CidrRoutingConfig: NotRequired[CidrRoutingConfigTypeDef],  # (7)
    GeoProximityLocation: NotRequired[GeoProximityLocationTypeDef],  # (8)
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
2. See [:material-code-brackets: ResourceRecordSetRegionType](./literals.md#resourcerecordsetregiontype) 
3. See [:material-code-braces: GeoLocationTypeDef](./type_defs.md#geolocationtypedef) 
4. See [:material-code-brackets: ResourceRecordSetFailoverType](./literals.md#resourcerecordsetfailovertype) 
5. See [:material-code-braces: ResourceRecordTypeDef](./type_defs.md#resourcerecordtypedef) 
6. See [:material-code-braces: AliasTargetTypeDef](./type_defs.md#aliastargettypedef) 
7. See [:material-code-braces: CidrRoutingConfigTypeDef](./type_defs.md#cidrroutingconfigtypedef) 
8. See [:material-code-braces: GeoProximityLocationTypeDef](./type_defs.md#geoproximitylocationtypedef) 
## ResourceRecordSetTypeDef

```python
# ResourceRecordSetTypeDef definition

class ResourceRecordSetTypeDef(TypedDict):
    Name: str,
    Type: RRTypeType,  # (1)
    SetIdentifier: NotRequired[str],
    Weight: NotRequired[int],
    Region: NotRequired[ResourceRecordSetRegionType],  # (2)
    GeoLocation: NotRequired[GeoLocationTypeDef],  # (3)
    Failover: NotRequired[ResourceRecordSetFailoverType],  # (4)
    MultiValueAnswer: NotRequired[bool],
    TTL: NotRequired[int],
    ResourceRecords: NotRequired[Sequence[ResourceRecordTypeDef]],  # (5)
    AliasTarget: NotRequired[AliasTargetTypeDef],  # (6)
    HealthCheckId: NotRequired[str],
    TrafficPolicyInstanceId: NotRequired[str],
    CidrRoutingConfig: NotRequired[CidrRoutingConfigTypeDef],  # (7)
    GeoProximityLocation: NotRequired[GeoProximityLocationTypeDef],  # (8)
```

1. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
2. See [:material-code-brackets: ResourceRecordSetRegionType](./literals.md#resourcerecordsetregiontype) 
3. See [:material-code-braces: GeoLocationTypeDef](./type_defs.md#geolocationtypedef) 
4. See [:material-code-brackets: ResourceRecordSetFailoverType](./literals.md#resourcerecordsetfailovertype) 
5. See [:material-code-braces: ResourceRecordTypeDef](./type_defs.md#resourcerecordtypedef) 
6. See [:material-code-braces: AliasTargetTypeDef](./type_defs.md#aliastargettypedef) 
7. See [:material-code-braces: CidrRoutingConfigTypeDef](./type_defs.md#cidrroutingconfigtypedef) 
8. See [:material-code-braces: GeoProximityLocationTypeDef](./type_defs.md#geoproximitylocationtypedef) 
## GetHealthCheckLastFailureReasonResponseTypeDef

```python
# GetHealthCheckLastFailureReasonResponseTypeDef definition

class GetHealthCheckLastFailureReasonResponseTypeDef(TypedDict):
    HealthCheckObservations: List[HealthCheckObservationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HealthCheckObservationTypeDef](./type_defs.md#healthcheckobservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHealthCheckStatusResponseTypeDef

```python
# GetHealthCheckStatusResponseTypeDef definition

class GetHealthCheckStatusResponseTypeDef(TypedDict):
    HealthCheckObservations: List[HealthCheckObservationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HealthCheckObservationTypeDef](./type_defs.md#healthcheckobservationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHostedZoneResponseTypeDef

```python
# CreateHostedZoneResponseTypeDef definition

class CreateHostedZoneResponseTypeDef(TypedDict):
    HostedZone: HostedZoneTypeDef,  # (1)
    ChangeInfo: ChangeInfoTypeDef,  # (2)
    DelegationSet: DelegationSetTypeDef,  # (3)
    VPC: VPCTypeDef,  # (4)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: HostedZoneTypeDef](./type_defs.md#hostedzonetypedef) 
2. See [:material-code-braces: ChangeInfoTypeDef](./type_defs.md#changeinfotypedef) 
3. See [:material-code-braces: DelegationSetTypeDef](./type_defs.md#delegationsettypedef) 
4. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHostedZoneResponseTypeDef

```python
# GetHostedZoneResponseTypeDef definition

class GetHostedZoneResponseTypeDef(TypedDict):
    HostedZone: HostedZoneTypeDef,  # (1)
    DelegationSet: DelegationSetTypeDef,  # (2)
    VPCs: List[VPCTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: HostedZoneTypeDef](./type_defs.md#hostedzonetypedef) 
2. See [:material-code-braces: DelegationSetTypeDef](./type_defs.md#delegationsettypedef) 
3. See [:material-code-braces: VPCTypeDef](./type_defs.md#vpctypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHostedZonesByNameResponseTypeDef

```python
# ListHostedZonesByNameResponseTypeDef definition

class ListHostedZonesByNameResponseTypeDef(TypedDict):
    HostedZones: List[HostedZoneTypeDef],  # (1)
    DNSName: str,
    HostedZoneId: str,
    IsTruncated: bool,
    NextDNSName: str,
    NextHostedZoneId: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HostedZoneTypeDef](./type_defs.md#hostedzonetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHostedZonesResponseTypeDef

```python
# ListHostedZonesResponseTypeDef definition

class ListHostedZonesResponseTypeDef(TypedDict):
    HostedZones: List[HostedZoneTypeDef],  # (1)
    Marker: str,
    IsTruncated: bool,
    NextMarker: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HostedZoneTypeDef](./type_defs.md#hostedzonetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateHostedZoneCommentResponseTypeDef

```python
# UpdateHostedZoneCommentResponseTypeDef definition

class UpdateHostedZoneCommentResponseTypeDef(TypedDict):
    HostedZone: HostedZoneTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HostedZoneTypeDef](./type_defs.md#hostedzonetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHostedZonesByVPCResponseTypeDef

```python
# ListHostedZonesByVPCResponseTypeDef definition

class ListHostedZonesByVPCResponseTypeDef(TypedDict):
    HostedZoneSummaries: List[HostedZoneSummaryTypeDef],  # (1)
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HostedZoneSummaryTypeDef](./type_defs.md#hostedzonesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHealthCheckResponseTypeDef

```python
# CreateHealthCheckResponseTypeDef definition

class CreateHealthCheckResponseTypeDef(TypedDict):
    HealthCheck: HealthCheckTypeDef,  # (1)
    Location: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHealthCheckResponseTypeDef

```python
# GetHealthCheckResponseTypeDef definition

class GetHealthCheckResponseTypeDef(TypedDict):
    HealthCheck: HealthCheckTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHealthChecksResponseTypeDef

```python
# ListHealthChecksResponseTypeDef definition

class ListHealthChecksResponseTypeDef(TypedDict):
    HealthChecks: List[HealthCheckTypeDef],  # (1)
    Marker: str,
    IsTruncated: bool,
    NextMarker: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateHealthCheckResponseTypeDef

```python
# UpdateHealthCheckResponseTypeDef definition

class UpdateHealthCheckResponseTypeDef(TypedDict):
    HealthCheck: HealthCheckTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HealthCheckTypeDef](./type_defs.md#healthchecktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceRecordSetsResponseTypeDef

```python
# ListResourceRecordSetsResponseTypeDef definition

class ListResourceRecordSetsResponseTypeDef(TypedDict):
    ResourceRecordSets: List[ResourceRecordSetOutputTypeDef],  # (1)
    IsTruncated: bool,
    NextRecordName: str,
    NextRecordType: RRTypeType,  # (2)
    NextRecordIdentifier: str,
    MaxItems: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourceRecordSetOutputTypeDef](./type_defs.md#resourcerecordsetoutputtypedef) 
2. See [:material-code-brackets: RRTypeType](./literals.md#rrtypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeTypeDef

```python
# ChangeTypeDef definition

class ChangeTypeDef(TypedDict):
    Action: ChangeActionType,  # (1)
    ResourceRecordSet: ResourceRecordSetUnionTypeDef,  # (2)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-braces: ResourceRecordSetTypeDef](./type_defs.md#resourcerecordsettypedef) [:material-code-braces: ResourceRecordSetOutputTypeDef](./type_defs.md#resourcerecordsetoutputtypedef) 
## ChangeBatchTypeDef

```python
# ChangeBatchTypeDef definition

class ChangeBatchTypeDef(TypedDict):
    Changes: Sequence[ChangeTypeDef],  # (1)
    Comment: NotRequired[str],
```

1. See [:material-code-braces: ChangeTypeDef](./type_defs.md#changetypedef) 
## ChangeResourceRecordSetsRequestRequestTypeDef

```python
# ChangeResourceRecordSetsRequestRequestTypeDef definition

class ChangeResourceRecordSetsRequestRequestTypeDef(TypedDict):
    HostedZoneId: str,
    ChangeBatch: ChangeBatchTypeDef,  # (1)
```

1. See [:material-code-braces: ChangeBatchTypeDef](./type_defs.md#changebatchtypedef) 
