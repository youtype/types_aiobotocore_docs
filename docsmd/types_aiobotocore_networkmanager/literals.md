# Literals

> [Index](../README.md) > [NetworkManager](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [NetworkManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
    type annotations stubs module [types-aiobotocore-networkmanager](https://pypi.org/project/types-aiobotocore-networkmanager/).

## AttachmentStateType

```python
# AttachmentStateType usage example

from types_aiobotocore_networkmanager.literals import AttachmentStateType

def get_value() -> AttachmentStateType:
    return "AVAILABLE"
```

```python
# AttachmentStateType definition

AttachmentStateType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETING",
    "FAILED",
    "PENDING_ATTACHMENT_ACCEPTANCE",
    "PENDING_NETWORK_UPDATE",
    "PENDING_TAG_ACCEPTANCE",
    "REJECTED",
    "UPDATING",
]
```
## AttachmentTypeType

```python
# AttachmentTypeType usage example

from types_aiobotocore_networkmanager.literals import AttachmentTypeType

def get_value() -> AttachmentTypeType:
    return "CONNECT"
```

```python
# AttachmentTypeType definition

AttachmentTypeType = Literal[
    "CONNECT",
    "SITE_TO_SITE_VPN",
    "TRANSIT_GATEWAY_ROUTE_TABLE",
    "VPC",
]
```
## ChangeActionType

```python
# ChangeActionType usage example

from types_aiobotocore_networkmanager.literals import ChangeActionType

def get_value() -> ChangeActionType:
    return "ADD"
```

```python
# ChangeActionType definition

ChangeActionType = Literal[
    "ADD",
    "MODIFY",
    "REMOVE",
]
```
## ChangeSetStateType

```python
# ChangeSetStateType usage example

from types_aiobotocore_networkmanager.literals import ChangeSetStateType

def get_value() -> ChangeSetStateType:
    return "EXECUTING"
```

```python
# ChangeSetStateType definition

ChangeSetStateType = Literal[
    "EXECUTING",
    "EXECUTION_SUCCEEDED",
    "FAILED_GENERATION",
    "OUT_OF_DATE",
    "PENDING_GENERATION",
    "READY_TO_EXECUTE",
]
```
## ChangeStatusType

```python
# ChangeStatusType usage example

from types_aiobotocore_networkmanager.literals import ChangeStatusType

def get_value() -> ChangeStatusType:
    return "COMPLETE"
```

```python
# ChangeStatusType definition

ChangeStatusType = Literal[
    "COMPLETE",
    "FAILED",
    "IN_PROGRESS",
    "NOT_STARTED",
]
```
## ChangeTypeType

```python
# ChangeTypeType usage example

from types_aiobotocore_networkmanager.literals import ChangeTypeType

def get_value() -> ChangeTypeType:
    return "ATTACHMENT_MAPPING"
```

```python
# ChangeTypeType definition

ChangeTypeType = Literal[
    "ATTACHMENT_MAPPING",
    "ATTACHMENT_POLICIES_CONFIGURATION",
    "ATTACHMENT_ROUTE_PROPAGATION",
    "ATTACHMENT_ROUTE_STATIC",
    "CORE_NETWORK_CONFIGURATION",
    "CORE_NETWORK_EDGE",
    "CORE_NETWORK_SEGMENT",
    "SEGMENT_ACTIONS_CONFIGURATION",
    "SEGMENTS_CONFIGURATION",
]
```
## ConnectPeerAssociationStateType

```python
# ConnectPeerAssociationStateType usage example

from types_aiobotocore_networkmanager.literals import ConnectPeerAssociationStateType

def get_value() -> ConnectPeerAssociationStateType:
    return "AVAILABLE"
```

```python
# ConnectPeerAssociationStateType definition

ConnectPeerAssociationStateType = Literal[
    "AVAILABLE",
    "DELETED",
    "DELETING",
    "PENDING",
]
```
## ConnectPeerStateType

```python
# ConnectPeerStateType usage example

from types_aiobotocore_networkmanager.literals import ConnectPeerStateType

def get_value() -> ConnectPeerStateType:
    return "AVAILABLE"
```

```python
# ConnectPeerStateType definition

ConnectPeerStateType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETING",
    "FAILED",
]
```
## ConnectionStateType

```python
# ConnectionStateType usage example

from types_aiobotocore_networkmanager.literals import ConnectionStateType

def get_value() -> ConnectionStateType:
    return "AVAILABLE"
```

```python
# ConnectionStateType definition

ConnectionStateType = Literal[
    "AVAILABLE",
    "DELETING",
    "PENDING",
    "UPDATING",
]
```
## ConnectionStatusType

```python
# ConnectionStatusType usage example

from types_aiobotocore_networkmanager.literals import ConnectionStatusType

def get_value() -> ConnectionStatusType:
    return "DOWN"
```

```python
# ConnectionStatusType definition

ConnectionStatusType = Literal[
    "DOWN",
    "UP",
]
```
## ConnectionTypeType

```python
# ConnectionTypeType usage example

from types_aiobotocore_networkmanager.literals import ConnectionTypeType

def get_value() -> ConnectionTypeType:
    return "BGP"
```

```python
# ConnectionTypeType definition

ConnectionTypeType = Literal[
    "BGP",
    "IPSEC",
]
```
## CoreNetworkPolicyAliasType

```python
# CoreNetworkPolicyAliasType usage example

from types_aiobotocore_networkmanager.literals import CoreNetworkPolicyAliasType

def get_value() -> CoreNetworkPolicyAliasType:
    return "LATEST"
```

```python
# CoreNetworkPolicyAliasType definition

CoreNetworkPolicyAliasType = Literal[
    "LATEST",
    "LIVE",
]
```
## CoreNetworkStateType

```python
# CoreNetworkStateType usage example

from types_aiobotocore_networkmanager.literals import CoreNetworkStateType

def get_value() -> CoreNetworkStateType:
    return "AVAILABLE"
```

```python
# CoreNetworkStateType definition

CoreNetworkStateType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETING",
    "UPDATING",
]
```
## CustomerGatewayAssociationStateType

```python
# CustomerGatewayAssociationStateType usage example

from types_aiobotocore_networkmanager.literals import CustomerGatewayAssociationStateType

def get_value() -> CustomerGatewayAssociationStateType:
    return "AVAILABLE"
```

```python
# CustomerGatewayAssociationStateType definition

CustomerGatewayAssociationStateType = Literal[
    "AVAILABLE",
    "DELETED",
    "DELETING",
    "PENDING",
]
```
## DescribeGlobalNetworksPaginatorName

```python
# DescribeGlobalNetworksPaginatorName usage example

from types_aiobotocore_networkmanager.literals import DescribeGlobalNetworksPaginatorName

def get_value() -> DescribeGlobalNetworksPaginatorName:
    return "describe_global_networks"
```

```python
# DescribeGlobalNetworksPaginatorName definition

DescribeGlobalNetworksPaginatorName = Literal[
    "describe_global_networks",
]
```
## DeviceStateType

```python
# DeviceStateType usage example

from types_aiobotocore_networkmanager.literals import DeviceStateType

def get_value() -> DeviceStateType:
    return "AVAILABLE"
```

```python
# DeviceStateType definition

DeviceStateType = Literal[
    "AVAILABLE",
    "DELETING",
    "PENDING",
    "UPDATING",
]
```
## GetConnectPeerAssociationsPaginatorName

```python
# GetConnectPeerAssociationsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetConnectPeerAssociationsPaginatorName

def get_value() -> GetConnectPeerAssociationsPaginatorName:
    return "get_connect_peer_associations"
```

```python
# GetConnectPeerAssociationsPaginatorName definition

GetConnectPeerAssociationsPaginatorName = Literal[
    "get_connect_peer_associations",
]
```
## GetConnectionsPaginatorName

```python
# GetConnectionsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetConnectionsPaginatorName

def get_value() -> GetConnectionsPaginatorName:
    return "get_connections"
```

```python
# GetConnectionsPaginatorName definition

GetConnectionsPaginatorName = Literal[
    "get_connections",
]
```
## GetCoreNetworkChangeEventsPaginatorName

```python
# GetCoreNetworkChangeEventsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetCoreNetworkChangeEventsPaginatorName

def get_value() -> GetCoreNetworkChangeEventsPaginatorName:
    return "get_core_network_change_events"
```

```python
# GetCoreNetworkChangeEventsPaginatorName definition

GetCoreNetworkChangeEventsPaginatorName = Literal[
    "get_core_network_change_events",
]
```
## GetCoreNetworkChangeSetPaginatorName

```python
# GetCoreNetworkChangeSetPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetCoreNetworkChangeSetPaginatorName

def get_value() -> GetCoreNetworkChangeSetPaginatorName:
    return "get_core_network_change_set"
```

```python
# GetCoreNetworkChangeSetPaginatorName definition

GetCoreNetworkChangeSetPaginatorName = Literal[
    "get_core_network_change_set",
]
```
## GetCustomerGatewayAssociationsPaginatorName

```python
# GetCustomerGatewayAssociationsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetCustomerGatewayAssociationsPaginatorName

def get_value() -> GetCustomerGatewayAssociationsPaginatorName:
    return "get_customer_gateway_associations"
```

```python
# GetCustomerGatewayAssociationsPaginatorName definition

GetCustomerGatewayAssociationsPaginatorName = Literal[
    "get_customer_gateway_associations",
]
```
## GetDevicesPaginatorName

```python
# GetDevicesPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetDevicesPaginatorName

def get_value() -> GetDevicesPaginatorName:
    return "get_devices"
```

```python
# GetDevicesPaginatorName definition

GetDevicesPaginatorName = Literal[
    "get_devices",
]
```
## GetLinkAssociationsPaginatorName

```python
# GetLinkAssociationsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetLinkAssociationsPaginatorName

def get_value() -> GetLinkAssociationsPaginatorName:
    return "get_link_associations"
```

```python
# GetLinkAssociationsPaginatorName definition

GetLinkAssociationsPaginatorName = Literal[
    "get_link_associations",
]
```
## GetLinksPaginatorName

```python
# GetLinksPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetLinksPaginatorName

def get_value() -> GetLinksPaginatorName:
    return "get_links"
```

```python
# GetLinksPaginatorName definition

GetLinksPaginatorName = Literal[
    "get_links",
]
```
## GetNetworkResourceCountsPaginatorName

```python
# GetNetworkResourceCountsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetNetworkResourceCountsPaginatorName

def get_value() -> GetNetworkResourceCountsPaginatorName:
    return "get_network_resource_counts"
```

```python
# GetNetworkResourceCountsPaginatorName definition

GetNetworkResourceCountsPaginatorName = Literal[
    "get_network_resource_counts",
]
```
## GetNetworkResourceRelationshipsPaginatorName

```python
# GetNetworkResourceRelationshipsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetNetworkResourceRelationshipsPaginatorName

def get_value() -> GetNetworkResourceRelationshipsPaginatorName:
    return "get_network_resource_relationships"
```

```python
# GetNetworkResourceRelationshipsPaginatorName definition

GetNetworkResourceRelationshipsPaginatorName = Literal[
    "get_network_resource_relationships",
]
```
## GetNetworkResourcesPaginatorName

```python
# GetNetworkResourcesPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetNetworkResourcesPaginatorName

def get_value() -> GetNetworkResourcesPaginatorName:
    return "get_network_resources"
```

```python
# GetNetworkResourcesPaginatorName definition

GetNetworkResourcesPaginatorName = Literal[
    "get_network_resources",
]
```
## GetNetworkTelemetryPaginatorName

```python
# GetNetworkTelemetryPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetNetworkTelemetryPaginatorName

def get_value() -> GetNetworkTelemetryPaginatorName:
    return "get_network_telemetry"
```

```python
# GetNetworkTelemetryPaginatorName definition

GetNetworkTelemetryPaginatorName = Literal[
    "get_network_telemetry",
]
```
## GetSitesPaginatorName

```python
# GetSitesPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetSitesPaginatorName

def get_value() -> GetSitesPaginatorName:
    return "get_sites"
```

```python
# GetSitesPaginatorName definition

GetSitesPaginatorName = Literal[
    "get_sites",
]
```
## GetTransitGatewayConnectPeerAssociationsPaginatorName

```python
# GetTransitGatewayConnectPeerAssociationsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetTransitGatewayConnectPeerAssociationsPaginatorName

def get_value() -> GetTransitGatewayConnectPeerAssociationsPaginatorName:
    return "get_transit_gateway_connect_peer_associations"
```

```python
# GetTransitGatewayConnectPeerAssociationsPaginatorName definition

GetTransitGatewayConnectPeerAssociationsPaginatorName = Literal[
    "get_transit_gateway_connect_peer_associations",
]
```
## GetTransitGatewayRegistrationsPaginatorName

```python
# GetTransitGatewayRegistrationsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import GetTransitGatewayRegistrationsPaginatorName

def get_value() -> GetTransitGatewayRegistrationsPaginatorName:
    return "get_transit_gateway_registrations"
```

```python
# GetTransitGatewayRegistrationsPaginatorName definition

GetTransitGatewayRegistrationsPaginatorName = Literal[
    "get_transit_gateway_registrations",
]
```
## GlobalNetworkStateType

```python
# GlobalNetworkStateType usage example

from types_aiobotocore_networkmanager.literals import GlobalNetworkStateType

def get_value() -> GlobalNetworkStateType:
    return "AVAILABLE"
```

```python
# GlobalNetworkStateType definition

GlobalNetworkStateType = Literal[
    "AVAILABLE",
    "DELETING",
    "PENDING",
    "UPDATING",
]
```
## LinkAssociationStateType

```python
# LinkAssociationStateType usage example

from types_aiobotocore_networkmanager.literals import LinkAssociationStateType

def get_value() -> LinkAssociationStateType:
    return "AVAILABLE"
```

```python
# LinkAssociationStateType definition

LinkAssociationStateType = Literal[
    "AVAILABLE",
    "DELETED",
    "DELETING",
    "PENDING",
]
```
## LinkStateType

```python
# LinkStateType usage example

from types_aiobotocore_networkmanager.literals import LinkStateType

def get_value() -> LinkStateType:
    return "AVAILABLE"
```

```python
# LinkStateType definition

LinkStateType = Literal[
    "AVAILABLE",
    "DELETING",
    "PENDING",
    "UPDATING",
]
```
## ListAttachmentsPaginatorName

```python
# ListAttachmentsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import ListAttachmentsPaginatorName

def get_value() -> ListAttachmentsPaginatorName:
    return "list_attachments"
```

```python
# ListAttachmentsPaginatorName definition

ListAttachmentsPaginatorName = Literal[
    "list_attachments",
]
```
## ListConnectPeersPaginatorName

```python
# ListConnectPeersPaginatorName usage example

from types_aiobotocore_networkmanager.literals import ListConnectPeersPaginatorName

def get_value() -> ListConnectPeersPaginatorName:
    return "list_connect_peers"
```

```python
# ListConnectPeersPaginatorName definition

ListConnectPeersPaginatorName = Literal[
    "list_connect_peers",
]
```
## ListCoreNetworkPolicyVersionsPaginatorName

```python
# ListCoreNetworkPolicyVersionsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import ListCoreNetworkPolicyVersionsPaginatorName

def get_value() -> ListCoreNetworkPolicyVersionsPaginatorName:
    return "list_core_network_policy_versions"
```

```python
# ListCoreNetworkPolicyVersionsPaginatorName definition

ListCoreNetworkPolicyVersionsPaginatorName = Literal[
    "list_core_network_policy_versions",
]
```
## ListCoreNetworksPaginatorName

```python
# ListCoreNetworksPaginatorName usage example

from types_aiobotocore_networkmanager.literals import ListCoreNetworksPaginatorName

def get_value() -> ListCoreNetworksPaginatorName:
    return "list_core_networks"
```

```python
# ListCoreNetworksPaginatorName definition

ListCoreNetworksPaginatorName = Literal[
    "list_core_networks",
]
```
## ListPeeringsPaginatorName

```python
# ListPeeringsPaginatorName usage example

from types_aiobotocore_networkmanager.literals import ListPeeringsPaginatorName

def get_value() -> ListPeeringsPaginatorName:
    return "list_peerings"
```

```python
# ListPeeringsPaginatorName definition

ListPeeringsPaginatorName = Literal[
    "list_peerings",
]
```
## PeeringStateType

```python
# PeeringStateType usage example

from types_aiobotocore_networkmanager.literals import PeeringStateType

def get_value() -> PeeringStateType:
    return "AVAILABLE"
```

```python
# PeeringStateType definition

PeeringStateType = Literal[
    "AVAILABLE",
    "CREATING",
    "DELETING",
    "FAILED",
]
```
## PeeringTypeType

```python
# PeeringTypeType usage example

from types_aiobotocore_networkmanager.literals import PeeringTypeType

def get_value() -> PeeringTypeType:
    return "TRANSIT_GATEWAY"
```

```python
# PeeringTypeType definition

PeeringTypeType = Literal[
    "TRANSIT_GATEWAY",
]
```
## RouteAnalysisCompletionReasonCodeType

```python
# RouteAnalysisCompletionReasonCodeType usage example

from types_aiobotocore_networkmanager.literals import RouteAnalysisCompletionReasonCodeType

def get_value() -> RouteAnalysisCompletionReasonCodeType:
    return "BLACKHOLE_ROUTE_FOR_DESTINATION_FOUND"
```

```python
# RouteAnalysisCompletionReasonCodeType definition

RouteAnalysisCompletionReasonCodeType = Literal[
    "BLACKHOLE_ROUTE_FOR_DESTINATION_FOUND",
    "CYCLIC_PATH_DETECTED",
    "INACTIVE_ROUTE_FOR_DESTINATION_FOUND",
    "MAX_HOPS_EXCEEDED",
    "NO_DESTINATION_ARN_PROVIDED",
    "POSSIBLE_MIDDLEBOX",
    "ROUTE_NOT_FOUND",
    "TRANSIT_GATEWAY_ATTACHMENT_ATTACH_ARN_NO_MATCH",
    "TRANSIT_GATEWAY_ATTACHMENT_NOT_FOUND",
    "TRANSIT_GATEWAY_ATTACHMENT_NOT_IN_TRANSIT_GATEWAY",
    "TRANSIT_GATEWAY_ATTACHMENT_STABLE_ROUTE_TABLE_NOT_FOUND",
]
```
## RouteAnalysisCompletionResultCodeType

```python
# RouteAnalysisCompletionResultCodeType usage example

from types_aiobotocore_networkmanager.literals import RouteAnalysisCompletionResultCodeType

def get_value() -> RouteAnalysisCompletionResultCodeType:
    return "CONNECTED"
```

```python
# RouteAnalysisCompletionResultCodeType definition

RouteAnalysisCompletionResultCodeType = Literal[
    "CONNECTED",
    "NOT_CONNECTED",
]
```
## RouteAnalysisStatusType

```python
# RouteAnalysisStatusType usage example

from types_aiobotocore_networkmanager.literals import RouteAnalysisStatusType

def get_value() -> RouteAnalysisStatusType:
    return "COMPLETED"
```

```python
# RouteAnalysisStatusType definition

RouteAnalysisStatusType = Literal[
    "COMPLETED",
    "FAILED",
    "RUNNING",
]
```
## RouteStateType

```python
# RouteStateType usage example

from types_aiobotocore_networkmanager.literals import RouteStateType

def get_value() -> RouteStateType:
    return "ACTIVE"
```

```python
# RouteStateType definition

RouteStateType = Literal[
    "ACTIVE",
    "BLACKHOLE",
]
```
## RouteTableTypeType

```python
# RouteTableTypeType usage example

from types_aiobotocore_networkmanager.literals import RouteTableTypeType

def get_value() -> RouteTableTypeType:
    return "CORE_NETWORK_SEGMENT"
```

```python
# RouteTableTypeType definition

RouteTableTypeType = Literal[
    "CORE_NETWORK_SEGMENT",
    "TRANSIT_GATEWAY_ROUTE_TABLE",
]
```
## RouteTypeType

```python
# RouteTypeType usage example

from types_aiobotocore_networkmanager.literals import RouteTypeType

def get_value() -> RouteTypeType:
    return "PROPAGATED"
```

```python
# RouteTypeType definition

RouteTypeType = Literal[
    "PROPAGATED",
    "STATIC",
]
```
## SiteStateType

```python
# SiteStateType usage example

from types_aiobotocore_networkmanager.literals import SiteStateType

def get_value() -> SiteStateType:
    return "AVAILABLE"
```

```python
# SiteStateType definition

SiteStateType = Literal[
    "AVAILABLE",
    "DELETING",
    "PENDING",
    "UPDATING",
]
```
## TransitGatewayConnectPeerAssociationStateType

```python
# TransitGatewayConnectPeerAssociationStateType usage example

from types_aiobotocore_networkmanager.literals import TransitGatewayConnectPeerAssociationStateType

def get_value() -> TransitGatewayConnectPeerAssociationStateType:
    return "AVAILABLE"
```

```python
# TransitGatewayConnectPeerAssociationStateType definition

TransitGatewayConnectPeerAssociationStateType = Literal[
    "AVAILABLE",
    "DELETED",
    "DELETING",
    "PENDING",
]
```
## TransitGatewayRegistrationStateType

```python
# TransitGatewayRegistrationStateType usage example

from types_aiobotocore_networkmanager.literals import TransitGatewayRegistrationStateType

def get_value() -> TransitGatewayRegistrationStateType:
    return "AVAILABLE"
```

```python
# TransitGatewayRegistrationStateType definition

TransitGatewayRegistrationStateType = Literal[
    "AVAILABLE",
    "DELETED",
    "DELETING",
    "FAILED",
    "PENDING",
]
```
## TunnelProtocolType

```python
# TunnelProtocolType usage example

from types_aiobotocore_networkmanager.literals import TunnelProtocolType

def get_value() -> TunnelProtocolType:
    return "GRE"
```

```python
# TunnelProtocolType definition

TunnelProtocolType = Literal[
    "GRE",
]
```
## NetworkManagerServiceName

```python
# NetworkManagerServiceName usage example

from types_aiobotocore_networkmanager.literals import NetworkManagerServiceName

def get_value() -> NetworkManagerServiceName:
    return "networkmanager"
```

```python
# NetworkManagerServiceName definition

NetworkManagerServiceName = Literal[
    "networkmanager",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_networkmanager.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_networkmanager.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_networkmanager.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_global_networks"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "describe_global_networks",
    "get_connect_peer_associations",
    "get_connections",
    "get_core_network_change_events",
    "get_core_network_change_set",
    "get_customer_gateway_associations",
    "get_devices",
    "get_link_associations",
    "get_links",
    "get_network_resource_counts",
    "get_network_resource_relationships",
    "get_network_resources",
    "get_network_telemetry",
    "get_sites",
    "get_transit_gateway_connect_peer_associations",
    "get_transit_gateway_registrations",
    "list_attachments",
    "list_connect_peers",
    "list_core_network_policy_versions",
    "list_core_networks",
    "list_peerings",
]
```
