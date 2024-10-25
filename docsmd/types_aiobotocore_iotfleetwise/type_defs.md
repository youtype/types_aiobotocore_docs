# Type definitions

> [Index](../README.md) > [IoTFleetWise](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTFleetWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
    type annotations stubs module [types-aiobotocore-iotfleetwise](https://pypi.org/project/types-aiobotocore-iotfleetwise/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ActuatorUnionTypeDef

```python
# ActuatorUnionTypeDef definition

ActuatorUnionTypeDef = Union[
    ActuatorTypeDef,  # (1)
    ActuatorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActuatorTypeDef](./type_defs.md#actuatortypedef) 
2. See [:material-code-braces: ActuatorOutputTypeDef](./type_defs.md#actuatoroutputtypedef) 

## AttributeUnionTypeDef

```python
# AttributeUnionTypeDef definition

AttributeUnionTypeDef = Union[
    AttributeTypeDef,  # (1)
    AttributeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: AttributeOutputTypeDef](./type_defs.md#attributeoutputtypedef) 

## SensorUnionTypeDef

```python
# SensorUnionTypeDef definition

SensorUnionTypeDef = Union[
    SensorTypeDef,  # (1)
    SensorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SensorTypeDef](./type_defs.md#sensortypedef) 
2. See [:material-code-braces: SensorOutputTypeDef](./type_defs.md#sensoroutputtypedef) 

## StructuredMessageFieldNameAndDataTypePairUnionTypeDef

```python
# StructuredMessageFieldNameAndDataTypePairUnionTypeDef definition

StructuredMessageFieldNameAndDataTypePairUnionTypeDef = Union[
    StructuredMessageFieldNameAndDataTypePairTypeDef,  # (1)
    StructuredMessageFieldNameAndDataTypePairOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StructuredMessageFieldNameAndDataTypePairTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairtypedef) 
2. See [:material-code-braces: StructuredMessageFieldNameAndDataTypePairOutputTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairoutputtypedef) 

## StructuredMessageListDefinitionUnionTypeDef

```python
# StructuredMessageListDefinitionUnionTypeDef definition

StructuredMessageListDefinitionUnionTypeDef = Union[
    StructuredMessageListDefinitionTypeDef,  # (1)
    StructuredMessageListDefinitionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StructuredMessageListDefinitionTypeDef](./type_defs.md#structuredmessagelistdefinitiontypedef) 
2. See [:material-code-braces: StructuredMessageListDefinitionOutputTypeDef](./type_defs.md#structuredmessagelistdefinitionoutputtypedef) 

## NodeUnionTypeDef

```python
# NodeUnionTypeDef definition

NodeUnionTypeDef = Union[
    NodeTypeDef,  # (1)
    NodeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
2. See [:material-code-braces: NodeOutputTypeDef](./type_defs.md#nodeoutputtypedef) 

## StructuredMessageUnionTypeDef

```python
# StructuredMessageUnionTypeDef definition

StructuredMessageUnionTypeDef = Union[
    StructuredMessageTypeDef,  # (1)
    StructuredMessageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StructuredMessageTypeDef](./type_defs.md#structuredmessagetypedef) 
2. See [:material-code-braces: StructuredMessageOutputTypeDef](./type_defs.md#structuredmessageoutputtypedef) 

## MessageSignalUnionTypeDef

```python
# MessageSignalUnionTypeDef definition

MessageSignalUnionTypeDef = Union[
    MessageSignalTypeDef,  # (1)
    MessageSignalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageSignalTypeDef](./type_defs.md#messagesignaltypedef) 
2. See [:material-code-braces: MessageSignalOutputTypeDef](./type_defs.md#messagesignaloutputtypedef) 

## SignalDecoderUnionTypeDef

```python
# SignalDecoderUnionTypeDef definition

SignalDecoderUnionTypeDef = Union[
    SignalDecoderTypeDef,  # (1)
    SignalDecoderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SignalDecoderTypeDef](./type_defs.md#signaldecodertypedef) 
2. See [:material-code-braces: SignalDecoderOutputTypeDef](./type_defs.md#signaldecoderoutputtypedef) 



## ActuatorOutputTypeDef

```python
# ActuatorOutputTypeDef definition

class ActuatorOutputTypeDef(TypedDict):
    fullyQualifiedName: str,
    dataType: NodeDataTypeType,  # (1)
    description: NotRequired[str],
    unit: NotRequired[str],
    allowedValues: NotRequired[List[str]],
    min: NotRequired[float],
    max: NotRequired[float],
    assignedValue: NotRequired[str],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
    structFullyQualifiedName: NotRequired[str],
```

1. See [:material-code-brackets: NodeDataTypeType](./literals.md#nodedatatypetype) 
## ActuatorTypeDef

```python
# ActuatorTypeDef definition

class ActuatorTypeDef(TypedDict):
    fullyQualifiedName: str,
    dataType: NodeDataTypeType,  # (1)
    description: NotRequired[str],
    unit: NotRequired[str],
    allowedValues: NotRequired[Sequence[str]],
    min: NotRequired[float],
    max: NotRequired[float],
    assignedValue: NotRequired[str],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
    structFullyQualifiedName: NotRequired[str],
```

1. See [:material-code-brackets: NodeDataTypeType](./literals.md#nodedatatypetype) 
## AssociateVehicleFleetRequestRequestTypeDef

```python
# AssociateVehicleFleetRequestRequestTypeDef definition

class AssociateVehicleFleetRequestRequestTypeDef(TypedDict):
    vehicleName: str,
    fleetId: str,
```

## AttributeOutputTypeDef

```python
# AttributeOutputTypeDef definition

class AttributeOutputTypeDef(TypedDict):
    fullyQualifiedName: str,
    dataType: NodeDataTypeType,  # (1)
    description: NotRequired[str],
    unit: NotRequired[str],
    allowedValues: NotRequired[List[str]],
    min: NotRequired[float],
    max: NotRequired[float],
    assignedValue: NotRequired[str],
    defaultValue: NotRequired[str],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
```

1. See [:material-code-brackets: NodeDataTypeType](./literals.md#nodedatatypetype) 
## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    fullyQualifiedName: str,
    dataType: NodeDataTypeType,  # (1)
    description: NotRequired[str],
    unit: NotRequired[str],
    allowedValues: NotRequired[Sequence[str]],
    min: NotRequired[float],
    max: NotRequired[float],
    assignedValue: NotRequired[str],
    defaultValue: NotRequired[str],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
```

1. See [:material-code-brackets: NodeDataTypeType](./literals.md#nodedatatypetype) 
## CreateVehicleErrorTypeDef

```python
# CreateVehicleErrorTypeDef definition

class CreateVehicleErrorTypeDef(TypedDict):
    vehicleName: NotRequired[str],
    code: NotRequired[str],
    message: NotRequired[str],
```

## CreateVehicleResponseItemTypeDef

```python
# CreateVehicleResponseItemTypeDef definition

class CreateVehicleResponseItemTypeDef(TypedDict):
    vehicleName: NotRequired[str],
    arn: NotRequired[str],
    thingArn: NotRequired[str],
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

## UpdateVehicleRequestItemTypeDef

```python
# UpdateVehicleRequestItemTypeDef definition

class UpdateVehicleRequestItemTypeDef(TypedDict):
    vehicleName: str,
    modelManifestArn: NotRequired[str],
    decoderManifestArn: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    attributeUpdateMode: NotRequired[UpdateModeType],  # (1)
```

1. See [:material-code-brackets: UpdateModeType](./literals.md#updatemodetype) 
## UpdateVehicleErrorTypeDef

```python
# UpdateVehicleErrorTypeDef definition

class UpdateVehicleErrorTypeDef(TypedDict):
    vehicleName: NotRequired[str],
    code: NotRequired[int],
    message: NotRequired[str],
```

## UpdateVehicleResponseItemTypeDef

```python
# UpdateVehicleResponseItemTypeDef definition

class UpdateVehicleResponseItemTypeDef(TypedDict):
    vehicleName: NotRequired[str],
    arn: NotRequired[str],
```

## BranchTypeDef

```python
# BranchTypeDef definition

class BranchTypeDef(TypedDict):
    fullyQualifiedName: str,
    description: NotRequired[str],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
```

## CampaignSummaryTypeDef

```python
# CampaignSummaryTypeDef definition

class CampaignSummaryTypeDef(TypedDict):
    creationTime: datetime,
    lastModificationTime: datetime,
    arn: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    signalCatalogArn: NotRequired[str],
    targetArn: NotRequired[str],
    status: NotRequired[CampaignStatusType],  # (1)
```

1. See [:material-code-brackets: CampaignStatusType](./literals.md#campaignstatustype) 
## CanInterfaceTypeDef

```python
# CanInterfaceTypeDef definition

class CanInterfaceTypeDef(TypedDict):
    name: str,
    protocolName: NotRequired[str],
    protocolVersion: NotRequired[str],
```

## CanSignalTypeDef

```python
# CanSignalTypeDef definition

class CanSignalTypeDef(TypedDict):
    messageId: int,
    isBigEndian: bool,
    isSigned: bool,
    startBit: int,
    offset: float,
    factor: float,
    length: int,
    name: NotRequired[str],
```

## CloudWatchLogDeliveryOptionsTypeDef

```python
# CloudWatchLogDeliveryOptionsTypeDef definition

class CloudWatchLogDeliveryOptionsTypeDef(TypedDict):
    logType: LogTypeType,  # (1)
    logGroupName: NotRequired[str],
```

1. See [:material-code-brackets: LogTypeType](./literals.md#logtypetype) 
## ConditionBasedCollectionSchemeTypeDef

```python
# ConditionBasedCollectionSchemeTypeDef definition

class ConditionBasedCollectionSchemeTypeDef(TypedDict):
    expression: str,
    minimumTriggerIntervalMs: NotRequired[int],
    triggerMode: NotRequired[TriggerModeType],  # (1)
    conditionLanguageVersion: NotRequired[int],
```

1. See [:material-code-brackets: TriggerModeType](./literals.md#triggermodetype) 
## TimeBasedCollectionSchemeTypeDef

```python
# TimeBasedCollectionSchemeTypeDef definition

class TimeBasedCollectionSchemeTypeDef(TypedDict):
    periodMs: int,
```

## SignalInformationTypeDef

```python
# SignalInformationTypeDef definition

class SignalInformationTypeDef(TypedDict):
    name: str,
    maxSampleCount: NotRequired[int],
    minimumSamplingIntervalMs: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CustomPropertyTypeDef

```python
# CustomPropertyTypeDef definition

class CustomPropertyTypeDef(TypedDict):
    fullyQualifiedName: str,
    dataType: NodeDataTypeType,  # (1)
    dataEncoding: NotRequired[NodeDataEncodingType],  # (2)
    description: NotRequired[str],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
    structFullyQualifiedName: NotRequired[str],
```

1. See [:material-code-brackets: NodeDataTypeType](./literals.md#nodedatatypetype) 
2. See [:material-code-brackets: NodeDataEncodingType](./literals.md#nodedataencodingtype) 
## CustomStructTypeDef

```python
# CustomStructTypeDef definition

class CustomStructTypeDef(TypedDict):
    fullyQualifiedName: str,
    description: NotRequired[str],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
```

## S3ConfigTypeDef

```python
# S3ConfigTypeDef definition

class S3ConfigTypeDef(TypedDict):
    bucketArn: str,
    dataFormat: NotRequired[DataFormatType],  # (1)
    storageCompressionFormat: NotRequired[StorageCompressionFormatType],  # (2)
    prefix: NotRequired[str],
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: StorageCompressionFormatType](./literals.md#storagecompressionformattype) 
## TimestreamConfigTypeDef

```python
# TimestreamConfigTypeDef definition

class TimestreamConfigTypeDef(TypedDict):
    timestreamTableArn: str,
    executionRoleArn: str,
```

## DecoderManifestSummaryTypeDef

```python
# DecoderManifestSummaryTypeDef definition

class DecoderManifestSummaryTypeDef(TypedDict):
    creationTime: datetime,
    lastModificationTime: datetime,
    name: NotRequired[str],
    arn: NotRequired[str],
    modelManifestArn: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[ManifestStatusType],  # (1)
    message: NotRequired[str],
```

1. See [:material-code-brackets: ManifestStatusType](./literals.md#manifeststatustype) 
## DeleteCampaignRequestRequestTypeDef

```python
# DeleteCampaignRequestRequestTypeDef definition

class DeleteCampaignRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteDecoderManifestRequestRequestTypeDef

```python
# DeleteDecoderManifestRequestRequestTypeDef definition

class DeleteDecoderManifestRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteFleetRequestRequestTypeDef

```python
# DeleteFleetRequestRequestTypeDef definition

class DeleteFleetRequestRequestTypeDef(TypedDict):
    fleetId: str,
```

## DeleteModelManifestRequestRequestTypeDef

```python
# DeleteModelManifestRequestRequestTypeDef definition

class DeleteModelManifestRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteSignalCatalogRequestRequestTypeDef

```python
# DeleteSignalCatalogRequestRequestTypeDef definition

class DeleteSignalCatalogRequestRequestTypeDef(TypedDict):
    name: str,
```

## DeleteVehicleRequestRequestTypeDef

```python
# DeleteVehicleRequestRequestTypeDef definition

class DeleteVehicleRequestRequestTypeDef(TypedDict):
    vehicleName: str,
```

## DisassociateVehicleFleetRequestRequestTypeDef

```python
# DisassociateVehicleFleetRequestRequestTypeDef definition

class DisassociateVehicleFleetRequestRequestTypeDef(TypedDict):
    vehicleName: str,
    fleetId: str,
```

## FleetSummaryTypeDef

```python
# FleetSummaryTypeDef definition

class FleetSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    signalCatalogArn: str,
    creationTime: datetime,
    description: NotRequired[str],
    lastModificationTime: NotRequired[datetime],
```

## FormattedVssTypeDef

```python
# FormattedVssTypeDef definition

class FormattedVssTypeDef(TypedDict):
    vssJson: NotRequired[str],
```

## GetCampaignRequestRequestTypeDef

```python
# GetCampaignRequestRequestTypeDef definition

class GetCampaignRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetDecoderManifestRequestRequestTypeDef

```python
# GetDecoderManifestRequestRequestTypeDef definition

class GetDecoderManifestRequestRequestTypeDef(TypedDict):
    name: str,
```

## GetFleetRequestRequestTypeDef

```python
# GetFleetRequestRequestTypeDef definition

class GetFleetRequestRequestTypeDef(TypedDict):
    fleetId: str,
```

## GetModelManifestRequestRequestTypeDef

```python
# GetModelManifestRequestRequestTypeDef definition

class GetModelManifestRequestRequestTypeDef(TypedDict):
    name: str,
```

## IamRegistrationResponseTypeDef

```python
# IamRegistrationResponseTypeDef definition

class IamRegistrationResponseTypeDef(TypedDict):
    roleArn: str,
    registrationStatus: RegistrationStatusType,  # (1)
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## TimestreamRegistrationResponseTypeDef

```python
# TimestreamRegistrationResponseTypeDef definition

class TimestreamRegistrationResponseTypeDef(TypedDict):
    timestreamDatabaseName: str,
    timestreamTableName: str,
    registrationStatus: RegistrationStatusType,  # (1)
    timestreamDatabaseArn: NotRequired[str],
    timestreamTableArn: NotRequired[str],
    errorMessage: NotRequired[str],
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
## GetSignalCatalogRequestRequestTypeDef

```python
# GetSignalCatalogRequestRequestTypeDef definition

class GetSignalCatalogRequestRequestTypeDef(TypedDict):
    name: str,
```

## NodeCountsTypeDef

```python
# NodeCountsTypeDef definition

class NodeCountsTypeDef(TypedDict):
    totalNodes: NotRequired[int],
    totalBranches: NotRequired[int],
    totalSensors: NotRequired[int],
    totalAttributes: NotRequired[int],
    totalActuators: NotRequired[int],
    totalStructs: NotRequired[int],
    totalProperties: NotRequired[int],
```

## GetVehicleRequestRequestTypeDef

```python
# GetVehicleRequestRequestTypeDef definition

class GetVehicleRequestRequestTypeDef(TypedDict):
    vehicleName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetVehicleStatusRequestRequestTypeDef

```python
# GetVehicleStatusRequestRequestTypeDef definition

class GetVehicleStatusRequestRequestTypeDef(TypedDict):
    vehicleName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## VehicleStatusTypeDef

```python
# VehicleStatusTypeDef definition

class VehicleStatusTypeDef(TypedDict):
    campaignName: NotRequired[str],
    vehicleName: NotRequired[str],
    status: NotRequired[VehicleStateType],  # (1)
```

1. See [:material-code-brackets: VehicleStateType](./literals.md#vehiclestatetype) 
## IamResourcesTypeDef

```python
# IamResourcesTypeDef definition

class IamResourcesTypeDef(TypedDict):
    roleArn: str,
```

## ListCampaignsRequestRequestTypeDef

```python
# ListCampaignsRequestRequestTypeDef definition

class ListCampaignsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    status: NotRequired[str],
```

## ListDecoderManifestNetworkInterfacesRequestRequestTypeDef

```python
# ListDecoderManifestNetworkInterfacesRequestRequestTypeDef definition

class ListDecoderManifestNetworkInterfacesRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDecoderManifestSignalsRequestRequestTypeDef

```python
# ListDecoderManifestSignalsRequestRequestTypeDef definition

class ListDecoderManifestSignalsRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDecoderManifestsRequestRequestTypeDef

```python
# ListDecoderManifestsRequestRequestTypeDef definition

class ListDecoderManifestsRequestRequestTypeDef(TypedDict):
    modelManifestArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFleetsForVehicleRequestRequestTypeDef

```python
# ListFleetsForVehicleRequestRequestTypeDef definition

class ListFleetsForVehicleRequestRequestTypeDef(TypedDict):
    vehicleName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListFleetsRequestRequestTypeDef

```python
# ListFleetsRequestRequestTypeDef definition

class ListFleetsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListModelManifestNodesRequestRequestTypeDef

```python
# ListModelManifestNodesRequestRequestTypeDef definition

class ListModelManifestNodesRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListModelManifestsRequestRequestTypeDef

```python
# ListModelManifestsRequestRequestTypeDef definition

class ListModelManifestsRequestRequestTypeDef(TypedDict):
    signalCatalogArn: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ModelManifestSummaryTypeDef

```python
# ModelManifestSummaryTypeDef definition

class ModelManifestSummaryTypeDef(TypedDict):
    creationTime: datetime,
    lastModificationTime: datetime,
    name: NotRequired[str],
    arn: NotRequired[str],
    signalCatalogArn: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[ManifestStatusType],  # (1)
```

1. See [:material-code-brackets: ManifestStatusType](./literals.md#manifeststatustype) 
## ListSignalCatalogNodesRequestRequestTypeDef

```python
# ListSignalCatalogNodesRequestRequestTypeDef definition

class ListSignalCatalogNodesRequestRequestTypeDef(TypedDict):
    name: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    signalNodeType: NotRequired[SignalNodeTypeType],  # (1)
```

1. See [:material-code-brackets: SignalNodeTypeType](./literals.md#signalnodetypetype) 
## ListSignalCatalogsRequestRequestTypeDef

```python
# ListSignalCatalogsRequestRequestTypeDef definition

class ListSignalCatalogsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## SignalCatalogSummaryTypeDef

```python
# SignalCatalogSummaryTypeDef definition

class SignalCatalogSummaryTypeDef(TypedDict):
    name: NotRequired[str],
    arn: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastModificationTime: NotRequired[datetime],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListVehiclesInFleetRequestRequestTypeDef

```python
# ListVehiclesInFleetRequestRequestTypeDef definition

class ListVehiclesInFleetRequestRequestTypeDef(TypedDict):
    fleetId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListVehiclesRequestRequestTypeDef

```python
# ListVehiclesRequestRequestTypeDef definition

class ListVehiclesRequestRequestTypeDef(TypedDict):
    modelManifestArn: NotRequired[str],
    attributeNames: NotRequired[Sequence[str]],
    attributeValues: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## VehicleSummaryTypeDef

```python
# VehicleSummaryTypeDef definition

class VehicleSummaryTypeDef(TypedDict):
    vehicleName: str,
    arn: str,
    modelManifestArn: str,
    decoderManifestArn: str,
    creationTime: datetime,
    lastModificationTime: datetime,
    attributes: NotRequired[Dict[str, str]],
```

## ObdInterfaceTypeDef

```python
# ObdInterfaceTypeDef definition

class ObdInterfaceTypeDef(TypedDict):
    name: str,
    requestMessageId: int,
    obdStandard: NotRequired[str],
    pidRequestIntervalSeconds: NotRequired[int],
    dtcRequestIntervalSeconds: NotRequired[int],
    useExtendedIds: NotRequired[bool],
    hasTransmissionEcu: NotRequired[bool],
```

## VehicleMiddlewareTypeDef

```python
# VehicleMiddlewareTypeDef definition

class VehicleMiddlewareTypeDef(TypedDict):
    name: str,
    protocolName: VehicleMiddlewareProtocolType,  # (1)
```

1. See [:material-code-brackets: VehicleMiddlewareProtocolType](./literals.md#vehiclemiddlewareprotocoltype) 
## SensorOutputTypeDef

```python
# SensorOutputTypeDef definition

class SensorOutputTypeDef(TypedDict):
    fullyQualifiedName: str,
    dataType: NodeDataTypeType,  # (1)
    description: NotRequired[str],
    unit: NotRequired[str],
    allowedValues: NotRequired[List[str]],
    min: NotRequired[float],
    max: NotRequired[float],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
    structFullyQualifiedName: NotRequired[str],
```

1. See [:material-code-brackets: NodeDataTypeType](./literals.md#nodedatatypetype) 
## ObdSignalTypeDef

```python
# ObdSignalTypeDef definition

class ObdSignalTypeDef(TypedDict):
    pidResponseLength: int,
    serviceMode: int,
    pid: int,
    scaling: float,
    offset: float,
    startByte: int,
    byteLength: int,
    bitRightShift: NotRequired[int],
    bitMaskLength: NotRequired[int],
```

## ROS2PrimitiveMessageDefinitionTypeDef

```python
# ROS2PrimitiveMessageDefinitionTypeDef definition

class ROS2PrimitiveMessageDefinitionTypeDef(TypedDict):
    primitiveType: ROS2PrimitiveTypeType,  # (1)
    offset: NotRequired[float],
    scaling: NotRequired[float],
    upperBound: NotRequired[int],
```

1. See [:material-code-brackets: ROS2PrimitiveTypeType](./literals.md#ros2primitivetypetype) 
## PutEncryptionConfigurationRequestRequestTypeDef

```python
# PutEncryptionConfigurationRequestRequestTypeDef definition

class PutEncryptionConfigurationRequestRequestTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## TimestreamResourcesTypeDef

```python
# TimestreamResourcesTypeDef definition

class TimestreamResourcesTypeDef(TypedDict):
    timestreamDatabaseName: str,
    timestreamTableName: str,
```

## SensorTypeDef

```python
# SensorTypeDef definition

class SensorTypeDef(TypedDict):
    fullyQualifiedName: str,
    dataType: NodeDataTypeType,  # (1)
    description: NotRequired[str],
    unit: NotRequired[str],
    allowedValues: NotRequired[Sequence[str]],
    min: NotRequired[float],
    max: NotRequired[float],
    deprecationMessage: NotRequired[str],
    comment: NotRequired[str],
    structFullyQualifiedName: NotRequired[str],
```

1. See [:material-code-brackets: NodeDataTypeType](./literals.md#nodedatatypetype) 
## StructuredMessageFieldNameAndDataTypePairOutputTypeDef

```python
# StructuredMessageFieldNameAndDataTypePairOutputTypeDef definition

class StructuredMessageFieldNameAndDataTypePairOutputTypeDef(TypedDict):
    fieldName: str,
    dataType: Dict[str, Any],
```

## StructuredMessageFieldNameAndDataTypePairPaginatorTypeDef

```python
# StructuredMessageFieldNameAndDataTypePairPaginatorTypeDef definition

class StructuredMessageFieldNameAndDataTypePairPaginatorTypeDef(TypedDict):
    fieldName: str,
    dataType: Dict[str, Any],
```

## StructuredMessageFieldNameAndDataTypePairTypeDef

```python
# StructuredMessageFieldNameAndDataTypePairTypeDef definition

class StructuredMessageFieldNameAndDataTypePairTypeDef(TypedDict):
    fieldName: str,
    dataType: Mapping[str, Any],
```

## StructuredMessageListDefinitionOutputTypeDef

```python
# StructuredMessageListDefinitionOutputTypeDef definition

class StructuredMessageListDefinitionOutputTypeDef(TypedDict):
    name: str,
    memberType: Dict[str, Any],
    listType: StructuredMessageListTypeType,  # (1)
    capacity: NotRequired[int],
```

1. See [:material-code-brackets: StructuredMessageListTypeType](./literals.md#structuredmessagelisttypetype) 
## StructuredMessageListDefinitionPaginatorTypeDef

```python
# StructuredMessageListDefinitionPaginatorTypeDef definition

class StructuredMessageListDefinitionPaginatorTypeDef(TypedDict):
    name: str,
    memberType: Dict[str, Any],
    listType: StructuredMessageListTypeType,  # (1)
    capacity: NotRequired[int],
```

1. See [:material-code-brackets: StructuredMessageListTypeType](./literals.md#structuredmessagelisttypetype) 
## StructuredMessageListDefinitionTypeDef

```python
# StructuredMessageListDefinitionTypeDef definition

class StructuredMessageListDefinitionTypeDef(TypedDict):
    name: str,
    memberType: Mapping[str, Any],
    listType: StructuredMessageListTypeType,  # (1)
    capacity: NotRequired[int],
```

1. See [:material-code-brackets: StructuredMessageListTypeType](./literals.md#structuredmessagelisttypetype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateCampaignRequestRequestTypeDef

```python
# UpdateCampaignRequestRequestTypeDef definition

class UpdateCampaignRequestRequestTypeDef(TypedDict):
    name: str,
    action: UpdateCampaignActionType,  # (1)
    description: NotRequired[str],
    dataExtraDimensions: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: UpdateCampaignActionType](./literals.md#updatecampaignactiontype) 
## UpdateFleetRequestRequestTypeDef

```python
# UpdateFleetRequestRequestTypeDef definition

class UpdateFleetRequestRequestTypeDef(TypedDict):
    fleetId: str,
    description: NotRequired[str],
```

## UpdateModelManifestRequestRequestTypeDef

```python
# UpdateModelManifestRequestRequestTypeDef definition

class UpdateModelManifestRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    nodesToAdd: NotRequired[Sequence[str]],
    nodesToRemove: NotRequired[Sequence[str]],
    status: NotRequired[ManifestStatusType],  # (1)
```

1. See [:material-code-brackets: ManifestStatusType](./literals.md#manifeststatustype) 
## UpdateVehicleRequestRequestTypeDef

```python
# UpdateVehicleRequestRequestTypeDef definition

class UpdateVehicleRequestRequestTypeDef(TypedDict):
    vehicleName: str,
    modelManifestArn: NotRequired[str],
    decoderManifestArn: NotRequired[str],
    attributes: NotRequired[Mapping[str, str]],
    attributeUpdateMode: NotRequired[UpdateModeType],  # (1)
```

1. See [:material-code-brackets: UpdateModeType](./literals.md#updatemodetype) 
## BatchCreateVehicleResponseTypeDef

```python
# BatchCreateVehicleResponseTypeDef definition

class BatchCreateVehicleResponseTypeDef(TypedDict):
    vehicles: List[CreateVehicleResponseItemTypeDef],  # (1)
    errors: List[CreateVehicleErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CreateVehicleResponseItemTypeDef](./type_defs.md#createvehicleresponseitemtypedef) 
2. See [:material-code-braces: CreateVehicleErrorTypeDef](./type_defs.md#createvehicleerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCampaignResponseTypeDef

```python
# CreateCampaignResponseTypeDef definition

class CreateCampaignResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDecoderManifestResponseTypeDef

```python
# CreateDecoderManifestResponseTypeDef definition

class CreateDecoderManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFleetResponseTypeDef

```python
# CreateFleetResponseTypeDef definition

class CreateFleetResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateModelManifestResponseTypeDef

```python
# CreateModelManifestResponseTypeDef definition

class CreateModelManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSignalCatalogResponseTypeDef

```python
# CreateSignalCatalogResponseTypeDef definition

class CreateSignalCatalogResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVehicleResponseTypeDef

```python
# CreateVehicleResponseTypeDef definition

class CreateVehicleResponseTypeDef(TypedDict):
    vehicleName: str,
    arn: str,
    thingArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCampaignResponseTypeDef

```python
# DeleteCampaignResponseTypeDef definition

class DeleteCampaignResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDecoderManifestResponseTypeDef

```python
# DeleteDecoderManifestResponseTypeDef definition

class DeleteDecoderManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFleetResponseTypeDef

```python
# DeleteFleetResponseTypeDef definition

class DeleteFleetResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteModelManifestResponseTypeDef

```python
# DeleteModelManifestResponseTypeDef definition

class DeleteModelManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSignalCatalogResponseTypeDef

```python
# DeleteSignalCatalogResponseTypeDef definition

class DeleteSignalCatalogResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVehicleResponseTypeDef

```python
# DeleteVehicleResponseTypeDef definition

class DeleteVehicleResponseTypeDef(TypedDict):
    vehicleName: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDecoderManifestResponseTypeDef

```python
# GetDecoderManifestResponseTypeDef definition

class GetDecoderManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    description: str,
    modelManifestArn: str,
    status: ManifestStatusType,  # (1)
    creationTime: datetime,
    lastModificationTime: datetime,
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ManifestStatusType](./literals.md#manifeststatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEncryptionConfigurationResponseTypeDef

```python
# GetEncryptionConfigurationResponseTypeDef definition

class GetEncryptionConfigurationResponseTypeDef(TypedDict):
    kmsKeyId: str,
    encryptionStatus: EncryptionStatusType,  # (1)
    encryptionType: EncryptionTypeType,  # (2)
    errorMessage: str,
    creationTime: datetime,
    lastModificationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EncryptionStatusType](./literals.md#encryptionstatustype) 
2. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFleetResponseTypeDef

```python
# GetFleetResponseTypeDef definition

class GetFleetResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    description: str,
    signalCatalogArn: str,
    creationTime: datetime,
    lastModificationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetModelManifestResponseTypeDef

```python
# GetModelManifestResponseTypeDef definition

class GetModelManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    description: str,
    signalCatalogArn: str,
    status: ManifestStatusType,  # (1)
    creationTime: datetime,
    lastModificationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ManifestStatusType](./literals.md#manifeststatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVehicleResponseTypeDef

```python
# GetVehicleResponseTypeDef definition

class GetVehicleResponseTypeDef(TypedDict):
    vehicleName: str,
    arn: str,
    modelManifestArn: str,
    decoderManifestArn: str,
    attributes: Dict[str, str],
    creationTime: datetime,
    lastModificationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportDecoderManifestResponseTypeDef

```python
# ImportDecoderManifestResponseTypeDef definition

class ImportDecoderManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportSignalCatalogResponseTypeDef

```python
# ImportSignalCatalogResponseTypeDef definition

class ImportSignalCatalogResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFleetsForVehicleResponseTypeDef

```python
# ListFleetsForVehicleResponseTypeDef definition

class ListFleetsForVehicleResponseTypeDef(TypedDict):
    fleets: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVehiclesInFleetResponseTypeDef

```python
# ListVehiclesInFleetResponseTypeDef definition

class ListVehiclesInFleetResponseTypeDef(TypedDict):
    vehicles: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEncryptionConfigurationResponseTypeDef

```python
# PutEncryptionConfigurationResponseTypeDef definition

class PutEncryptionConfigurationResponseTypeDef(TypedDict):
    kmsKeyId: str,
    encryptionStatus: EncryptionStatusType,  # (1)
    encryptionType: EncryptionTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: EncryptionStatusType](./literals.md#encryptionstatustype) 
2. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCampaignResponseTypeDef

```python
# UpdateCampaignResponseTypeDef definition

class UpdateCampaignResponseTypeDef(TypedDict):
    arn: str,
    name: str,
    status: CampaignStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CampaignStatusType](./literals.md#campaignstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDecoderManifestResponseTypeDef

```python
# UpdateDecoderManifestResponseTypeDef definition

class UpdateDecoderManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFleetResponseTypeDef

```python
# UpdateFleetResponseTypeDef definition

class UpdateFleetResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateModelManifestResponseTypeDef

```python
# UpdateModelManifestResponseTypeDef definition

class UpdateModelManifestResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSignalCatalogResponseTypeDef

```python
# UpdateSignalCatalogResponseTypeDef definition

class UpdateSignalCatalogResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVehicleResponseTypeDef

```python
# UpdateVehicleResponseTypeDef definition

class UpdateVehicleResponseTypeDef(TypedDict):
    vehicleName: str,
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateVehicleRequestRequestTypeDef

```python
# BatchUpdateVehicleRequestRequestTypeDef definition

class BatchUpdateVehicleRequestRequestTypeDef(TypedDict):
    vehicles: Sequence[UpdateVehicleRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: UpdateVehicleRequestItemTypeDef](./type_defs.md#updatevehiclerequestitemtypedef) 
## BatchUpdateVehicleResponseTypeDef

```python
# BatchUpdateVehicleResponseTypeDef definition

class BatchUpdateVehicleResponseTypeDef(TypedDict):
    vehicles: List[UpdateVehicleResponseItemTypeDef],  # (1)
    errors: List[UpdateVehicleErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: UpdateVehicleResponseItemTypeDef](./type_defs.md#updatevehicleresponseitemtypedef) 
2. See [:material-code-braces: UpdateVehicleErrorTypeDef](./type_defs.md#updatevehicleerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CanDbcDefinitionTypeDef

```python
# CanDbcDefinitionTypeDef definition

class CanDbcDefinitionTypeDef(TypedDict):
    networkInterface: str,
    canDbcFiles: Sequence[BlobTypeDef],
    signalsMap: NotRequired[Mapping[str, str]],
```

## ListCampaignsResponseTypeDef

```python
# ListCampaignsResponseTypeDef definition

class ListCampaignsResponseTypeDef(TypedDict):
    campaignSummaries: List[CampaignSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CampaignSummaryTypeDef](./type_defs.md#campaignsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLoggingOptionsResponseTypeDef

```python
# GetLoggingOptionsResponseTypeDef definition

class GetLoggingOptionsResponseTypeDef(TypedDict):
    cloudWatchLogDelivery: CloudWatchLogDeliveryOptionsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CloudWatchLogDeliveryOptionsTypeDef](./type_defs.md#cloudwatchlogdeliveryoptionstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutLoggingOptionsRequestRequestTypeDef

```python
# PutLoggingOptionsRequestRequestTypeDef definition

class PutLoggingOptionsRequestRequestTypeDef(TypedDict):
    cloudWatchLogDelivery: CloudWatchLogDeliveryOptionsTypeDef,  # (1)
```

1. See [:material-code-braces: CloudWatchLogDeliveryOptionsTypeDef](./type_defs.md#cloudwatchlogdeliveryoptionstypedef) 
## CollectionSchemeTypeDef

```python
# CollectionSchemeTypeDef definition

class CollectionSchemeTypeDef(TypedDict):
    timeBasedCollectionScheme: NotRequired[TimeBasedCollectionSchemeTypeDef],  # (1)
    conditionBasedCollectionScheme: NotRequired[ConditionBasedCollectionSchemeTypeDef],  # (2)
```

1. See [:material-code-braces: TimeBasedCollectionSchemeTypeDef](./type_defs.md#timebasedcollectionschemetypedef) 
2. See [:material-code-braces: ConditionBasedCollectionSchemeTypeDef](./type_defs.md#conditionbasedcollectionschemetypedef) 
## CreateFleetRequestRequestTypeDef

```python
# CreateFleetRequestRequestTypeDef definition

class CreateFleetRequestRequestTypeDef(TypedDict):
    fleetId: str,
    signalCatalogArn: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateModelManifestRequestRequestTypeDef

```python
# CreateModelManifestRequestRequestTypeDef definition

class CreateModelManifestRequestRequestTypeDef(TypedDict):
    name: str,
    nodes: Sequence[str],
    signalCatalogArn: str,
    description: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVehicleRequestItemTypeDef

```python
# CreateVehicleRequestItemTypeDef definition

class CreateVehicleRequestItemTypeDef(TypedDict):
    vehicleName: str,
    modelManifestArn: str,
    decoderManifestArn: str,
    attributes: NotRequired[Mapping[str, str]],
    associationBehavior: NotRequired[VehicleAssociationBehaviorType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: VehicleAssociationBehaviorType](./literals.md#vehicleassociationbehaviortype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateVehicleRequestRequestTypeDef

```python
# CreateVehicleRequestRequestTypeDef definition

class CreateVehicleRequestRequestTypeDef(TypedDict):
    vehicleName: str,
    modelManifestArn: str,
    decoderManifestArn: str,
    attributes: NotRequired[Mapping[str, str]],
    associationBehavior: NotRequired[VehicleAssociationBehaviorType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: VehicleAssociationBehaviorType](./literals.md#vehicleassociationbehaviortype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DataDestinationConfigTypeDef

```python
# DataDestinationConfigTypeDef definition

class DataDestinationConfigTypeDef(TypedDict):
    s3Config: NotRequired[S3ConfigTypeDef],  # (1)
    timestreamConfig: NotRequired[TimestreamConfigTypeDef],  # (2)
```

1. See [:material-code-braces: S3ConfigTypeDef](./type_defs.md#s3configtypedef) 
2. See [:material-code-braces: TimestreamConfigTypeDef](./type_defs.md#timestreamconfigtypedef) 
## ListDecoderManifestsResponseTypeDef

```python
# ListDecoderManifestsResponseTypeDef definition

class ListDecoderManifestsResponseTypeDef(TypedDict):
    summaries: List[DecoderManifestSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DecoderManifestSummaryTypeDef](./type_defs.md#decodermanifestsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFleetsResponseTypeDef

```python
# ListFleetsResponseTypeDef definition

class ListFleetsResponseTypeDef(TypedDict):
    fleetSummaries: List[FleetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FleetSummaryTypeDef](./type_defs.md#fleetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportSignalCatalogRequestRequestTypeDef

```python
# ImportSignalCatalogRequestRequestTypeDef definition

class ImportSignalCatalogRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    vss: NotRequired[FormattedVssTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: FormattedVssTypeDef](./type_defs.md#formattedvsstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetRegisterAccountStatusResponseTypeDef

```python
# GetRegisterAccountStatusResponseTypeDef definition

class GetRegisterAccountStatusResponseTypeDef(TypedDict):
    customerAccountId: str,
    accountStatus: RegistrationStatusType,  # (1)
    timestreamRegistrationResponse: TimestreamRegistrationResponseTypeDef,  # (2)
    iamRegistrationResponse: IamRegistrationResponseTypeDef,  # (3)
    creationTime: datetime,
    lastModificationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: TimestreamRegistrationResponseTypeDef](./type_defs.md#timestreamregistrationresponsetypedef) 
3. See [:material-code-braces: IamRegistrationResponseTypeDef](./type_defs.md#iamregistrationresponsetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSignalCatalogResponseTypeDef

```python
# GetSignalCatalogResponseTypeDef definition

class GetSignalCatalogResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    description: str,
    nodeCounts: NodeCountsTypeDef,  # (1)
    creationTime: datetime,
    lastModificationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NodeCountsTypeDef](./type_defs.md#nodecountstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef

```python
# GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef definition

class GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef(TypedDict):
    vehicleName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCampaignsRequestListCampaignsPaginateTypeDef

```python
# ListCampaignsRequestListCampaignsPaginateTypeDef definition

class ListCampaignsRequestListCampaignsPaginateTypeDef(TypedDict):
    status: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef

```python
# ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef definition

class ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef(TypedDict):
    name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef

```python
# ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef definition

class ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef(TypedDict):
    name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef

```python
# ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef definition

class ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef(TypedDict):
    modelManifestArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef

```python
# ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef definition

class ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef(TypedDict):
    vehicleName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFleetsRequestListFleetsPaginateTypeDef

```python
# ListFleetsRequestListFleetsPaginateTypeDef definition

class ListFleetsRequestListFleetsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef

```python
# ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef definition

class ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef(TypedDict):
    name: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListModelManifestsRequestListModelManifestsPaginateTypeDef

```python
# ListModelManifestsRequestListModelManifestsPaginateTypeDef definition

class ListModelManifestsRequestListModelManifestsPaginateTypeDef(TypedDict):
    signalCatalogArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef

```python
# ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef definition

class ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef(TypedDict):
    name: str,
    signalNodeType: NotRequired[SignalNodeTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SignalNodeTypeType](./literals.md#signalnodetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef

```python
# ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef definition

class ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef

```python
# ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef definition

class ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef(TypedDict):
    fleetId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListVehiclesRequestListVehiclesPaginateTypeDef

```python
# ListVehiclesRequestListVehiclesPaginateTypeDef definition

class ListVehiclesRequestListVehiclesPaginateTypeDef(TypedDict):
    modelManifestArn: NotRequired[str],
    attributeNames: NotRequired[Sequence[str]],
    attributeValues: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetVehicleStatusResponseTypeDef

```python
# GetVehicleStatusResponseTypeDef definition

class GetVehicleStatusResponseTypeDef(TypedDict):
    campaigns: List[VehicleStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VehicleStatusTypeDef](./type_defs.md#vehiclestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelManifestsResponseTypeDef

```python
# ListModelManifestsResponseTypeDef definition

class ListModelManifestsResponseTypeDef(TypedDict):
    summaries: List[ModelManifestSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ModelManifestSummaryTypeDef](./type_defs.md#modelmanifestsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSignalCatalogsResponseTypeDef

```python
# ListSignalCatalogsResponseTypeDef definition

class ListSignalCatalogsResponseTypeDef(TypedDict):
    summaries: List[SignalCatalogSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SignalCatalogSummaryTypeDef](./type_defs.md#signalcatalogsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListVehiclesResponseTypeDef

```python
# ListVehiclesResponseTypeDef definition

class ListVehiclesResponseTypeDef(TypedDict):
    vehicleSummaries: List[VehicleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: VehicleSummaryTypeDef](./type_defs.md#vehiclesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    interfaceId: str,
    type: NetworkInterfaceTypeType,  # (1)
    canInterface: NotRequired[CanInterfaceTypeDef],  # (2)
    obdInterface: NotRequired[ObdInterfaceTypeDef],  # (3)
    vehicleMiddleware: NotRequired[VehicleMiddlewareTypeDef],  # (4)
```

1. See [:material-code-brackets: NetworkInterfaceTypeType](./literals.md#networkinterfacetypetype) 
2. See [:material-code-braces: CanInterfaceTypeDef](./type_defs.md#caninterfacetypedef) 
3. See [:material-code-braces: ObdInterfaceTypeDef](./type_defs.md#obdinterfacetypedef) 
4. See [:material-code-braces: VehicleMiddlewareTypeDef](./type_defs.md#vehiclemiddlewaretypedef) 
## NodeOutputTypeDef

```python
# NodeOutputTypeDef definition

class NodeOutputTypeDef(TypedDict):
    branch: NotRequired[BranchTypeDef],  # (1)
    sensor: NotRequired[SensorOutputTypeDef],  # (2)
    actuator: NotRequired[ActuatorOutputTypeDef],  # (3)
    attribute: NotRequired[AttributeOutputTypeDef],  # (4)
    struct: NotRequired[CustomStructTypeDef],  # (5)
    property: NotRequired[CustomPropertyTypeDef],  # (6)
```

1. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef) 
2. See [:material-code-braces: SensorOutputTypeDef](./type_defs.md#sensoroutputtypedef) 
3. See [:material-code-braces: ActuatorOutputTypeDef](./type_defs.md#actuatoroutputtypedef) 
4. See [:material-code-braces: AttributeOutputTypeDef](./type_defs.md#attributeoutputtypedef) 
5. See [:material-code-braces: CustomStructTypeDef](./type_defs.md#customstructtypedef) 
6. See [:material-code-braces: CustomPropertyTypeDef](./type_defs.md#custompropertytypedef) 
## PrimitiveMessageDefinitionTypeDef

```python
# PrimitiveMessageDefinitionTypeDef definition

class PrimitiveMessageDefinitionTypeDef(TypedDict):
    ros2PrimitiveMessageDefinition: NotRequired[ROS2PrimitiveMessageDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: ROS2PrimitiveMessageDefinitionTypeDef](./type_defs.md#ros2primitivemessagedefinitiontypedef) 
## RegisterAccountRequestRequestTypeDef

```python
# RegisterAccountRequestRequestTypeDef definition

class RegisterAccountRequestRequestTypeDef(TypedDict):
    timestreamResources: NotRequired[TimestreamResourcesTypeDef],  # (1)
    iamResources: NotRequired[IamResourcesTypeDef],  # (2)
```

1. See [:material-code-braces: TimestreamResourcesTypeDef](./type_defs.md#timestreamresourcestypedef) 
2. See [:material-code-braces: IamResourcesTypeDef](./type_defs.md#iamresourcestypedef) 
## RegisterAccountResponseTypeDef

```python
# RegisterAccountResponseTypeDef definition

class RegisterAccountResponseTypeDef(TypedDict):
    registerAccountStatus: RegistrationStatusType,  # (1)
    timestreamResources: TimestreamResourcesTypeDef,  # (2)
    iamResources: IamResourcesTypeDef,  # (3)
    creationTime: datetime,
    lastModificationTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: RegistrationStatusType](./literals.md#registrationstatustype) 
2. See [:material-code-braces: TimestreamResourcesTypeDef](./type_defs.md#timestreamresourcestypedef) 
3. See [:material-code-braces: IamResourcesTypeDef](./type_defs.md#iamresourcestypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NetworkFileDefinitionTypeDef

```python
# NetworkFileDefinitionTypeDef definition

class NetworkFileDefinitionTypeDef(TypedDict):
    canDbc: NotRequired[CanDbcDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: CanDbcDefinitionTypeDef](./type_defs.md#candbcdefinitiontypedef) 
## BatchCreateVehicleRequestRequestTypeDef

```python
# BatchCreateVehicleRequestRequestTypeDef definition

class BatchCreateVehicleRequestRequestTypeDef(TypedDict):
    vehicles: Sequence[CreateVehicleRequestItemTypeDef],  # (1)
```

1. See [:material-code-braces: CreateVehicleRequestItemTypeDef](./type_defs.md#createvehiclerequestitemtypedef) 
## CreateCampaignRequestRequestTypeDef

```python
# CreateCampaignRequestRequestTypeDef definition

class CreateCampaignRequestRequestTypeDef(TypedDict):
    name: str,
    signalCatalogArn: str,
    targetArn: str,
    collectionScheme: CollectionSchemeTypeDef,  # (1)
    description: NotRequired[str],
    startTime: NotRequired[TimestampTypeDef],
    expiryTime: NotRequired[TimestampTypeDef],
    postTriggerCollectionDuration: NotRequired[int],
    diagnosticsMode: NotRequired[DiagnosticsModeType],  # (2)
    spoolingMode: NotRequired[SpoolingModeType],  # (3)
    compression: NotRequired[CompressionType],  # (4)
    priority: NotRequired[int],
    signalsToCollect: NotRequired[Sequence[SignalInformationTypeDef]],  # (5)
    dataExtraDimensions: NotRequired[Sequence[str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (6)
    dataDestinationConfigs: NotRequired[Sequence[DataDestinationConfigTypeDef]],  # (7)
```

1. See [:material-code-braces: CollectionSchemeTypeDef](./type_defs.md#collectionschemetypedef) 
2. See [:material-code-brackets: DiagnosticsModeType](./literals.md#diagnosticsmodetype) 
3. See [:material-code-brackets: SpoolingModeType](./literals.md#spoolingmodetype) 
4. See [:material-code-brackets: CompressionType](./literals.md#compressiontype) 
5. See [:material-code-braces: SignalInformationTypeDef](./type_defs.md#signalinformationtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: DataDestinationConfigTypeDef](./type_defs.md#datadestinationconfigtypedef) 
## GetCampaignResponseTypeDef

```python
# GetCampaignResponseTypeDef definition

class GetCampaignResponseTypeDef(TypedDict):
    name: str,
    arn: str,
    description: str,
    signalCatalogArn: str,
    targetArn: str,
    status: CampaignStatusType,  # (1)
    startTime: datetime,
    expiryTime: datetime,
    postTriggerCollectionDuration: int,
    diagnosticsMode: DiagnosticsModeType,  # (2)
    spoolingMode: SpoolingModeType,  # (3)
    compression: CompressionType,  # (4)
    priority: int,
    signalsToCollect: List[SignalInformationTypeDef],  # (5)
    collectionScheme: CollectionSchemeTypeDef,  # (6)
    dataExtraDimensions: List[str],
    creationTime: datetime,
    lastModificationTime: datetime,
    dataDestinationConfigs: List[DataDestinationConfigTypeDef],  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: CampaignStatusType](./literals.md#campaignstatustype) 
2. See [:material-code-brackets: DiagnosticsModeType](./literals.md#diagnosticsmodetype) 
3. See [:material-code-brackets: SpoolingModeType](./literals.md#spoolingmodetype) 
4. See [:material-code-brackets: CompressionType](./literals.md#compressiontype) 
5. See [:material-code-braces: SignalInformationTypeDef](./type_defs.md#signalinformationtypedef) 
6. See [:material-code-braces: CollectionSchemeTypeDef](./type_defs.md#collectionschemetypedef) 
7. See [:material-code-braces: DataDestinationConfigTypeDef](./type_defs.md#datadestinationconfigtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDecoderManifestNetworkInterfacesResponseTypeDef

```python
# ListDecoderManifestNetworkInterfacesResponseTypeDef definition

class ListDecoderManifestNetworkInterfacesResponseTypeDef(TypedDict):
    networkInterfaces: List[NetworkInterfaceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListModelManifestNodesResponseTypeDef

```python
# ListModelManifestNodesResponseTypeDef definition

class ListModelManifestNodesResponseTypeDef(TypedDict):
    nodes: List[NodeOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NodeOutputTypeDef](./type_defs.md#nodeoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSignalCatalogNodesResponseTypeDef

```python
# ListSignalCatalogNodesResponseTypeDef definition

class ListSignalCatalogNodesResponseTypeDef(TypedDict):
    nodes: List[NodeOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NodeOutputTypeDef](./type_defs.md#nodeoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StructuredMessageOutputTypeDef

```python
# StructuredMessageOutputTypeDef definition

class StructuredMessageOutputTypeDef(TypedDict):
    primitiveMessageDefinition: NotRequired[PrimitiveMessageDefinitionTypeDef],  # (1)
    structuredMessageListDefinition: NotRequired[StructuredMessageListDefinitionOutputTypeDef],  # (2)
    structuredMessageDefinition: NotRequired[List[StructuredMessageFieldNameAndDataTypePairOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: PrimitiveMessageDefinitionTypeDef](./type_defs.md#primitivemessagedefinitiontypedef) 
2. See [:material-code-braces: StructuredMessageListDefinitionOutputTypeDef](./type_defs.md#structuredmessagelistdefinitionoutputtypedef) 
3. See [:material-code-braces: StructuredMessageFieldNameAndDataTypePairOutputTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairoutputtypedef) 
## StructuredMessagePaginatorTypeDef

```python
# StructuredMessagePaginatorTypeDef definition

class StructuredMessagePaginatorTypeDef(TypedDict):
    primitiveMessageDefinition: NotRequired[PrimitiveMessageDefinitionTypeDef],  # (1)
    structuredMessageListDefinition: NotRequired[StructuredMessageListDefinitionPaginatorTypeDef],  # (2)
    structuredMessageDefinition: NotRequired[List[StructuredMessageFieldNameAndDataTypePairPaginatorTypeDef]],  # (3)
```

1. See [:material-code-braces: PrimitiveMessageDefinitionTypeDef](./type_defs.md#primitivemessagedefinitiontypedef) 
2. See [:material-code-braces: StructuredMessageListDefinitionPaginatorTypeDef](./type_defs.md#structuredmessagelistdefinitionpaginatortypedef) 
3. See [:material-code-braces: StructuredMessageFieldNameAndDataTypePairPaginatorTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairpaginatortypedef) 
## NodeTypeDef

```python
# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    branch: NotRequired[BranchTypeDef],  # (1)
    sensor: NotRequired[SensorUnionTypeDef],  # (2)
    actuator: NotRequired[ActuatorUnionTypeDef],  # (3)
    attribute: NotRequired[AttributeUnionTypeDef],  # (4)
    struct: NotRequired[CustomStructTypeDef],  # (5)
    property: NotRequired[CustomPropertyTypeDef],  # (6)
```

1. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef) 
2. See [:material-code-braces: SensorTypeDef](./type_defs.md#sensortypedef) [:material-code-braces: SensorOutputTypeDef](./type_defs.md#sensoroutputtypedef) 
3. See [:material-code-braces: ActuatorTypeDef](./type_defs.md#actuatortypedef) [:material-code-braces: ActuatorOutputTypeDef](./type_defs.md#actuatoroutputtypedef) 
4. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) [:material-code-braces: AttributeOutputTypeDef](./type_defs.md#attributeoutputtypedef) 
5. See [:material-code-braces: CustomStructTypeDef](./type_defs.md#customstructtypedef) 
6. See [:material-code-braces: CustomPropertyTypeDef](./type_defs.md#custompropertytypedef) 
## StructuredMessageTypeDef

```python
# StructuredMessageTypeDef definition

class StructuredMessageTypeDef(TypedDict):
    primitiveMessageDefinition: NotRequired[PrimitiveMessageDefinitionTypeDef],  # (1)
    structuredMessageListDefinition: NotRequired[StructuredMessageListDefinitionUnionTypeDef],  # (2)
    structuredMessageDefinition: NotRequired[Sequence[StructuredMessageFieldNameAndDataTypePairUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: PrimitiveMessageDefinitionTypeDef](./type_defs.md#primitivemessagedefinitiontypedef) 
2. See [:material-code-braces: StructuredMessageListDefinitionTypeDef](./type_defs.md#structuredmessagelistdefinitiontypedef) [:material-code-braces: StructuredMessageListDefinitionOutputTypeDef](./type_defs.md#structuredmessagelistdefinitionoutputtypedef) 
3. See [:material-code-braces: StructuredMessageFieldNameAndDataTypePairTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairtypedef) [:material-code-braces: StructuredMessageFieldNameAndDataTypePairOutputTypeDef](./type_defs.md#structuredmessagefieldnameanddatatypepairoutputtypedef) 
## ImportDecoderManifestRequestRequestTypeDef

```python
# ImportDecoderManifestRequestRequestTypeDef definition

class ImportDecoderManifestRequestRequestTypeDef(TypedDict):
    name: str,
    networkFileDefinitions: Sequence[NetworkFileDefinitionTypeDef],  # (1)
```

1. See [:material-code-braces: NetworkFileDefinitionTypeDef](./type_defs.md#networkfiledefinitiontypedef) 
## MessageSignalOutputTypeDef

```python
# MessageSignalOutputTypeDef definition

class MessageSignalOutputTypeDef(TypedDict):
    topicName: str,
    structuredMessage: StructuredMessageOutputTypeDef,  # (1)
```

1. See [:material-code-braces: StructuredMessageOutputTypeDef](./type_defs.md#structuredmessageoutputtypedef) 
## MessageSignalPaginatorTypeDef

```python
# MessageSignalPaginatorTypeDef definition

class MessageSignalPaginatorTypeDef(TypedDict):
    topicName: str,
    structuredMessage: StructuredMessagePaginatorTypeDef,  # (1)
```

1. See [:material-code-braces: StructuredMessagePaginatorTypeDef](./type_defs.md#structuredmessagepaginatortypedef) 
## UpdateSignalCatalogRequestRequestTypeDef

```python
# UpdateSignalCatalogRequestRequestTypeDef definition

class UpdateSignalCatalogRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    nodesToAdd: NotRequired[Sequence[NodeTypeDef]],  # (1)
    nodesToUpdate: NotRequired[Sequence[NodeTypeDef]],  # (1)
    nodesToRemove: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
2. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
## SignalDecoderOutputTypeDef

```python
# SignalDecoderOutputTypeDef definition

class SignalDecoderOutputTypeDef(TypedDict):
    fullyQualifiedName: str,
    type: SignalDecoderTypeType,  # (1)
    interfaceId: str,
    canSignal: NotRequired[CanSignalTypeDef],  # (2)
    obdSignal: NotRequired[ObdSignalTypeDef],  # (3)
    messageSignal: NotRequired[MessageSignalOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: SignalDecoderTypeType](./literals.md#signaldecodertypetype) 
2. See [:material-code-braces: CanSignalTypeDef](./type_defs.md#cansignaltypedef) 
3. See [:material-code-braces: ObdSignalTypeDef](./type_defs.md#obdsignaltypedef) 
4. See [:material-code-braces: MessageSignalOutputTypeDef](./type_defs.md#messagesignaloutputtypedef) 
## SignalDecoderPaginatorTypeDef

```python
# SignalDecoderPaginatorTypeDef definition

class SignalDecoderPaginatorTypeDef(TypedDict):
    fullyQualifiedName: str,
    type: SignalDecoderTypeType,  # (1)
    interfaceId: str,
    canSignal: NotRequired[CanSignalTypeDef],  # (2)
    obdSignal: NotRequired[ObdSignalTypeDef],  # (3)
    messageSignal: NotRequired[MessageSignalPaginatorTypeDef],  # (4)
```

1. See [:material-code-brackets: SignalDecoderTypeType](./literals.md#signaldecodertypetype) 
2. See [:material-code-braces: CanSignalTypeDef](./type_defs.md#cansignaltypedef) 
3. See [:material-code-braces: ObdSignalTypeDef](./type_defs.md#obdsignaltypedef) 
4. See [:material-code-braces: MessageSignalPaginatorTypeDef](./type_defs.md#messagesignalpaginatortypedef) 
## CreateSignalCatalogRequestRequestTypeDef

```python
# CreateSignalCatalogRequestRequestTypeDef definition

class CreateSignalCatalogRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    nodes: NotRequired[Sequence[NodeUnionTypeDef]],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) [:material-code-braces: NodeOutputTypeDef](./type_defs.md#nodeoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## MessageSignalTypeDef

```python
# MessageSignalTypeDef definition

class MessageSignalTypeDef(TypedDict):
    topicName: str,
    structuredMessage: StructuredMessageUnionTypeDef,  # (1)
```

1. See [:material-code-braces: StructuredMessageTypeDef](./type_defs.md#structuredmessagetypedef) [:material-code-braces: StructuredMessageOutputTypeDef](./type_defs.md#structuredmessageoutputtypedef) 
## ListDecoderManifestSignalsResponseTypeDef

```python
# ListDecoderManifestSignalsResponseTypeDef definition

class ListDecoderManifestSignalsResponseTypeDef(TypedDict):
    signalDecoders: List[SignalDecoderOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SignalDecoderOutputTypeDef](./type_defs.md#signaldecoderoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDecoderManifestSignalsResponsePaginatorTypeDef

```python
# ListDecoderManifestSignalsResponsePaginatorTypeDef definition

class ListDecoderManifestSignalsResponsePaginatorTypeDef(TypedDict):
    signalDecoders: List[SignalDecoderPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SignalDecoderPaginatorTypeDef](./type_defs.md#signaldecoderpaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SignalDecoderTypeDef

```python
# SignalDecoderTypeDef definition

class SignalDecoderTypeDef(TypedDict):
    fullyQualifiedName: str,
    type: SignalDecoderTypeType,  # (1)
    interfaceId: str,
    canSignal: NotRequired[CanSignalTypeDef],  # (2)
    obdSignal: NotRequired[ObdSignalTypeDef],  # (3)
    messageSignal: NotRequired[MessageSignalUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: SignalDecoderTypeType](./literals.md#signaldecodertypetype) 
2. See [:material-code-braces: CanSignalTypeDef](./type_defs.md#cansignaltypedef) 
3. See [:material-code-braces: ObdSignalTypeDef](./type_defs.md#obdsignaltypedef) 
4. See [:material-code-braces: MessageSignalTypeDef](./type_defs.md#messagesignaltypedef) [:material-code-braces: MessageSignalOutputTypeDef](./type_defs.md#messagesignaloutputtypedef) 
## UpdateDecoderManifestRequestRequestTypeDef

```python
# UpdateDecoderManifestRequestRequestTypeDef definition

class UpdateDecoderManifestRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    signalDecodersToAdd: NotRequired[Sequence[SignalDecoderTypeDef]],  # (1)
    signalDecodersToUpdate: NotRequired[Sequence[SignalDecoderTypeDef]],  # (1)
    signalDecodersToRemove: NotRequired[Sequence[str]],
    networkInterfacesToAdd: NotRequired[Sequence[NetworkInterfaceTypeDef]],  # (3)
    networkInterfacesToUpdate: NotRequired[Sequence[NetworkInterfaceTypeDef]],  # (3)
    networkInterfacesToRemove: NotRequired[Sequence[str]],
    status: NotRequired[ManifestStatusType],  # (5)
```

1. See [:material-code-braces: SignalDecoderTypeDef](./type_defs.md#signaldecodertypedef) 
2. See [:material-code-braces: SignalDecoderTypeDef](./type_defs.md#signaldecodertypedef) 
3. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
4. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
5. See [:material-code-brackets: ManifestStatusType](./literals.md#manifeststatustype) 
## CreateDecoderManifestRequestRequestTypeDef

```python
# CreateDecoderManifestRequestRequestTypeDef definition

class CreateDecoderManifestRequestRequestTypeDef(TypedDict):
    name: str,
    modelManifestArn: str,
    description: NotRequired[str],
    signalDecoders: NotRequired[Sequence[SignalDecoderUnionTypeDef]],  # (1)
    networkInterfaces: NotRequired[Sequence[NetworkInterfaceTypeDef]],  # (2)
    tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: SignalDecoderTypeDef](./type_defs.md#signaldecodertypedef) [:material-code-braces: SignalDecoderOutputTypeDef](./type_defs.md#signaldecoderoutputtypedef) 
2. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
