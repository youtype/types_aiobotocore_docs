# Type definitions

> [Index](../README.md) > [Glue](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

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


## AggregateOperationUnionTypeDef

```python
# AggregateOperationUnionTypeDef definition

AggregateOperationUnionTypeDef = Union[
    AggregateOperationTypeDef,  # (1)
    AggregateOperationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AggregateOperationTypeDef](./type_defs.md#aggregateoperationtypedef) 
2. See [:material-code-braces: AggregateOperationOutputTypeDef](./type_defs.md#aggregateoperationoutputtypedef) 

## BasicCatalogTargetUnionTypeDef

```python
# BasicCatalogTargetUnionTypeDef definition

BasicCatalogTargetUnionTypeDef = Union[
    BasicCatalogTargetTypeDef,  # (1)
    BasicCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BasicCatalogTargetTypeDef](./type_defs.md#basiccatalogtargettypedef) 
2. See [:material-code-braces: BasicCatalogTargetOutputTypeDef](./type_defs.md#basiccatalogtargetoutputtypedef) 

## PartitionValueListUnionTypeDef

```python
# PartitionValueListUnionTypeDef definition

PartitionValueListUnionTypeDef = Union[
    PartitionValueListTypeDef,  # (1)
    PartitionValueListOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
2. See [:material-code-braces: PartitionValueListOutputTypeDef](./type_defs.md#partitionvaluelistoutputtypedef) 

## CatalogTargetUnionTypeDef

```python
# CatalogTargetUnionTypeDef definition

CatalogTargetUnionTypeDef = Union[
    CatalogTargetTypeDef,  # (1)
    CatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CatalogTargetTypeDef](./type_defs.md#catalogtargettypedef) 
2. See [:material-code-braces: CatalogTargetOutputTypeDef](./type_defs.md#catalogtargetoutputtypedef) 

## ColumnUnionTypeDef

```python
# ColumnUnionTypeDef definition

ColumnUnionTypeDef = Union[
    ColumnTypeDef,  # (1)
    ColumnOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: ColumnOutputTypeDef](./type_defs.md#columnoutputtypedef) 

## ConfigurationObjectUnionTypeDef

```python
# ConfigurationObjectUnionTypeDef definition

ConfigurationObjectUnionTypeDef = Union[
    ConfigurationObjectTypeDef,  # (1)
    ConfigurationObjectOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfigurationObjectTypeDef](./type_defs.md#configurationobjecttypedef) 
2. See [:material-code-braces: ConfigurationObjectOutputTypeDef](./type_defs.md#configurationobjectoutputtypedef) 

## ConnectionsListUnionTypeDef

```python
# ConnectionsListUnionTypeDef definition

ConnectionsListUnionTypeDef = Union[
    ConnectionsListTypeDef,  # (1)
    ConnectionsListOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
2. See [:material-code-braces: ConnectionsListOutputTypeDef](./type_defs.md#connectionslistoutputtypedef) 

## ConnectorDataTargetUnionTypeDef

```python
# ConnectorDataTargetUnionTypeDef definition

ConnectorDataTargetUnionTypeDef = Union[
    ConnectorDataTargetTypeDef,  # (1)
    ConnectorDataTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConnectorDataTargetTypeDef](./type_defs.md#connectordatatargettypedef) 
2. See [:material-code-braces: ConnectorDataTargetOutputTypeDef](./type_defs.md#connectordatatargetoutputtypedef) 

## DeltaTargetUnionTypeDef

```python
# DeltaTargetUnionTypeDef definition

DeltaTargetUnionTypeDef = Union[
    DeltaTargetTypeDef,  # (1)
    DeltaTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DeltaTargetTypeDef](./type_defs.md#deltatargettypedef) 
2. See [:material-code-braces: DeltaTargetOutputTypeDef](./type_defs.md#deltatargetoutputtypedef) 

## DropDuplicatesUnionTypeDef

```python
# DropDuplicatesUnionTypeDef definition

DropDuplicatesUnionTypeDef = Union[
    DropDuplicatesTypeDef,  # (1)
    DropDuplicatesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DropDuplicatesTypeDef](./type_defs.md#dropduplicatestypedef) 
2. See [:material-code-braces: DropDuplicatesOutputTypeDef](./type_defs.md#dropduplicatesoutputtypedef) 

## DropFieldsUnionTypeDef

```python
# DropFieldsUnionTypeDef definition

DropFieldsUnionTypeDef = Union[
    DropFieldsTypeDef,  # (1)
    DropFieldsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DropFieldsTypeDef](./type_defs.md#dropfieldstypedef) 
2. See [:material-code-braces: DropFieldsOutputTypeDef](./type_defs.md#dropfieldsoutputtypedef) 

## FillMissingValuesUnionTypeDef

```python
# FillMissingValuesUnionTypeDef definition

FillMissingValuesUnionTypeDef = Union[
    FillMissingValuesTypeDef,  # (1)
    FillMissingValuesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FillMissingValuesTypeDef](./type_defs.md#fillmissingvaluestypedef) 
2. See [:material-code-braces: FillMissingValuesOutputTypeDef](./type_defs.md#fillmissingvaluesoutputtypedef) 

## FilterValueUnionTypeDef

```python
# FilterValueUnionTypeDef definition

FilterValueUnionTypeDef = Union[
    FilterValueTypeDef,  # (1)
    FilterValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterValueTypeDef](./type_defs.md#filtervaluetypedef) 
2. See [:material-code-braces: FilterValueOutputTypeDef](./type_defs.md#filtervalueoutputtypedef) 

## GlueTableUnionTypeDef

```python
# GlueTableUnionTypeDef definition

GlueTableUnionTypeDef = Union[
    GlueTableTypeDef,  # (1)
    GlueTableOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) 
2. See [:material-code-braces: GlueTableOutputTypeDef](./type_defs.md#gluetableoutputtypedef) 

## HudiTargetUnionTypeDef

```python
# HudiTargetUnionTypeDef definition

HudiTargetUnionTypeDef = Union[
    HudiTargetTypeDef,  # (1)
    HudiTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HudiTargetTypeDef](./type_defs.md#huditargettypedef) 
2. See [:material-code-braces: HudiTargetOutputTypeDef](./type_defs.md#huditargetoutputtypedef) 

## IcebergTargetUnionTypeDef

```python
# IcebergTargetUnionTypeDef definition

IcebergTargetUnionTypeDef = Union[
    IcebergTargetTypeDef,  # (1)
    IcebergTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: IcebergTargetTypeDef](./type_defs.md#icebergtargettypedef) 
2. See [:material-code-braces: IcebergTargetOutputTypeDef](./type_defs.md#icebergtargetoutputtypedef) 

## JDBCConnectorOptionsUnionTypeDef

```python
# JDBCConnectorOptionsUnionTypeDef definition

JDBCConnectorOptionsUnionTypeDef = Union[
    JDBCConnectorOptionsTypeDef,  # (1)
    JDBCConnectorOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JDBCConnectorOptionsTypeDef](./type_defs.md#jdbcconnectoroptionstypedef) 
2. See [:material-code-braces: JDBCConnectorOptionsOutputTypeDef](./type_defs.md#jdbcconnectoroptionsoutputtypedef) 

## JdbcTargetUnionTypeDef

```python
# JdbcTargetUnionTypeDef definition

JdbcTargetUnionTypeDef = Union[
    JdbcTargetTypeDef,  # (1)
    JdbcTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JdbcTargetTypeDef](./type_defs.md#jdbctargettypedef) 
2. See [:material-code-braces: JdbcTargetOutputTypeDef](./type_defs.md#jdbctargetoutputtypedef) 

## JoinColumnUnionTypeDef

```python
# JoinColumnUnionTypeDef definition

JoinColumnUnionTypeDef = Union[
    JoinColumnTypeDef,  # (1)
    JoinColumnOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JoinColumnTypeDef](./type_defs.md#joincolumntypedef) 
2. See [:material-code-braces: JoinColumnOutputTypeDef](./type_defs.md#joincolumnoutputtypedef) 

## MappingUnionTypeDef

```python
# MappingUnionTypeDef definition

MappingUnionTypeDef = Union[
    MappingTypeDef,  # (1)
    MappingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) 
2. See [:material-code-braces: MappingOutputTypeDef](./type_defs.md#mappingoutputtypedef) 

## MergeUnionTypeDef

```python
# MergeUnionTypeDef definition

MergeUnionTypeDef = Union[
    MergeTypeDef,  # (1)
    MergeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MergeTypeDef](./type_defs.md#mergetypedef) 
2. See [:material-code-braces: MergeOutputTypeDef](./type_defs.md#mergeoutputtypedef) 

## MicrosoftSQLServerCatalogTargetUnionTypeDef

```python
# MicrosoftSQLServerCatalogTargetUnionTypeDef definition

MicrosoftSQLServerCatalogTargetUnionTypeDef = Union[
    MicrosoftSQLServerCatalogTargetTypeDef,  # (1)
    MicrosoftSQLServerCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MicrosoftSQLServerCatalogTargetTypeDef](./type_defs.md#microsoftsqlservercatalogtargettypedef) 
2. See [:material-code-braces: MicrosoftSQLServerCatalogTargetOutputTypeDef](./type_defs.md#microsoftsqlservercatalogtargetoutputtypedef) 

## MySQLCatalogTargetUnionTypeDef

```python
# MySQLCatalogTargetUnionTypeDef definition

MySQLCatalogTargetUnionTypeDef = Union[
    MySQLCatalogTargetTypeDef,  # (1)
    MySQLCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MySQLCatalogTargetTypeDef](./type_defs.md#mysqlcatalogtargettypedef) 
2. See [:material-code-braces: MySQLCatalogTargetOutputTypeDef](./type_defs.md#mysqlcatalogtargetoutputtypedef) 

## OracleSQLCatalogTargetUnionTypeDef

```python
# OracleSQLCatalogTargetUnionTypeDef definition

OracleSQLCatalogTargetUnionTypeDef = Union[
    OracleSQLCatalogTargetTypeDef,  # (1)
    OracleSQLCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OracleSQLCatalogTargetTypeDef](./type_defs.md#oraclesqlcatalogtargettypedef) 
2. See [:material-code-braces: OracleSQLCatalogTargetOutputTypeDef](./type_defs.md#oraclesqlcatalogtargetoutputtypedef) 

## PIIDetectionUnionTypeDef

```python
# PIIDetectionUnionTypeDef definition

PIIDetectionUnionTypeDef = Union[
    PIIDetectionTypeDef,  # (1)
    PIIDetectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PIIDetectionTypeDef](./type_defs.md#piidetectiontypedef) 
2. See [:material-code-braces: PIIDetectionOutputTypeDef](./type_defs.md#piidetectionoutputtypedef) 

## PhysicalConnectionRequirementsUnionTypeDef

```python
# PhysicalConnectionRequirementsUnionTypeDef definition

PhysicalConnectionRequirementsUnionTypeDef = Union[
    PhysicalConnectionRequirementsTypeDef,  # (1)
    PhysicalConnectionRequirementsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PhysicalConnectionRequirementsTypeDef](./type_defs.md#physicalconnectionrequirementstypedef) 
2. See [:material-code-braces: PhysicalConnectionRequirementsOutputTypeDef](./type_defs.md#physicalconnectionrequirementsoutputtypedef) 

## PostgreSQLCatalogTargetUnionTypeDef

```python
# PostgreSQLCatalogTargetUnionTypeDef definition

PostgreSQLCatalogTargetUnionTypeDef = Union[
    PostgreSQLCatalogTargetTypeDef,  # (1)
    PostgreSQLCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PostgreSQLCatalogTargetTypeDef](./type_defs.md#postgresqlcatalogtargettypedef) 
2. See [:material-code-braces: PostgreSQLCatalogTargetOutputTypeDef](./type_defs.md#postgresqlcatalogtargetoutputtypedef) 

## RecipeActionUnionTypeDef

```python
# RecipeActionUnionTypeDef definition

RecipeActionUnionTypeDef = Union[
    RecipeActionTypeDef,  # (1)
    RecipeActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RecipeActionTypeDef](./type_defs.md#recipeactiontypedef) 
2. See [:material-code-braces: RecipeActionOutputTypeDef](./type_defs.md#recipeactionoutputtypedef) 

## RenameFieldUnionTypeDef

```python
# RenameFieldUnionTypeDef definition

RenameFieldUnionTypeDef = Union[
    RenameFieldTypeDef,  # (1)
    RenameFieldOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RenameFieldTypeDef](./type_defs.md#renamefieldtypedef) 
2. See [:material-code-braces: RenameFieldOutputTypeDef](./type_defs.md#renamefieldoutputtypedef) 

## S3TargetUnionTypeDef

```python
# S3TargetUnionTypeDef definition

S3TargetUnionTypeDef = Union[
    S3TargetTypeDef,  # (1)
    S3TargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3TargetTypeDef](./type_defs.md#s3targettypedef) 
2. See [:material-code-braces: S3TargetOutputTypeDef](./type_defs.md#s3targetoutputtypedef) 

## SelectFieldsUnionTypeDef

```python
# SelectFieldsUnionTypeDef definition

SelectFieldsUnionTypeDef = Union[
    SelectFieldsTypeDef,  # (1)
    SelectFieldsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SelectFieldsTypeDef](./type_defs.md#selectfieldstypedef) 
2. See [:material-code-braces: SelectFieldsOutputTypeDef](./type_defs.md#selectfieldsoutputtypedef) 

## SelectFromCollectionUnionTypeDef

```python
# SelectFromCollectionUnionTypeDef definition

SelectFromCollectionUnionTypeDef = Union[
    SelectFromCollectionTypeDef,  # (1)
    SelectFromCollectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SelectFromCollectionTypeDef](./type_defs.md#selectfromcollectiontypedef) 
2. See [:material-code-braces: SelectFromCollectionOutputTypeDef](./type_defs.md#selectfromcollectionoutputtypedef) 

## SerDeInfoUnionTypeDef

```python
# SerDeInfoUnionTypeDef definition

SerDeInfoUnionTypeDef = Union[
    SerDeInfoTypeDef,  # (1)
    SerDeInfoOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SerDeInfoTypeDef](./type_defs.md#serdeinfotypedef) 
2. See [:material-code-braces: SerDeInfoOutputTypeDef](./type_defs.md#serdeinfooutputtypedef) 

## SkewedInfoUnionTypeDef

```python
# SkewedInfoUnionTypeDef definition

SkewedInfoUnionTypeDef = Union[
    SkewedInfoTypeDef,  # (1)
    SkewedInfoOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SkewedInfoTypeDef](./type_defs.md#skewedinfotypedef) 
2. See [:material-code-braces: SkewedInfoOutputTypeDef](./type_defs.md#skewedinfooutputtypedef) 

## SpigotUnionTypeDef

```python
# SpigotUnionTypeDef definition

SpigotUnionTypeDef = Union[
    SpigotTypeDef,  # (1)
    SpigotOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SpigotTypeDef](./type_defs.md#spigottypedef) 
2. See [:material-code-braces: SpigotOutputTypeDef](./type_defs.md#spigotoutputtypedef) 

## SplitFieldsUnionTypeDef

```python
# SplitFieldsUnionTypeDef definition

SplitFieldsUnionTypeDef = Union[
    SplitFieldsTypeDef,  # (1)
    SplitFieldsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SplitFieldsTypeDef](./type_defs.md#splitfieldstypedef) 
2. See [:material-code-braces: SplitFieldsOutputTypeDef](./type_defs.md#splitfieldsoutputtypedef) 

## TransformConfigParameterUnionTypeDef

```python
# TransformConfigParameterUnionTypeDef definition

TransformConfigParameterUnionTypeDef = Union[
    TransformConfigParameterTypeDef,  # (1)
    TransformConfigParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TransformConfigParameterTypeDef](./type_defs.md#transformconfigparametertypedef) 
2. See [:material-code-braces: TransformConfigParameterOutputTypeDef](./type_defs.md#transformconfigparameteroutputtypedef) 

## UnionUnionTypeDef

```python
# UnionUnionTypeDef definition

UnionUnionTypeDef = Union[
    UnionTypeDef,  # (1)
    UnionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UnionTypeDef](./type_defs.md#uniontypedef) 
2. See [:material-code-braces: UnionOutputTypeDef](./type_defs.md#unionoutputtypedef) 

## UpsertRedshiftTargetOptionsUnionTypeDef

```python
# UpsertRedshiftTargetOptionsUnionTypeDef definition

UpsertRedshiftTargetOptionsUnionTypeDef = Union[
    UpsertRedshiftTargetOptionsTypeDef,  # (1)
    UpsertRedshiftTargetOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UpsertRedshiftTargetOptionsTypeDef](./type_defs.md#upsertredshifttargetoptionstypedef) 
2. See [:material-code-braces: UpsertRedshiftTargetOptionsOutputTypeDef](./type_defs.md#upsertredshifttargetoptionsoutputtypedef) 

## ActionUnionTypeDef

```python
# ActionUnionTypeDef definition

ActionUnionTypeDef = Union[
    ActionTypeDef,  # (1)
    ActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 

## AmazonRedshiftNodeDataUnionTypeDef

```python
# AmazonRedshiftNodeDataUnionTypeDef definition

AmazonRedshiftNodeDataUnionTypeDef = Union[
    AmazonRedshiftNodeDataTypeDef,  # (1)
    AmazonRedshiftNodeDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AmazonRedshiftNodeDataTypeDef](./type_defs.md#amazonredshiftnodedatatypedef) 
2. See [:material-code-braces: AmazonRedshiftNodeDataOutputTypeDef](./type_defs.md#amazonredshiftnodedataoutputtypedef) 

## SnowflakeNodeDataUnionTypeDef

```python
# SnowflakeNodeDataUnionTypeDef definition

SnowflakeNodeDataUnionTypeDef = Union[
    SnowflakeNodeDataTypeDef,  # (1)
    SnowflakeNodeDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SnowflakeNodeDataTypeDef](./type_defs.md#snowflakenodedatatypedef) 
2. See [:material-code-braces: SnowflakeNodeDataOutputTypeDef](./type_defs.md#snowflakenodedataoutputtypedef) 

## DecimalNumberUnionTypeDef

```python
# DecimalNumberUnionTypeDef definition

DecimalNumberUnionTypeDef = Union[
    DecimalNumberTypeDef,  # (1)
    DecimalNumberOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DecimalNumberTypeDef](./type_defs.md#decimalnumbertypedef) 
2. See [:material-code-braces: DecimalNumberOutputTypeDef](./type_defs.md#decimalnumberoutputtypedef) 

## GovernedCatalogTargetUnionTypeDef

```python
# GovernedCatalogTargetUnionTypeDef definition

GovernedCatalogTargetUnionTypeDef = Union[
    GovernedCatalogTargetTypeDef,  # (1)
    GovernedCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GovernedCatalogTargetTypeDef](./type_defs.md#governedcatalogtargettypedef) 
2. See [:material-code-braces: GovernedCatalogTargetOutputTypeDef](./type_defs.md#governedcatalogtargetoutputtypedef) 

## S3CatalogTargetUnionTypeDef

```python
# S3CatalogTargetUnionTypeDef definition

S3CatalogTargetUnionTypeDef = Union[
    S3CatalogTargetTypeDef,  # (1)
    S3CatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3CatalogTargetTypeDef](./type_defs.md#s3catalogtargettypedef) 
2. See [:material-code-braces: S3CatalogTargetOutputTypeDef](./type_defs.md#s3catalogtargetoutputtypedef) 

## S3DeltaCatalogTargetUnionTypeDef

```python
# S3DeltaCatalogTargetUnionTypeDef definition

S3DeltaCatalogTargetUnionTypeDef = Union[
    S3DeltaCatalogTargetTypeDef,  # (1)
    S3DeltaCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3DeltaCatalogTargetTypeDef](./type_defs.md#s3deltacatalogtargettypedef) 
2. See [:material-code-braces: S3DeltaCatalogTargetOutputTypeDef](./type_defs.md#s3deltacatalogtargetoutputtypedef) 

## S3HudiCatalogTargetUnionTypeDef

```python
# S3HudiCatalogTargetUnionTypeDef definition

S3HudiCatalogTargetUnionTypeDef = Union[
    S3HudiCatalogTargetTypeDef,  # (1)
    S3HudiCatalogTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3HudiCatalogTargetTypeDef](./type_defs.md#s3hudicatalogtargettypedef) 
2. See [:material-code-braces: S3HudiCatalogTargetOutputTypeDef](./type_defs.md#s3hudicatalogtargetoutputtypedef) 

## CodeGenNodeUnionTypeDef

```python
# CodeGenNodeUnionTypeDef definition

CodeGenNodeUnionTypeDef = Union[
    CodeGenNodeTypeDef,  # (1)
    CodeGenNodeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CodeGenNodeTypeDef](./type_defs.md#codegennodetypedef) 
2. See [:material-code-braces: CodeGenNodeOutputTypeDef](./type_defs.md#codegennodeoutputtypedef) 

## DateColumnStatisticsDataUnionTypeDef

```python
# DateColumnStatisticsDataUnionTypeDef definition

DateColumnStatisticsDataUnionTypeDef = Union[
    DateColumnStatisticsDataTypeDef,  # (1)
    DateColumnStatisticsDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DateColumnStatisticsDataTypeDef](./type_defs.md#datecolumnstatisticsdatatypedef) 
2. See [:material-code-braces: DateColumnStatisticsDataOutputTypeDef](./type_defs.md#datecolumnstatisticsdataoutputtypedef) 

## KafkaStreamingSourceOptionsUnionTypeDef

```python
# KafkaStreamingSourceOptionsUnionTypeDef definition

KafkaStreamingSourceOptionsUnionTypeDef = Union[
    KafkaStreamingSourceOptionsTypeDef,  # (1)
    KafkaStreamingSourceOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KafkaStreamingSourceOptionsTypeDef](./type_defs.md#kafkastreamingsourceoptionstypedef) 
2. See [:material-code-braces: KafkaStreamingSourceOptionsOutputTypeDef](./type_defs.md#kafkastreamingsourceoptionsoutputtypedef) 

## KinesisStreamingSourceOptionsUnionTypeDef

```python
# KinesisStreamingSourceOptionsUnionTypeDef definition

KinesisStreamingSourceOptionsUnionTypeDef = Union[
    KinesisStreamingSourceOptionsTypeDef,  # (1)
    KinesisStreamingSourceOptionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: KinesisStreamingSourceOptionsTypeDef](./type_defs.md#kinesisstreamingsourceoptionstypedef) 
2. See [:material-code-braces: KinesisStreamingSourceOptionsOutputTypeDef](./type_defs.md#kinesisstreamingsourceoptionsoutputtypedef) 

## PredicateUnionTypeDef

```python
# PredicateUnionTypeDef definition

PredicateUnionTypeDef = Union[
    PredicateTypeDef,  # (1)
    PredicateOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
2. See [:material-code-braces: PredicateOutputTypeDef](./type_defs.md#predicateoutputtypedef) 

## EvaluateDataQualityMultiFrameUnionTypeDef

```python
# EvaluateDataQualityMultiFrameUnionTypeDef definition

EvaluateDataQualityMultiFrameUnionTypeDef = Union[
    EvaluateDataQualityMultiFrameTypeDef,  # (1)
    EvaluateDataQualityMultiFrameOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluateDataQualityMultiFrameTypeDef](./type_defs.md#evaluatedataqualitymultiframetypedef) 
2. See [:material-code-braces: EvaluateDataQualityMultiFrameOutputTypeDef](./type_defs.md#evaluatedataqualitymultiframeoutputtypedef) 

## EvaluateDataQualityUnionTypeDef

```python
# EvaluateDataQualityUnionTypeDef definition

EvaluateDataQualityUnionTypeDef = Union[
    EvaluateDataQualityTypeDef,  # (1)
    EvaluateDataQualityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluateDataQualityTypeDef](./type_defs.md#evaluatedataqualitytypedef) 
2. See [:material-code-braces: EvaluateDataQualityOutputTypeDef](./type_defs.md#evaluatedataqualityoutputtypedef) 

## PrincipalPermissionsUnionTypeDef

```python
# PrincipalPermissionsUnionTypeDef definition

PrincipalPermissionsUnionTypeDef = Union[
    PrincipalPermissionsTypeDef,  # (1)
    PrincipalPermissionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) 
2. See [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 

## S3DeltaDirectTargetUnionTypeDef

```python
# S3DeltaDirectTargetUnionTypeDef definition

S3DeltaDirectTargetUnionTypeDef = Union[
    S3DeltaDirectTargetTypeDef,  # (1)
    S3DeltaDirectTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3DeltaDirectTargetTypeDef](./type_defs.md#s3deltadirecttargettypedef) 
2. See [:material-code-braces: S3DeltaDirectTargetOutputTypeDef](./type_defs.md#s3deltadirecttargetoutputtypedef) 

## S3DirectTargetUnionTypeDef

```python
# S3DirectTargetUnionTypeDef definition

S3DirectTargetUnionTypeDef = Union[
    S3DirectTargetTypeDef,  # (1)
    S3DirectTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3DirectTargetTypeDef](./type_defs.md#s3directtargettypedef) 
2. See [:material-code-braces: S3DirectTargetOutputTypeDef](./type_defs.md#s3directtargetoutputtypedef) 

## S3GlueParquetTargetUnionTypeDef

```python
# S3GlueParquetTargetUnionTypeDef definition

S3GlueParquetTargetUnionTypeDef = Union[
    S3GlueParquetTargetTypeDef,  # (1)
    S3GlueParquetTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3GlueParquetTargetTypeDef](./type_defs.md#s3glueparquettargettypedef) 
2. See [:material-code-braces: S3GlueParquetTargetOutputTypeDef](./type_defs.md#s3glueparquettargetoutputtypedef) 

## S3HudiDirectTargetUnionTypeDef

```python
# S3HudiDirectTargetUnionTypeDef definition

S3HudiDirectTargetUnionTypeDef = Union[
    S3HudiDirectTargetTypeDef,  # (1)
    S3HudiDirectTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3HudiDirectTargetTypeDef](./type_defs.md#s3hudidirecttargettypedef) 
2. See [:material-code-braces: S3HudiDirectTargetOutputTypeDef](./type_defs.md#s3hudidirecttargetoutputtypedef) 

## GlueSchemaUnionTypeDef

```python
# GlueSchemaUnionTypeDef definition

GlueSchemaUnionTypeDef = Union[
    GlueSchemaTypeDef,  # (1)
    GlueSchemaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
2. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 

## AggregateUnionTypeDef

```python
# AggregateUnionTypeDef definition

AggregateUnionTypeDef = Union[
    AggregateTypeDef,  # (1)
    AggregateOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AggregateTypeDef](./type_defs.md#aggregatetypedef) 
2. See [:material-code-braces: AggregateOutputTypeDef](./type_defs.md#aggregateoutputtypedef) 

## DropNullFieldsUnionTypeDef

```python
# DropNullFieldsUnionTypeDef definition

DropNullFieldsUnionTypeDef = Union[
    DropNullFieldsTypeDef,  # (1)
    DropNullFieldsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DropNullFieldsTypeDef](./type_defs.md#dropnullfieldstypedef) 
2. See [:material-code-braces: DropNullFieldsOutputTypeDef](./type_defs.md#dropnullfieldsoutputtypedef) 

## FilterExpressionUnionTypeDef

```python
# FilterExpressionUnionTypeDef definition

FilterExpressionUnionTypeDef = Union[
    FilterExpressionTypeDef,  # (1)
    FilterExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) 
2. See [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 

## AthenaConnectorSourceUnionTypeDef

```python
# AthenaConnectorSourceUnionTypeDef definition

AthenaConnectorSourceUnionTypeDef = Union[
    AthenaConnectorSourceTypeDef,  # (1)
    AthenaConnectorSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AthenaConnectorSourceTypeDef](./type_defs.md#athenaconnectorsourcetypedef) 
2. See [:material-code-braces: AthenaConnectorSourceOutputTypeDef](./type_defs.md#athenaconnectorsourceoutputtypedef) 

## CatalogDeltaSourceUnionTypeDef

```python
# CatalogDeltaSourceUnionTypeDef definition

CatalogDeltaSourceUnionTypeDef = Union[
    CatalogDeltaSourceTypeDef,  # (1)
    CatalogDeltaSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CatalogDeltaSourceTypeDef](./type_defs.md#catalogdeltasourcetypedef) 
2. See [:material-code-braces: CatalogDeltaSourceOutputTypeDef](./type_defs.md#catalogdeltasourceoutputtypedef) 

## CatalogHudiSourceUnionTypeDef

```python
# CatalogHudiSourceUnionTypeDef definition

CatalogHudiSourceUnionTypeDef = Union[
    CatalogHudiSourceTypeDef,  # (1)
    CatalogHudiSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CatalogHudiSourceTypeDef](./type_defs.md#cataloghudisourcetypedef) 
2. See [:material-code-braces: CatalogHudiSourceOutputTypeDef](./type_defs.md#cataloghudisourceoutputtypedef) 

## CustomCodeUnionTypeDef

```python
# CustomCodeUnionTypeDef definition

CustomCodeUnionTypeDef = Union[
    CustomCodeTypeDef,  # (1)
    CustomCodeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomCodeTypeDef](./type_defs.md#customcodetypedef) 
2. See [:material-code-braces: CustomCodeOutputTypeDef](./type_defs.md#customcodeoutputtypedef) 

## JDBCConnectorTargetUnionTypeDef

```python
# JDBCConnectorTargetUnionTypeDef definition

JDBCConnectorTargetUnionTypeDef = Union[
    JDBCConnectorTargetTypeDef,  # (1)
    JDBCConnectorTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JDBCConnectorTargetTypeDef](./type_defs.md#jdbcconnectortargettypedef) 
2. See [:material-code-braces: JDBCConnectorTargetOutputTypeDef](./type_defs.md#jdbcconnectortargetoutputtypedef) 

## S3CatalogDeltaSourceUnionTypeDef

```python
# S3CatalogDeltaSourceUnionTypeDef definition

S3CatalogDeltaSourceUnionTypeDef = Union[
    S3CatalogDeltaSourceTypeDef,  # (1)
    S3CatalogDeltaSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3CatalogDeltaSourceTypeDef](./type_defs.md#s3catalogdeltasourcetypedef) 
2. See [:material-code-braces: S3CatalogDeltaSourceOutputTypeDef](./type_defs.md#s3catalogdeltasourceoutputtypedef) 

## S3CatalogHudiSourceUnionTypeDef

```python
# S3CatalogHudiSourceUnionTypeDef definition

S3CatalogHudiSourceUnionTypeDef = Union[
    S3CatalogHudiSourceTypeDef,  # (1)
    S3CatalogHudiSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3CatalogHudiSourceTypeDef](./type_defs.md#s3cataloghudisourcetypedef) 
2. See [:material-code-braces: S3CatalogHudiSourceOutputTypeDef](./type_defs.md#s3cataloghudisourceoutputtypedef) 

## S3CsvSourceUnionTypeDef

```python
# S3CsvSourceUnionTypeDef definition

S3CsvSourceUnionTypeDef = Union[
    S3CsvSourceTypeDef,  # (1)
    S3CsvSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3CsvSourceTypeDef](./type_defs.md#s3csvsourcetypedef) 
2. See [:material-code-braces: S3CsvSourceOutputTypeDef](./type_defs.md#s3csvsourceoutputtypedef) 

## S3DeltaSourceUnionTypeDef

```python
# S3DeltaSourceUnionTypeDef definition

S3DeltaSourceUnionTypeDef = Union[
    S3DeltaSourceTypeDef,  # (1)
    S3DeltaSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3DeltaSourceTypeDef](./type_defs.md#s3deltasourcetypedef) 
2. See [:material-code-braces: S3DeltaSourceOutputTypeDef](./type_defs.md#s3deltasourceoutputtypedef) 

## S3HudiSourceUnionTypeDef

```python
# S3HudiSourceUnionTypeDef definition

S3HudiSourceUnionTypeDef = Union[
    S3HudiSourceTypeDef,  # (1)
    S3HudiSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3HudiSourceTypeDef](./type_defs.md#s3hudisourcetypedef) 
2. See [:material-code-braces: S3HudiSourceOutputTypeDef](./type_defs.md#s3hudisourceoutputtypedef) 

## S3JsonSourceUnionTypeDef

```python
# S3JsonSourceUnionTypeDef definition

S3JsonSourceUnionTypeDef = Union[
    S3JsonSourceTypeDef,  # (1)
    S3JsonSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3JsonSourceTypeDef](./type_defs.md#s3jsonsourcetypedef) 
2. See [:material-code-braces: S3JsonSourceOutputTypeDef](./type_defs.md#s3jsonsourceoutputtypedef) 

## S3ParquetSourceUnionTypeDef

```python
# S3ParquetSourceUnionTypeDef definition

S3ParquetSourceUnionTypeDef = Union[
    S3ParquetSourceTypeDef,  # (1)
    S3ParquetSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3ParquetSourceTypeDef](./type_defs.md#s3parquetsourcetypedef) 
2. See [:material-code-braces: S3ParquetSourceOutputTypeDef](./type_defs.md#s3parquetsourceoutputtypedef) 

## SparkConnectorSourceUnionTypeDef

```python
# SparkConnectorSourceUnionTypeDef definition

SparkConnectorSourceUnionTypeDef = Union[
    SparkConnectorSourceTypeDef,  # (1)
    SparkConnectorSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SparkConnectorSourceTypeDef](./type_defs.md#sparkconnectorsourcetypedef) 
2. See [:material-code-braces: SparkConnectorSourceOutputTypeDef](./type_defs.md#sparkconnectorsourceoutputtypedef) 

## SparkConnectorTargetUnionTypeDef

```python
# SparkConnectorTargetUnionTypeDef definition

SparkConnectorTargetUnionTypeDef = Union[
    SparkConnectorTargetTypeDef,  # (1)
    SparkConnectorTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SparkConnectorTargetTypeDef](./type_defs.md#sparkconnectortargettypedef) 
2. See [:material-code-braces: SparkConnectorTargetOutputTypeDef](./type_defs.md#sparkconnectortargetoutputtypedef) 

## SparkSQLUnionTypeDef

```python
# SparkSQLUnionTypeDef definition

SparkSQLUnionTypeDef = Union[
    SparkSQLTypeDef,  # (1)
    SparkSQLOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SparkSQLTypeDef](./type_defs.md#sparksqltypedef) 
2. See [:material-code-braces: SparkSQLOutputTypeDef](./type_defs.md#sparksqloutputtypedef) 

## DataSourceUnionTypeDef

```python
# DataSourceUnionTypeDef definition

DataSourceUnionTypeDef = Union[
    DataSourceTypeDef,  # (1)
    DataSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 

## JDBCConnectorSourceUnionTypeDef

```python
# JDBCConnectorSourceUnionTypeDef definition

JDBCConnectorSourceUnionTypeDef = Union[
    JDBCConnectorSourceTypeDef,  # (1)
    JDBCConnectorSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JDBCConnectorSourceTypeDef](./type_defs.md#jdbcconnectorsourcetypedef) 
2. See [:material-code-braces: JDBCConnectorSourceOutputTypeDef](./type_defs.md#jdbcconnectorsourceoutputtypedef) 

## JoinUnionTypeDef

```python
# JoinUnionTypeDef definition

JoinUnionTypeDef = Union[
    JoinTypeDef,  # (1)
    JoinOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JoinTypeDef](./type_defs.md#jointypedef) 
2. See [:material-code-braces: JoinOutputTypeDef](./type_defs.md#joinoutputtypedef) 

## ApplyMappingUnionTypeDef

```python
# ApplyMappingUnionTypeDef definition

ApplyMappingUnionTypeDef = Union[
    ApplyMappingTypeDef,  # (1)
    ApplyMappingOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ApplyMappingTypeDef](./type_defs.md#applymappingtypedef) 
2. See [:material-code-braces: ApplyMappingOutputTypeDef](./type_defs.md#applymappingoutputtypedef) 

## RecipeStepUnionTypeDef

```python
# RecipeStepUnionTypeDef definition

RecipeStepUnionTypeDef = Union[
    RecipeStepTypeDef,  # (1)
    RecipeStepOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RecipeStepTypeDef](./type_defs.md#recipesteptypedef) 
2. See [:material-code-braces: RecipeStepOutputTypeDef](./type_defs.md#recipestepoutputtypedef) 

## StorageDescriptorUnionTypeDef

```python
# StorageDescriptorUnionTypeDef definition

StorageDescriptorUnionTypeDef = Union[
    StorageDescriptorTypeDef,  # (1)
    StorageDescriptorOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StorageDescriptorTypeDef](./type_defs.md#storagedescriptortypedef) 
2. See [:material-code-braces: StorageDescriptorOutputTypeDef](./type_defs.md#storagedescriptoroutputtypedef) 

## DynamicTransformUnionTypeDef

```python
# DynamicTransformUnionTypeDef definition

DynamicTransformUnionTypeDef = Union[
    DynamicTransformTypeDef,  # (1)
    DynamicTransformOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DynamicTransformTypeDef](./type_defs.md#dynamictransformtypedef) 
2. See [:material-code-braces: DynamicTransformOutputTypeDef](./type_defs.md#dynamictransformoutputtypedef) 

## RedshiftTargetUnionTypeDef

```python
# RedshiftTargetUnionTypeDef definition

RedshiftTargetUnionTypeDef = Union[
    RedshiftTargetTypeDef,  # (1)
    RedshiftTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RedshiftTargetTypeDef](./type_defs.md#redshifttargettypedef) 
2. See [:material-code-braces: RedshiftTargetOutputTypeDef](./type_defs.md#redshifttargetoutputtypedef) 

## AmazonRedshiftSourceUnionTypeDef

```python
# AmazonRedshiftSourceUnionTypeDef definition

AmazonRedshiftSourceUnionTypeDef = Union[
    AmazonRedshiftSourceTypeDef,  # (1)
    AmazonRedshiftSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AmazonRedshiftSourceTypeDef](./type_defs.md#amazonredshiftsourcetypedef) 
2. See [:material-code-braces: AmazonRedshiftSourceOutputTypeDef](./type_defs.md#amazonredshiftsourceoutputtypedef) 

## AmazonRedshiftTargetUnionTypeDef

```python
# AmazonRedshiftTargetUnionTypeDef definition

AmazonRedshiftTargetUnionTypeDef = Union[
    AmazonRedshiftTargetTypeDef,  # (1)
    AmazonRedshiftTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AmazonRedshiftTargetTypeDef](./type_defs.md#amazonredshifttargettypedef) 
2. See [:material-code-braces: AmazonRedshiftTargetOutputTypeDef](./type_defs.md#amazonredshifttargetoutputtypedef) 

## SnowflakeTargetUnionTypeDef

```python
# SnowflakeTargetUnionTypeDef definition

SnowflakeTargetUnionTypeDef = Union[
    SnowflakeTargetTypeDef,  # (1)
    SnowflakeTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SnowflakeTargetTypeDef](./type_defs.md#snowflaketargettypedef) 
2. See [:material-code-braces: SnowflakeTargetOutputTypeDef](./type_defs.md#snowflaketargetoutputtypedef) 

## DecimalColumnStatisticsDataUnionTypeDef

```python
# DecimalColumnStatisticsDataUnionTypeDef definition

DecimalColumnStatisticsDataUnionTypeDef = Union[
    DecimalColumnStatisticsDataTypeDef,  # (1)
    DecimalColumnStatisticsDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DecimalColumnStatisticsDataTypeDef](./type_defs.md#decimalcolumnstatisticsdatatypedef) 
2. See [:material-code-braces: DecimalColumnStatisticsDataOutputTypeDef](./type_defs.md#decimalcolumnstatisticsdataoutputtypedef) 

## CatalogKafkaSourceUnionTypeDef

```python
# CatalogKafkaSourceUnionTypeDef definition

CatalogKafkaSourceUnionTypeDef = Union[
    CatalogKafkaSourceTypeDef,  # (1)
    CatalogKafkaSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CatalogKafkaSourceTypeDef](./type_defs.md#catalogkafkasourcetypedef) 
2. See [:material-code-braces: CatalogKafkaSourceOutputTypeDef](./type_defs.md#catalogkafkasourceoutputtypedef) 

## DirectKafkaSourceUnionTypeDef

```python
# DirectKafkaSourceUnionTypeDef definition

DirectKafkaSourceUnionTypeDef = Union[
    DirectKafkaSourceTypeDef,  # (1)
    DirectKafkaSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DirectKafkaSourceTypeDef](./type_defs.md#directkafkasourcetypedef) 
2. See [:material-code-braces: DirectKafkaSourceOutputTypeDef](./type_defs.md#directkafkasourceoutputtypedef) 

## CatalogKinesisSourceUnionTypeDef

```python
# CatalogKinesisSourceUnionTypeDef definition

CatalogKinesisSourceUnionTypeDef = Union[
    CatalogKinesisSourceTypeDef,  # (1)
    CatalogKinesisSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CatalogKinesisSourceTypeDef](./type_defs.md#catalogkinesissourcetypedef) 
2. See [:material-code-braces: CatalogKinesisSourceOutputTypeDef](./type_defs.md#catalogkinesissourceoutputtypedef) 

## DirectKinesisSourceUnionTypeDef

```python
# DirectKinesisSourceUnionTypeDef definition

DirectKinesisSourceUnionTypeDef = Union[
    DirectKinesisSourceTypeDef,  # (1)
    DirectKinesisSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DirectKinesisSourceTypeDef](./type_defs.md#directkinesissourcetypedef) 
2. See [:material-code-braces: DirectKinesisSourceOutputTypeDef](./type_defs.md#directkinesissourceoutputtypedef) 

## ConnectorDataSourceUnionTypeDef

```python
# ConnectorDataSourceUnionTypeDef definition

ConnectorDataSourceUnionTypeDef = Union[
    ConnectorDataSourceTypeDef,  # (1)
    ConnectorDataSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConnectorDataSourceTypeDef](./type_defs.md#connectordatasourcetypedef) 
2. See [:material-code-braces: ConnectorDataSourceOutputTypeDef](./type_defs.md#connectordatasourceoutputtypedef) 

## SnowflakeSourceUnionTypeDef

```python
# SnowflakeSourceUnionTypeDef definition

SnowflakeSourceUnionTypeDef = Union[
    SnowflakeSourceTypeDef,  # (1)
    SnowflakeSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SnowflakeSourceTypeDef](./type_defs.md#snowflakesourcetypedef) 
2. See [:material-code-braces: SnowflakeSourceOutputTypeDef](./type_defs.md#snowflakesourceoutputtypedef) 

## FilterUnionTypeDef

```python
# FilterUnionTypeDef definition

FilterUnionTypeDef = Union[
    FilterTypeDef,  # (1)
    FilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef) 

## RecipeUnionTypeDef

```python
# RecipeUnionTypeDef definition

RecipeUnionTypeDef = Union[
    RecipeTypeDef,  # (1)
    RecipeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RecipeTypeDef](./type_defs.md#recipetypedef) 
2. See [:material-code-braces: RecipeOutputTypeDef](./type_defs.md#recipeoutputtypedef) 

## ColumnStatisticsDataUnionTypeDef

```python
# ColumnStatisticsDataUnionTypeDef definition

ColumnStatisticsDataUnionTypeDef = Union[
    ColumnStatisticsDataTypeDef,  # (1)
    ColumnStatisticsDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnStatisticsDataTypeDef](./type_defs.md#columnstatisticsdatatypedef) 
2. See [:material-code-braces: ColumnStatisticsDataOutputTypeDef](./type_defs.md#columnstatisticsdataoutputtypedef) 

## CodeGenConfigurationNodeUnionTypeDef

```python
# CodeGenConfigurationNodeUnionTypeDef definition

CodeGenConfigurationNodeUnionTypeDef = Union[
    CodeGenConfigurationNodeTypeDef,  # (1)
    CodeGenConfigurationNodeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CodeGenConfigurationNodeTypeDef](./type_defs.md#codegenconfigurationnodetypedef) 
2. See [:material-code-braces: CodeGenConfigurationNodeOutputTypeDef](./type_defs.md#codegenconfigurationnodeoutputtypedef) 

## ColumnStatisticsUnionTypeDef

```python
# ColumnStatisticsUnionTypeDef definition

ColumnStatisticsUnionTypeDef = Union[
    ColumnStatisticsTypeDef,  # (1)
    ColumnStatisticsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
2. See [:material-code-braces: ColumnStatisticsOutputTypeDef](./type_defs.md#columnstatisticsoutputtypedef) 



## NotificationPropertyTypeDef

```python
# NotificationPropertyTypeDef definition

class NotificationPropertyTypeDef(TypedDict):
    NotifyDelayAfter: NotRequired[int],
```

## AggregateOperationOutputTypeDef

```python
# AggregateOperationOutputTypeDef definition

class AggregateOperationOutputTypeDef(TypedDict):
    Column: List[str],
    AggFunc: AggFunctionType,  # (1)
```

1. See [:material-code-brackets: AggFunctionType](./literals.md#aggfunctiontype) 
## AggregateOperationTypeDef

```python
# AggregateOperationTypeDef definition

class AggregateOperationTypeDef(TypedDict):
    Column: Sequence[str],
    AggFunc: AggFunctionType,  # (1)
```

1. See [:material-code-brackets: AggFunctionType](./literals.md#aggfunctiontype) 
## AllowedValueTypeDef

```python
# AllowedValueTypeDef definition

class AllowedValueTypeDef(TypedDict):
    Value: str,
    Description: NotRequired[str],
```

## AmazonRedshiftAdvancedOptionTypeDef

```python
# AmazonRedshiftAdvancedOptionTypeDef definition

class AmazonRedshiftAdvancedOptionTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## OptionTypeDef

```python
# OptionTypeDef definition

class OptionTypeDef(TypedDict):
    Value: NotRequired[str],
    Label: NotRequired[str],
    Description: NotRequired[str],
```

## AnnotationErrorTypeDef

```python
# AnnotationErrorTypeDef definition

class AnnotationErrorTypeDef(TypedDict):
    ProfileId: NotRequired[str],
    StatisticId: NotRequired[str],
    FailureReason: NotRequired[str],
```

## MappingOutputTypeDef

```python
# MappingOutputTypeDef definition

class MappingOutputTypeDef(TypedDict):
    ToKey: NotRequired[str],
    FromPath: NotRequired[List[str]],
    FromType: NotRequired[str],
    ToType: NotRequired[str],
    Dropped: NotRequired[bool],
    Children: NotRequired[List[Dict[str, Any]]],
```

## MappingPaginatorTypeDef

```python
# MappingPaginatorTypeDef definition

class MappingPaginatorTypeDef(TypedDict):
    ToKey: NotRequired[str],
    FromPath: NotRequired[List[str]],
    FromType: NotRequired[str],
    ToType: NotRequired[str],
    Dropped: NotRequired[bool],
    Children: NotRequired[List[Dict[str, Any]]],
```

## AuditContextTypeDef

```python
# AuditContextTypeDef definition

class AuditContextTypeDef(TypedDict):
    AdditionalAuditContext: NotRequired[str],
    RequestedColumns: NotRequired[Sequence[str]],
    AllColumnsRequested: NotRequired[bool],
```

## BasicAuthenticationCredentialsTypeDef

```python
# BasicAuthenticationCredentialsTypeDef definition

class BasicAuthenticationCredentialsTypeDef(TypedDict):
    Username: NotRequired[str],
    Password: NotRequired[str],
```

## AuthorizationCodePropertiesTypeDef

```python
# AuthorizationCodePropertiesTypeDef definition

class AuthorizationCodePropertiesTypeDef(TypedDict):
    AuthorizationCode: NotRequired[str],
    RedirectUri: NotRequired[str],
```

## PartitionValueListOutputTypeDef

```python
# PartitionValueListOutputTypeDef definition

class PartitionValueListOutputTypeDef(TypedDict):
    Values: List[str],
```

## BasicCatalogTargetOutputTypeDef

```python
# BasicCatalogTargetOutputTypeDef definition

class BasicCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
    PartitionKeys: NotRequired[List[List[str]]],
```

## BasicCatalogTargetTypeDef

```python
# BasicCatalogTargetTypeDef definition

class BasicCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Database: str,
    Table: str,
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
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

## BatchDeleteConnectionRequestRequestTypeDef

```python
# BatchDeleteConnectionRequestRequestTypeDef definition

class BatchDeleteConnectionRequestRequestTypeDef(TypedDict):
    ConnectionNameList: Sequence[str],
    CatalogId: NotRequired[str],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchDeleteTableRequestRequestTypeDef

```python
# BatchDeleteTableRequestRequestTypeDef definition

class BatchDeleteTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TablesToDelete: Sequence[str],
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
```

## BatchDeleteTableVersionRequestRequestTypeDef

```python
# BatchDeleteTableVersionRequestRequestTypeDef definition

class BatchDeleteTableVersionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    VersionIds: Sequence[str],
    CatalogId: NotRequired[str],
```

## BatchGetBlueprintsRequestRequestTypeDef

```python
# BatchGetBlueprintsRequestRequestTypeDef definition

class BatchGetBlueprintsRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
    IncludeBlueprint: NotRequired[bool],
    IncludeParameterSpec: NotRequired[bool],
```

## BatchGetCrawlersRequestRequestTypeDef

```python
# BatchGetCrawlersRequestRequestTypeDef definition

class BatchGetCrawlersRequestRequestTypeDef(TypedDict):
    CrawlerNames: Sequence[str],
```

## BatchGetCustomEntityTypesRequestRequestTypeDef

```python
# BatchGetCustomEntityTypesRequestRequestTypeDef definition

class BatchGetCustomEntityTypesRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
```

## CustomEntityTypeTypeDef

```python
# CustomEntityTypeTypeDef definition

class CustomEntityTypeTypeDef(TypedDict):
    Name: str,
    RegexString: str,
    ContextWords: NotRequired[List[str]],
```

## BatchGetDataQualityResultRequestRequestTypeDef

```python
# BatchGetDataQualityResultRequestRequestTypeDef definition

class BatchGetDataQualityResultRequestRequestTypeDef(TypedDict):
    ResultIds: Sequence[str],
```

## BatchGetDevEndpointsRequestRequestTypeDef

```python
# BatchGetDevEndpointsRequestRequestTypeDef definition

class BatchGetDevEndpointsRequestRequestTypeDef(TypedDict):
    DevEndpointNames: Sequence[str],
```

## DevEndpointTypeDef

```python
# DevEndpointTypeDef definition

class DevEndpointTypeDef(TypedDict):
    EndpointName: NotRequired[str],
    RoleArn: NotRequired[str],
    SecurityGroupIds: NotRequired[List[str]],
    SubnetId: NotRequired[str],
    YarnEndpointAddress: NotRequired[str],
    PrivateAddress: NotRequired[str],
    ZeppelinRemoteSparkInterpreterPort: NotRequired[int],
    PublicAddress: NotRequired[str],
    Status: NotRequired[str],
    WorkerType: NotRequired[WorkerTypeType],  # (1)
    GlueVersion: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    NumberOfNodes: NotRequired[int],
    AvailabilityZone: NotRequired[str],
    VpcId: NotRequired[str],
    ExtraPythonLibsS3Path: NotRequired[str],
    ExtraJarsS3Path: NotRequired[str],
    FailureReason: NotRequired[str],
    LastUpdateStatus: NotRequired[str],
    CreatedTimestamp: NotRequired[datetime],
    LastModifiedTimestamp: NotRequired[datetime],
    PublicKey: NotRequired[str],
    PublicKeys: NotRequired[List[str]],
    SecurityConfiguration: NotRequired[str],
    Arguments: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## BatchGetJobsRequestRequestTypeDef

```python
# BatchGetJobsRequestRequestTypeDef definition

class BatchGetJobsRequestRequestTypeDef(TypedDict):
    JobNames: Sequence[str],
```

## PartitionValueListTypeDef

```python
# PartitionValueListTypeDef definition

class PartitionValueListTypeDef(TypedDict):
    Values: Sequence[str],
```

## BatchGetTableOptimizerEntryTypeDef

```python
# BatchGetTableOptimizerEntryTypeDef definition

class BatchGetTableOptimizerEntryTypeDef(TypedDict):
    catalogId: NotRequired[str],
    databaseName: NotRequired[str],
    tableName: NotRequired[str],
    type: NotRequired[TableOptimizerTypeType],  # (1)
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
## BatchGetTriggersRequestRequestTypeDef

```python
# BatchGetTriggersRequestRequestTypeDef definition

class BatchGetTriggersRequestRequestTypeDef(TypedDict):
    TriggerNames: Sequence[str],
```

## BatchGetWorkflowsRequestRequestTypeDef

```python
# BatchGetWorkflowsRequestRequestTypeDef definition

class BatchGetWorkflowsRequestRequestTypeDef(TypedDict):
    Names: Sequence[str],
    IncludeGraph: NotRequired[bool],
```

## DatapointInclusionAnnotationTypeDef

```python
# DatapointInclusionAnnotationTypeDef definition

class DatapointInclusionAnnotationTypeDef(TypedDict):
    ProfileId: NotRequired[str],
    StatisticId: NotRequired[str],
    InclusionAnnotation: NotRequired[InclusionAnnotationValueType],  # (1)
```

1. See [:material-code-brackets: InclusionAnnotationValueType](./literals.md#inclusionannotationvaluetype) 
## BatchStopJobRunRequestRequestTypeDef

```python
# BatchStopJobRunRequestRequestTypeDef definition

class BatchStopJobRunRequestRequestTypeDef(TypedDict):
    JobName: str,
    JobRunIds: Sequence[str],
```

## BatchStopJobRunSuccessfulSubmissionTypeDef

```python
# BatchStopJobRunSuccessfulSubmissionTypeDef definition

class BatchStopJobRunSuccessfulSubmissionTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
```

## BinaryColumnStatisticsDataTypeDef

```python
# BinaryColumnStatisticsDataTypeDef definition

class BinaryColumnStatisticsDataTypeDef(TypedDict):
    MaximumLength: int,
    AverageLength: float,
    NumberOfNulls: int,
```

## BlueprintDetailsTypeDef

```python
# BlueprintDetailsTypeDef definition

class BlueprintDetailsTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
    RunId: NotRequired[str],
```

## BlueprintRunTypeDef

```python
# BlueprintRunTypeDef definition

class BlueprintRunTypeDef(TypedDict):
    BlueprintName: NotRequired[str],
    RunId: NotRequired[str],
    WorkflowName: NotRequired[str],
    State: NotRequired[BlueprintRunStateType],  # (1)
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
    RollbackErrorMessage: NotRequired[str],
    Parameters: NotRequired[str],
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: BlueprintRunStateType](./literals.md#blueprintrunstatetype) 
## LastActiveDefinitionTypeDef

```python
# LastActiveDefinitionTypeDef definition

class LastActiveDefinitionTypeDef(TypedDict):
    Description: NotRequired[str],
    LastModifiedOn: NotRequired[datetime],
    ParameterSpec: NotRequired[str],
    BlueprintLocation: NotRequired[str],
    BlueprintServiceLocation: NotRequired[str],
```

## BooleanColumnStatisticsDataTypeDef

```python
# BooleanColumnStatisticsDataTypeDef definition

class BooleanColumnStatisticsDataTypeDef(TypedDict):
    NumberOfTrues: int,
    NumberOfFalses: int,
    NumberOfNulls: int,
```

## CancelDataQualityRuleRecommendationRunRequestRequestTypeDef

```python
# CancelDataQualityRuleRecommendationRunRequestRequestTypeDef definition

class CancelDataQualityRuleRecommendationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef

```python
# CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef definition

class CancelDataQualityRulesetEvaluationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## CancelMLTaskRunRequestRequestTypeDef

```python
# CancelMLTaskRunRequestRequestTypeDef definition

class CancelMLTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
```

## CancelStatementRequestRequestTypeDef

```python
# CancelStatementRequestRequestTypeDef definition

class CancelStatementRequestRequestTypeDef(TypedDict):
    SessionId: str,
    Id: int,
    RequestOrigin: NotRequired[str],
```

## CapabilitiesTypeDef

```python
# CapabilitiesTypeDef definition

class CapabilitiesTypeDef(TypedDict):
    SupportedAuthenticationTypes: List[AuthenticationTypeType],  # (1)
    SupportedDataOperations: List[DataOperationType],  # (2)
    SupportedComputeEnvironments: List[ComputeEnvironmentType],  # (3)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-brackets: DataOperationType](./literals.md#dataoperationtype) 
3. See [:material-code-brackets: ComputeEnvironmentType](./literals.md#computeenvironmenttype) 
## CatalogEntryTypeDef

```python
# CatalogEntryTypeDef definition

class CatalogEntryTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## CatalogImportStatusTypeDef

```python
# CatalogImportStatusTypeDef definition

class CatalogImportStatusTypeDef(TypedDict):
    ImportCompleted: NotRequired[bool],
    ImportTime: NotRequired[datetime],
    ImportedBy: NotRequired[str],
```

## FederatedCatalogTypeDef

```python
# FederatedCatalogTypeDef definition

class FederatedCatalogTypeDef(TypedDict):
    Identifier: NotRequired[str],
    ConnectionName: NotRequired[str],
```

## TargetRedshiftCatalogTypeDef

```python
# TargetRedshiftCatalogTypeDef definition

class TargetRedshiftCatalogTypeDef(TypedDict):
    CatalogArn: str,
```

## KafkaStreamingSourceOptionsOutputTypeDef

```python
# KafkaStreamingSourceOptionsOutputTypeDef definition

class KafkaStreamingSourceOptionsOutputTypeDef(TypedDict):
    BootstrapServers: NotRequired[str],
    SecurityProtocol: NotRequired[str],
    ConnectionName: NotRequired[str],
    TopicName: NotRequired[str],
    Assign: NotRequired[str],
    SubscribePattern: NotRequired[str],
    Classification: NotRequired[str],
    Delimiter: NotRequired[str],
    StartingOffsets: NotRequired[str],
    EndingOffsets: NotRequired[str],
    PollTimeoutMs: NotRequired[int],
    NumRetries: NotRequired[int],
    RetryIntervalMs: NotRequired[int],
    MaxOffsetsPerTrigger: NotRequired[int],
    MinPartitions: NotRequired[int],
    IncludeHeaders: NotRequired[bool],
    AddRecordTimestamp: NotRequired[str],
    EmitConsumerLagMetrics: NotRequired[str],
    StartingTimestamp: NotRequired[datetime],
```

## StreamingDataPreviewOptionsTypeDef

```python
# StreamingDataPreviewOptionsTypeDef definition

class StreamingDataPreviewOptionsTypeDef(TypedDict):
    PollingTime: NotRequired[int],
    RecordPollingLimit: NotRequired[int],
```

## KinesisStreamingSourceOptionsOutputTypeDef

```python
# KinesisStreamingSourceOptionsOutputTypeDef definition

class KinesisStreamingSourceOptionsOutputTypeDef(TypedDict):
    EndpointUrl: NotRequired[str],
    StreamName: NotRequired[str],
    Classification: NotRequired[str],
    Delimiter: NotRequired[str],
    StartingPosition: NotRequired[StartingPositionType],  # (1)
    MaxFetchTimeInMs: NotRequired[int],
    MaxFetchRecordsPerShard: NotRequired[int],
    MaxRecordPerRead: NotRequired[int],
    AddIdleTimeBetweenReads: NotRequired[bool],
    IdleTimeBetweenReadsInMs: NotRequired[int],
    DescribeShardInterval: NotRequired[int],
    NumRetries: NotRequired[int],
    RetryIntervalMs: NotRequired[int],
    MaxRetryIntervalMs: NotRequired[int],
    AvoidEmptyBatches: NotRequired[bool],
    StreamArn: NotRequired[str],
    RoleArn: NotRequired[str],
    RoleSessionName: NotRequired[str],
    AddRecordTimestamp: NotRequired[str],
    EmitConsumerLagMetrics: NotRequired[str],
    StartingTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: StartingPositionType](./literals.md#startingpositiontype) 
## DataLakeAccessPropertiesOutputTypeDef

```python
# DataLakeAccessPropertiesOutputTypeDef definition

class DataLakeAccessPropertiesOutputTypeDef(TypedDict):
    DataLakeAccess: NotRequired[bool],
    DataTransferRole: NotRequired[str],
    KmsKey: NotRequired[str],
    ManagedWorkgroupName: NotRequired[str],
    ManagedWorkgroupStatus: NotRequired[str],
    RedshiftDatabaseName: NotRequired[str],
    StatusMessage: NotRequired[str],
    CatalogType: NotRequired[str],
```

## DataLakeAccessPropertiesTypeDef

```python
# DataLakeAccessPropertiesTypeDef definition

class DataLakeAccessPropertiesTypeDef(TypedDict):
    DataLakeAccess: NotRequired[bool],
    DataTransferRole: NotRequired[str],
    KmsKey: NotRequired[str],
    CatalogType: NotRequired[str],
```

## CatalogSchemaChangePolicyTypeDef

```python
# CatalogSchemaChangePolicyTypeDef definition

class CatalogSchemaChangePolicyTypeDef(TypedDict):
    EnableUpdateCatalog: NotRequired[bool],
    UpdateBehavior: NotRequired[UpdateCatalogBehaviorType],  # (1)
```

1. See [:material-code-brackets: UpdateCatalogBehaviorType](./literals.md#updatecatalogbehaviortype) 
## CatalogSourceTypeDef

```python
# CatalogSourceTypeDef definition

class CatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## CatalogTargetOutputTypeDef

```python
# CatalogTargetOutputTypeDef definition

class CatalogTargetOutputTypeDef(TypedDict):
    DatabaseName: str,
    Tables: List[str],
    ConnectionName: NotRequired[str],
    EventQueueArn: NotRequired[str],
    DlqEventQueueArn: NotRequired[str],
```

## CatalogTargetTypeDef

```python
# CatalogTargetTypeDef definition

class CatalogTargetTypeDef(TypedDict):
    DatabaseName: str,
    Tables: Sequence[str],
    ConnectionName: NotRequired[str],
    EventQueueArn: NotRequired[str],
    DlqEventQueueArn: NotRequired[str],
```

## CheckSchemaVersionValidityInputRequestTypeDef

```python
# CheckSchemaVersionValidityInputRequestTypeDef definition

class CheckSchemaVersionValidityInputRequestTypeDef(TypedDict):
    DataFormat: DataFormatType,  # (1)
    SchemaDefinition: str,
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
## CsvClassifierTypeDef

```python
# CsvClassifierTypeDef definition

class CsvClassifierTypeDef(TypedDict):
    Name: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
    Delimiter: NotRequired[str],
    QuoteSymbol: NotRequired[str],
    ContainsHeader: NotRequired[CsvHeaderOptionType],  # (1)
    Header: NotRequired[List[str]],
    DisableValueTrimming: NotRequired[bool],
    AllowSingleColumn: NotRequired[bool],
    CustomDatatypeConfigured: NotRequired[bool],
    CustomDatatypes: NotRequired[List[str]],
    Serde: NotRequired[CsvSerdeOptionType],  # (2)
```

1. See [:material-code-brackets: CsvHeaderOptionType](./literals.md#csvheaderoptiontype) 
2. See [:material-code-brackets: CsvSerdeOptionType](./literals.md#csvserdeoptiontype) 
## GrokClassifierTypeDef

```python
# GrokClassifierTypeDef definition

class GrokClassifierTypeDef(TypedDict):
    Name: str,
    Classification: str,
    GrokPattern: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
    CustomPatterns: NotRequired[str],
```

## JsonClassifierTypeDef

```python
# JsonClassifierTypeDef definition

class JsonClassifierTypeDef(TypedDict):
    Name: str,
    JsonPath: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
```

## XMLClassifierTypeDef

```python
# XMLClassifierTypeDef definition

class XMLClassifierTypeDef(TypedDict):
    Name: str,
    Classification: str,
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Version: NotRequired[int],
    RowTag: NotRequired[str],
```

## CloudWatchEncryptionTypeDef

```python
# CloudWatchEncryptionTypeDef definition

class CloudWatchEncryptionTypeDef(TypedDict):
    CloudWatchEncryptionMode: NotRequired[CloudWatchEncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: CloudWatchEncryptionModeType](./literals.md#cloudwatchencryptionmodetype) 
## ConnectorDataTargetOutputTypeDef

```python
# ConnectorDataTargetOutputTypeDef definition

class ConnectorDataTargetOutputTypeDef(TypedDict):
    Name: str,
    ConnectionType: str,
    Data: Dict[str, str],
    Inputs: NotRequired[List[str]],
```

## DirectJDBCSourceTypeDef

```python
# DirectJDBCSourceTypeDef definition

class DirectJDBCSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    ConnectionName: str,
    ConnectionType: JDBCConnectionTypeType,  # (1)
    RedshiftTmpDir: NotRequired[str],
```

1. See [:material-code-brackets: JDBCConnectionTypeType](./literals.md#jdbcconnectiontypetype) 
## DropDuplicatesOutputTypeDef

```python
# DropDuplicatesOutputTypeDef definition

class DropDuplicatesOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Columns: NotRequired[List[List[str]]],
```

## DropFieldsOutputTypeDef

```python
# DropFieldsOutputTypeDef definition

class DropFieldsOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Paths: List[List[str]],
```

## DynamoDBCatalogSourceTypeDef

```python
# DynamoDBCatalogSourceTypeDef definition

class DynamoDBCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## FillMissingValuesOutputTypeDef

```python
# FillMissingValuesOutputTypeDef definition

class FillMissingValuesOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    ImputedPath: str,
    FilledPath: NotRequired[str],
```

## MergeOutputTypeDef

```python
# MergeOutputTypeDef definition

class MergeOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Source: str,
    PrimaryKeys: List[List[str]],
```

## MicrosoftSQLServerCatalogSourceTypeDef

```python
# MicrosoftSQLServerCatalogSourceTypeDef definition

class MicrosoftSQLServerCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## MicrosoftSQLServerCatalogTargetOutputTypeDef

```python
# MicrosoftSQLServerCatalogTargetOutputTypeDef definition

class MicrosoftSQLServerCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## MySQLCatalogSourceTypeDef

```python
# MySQLCatalogSourceTypeDef definition

class MySQLCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## MySQLCatalogTargetOutputTypeDef

```python
# MySQLCatalogTargetOutputTypeDef definition

class MySQLCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## OracleSQLCatalogSourceTypeDef

```python
# OracleSQLCatalogSourceTypeDef definition

class OracleSQLCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## OracleSQLCatalogTargetOutputTypeDef

```python
# OracleSQLCatalogTargetOutputTypeDef definition

class OracleSQLCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## PIIDetectionOutputTypeDef

```python
# PIIDetectionOutputTypeDef definition

class PIIDetectionOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    PiiType: PiiTypeType,  # (1)
    EntityTypesToDetect: List[str],
    OutputColumnName: NotRequired[str],
    SampleFraction: NotRequired[float],
    ThresholdFraction: NotRequired[float],
    MaskValue: NotRequired[str],
```

1. See [:material-code-brackets: PiiTypeType](./literals.md#piitypetype) 
## PostgreSQLCatalogSourceTypeDef

```python
# PostgreSQLCatalogSourceTypeDef definition

class PostgreSQLCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## PostgreSQLCatalogTargetOutputTypeDef

```python
# PostgreSQLCatalogTargetOutputTypeDef definition

class PostgreSQLCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
```

## RedshiftSourceTypeDef

```python
# RedshiftSourceTypeDef definition

class RedshiftSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    RedshiftTmpDir: NotRequired[str],
    TmpDirIAMRole: NotRequired[str],
```

## RelationalCatalogSourceTypeDef

```python
# RelationalCatalogSourceTypeDef definition

class RelationalCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
```

## RenameFieldOutputTypeDef

```python
# RenameFieldOutputTypeDef definition

class RenameFieldOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    SourcePath: List[str],
    TargetPath: List[str],
```

## SelectFieldsOutputTypeDef

```python
# SelectFieldsOutputTypeDef definition

class SelectFieldsOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Paths: List[List[str]],
```

## SelectFromCollectionOutputTypeDef

```python
# SelectFromCollectionOutputTypeDef definition

class SelectFromCollectionOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Index: int,
```

## SpigotOutputTypeDef

```python
# SpigotOutputTypeDef definition

class SpigotOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Topk: NotRequired[int],
    Prob: NotRequired[float],
```

## SplitFieldsOutputTypeDef

```python
# SplitFieldsOutputTypeDef definition

class SplitFieldsOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Paths: List[List[str]],
```

## UnionOutputTypeDef

```python
# UnionOutputTypeDef definition

class UnionOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    UnionType: UnionTypeType,  # (1)
```

1. See [:material-code-brackets: UnionTypeType](./literals.md#uniontypetype) 
## CodeGenEdgeTypeDef

```python
# CodeGenEdgeTypeDef definition

class CodeGenEdgeTypeDef(TypedDict):
    Source: str,
    Target: str,
    TargetParameter: NotRequired[str],
```

## CodeGenNodeArgTypeDef

```python
# CodeGenNodeArgTypeDef definition

class CodeGenNodeArgTypeDef(TypedDict):
    Name: str,
    Value: str,
    Param: NotRequired[bool],
```

## ColumnImportanceTypeDef

```python
# ColumnImportanceTypeDef definition

class ColumnImportanceTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    Importance: NotRequired[float],
```

## ColumnOutputTypeDef

```python
# ColumnOutputTypeDef definition

class ColumnOutputTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[str],
    Comment: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
```

## ColumnRowFilterTypeDef

```python
# ColumnRowFilterTypeDef definition

class ColumnRowFilterTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    RowFilterExpression: NotRequired[str],
```

## DateColumnStatisticsDataOutputTypeDef

```python
# DateColumnStatisticsDataOutputTypeDef definition

class DateColumnStatisticsDataOutputTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[datetime],
    MaximumValue: NotRequired[datetime],
```

## DoubleColumnStatisticsDataTypeDef

```python
# DoubleColumnStatisticsDataTypeDef definition

class DoubleColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[float],
    MaximumValue: NotRequired[float],
```

## LongColumnStatisticsDataTypeDef

```python
# LongColumnStatisticsDataTypeDef definition

class LongColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[int],
    MaximumValue: NotRequired[int],
```

## StringColumnStatisticsDataTypeDef

```python
# StringColumnStatisticsDataTypeDef definition

class StringColumnStatisticsDataTypeDef(TypedDict):
    MaximumLength: int,
    AverageLength: float,
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
```

## ColumnStatisticsTaskRunTypeDef

```python
# ColumnStatisticsTaskRunTypeDef definition

class ColumnStatisticsTaskRunTypeDef(TypedDict):
    CustomerId: NotRequired[str],
    ColumnStatisticsTaskRunId: NotRequired[str],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    ColumnNameList: NotRequired[List[str]],
    CatalogID: NotRequired[str],
    Role: NotRequired[str],
    SampleSize: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    WorkerType: NotRequired[str],
    ComputationType: NotRequired[ComputationTypeType],  # (1)
    Status: NotRequired[ColumnStatisticsStateType],  # (2)
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
    DPUSeconds: NotRequired[float],
```

1. See [:material-code-brackets: ComputationTypeType](./literals.md#computationtypetype) 
2. See [:material-code-brackets: ColumnStatisticsStateType](./literals.md#columnstatisticsstatetype) 
## ExecutionAttemptTypeDef

```python
# ExecutionAttemptTypeDef definition

class ExecutionAttemptTypeDef(TypedDict):
    Status: NotRequired[ExecutionStatusType],  # (1)
    ColumnStatisticsTaskRunId: NotRequired[str],
    ExecutionTimestamp: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    ScheduleExpression: NotRequired[str],
    State: NotRequired[ScheduleStateType],  # (1)
```

1. See [:material-code-brackets: ScheduleStateType](./literals.md#schedulestatetype) 
## ColumnTypeDef

```python
# ColumnTypeDef definition

class ColumnTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[str],
    Comment: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
```

## IcebergCompactionMetricsTypeDef

```python
# IcebergCompactionMetricsTypeDef definition

class IcebergCompactionMetricsTypeDef(TypedDict):
    NumberOfBytesCompacted: NotRequired[int],
    NumberOfFilesCompacted: NotRequired[int],
    NumberOfDpus: NotRequired[int],
    JobDurationInHour: NotRequired[float],
```

## ConditionExpressionTypeDef

```python
# ConditionExpressionTypeDef definition

class ConditionExpressionTypeDef(TypedDict):
    Condition: str,
    TargetColumn: str,
    Value: NotRequired[str],
```

## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    LogicalOperator: NotRequired[LogicalOperatorType],  # (1)
    JobName: NotRequired[str],
    State: NotRequired[JobRunStateType],  # (2)
    CrawlerName: NotRequired[str],
    CrawlState: NotRequired[CrawlStateType],  # (3)
```

1. See [:material-code-brackets: LogicalOperatorType](./literals.md#logicaloperatortype) 
2. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
3. See [:material-code-brackets: CrawlStateType](./literals.md#crawlstatetype) 
## ConfigurationObjectOutputTypeDef

```python
# ConfigurationObjectOutputTypeDef definition

class ConfigurationObjectOutputTypeDef(TypedDict):
    DefaultValue: NotRequired[str],
    AllowedValues: NotRequired[List[str]],
    MinValue: NotRequired[str],
    MaxValue: NotRequired[str],
```

## ConfigurationObjectTypeDef

```python
# ConfigurationObjectTypeDef definition

class ConfigurationObjectTypeDef(TypedDict):
    DefaultValue: NotRequired[str],
    AllowedValues: NotRequired[Sequence[str]],
    MinValue: NotRequired[str],
    MaxValue: NotRequired[str],
```

## ConfusionMatrixTypeDef

```python
# ConfusionMatrixTypeDef definition

class ConfusionMatrixTypeDef(TypedDict):
    NumTruePositives: NotRequired[int],
    NumFalsePositives: NotRequired[int],
    NumTrueNegatives: NotRequired[int],
    NumFalseNegatives: NotRequired[int],
```

## ConnectionPasswordEncryptionTypeDef

```python
# ConnectionPasswordEncryptionTypeDef definition

class ConnectionPasswordEncryptionTypeDef(TypedDict):
    ReturnConnectionPasswordEncrypted: bool,
    AwsKmsKeyId: NotRequired[str],
```

## PhysicalConnectionRequirementsOutputTypeDef

```python
# PhysicalConnectionRequirementsOutputTypeDef definition

class PhysicalConnectionRequirementsOutputTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    SecurityGroupIdList: NotRequired[List[str]],
    AvailabilityZone: NotRequired[str],
```

## ConnectionsListOutputTypeDef

```python
# ConnectionsListOutputTypeDef definition

class ConnectionsListOutputTypeDef(TypedDict):
    Connections: NotRequired[List[str]],
```

## ConnectionsListTypeDef

```python
# ConnectionsListTypeDef definition

class ConnectionsListTypeDef(TypedDict):
    Connections: NotRequired[Sequence[str]],
```

## ConnectorDataTargetTypeDef

```python
# ConnectorDataTargetTypeDef definition

class ConnectorDataTargetTypeDef(TypedDict):
    Name: str,
    ConnectionType: str,
    Data: Mapping[str, str],
    Inputs: NotRequired[Sequence[str]],
```

## CrawlTypeDef

```python
# CrawlTypeDef definition

class CrawlTypeDef(TypedDict):
    State: NotRequired[CrawlStateType],  # (1)
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    ErrorMessage: NotRequired[str],
    LogGroup: NotRequired[str],
    LogStream: NotRequired[str],
```

1. See [:material-code-brackets: CrawlStateType](./literals.md#crawlstatetype) 
## CrawlerHistoryTypeDef

```python
# CrawlerHistoryTypeDef definition

class CrawlerHistoryTypeDef(TypedDict):
    CrawlId: NotRequired[str],
    State: NotRequired[CrawlerHistoryStateType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Summary: NotRequired[str],
    ErrorMessage: NotRequired[str],
    LogGroup: NotRequired[str],
    LogStream: NotRequired[str],
    MessagePrefix: NotRequired[str],
    DPUHour: NotRequired[float],
```

1. See [:material-code-brackets: CrawlerHistoryStateType](./literals.md#crawlerhistorystatetype) 
## CrawlerMetricsTypeDef

```python
# CrawlerMetricsTypeDef definition

class CrawlerMetricsTypeDef(TypedDict):
    CrawlerName: NotRequired[str],
    TimeLeftSeconds: NotRequired[float],
    StillEstimating: NotRequired[bool],
    LastRuntimeSeconds: NotRequired[float],
    MedianRuntimeSeconds: NotRequired[float],
    TablesCreated: NotRequired[int],
    TablesUpdated: NotRequired[int],
    TablesDeleted: NotRequired[int],
```

## DeltaTargetOutputTypeDef

```python
# DeltaTargetOutputTypeDef definition

class DeltaTargetOutputTypeDef(TypedDict):
    DeltaTables: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    WriteManifest: NotRequired[bool],
    CreateNativeDeltaTable: NotRequired[bool],
```

## DynamoDBTargetTypeDef

```python
# DynamoDBTargetTypeDef definition

class DynamoDBTargetTypeDef(TypedDict):
    Path: NotRequired[str],
    scanAll: NotRequired[bool],
    scanRate: NotRequired[float],
```

## HudiTargetOutputTypeDef

```python
# HudiTargetOutputTypeDef definition

class HudiTargetOutputTypeDef(TypedDict):
    Paths: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    MaximumTraversalDepth: NotRequired[int],
```

## IcebergTargetOutputTypeDef

```python
# IcebergTargetOutputTypeDef definition

class IcebergTargetOutputTypeDef(TypedDict):
    Paths: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    MaximumTraversalDepth: NotRequired[int],
```

## JdbcTargetOutputTypeDef

```python
# JdbcTargetOutputTypeDef definition

class JdbcTargetOutputTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    Path: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    EnableAdditionalMetadata: NotRequired[List[JdbcMetadataEntryType]],  # (1)
```

1. See [:material-code-brackets: JdbcMetadataEntryType](./literals.md#jdbcmetadataentrytype) 
## MongoDBTargetTypeDef

```python
# MongoDBTargetTypeDef definition

class MongoDBTargetTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    Path: NotRequired[str],
    ScanAll: NotRequired[bool],
```

## S3TargetOutputTypeDef

```python
# S3TargetOutputTypeDef definition

class S3TargetOutputTypeDef(TypedDict):
    Path: NotRequired[str],
    Exclusions: NotRequired[List[str]],
    ConnectionName: NotRequired[str],
    SampleSize: NotRequired[int],
    EventQueueArn: NotRequired[str],
    DlqEventQueueArn: NotRequired[str],
```

## LakeFormationConfigurationTypeDef

```python
# LakeFormationConfigurationTypeDef definition

class LakeFormationConfigurationTypeDef(TypedDict):
    UseLakeFormationCredentials: NotRequired[bool],
    AccountId: NotRequired[str],
```

## LastCrawlInfoTypeDef

```python
# LastCrawlInfoTypeDef definition

class LastCrawlInfoTypeDef(TypedDict):
    Status: NotRequired[LastCrawlStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    LogGroup: NotRequired[str],
    LogStream: NotRequired[str],
    MessagePrefix: NotRequired[str],
    StartTime: NotRequired[datetime],
```

1. See [:material-code-brackets: LastCrawlStatusType](./literals.md#lastcrawlstatustype) 
## LineageConfigurationTypeDef

```python
# LineageConfigurationTypeDef definition

class LineageConfigurationTypeDef(TypedDict):
    CrawlerLineageSettings: NotRequired[CrawlerLineageSettingsType],  # (1)
```

1. See [:material-code-brackets: CrawlerLineageSettingsType](./literals.md#crawlerlineagesettingstype) 
## RecrawlPolicyTypeDef

```python
# RecrawlPolicyTypeDef definition

class RecrawlPolicyTypeDef(TypedDict):
    RecrawlBehavior: NotRequired[RecrawlBehaviorType],  # (1)
```

1. See [:material-code-brackets: RecrawlBehaviorType](./literals.md#recrawlbehaviortype) 
## SchemaChangePolicyTypeDef

```python
# SchemaChangePolicyTypeDef definition

class SchemaChangePolicyTypeDef(TypedDict):
    UpdateBehavior: NotRequired[UpdateBehaviorType],  # (1)
    DeleteBehavior: NotRequired[DeleteBehaviorType],  # (2)
```

1. See [:material-code-brackets: UpdateBehaviorType](./literals.md#updatebehaviortype) 
2. See [:material-code-brackets: DeleteBehaviorType](./literals.md#deletebehaviortype) 
## CrawlsFilterTypeDef

```python
# CrawlsFilterTypeDef definition

class CrawlsFilterTypeDef(TypedDict):
    FieldName: NotRequired[FieldNameType],  # (1)
    FilterOperator: NotRequired[FilterOperatorType],  # (2)
    FieldValue: NotRequired[str],
```

1. See [:material-code-brackets: FieldNameType](./literals.md#fieldnametype) 
2. See [:material-code-brackets: FilterOperatorType](./literals.md#filteroperatortype) 
## CreateBlueprintRequestRequestTypeDef

```python
# CreateBlueprintRequestRequestTypeDef definition

class CreateBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
    BlueprintLocation: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateCsvClassifierRequestTypeDef

```python
# CreateCsvClassifierRequestTypeDef definition

class CreateCsvClassifierRequestTypeDef(TypedDict):
    Name: str,
    Delimiter: NotRequired[str],
    QuoteSymbol: NotRequired[str],
    ContainsHeader: NotRequired[CsvHeaderOptionType],  # (1)
    Header: NotRequired[Sequence[str]],
    DisableValueTrimming: NotRequired[bool],
    AllowSingleColumn: NotRequired[bool],
    CustomDatatypeConfigured: NotRequired[bool],
    CustomDatatypes: NotRequired[Sequence[str]],
    Serde: NotRequired[CsvSerdeOptionType],  # (2)
```

1. See [:material-code-brackets: CsvHeaderOptionType](./literals.md#csvheaderoptiontype) 
2. See [:material-code-brackets: CsvSerdeOptionType](./literals.md#csvserdeoptiontype) 
## CreateGrokClassifierRequestTypeDef

```python
# CreateGrokClassifierRequestTypeDef definition

class CreateGrokClassifierRequestTypeDef(TypedDict):
    Classification: str,
    Name: str,
    GrokPattern: str,
    CustomPatterns: NotRequired[str],
```

## CreateJsonClassifierRequestTypeDef

```python
# CreateJsonClassifierRequestTypeDef definition

class CreateJsonClassifierRequestTypeDef(TypedDict):
    Name: str,
    JsonPath: str,
```

## CreateXMLClassifierRequestTypeDef

```python
# CreateXMLClassifierRequestTypeDef definition

class CreateXMLClassifierRequestTypeDef(TypedDict):
    Classification: str,
    Name: str,
    RowTag: NotRequired[str],
```

## CreateColumnStatisticsTaskSettingsRequestRequestTypeDef

```python
# CreateColumnStatisticsTaskSettingsRequestRequestTypeDef definition

class CreateColumnStatisticsTaskSettingsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    Role: str,
    Schedule: NotRequired[str],
    ColumnNameList: NotRequired[Sequence[str]],
    SampleSize: NotRequired[float],
    CatalogID: NotRequired[str],
    SecurityConfiguration: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## CreateCustomEntityTypeRequestRequestTypeDef

```python
# CreateCustomEntityTypeRequestRequestTypeDef definition

class CreateCustomEntityTypeRequestRequestTypeDef(TypedDict):
    Name: str,
    RegexString: str,
    ContextWords: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## DataQualityTargetTableTypeDef

```python
# DataQualityTargetTableTypeDef definition

class DataQualityTargetTableTypeDef(TypedDict):
    TableName: str,
    DatabaseName: str,
    CatalogId: NotRequired[str],
```

## CreateDevEndpointRequestRequestTypeDef

```python
# CreateDevEndpointRequestRequestTypeDef definition

class CreateDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
    RoleArn: str,
    SecurityGroupIds: NotRequired[Sequence[str]],
    SubnetId: NotRequired[str],
    PublicKey: NotRequired[str],
    PublicKeys: NotRequired[Sequence[str]],
    NumberOfNodes: NotRequired[int],
    WorkerType: NotRequired[WorkerTypeType],  # (1)
    GlueVersion: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    ExtraPythonLibsS3Path: NotRequired[str],
    ExtraJarsS3Path: NotRequired[str],
    SecurityConfiguration: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    Arguments: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## SourceProcessingPropertiesTypeDef

```python
# SourceProcessingPropertiesTypeDef definition

class SourceProcessingPropertiesTypeDef(TypedDict):
    RoleArn: NotRequired[str],
```

## TargetProcessingPropertiesTypeDef

```python
# TargetProcessingPropertiesTypeDef definition

class TargetProcessingPropertiesTypeDef(TypedDict):
    RoleArn: NotRequired[str],
    KmsArn: NotRequired[str],
    ConnectionName: NotRequired[str],
    EventBusArn: NotRequired[str],
```

## IntegrationErrorTypeDef

```python
# IntegrationErrorTypeDef definition

class IntegrationErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## SourceTableConfigTypeDef

```python
# SourceTableConfigTypeDef definition

class SourceTableConfigTypeDef(TypedDict):
    Fields: NotRequired[Sequence[str]],
    FilterPredicate: NotRequired[str],
    PrimaryKey: NotRequired[Sequence[str]],
    RecordUpdateField: NotRequired[str],
```

## ExecutionPropertyTypeDef

```python
# ExecutionPropertyTypeDef definition

class ExecutionPropertyTypeDef(TypedDict):
    MaxConcurrentRuns: NotRequired[int],
```

## JobCommandTypeDef

```python
# JobCommandTypeDef definition

class JobCommandTypeDef(TypedDict):
    Name: NotRequired[str],
    ScriptLocation: NotRequired[str],
    PythonVersion: NotRequired[str],
    Runtime: NotRequired[str],
```

## SourceControlDetailsTypeDef

```python
# SourceControlDetailsTypeDef definition

class SourceControlDetailsTypeDef(TypedDict):
    Provider: NotRequired[SourceControlProviderType],  # (1)
    Repository: NotRequired[str],
    Owner: NotRequired[str],
    Branch: NotRequired[str],
    Folder: NotRequired[str],
    LastCommitId: NotRequired[str],
    AuthStrategy: NotRequired[SourceControlAuthStrategyType],  # (2)
    AuthToken: NotRequired[str],
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
## PartitionIndexTypeDef

```python
# PartitionIndexTypeDef definition

class PartitionIndexTypeDef(TypedDict):
    Keys: Sequence[str],
    IndexName: str,
```

## CreateRegistryInputRequestTypeDef

```python
# CreateRegistryInputRequestTypeDef definition

class CreateRegistryInputRequestTypeDef(TypedDict):
    RegistryName: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## RegistryIdTypeDef

```python
# RegistryIdTypeDef definition

class RegistryIdTypeDef(TypedDict):
    RegistryName: NotRequired[str],
    RegistryArn: NotRequired[str],
```

## SessionCommandTypeDef

```python
# SessionCommandTypeDef definition

class SessionCommandTypeDef(TypedDict):
    Name: NotRequired[str],
    PythonVersion: NotRequired[str],
```

## EventBatchingConditionTypeDef

```python
# EventBatchingConditionTypeDef definition

class EventBatchingConditionTypeDef(TypedDict):
    BatchSize: int,
    BatchWindow: NotRequired[int],
```

## CreateWorkflowRequestRequestTypeDef

```python
# CreateWorkflowRequestRequestTypeDef definition

class CreateWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    DefaultRunProperties: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Mapping[str, str]],
    MaxConcurrentRuns: NotRequired[int],
```

## DQResultsPublishingOptionsTypeDef

```python
# DQResultsPublishingOptionsTypeDef definition

class DQResultsPublishingOptionsTypeDef(TypedDict):
    EvaluationContext: NotRequired[str],
    ResultsS3Prefix: NotRequired[str],
    CloudWatchMetricsEnabled: NotRequired[bool],
    ResultsPublishingEnabled: NotRequired[bool],
```

## DQStopJobOnFailureOptionsTypeDef

```python
# DQStopJobOnFailureOptionsTypeDef definition

class DQStopJobOnFailureOptionsTypeDef(TypedDict):
    StopJobOnFailureTiming: NotRequired[DQStopJobOnFailureTimingType],  # (1)
```

1. See [:material-code-brackets: DQStopJobOnFailureTimingType](./literals.md#dqstopjobonfailuretimingtype) 
## EncryptionAtRestTypeDef

```python
# EncryptionAtRestTypeDef definition

class EncryptionAtRestTypeDef(TypedDict):
    CatalogEncryptionMode: CatalogEncryptionModeType,  # (1)
    SseAwsKmsKeyId: NotRequired[str],
    CatalogEncryptionServiceRole: NotRequired[str],
```

1. See [:material-code-brackets: CatalogEncryptionModeType](./literals.md#catalogencryptionmodetype) 
## DataLakePrincipalTypeDef

```python
# DataLakePrincipalTypeDef definition

class DataLakePrincipalTypeDef(TypedDict):
    DataLakePrincipalIdentifier: NotRequired[str],
```

## DataQualityAnalyzerResultTypeDef

```python
# DataQualityAnalyzerResultTypeDef definition

class DataQualityAnalyzerResultTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    EvaluationMessage: NotRequired[str],
    EvaluatedMetrics: NotRequired[Dict[str, float]],
```

## DataQualityEncryptionTypeDef

```python
# DataQualityEncryptionTypeDef definition

class DataQualityEncryptionTypeDef(TypedDict):
    DataQualityEncryptionMode: NotRequired[DataQualityEncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: DataQualityEncryptionModeType](./literals.md#dataqualityencryptionmodetype) 
## DataQualityEvaluationRunAdditionalRunOptionsTypeDef

```python
# DataQualityEvaluationRunAdditionalRunOptionsTypeDef definition

class DataQualityEvaluationRunAdditionalRunOptionsTypeDef(TypedDict):
    CloudWatchMetricsEnabled: NotRequired[bool],
    ResultsS3Prefix: NotRequired[str],
    CompositeRuleEvaluationMethod: NotRequired[DQCompositeRuleEvaluationMethodType],  # (1)
```

1. See [:material-code-brackets: DQCompositeRuleEvaluationMethodType](./literals.md#dqcompositeruleevaluationmethodtype) 
## DataQualityMetricValuesTypeDef

```python
# DataQualityMetricValuesTypeDef definition

class DataQualityMetricValuesTypeDef(TypedDict):
    ActualValue: NotRequired[float],
    ExpectedValue: NotRequired[float],
    LowerLimit: NotRequired[float],
    UpperLimit: NotRequired[float],
```

## DataQualityRuleResultTypeDef

```python
# DataQualityRuleResultTypeDef definition

class DataQualityRuleResultTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    EvaluationMessage: NotRequired[str],
    Result: NotRequired[DataQualityRuleResultStatusType],  # (1)
    EvaluatedMetrics: NotRequired[Dict[str, float]],
    EvaluatedRule: NotRequired[str],
```

1. See [:material-code-brackets: DataQualityRuleResultStatusType](./literals.md#dataqualityruleresultstatustype) 
## GlueTableOutputTypeDef

```python
# GlueTableOutputTypeDef definition

class GlueTableOutputTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    ConnectionName: NotRequired[str],
    AdditionalOptions: NotRequired[Dict[str, str]],
```

## DatabaseIdentifierTypeDef

```python
# DatabaseIdentifierTypeDef definition

class DatabaseIdentifierTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    Region: NotRequired[str],
```

## FederatedDatabaseTypeDef

```python
# FederatedDatabaseTypeDef definition

class FederatedDatabaseTypeDef(TypedDict):
    Identifier: NotRequired[str],
    ConnectionName: NotRequired[str],
```

## DatatypeTypeDef

```python
# DatatypeTypeDef definition

class DatatypeTypeDef(TypedDict):
    Id: str,
    Label: str,
```

## DecimalNumberOutputTypeDef

```python
# DecimalNumberOutputTypeDef definition

class DecimalNumberOutputTypeDef(TypedDict):
    UnscaledValue: bytes,
    Scale: int,
```

## DeleteBlueprintRequestRequestTypeDef

```python
# DeleteBlueprintRequestRequestTypeDef definition

class DeleteBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteCatalogRequestRequestTypeDef

```python
# DeleteCatalogRequestRequestTypeDef definition

class DeleteCatalogRequestRequestTypeDef(TypedDict):
    CatalogId: str,
```

## DeleteClassifierRequestRequestTypeDef

```python
# DeleteClassifierRequestRequestTypeDef definition

class DeleteClassifierRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteColumnStatisticsForPartitionRequestRequestTypeDef

```python
# DeleteColumnStatisticsForPartitionRequestRequestTypeDef definition

class DeleteColumnStatisticsForPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnName: str,
    CatalogId: NotRequired[str],
```

## DeleteColumnStatisticsForTableRequestRequestTypeDef

```python
# DeleteColumnStatisticsForTableRequestRequestTypeDef definition

class DeleteColumnStatisticsForTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    ColumnName: str,
    CatalogId: NotRequired[str],
```

## DeleteColumnStatisticsTaskSettingsRequestRequestTypeDef

```python
# DeleteColumnStatisticsTaskSettingsRequestRequestTypeDef definition

class DeleteColumnStatisticsTaskSettingsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## DeleteConnectionRequestRequestTypeDef

```python
# DeleteConnectionRequestRequestTypeDef definition

class DeleteConnectionRequestRequestTypeDef(TypedDict):
    ConnectionName: str,
    CatalogId: NotRequired[str],
```

## DeleteCrawlerRequestRequestTypeDef

```python
# DeleteCrawlerRequestRequestTypeDef definition

class DeleteCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteCustomEntityTypeRequestRequestTypeDef

```python
# DeleteCustomEntityTypeRequestRequestTypeDef definition

class DeleteCustomEntityTypeRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDataQualityRulesetRequestRequestTypeDef

```python
# DeleteDataQualityRulesetRequestRequestTypeDef definition

class DeleteDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteDatabaseRequestRequestTypeDef

```python
# DeleteDatabaseRequestRequestTypeDef definition

class DeleteDatabaseRequestRequestTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
```

## DeleteDevEndpointRequestRequestTypeDef

```python
# DeleteDevEndpointRequestRequestTypeDef definition

class DeleteDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
```

## DeleteIntegrationRequestRequestTypeDef

```python
# DeleteIntegrationRequestRequestTypeDef definition

class DeleteIntegrationRequestRequestTypeDef(TypedDict):
    IntegrationIdentifier: str,
```

## DeleteIntegrationTablePropertiesRequestRequestTypeDef

```python
# DeleteIntegrationTablePropertiesRequestRequestTypeDef definition

class DeleteIntegrationTablePropertiesRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TableName: str,
```

## DeleteJobRequestRequestTypeDef

```python
# DeleteJobRequestRequestTypeDef definition

class DeleteJobRequestRequestTypeDef(TypedDict):
    JobName: str,
```

## DeleteMLTransformRequestRequestTypeDef

```python
# DeleteMLTransformRequestRequestTypeDef definition

class DeleteMLTransformRequestRequestTypeDef(TypedDict):
    TransformId: str,
```

## DeletePartitionIndexRequestRequestTypeDef

```python
# DeletePartitionIndexRequestRequestTypeDef definition

class DeletePartitionIndexRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    IndexName: str,
    CatalogId: NotRequired[str],
```

## DeletePartitionRequestRequestTypeDef

```python
# DeletePartitionRequestRequestTypeDef definition

class DeletePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    CatalogId: NotRequired[str],
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    PolicyHashCondition: NotRequired[str],
    ResourceArn: NotRequired[str],
```

## SchemaIdTypeDef

```python
# SchemaIdTypeDef definition

class SchemaIdTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    SchemaName: NotRequired[str],
    RegistryName: NotRequired[str],
```

## DeleteSecurityConfigurationRequestRequestTypeDef

```python
# DeleteSecurityConfigurationRequestRequestTypeDef definition

class DeleteSecurityConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteSessionRequestRequestTypeDef

```python
# DeleteSessionRequestRequestTypeDef definition

class DeleteSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    RequestOrigin: NotRequired[str],
```

## DeleteTableOptimizerRequestRequestTypeDef

```python
# DeleteTableOptimizerRequestRequestTypeDef definition

class DeleteTableOptimizerRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
## DeleteTableRequestRequestTypeDef

```python
# DeleteTableRequestRequestTypeDef definition

class DeleteTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    Name: str,
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
```

## DeleteTableVersionRequestRequestTypeDef

```python
# DeleteTableVersionRequestRequestTypeDef definition

class DeleteTableVersionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    VersionId: str,
    CatalogId: NotRequired[str],
```

## DeleteTriggerRequestRequestTypeDef

```python
# DeleteTriggerRequestRequestTypeDef definition

class DeleteTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteUsageProfileRequestRequestTypeDef

```python
# DeleteUsageProfileRequestRequestTypeDef definition

class DeleteUsageProfileRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteUserDefinedFunctionRequestRequestTypeDef

```python
# DeleteUserDefinedFunctionRequestRequestTypeDef definition

class DeleteUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionName: str,
    CatalogId: NotRequired[str],
```

## DeleteWorkflowRequestRequestTypeDef

```python
# DeleteWorkflowRequestRequestTypeDef definition

class DeleteWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
```

## DeltaTargetTypeDef

```python
# DeltaTargetTypeDef definition

class DeltaTargetTypeDef(TypedDict):
    DeltaTables: NotRequired[Sequence[str]],
    ConnectionName: NotRequired[str],
    WriteManifest: NotRequired[bool],
    CreateNativeDeltaTable: NotRequired[bool],
```

## DescribeConnectionTypeRequestRequestTypeDef

```python
# DescribeConnectionTypeRequestRequestTypeDef definition

class DescribeConnectionTypeRequestRequestTypeDef(TypedDict):
    ConnectionType: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeEntityRequestRequestTypeDef

```python
# DescribeEntityRequestRequestTypeDef definition

class DescribeEntityRequestRequestTypeDef(TypedDict):
    ConnectionName: str,
    EntityName: str,
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    DataStoreApiVersion: NotRequired[str],
```

## FieldTypeDef

```python
# FieldTypeDef definition

class FieldTypeDef(TypedDict):
    FieldName: NotRequired[str],
    Label: NotRequired[str],
    Description: NotRequired[str],
    FieldType: NotRequired[FieldDataTypeType],  # (1)
    IsPrimaryKey: NotRequired[bool],
    IsNullable: NotRequired[bool],
    IsRetrievable: NotRequired[bool],
    IsFilterable: NotRequired[bool],
    IsPartitionable: NotRequired[bool],
    IsCreateable: NotRequired[bool],
    IsUpdateable: NotRequired[bool],
    IsUpsertable: NotRequired[bool],
    IsDefaultOnCreate: NotRequired[bool],
    SupportedValues: NotRequired[List[str]],
    SupportedFilterOperators: NotRequired[List[FieldFilterOperatorType]],  # (2)
    ParentField: NotRequired[str],
    NativeDataType: NotRequired[str],
    CustomProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FieldDataTypeType](./literals.md#fielddatatypetype) 
2. See [:material-code-brackets: FieldFilterOperatorType](./literals.md#fieldfilteroperatortype) 
## DescribeInboundIntegrationsRequestRequestTypeDef

```python
# DescribeInboundIntegrationsRequestRequestTypeDef definition

class DescribeInboundIntegrationsRequestRequestTypeDef(TypedDict):
    IntegrationArn: NotRequired[str],
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
    TargetArn: NotRequired[str],
```

## IntegrationFilterTypeDef

```python
# IntegrationFilterTypeDef definition

class IntegrationFilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## DevEndpointCustomLibrariesTypeDef

```python
# DevEndpointCustomLibrariesTypeDef definition

class DevEndpointCustomLibrariesTypeDef(TypedDict):
    ExtraPythonLibsS3Path: NotRequired[str],
    ExtraJarsS3Path: NotRequired[str],
```

## DirectSchemaChangePolicyTypeDef

```python
# DirectSchemaChangePolicyTypeDef definition

class DirectSchemaChangePolicyTypeDef(TypedDict):
    EnableUpdateCatalog: NotRequired[bool],
    UpdateBehavior: NotRequired[UpdateCatalogBehaviorType],  # (1)
    Table: NotRequired[str],
    Database: NotRequired[str],
```

1. See [:material-code-brackets: UpdateCatalogBehaviorType](./literals.md#updatecatalogbehaviortype) 
## DropDuplicatesTypeDef

```python
# DropDuplicatesTypeDef definition

class DropDuplicatesTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Columns: NotRequired[Sequence[Sequence[str]]],
```

## DropFieldsTypeDef

```python
# DropFieldsTypeDef definition

class DropFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Paths: Sequence[Sequence[str]],
```

## NullCheckBoxListTypeDef

```python
# NullCheckBoxListTypeDef definition

class NullCheckBoxListTypeDef(TypedDict):
    IsEmpty: NotRequired[bool],
    IsNullString: NotRequired[bool],
    IsNegOne: NotRequired[bool],
```

## TransformConfigParameterOutputTypeDef

```python
# TransformConfigParameterOutputTypeDef definition

class TransformConfigParameterOutputTypeDef(TypedDict):
    Name: str,
    Type: ParamTypeType,  # (1)
    ValidationRule: NotRequired[str],
    ValidationMessage: NotRequired[str],
    Value: NotRequired[List[str]],
    ListType: NotRequired[ParamTypeType],  # (1)
    IsOptional: NotRequired[bool],
```

1. See [:material-code-brackets: ParamTypeType](./literals.md#paramtypetype) 
2. See [:material-code-brackets: ParamTypeType](./literals.md#paramtypetype) 
## EdgeTypeDef

```python
# EdgeTypeDef definition

class EdgeTypeDef(TypedDict):
    SourceId: NotRequired[str],
    DestinationId: NotRequired[str],
```

## JobBookmarksEncryptionTypeDef

```python
# JobBookmarksEncryptionTypeDef definition

class JobBookmarksEncryptionTypeDef(TypedDict):
    JobBookmarksEncryptionMode: NotRequired[JobBookmarksEncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: JobBookmarksEncryptionModeType](./literals.md#jobbookmarksencryptionmodetype) 
## S3EncryptionTypeDef

```python
# S3EncryptionTypeDef definition

class S3EncryptionTypeDef(TypedDict):
    S3EncryptionMode: NotRequired[S3EncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: S3EncryptionModeType](./literals.md#s3encryptionmodetype) 
## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    EntityName: NotRequired[str],
    Label: NotRequired[str],
    IsParentEntity: NotRequired[bool],
    Description: NotRequired[str],
    Category: NotRequired[str],
    CustomProperties: NotRequired[Dict[str, str]],
```

## ErrorDetailsTypeDef

```python
# ErrorDetailsTypeDef definition

class ErrorDetailsTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## ExportLabelsTaskRunPropertiesTypeDef

```python
# ExportLabelsTaskRunPropertiesTypeDef definition

class ExportLabelsTaskRunPropertiesTypeDef(TypedDict):
    OutputS3Path: NotRequired[str],
```

## FederatedTableTypeDef

```python
# FederatedTableTypeDef definition

class FederatedTableTypeDef(TypedDict):
    Identifier: NotRequired[str],
    DatabaseIdentifier: NotRequired[str],
    ConnectionName: NotRequired[str],
```

## FillMissingValuesTypeDef

```python
# FillMissingValuesTypeDef definition

class FillMissingValuesTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    ImputedPath: str,
    FilledPath: NotRequired[str],
```

## FilterValueOutputTypeDef

```python
# FilterValueOutputTypeDef definition

class FilterValueOutputTypeDef(TypedDict):
    Type: FilterValueTypeType,  # (1)
    Value: List[str],
```

1. See [:material-code-brackets: FilterValueTypeType](./literals.md#filtervaluetypetype) 
## FilterValueTypeDef

```python
# FilterValueTypeDef definition

class FilterValueTypeDef(TypedDict):
    Type: FilterValueTypeType,  # (1)
    Value: Sequence[str],
```

1. See [:material-code-brackets: FilterValueTypeType](./literals.md#filtervaluetypetype) 
## FindMatchesParametersTypeDef

```python
# FindMatchesParametersTypeDef definition

class FindMatchesParametersTypeDef(TypedDict):
    PrimaryKeyColumnName: NotRequired[str],
    PrecisionRecallTradeoff: NotRequired[float],
    AccuracyCostTradeoff: NotRequired[float],
    EnforceProvidedLabels: NotRequired[bool],
```

## FindMatchesTaskRunPropertiesTypeDef

```python
# FindMatchesTaskRunPropertiesTypeDef definition

class FindMatchesTaskRunPropertiesTypeDef(TypedDict):
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
```

## GetBlueprintRequestRequestTypeDef

```python
# GetBlueprintRequestRequestTypeDef definition

class GetBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
    IncludeBlueprint: NotRequired[bool],
    IncludeParameterSpec: NotRequired[bool],
```

## GetBlueprintRunRequestRequestTypeDef

```python
# GetBlueprintRunRequestRequestTypeDef definition

class GetBlueprintRunRequestRequestTypeDef(TypedDict):
    BlueprintName: str,
    RunId: str,
```

## GetBlueprintRunsRequestRequestTypeDef

```python
# GetBlueprintRunsRequestRequestTypeDef definition

class GetBlueprintRunsRequestRequestTypeDef(TypedDict):
    BlueprintName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetCatalogImportStatusRequestRequestTypeDef

```python
# GetCatalogImportStatusRequestRequestTypeDef definition

class GetCatalogImportStatusRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## GetCatalogRequestRequestTypeDef

```python
# GetCatalogRequestRequestTypeDef definition

class GetCatalogRequestRequestTypeDef(TypedDict):
    CatalogId: str,
```

## GetCatalogsRequestRequestTypeDef

```python
# GetCatalogsRequestRequestTypeDef definition

class GetCatalogsRequestRequestTypeDef(TypedDict):
    ParentCatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Recursive: NotRequired[bool],
    IncludeRoot: NotRequired[bool],
```

## GetClassifierRequestRequestTypeDef

```python
# GetClassifierRequestRequestTypeDef definition

class GetClassifierRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetClassifiersRequestRequestTypeDef

```python
# GetClassifiersRequestRequestTypeDef definition

class GetClassifiersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetColumnStatisticsForPartitionRequestRequestTypeDef

```python
# GetColumnStatisticsForPartitionRequestRequestTypeDef definition

class GetColumnStatisticsForPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnNames: Sequence[str],
    CatalogId: NotRequired[str],
```

## GetColumnStatisticsForTableRequestRequestTypeDef

```python
# GetColumnStatisticsForTableRequestRequestTypeDef definition

class GetColumnStatisticsForTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    ColumnNames: Sequence[str],
    CatalogId: NotRequired[str],
```

## GetColumnStatisticsTaskRunRequestRequestTypeDef

```python
# GetColumnStatisticsTaskRunRequestRequestTypeDef definition

class GetColumnStatisticsTaskRunRequestRequestTypeDef(TypedDict):
    ColumnStatisticsTaskRunId: str,
```

## GetColumnStatisticsTaskRunsRequestRequestTypeDef

```python
# GetColumnStatisticsTaskRunsRequestRequestTypeDef definition

class GetColumnStatisticsTaskRunsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetColumnStatisticsTaskSettingsRequestRequestTypeDef

```python
# GetColumnStatisticsTaskSettingsRequestRequestTypeDef definition

class GetColumnStatisticsTaskSettingsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## GetConnectionRequestRequestTypeDef

```python
# GetConnectionRequestRequestTypeDef definition

class GetConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
    HidePassword: NotRequired[bool],
    ApplyOverrideForComputeEnvironment: NotRequired[ComputeEnvironmentType],  # (1)
```

1. See [:material-code-brackets: ComputeEnvironmentType](./literals.md#computeenvironmenttype) 
## GetConnectionsFilterTypeDef

```python
# GetConnectionsFilterTypeDef definition

class GetConnectionsFilterTypeDef(TypedDict):
    MatchCriteria: NotRequired[Sequence[str]],
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
    ConnectionSchemaVersion: NotRequired[int],
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
## GetCrawlerMetricsRequestRequestTypeDef

```python
# GetCrawlerMetricsRequestRequestTypeDef definition

class GetCrawlerMetricsRequestRequestTypeDef(TypedDict):
    CrawlerNameList: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetCrawlerRequestRequestTypeDef

```python
# GetCrawlerRequestRequestTypeDef definition

class GetCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetCrawlersRequestRequestTypeDef

```python
# GetCrawlersRequestRequestTypeDef definition

class GetCrawlersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetCustomEntityTypeRequestRequestTypeDef

```python
# GetCustomEntityTypeRequestRequestTypeDef definition

class GetCustomEntityTypeRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetDataCatalogEncryptionSettingsRequestRequestTypeDef

```python
# GetDataCatalogEncryptionSettingsRequestRequestTypeDef definition

class GetDataCatalogEncryptionSettingsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## GetDataQualityModelRequestRequestTypeDef

```python
# GetDataQualityModelRequestRequestTypeDef definition

class GetDataQualityModelRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    StatisticId: NotRequired[str],
```

## GetDataQualityModelResultRequestRequestTypeDef

```python
# GetDataQualityModelResultRequestRequestTypeDef definition

class GetDataQualityModelResultRequestRequestTypeDef(TypedDict):
    StatisticId: str,
    ProfileId: str,
```

## StatisticModelResultTypeDef

```python
# StatisticModelResultTypeDef definition

class StatisticModelResultTypeDef(TypedDict):
    LowerBound: NotRequired[float],
    UpperBound: NotRequired[float],
    PredictedValue: NotRequired[float],
    ActualValue: NotRequired[float],
    Date: NotRequired[datetime],
    InclusionAnnotation: NotRequired[InclusionAnnotationValueType],  # (1)
```

1. See [:material-code-brackets: InclusionAnnotationValueType](./literals.md#inclusionannotationvaluetype) 
## GetDataQualityResultRequestRequestTypeDef

```python
# GetDataQualityResultRequestRequestTypeDef definition

class GetDataQualityResultRequestRequestTypeDef(TypedDict):
    ResultId: str,
```

## GetDataQualityRuleRecommendationRunRequestRequestTypeDef

```python
# GetDataQualityRuleRecommendationRunRequestRequestTypeDef definition

class GetDataQualityRuleRecommendationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## GetDataQualityRulesetEvaluationRunRequestRequestTypeDef

```python
# GetDataQualityRulesetEvaluationRunRequestRequestTypeDef definition

class GetDataQualityRulesetEvaluationRunRequestRequestTypeDef(TypedDict):
    RunId: str,
```

## GetDataQualityRulesetRequestRequestTypeDef

```python
# GetDataQualityRulesetRequestRequestTypeDef definition

class GetDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetDatabaseRequestRequestTypeDef

```python
# GetDatabaseRequestRequestTypeDef definition

class GetDatabaseRequestRequestTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
```

## GetDatabasesRequestRequestTypeDef

```python
# GetDatabasesRequestRequestTypeDef definition

class GetDatabasesRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (1)
    AttributesToGet: NotRequired[Sequence[DatabaseAttributesType]],  # (2)
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-brackets: DatabaseAttributesType](./literals.md#databaseattributestype) 
## GetDataflowGraphRequestRequestTypeDef

```python
# GetDataflowGraphRequestRequestTypeDef definition

class GetDataflowGraphRequestRequestTypeDef(TypedDict):
    PythonScript: NotRequired[str],
```

## GetDevEndpointRequestRequestTypeDef

```python
# GetDevEndpointRequestRequestTypeDef definition

class GetDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
```

## GetDevEndpointsRequestRequestTypeDef

```python
# GetDevEndpointsRequestRequestTypeDef definition

class GetDevEndpointsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetEntityRecordsRequestRequestTypeDef

```python
# GetEntityRecordsRequestRequestTypeDef definition

class GetEntityRecordsRequestRequestTypeDef(TypedDict):
    EntityName: str,
    Limit: int,
    ConnectionName: NotRequired[str],
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    DataStoreApiVersion: NotRequired[str],
    ConnectionOptions: NotRequired[Mapping[str, str]],
    FilterPredicate: NotRequired[str],
    OrderBy: NotRequired[str],
    SelectedFields: NotRequired[Sequence[str]],
```

## GetIntegrationResourcePropertyRequestRequestTypeDef

```python
# GetIntegrationResourcePropertyRequestRequestTypeDef definition

class GetIntegrationResourcePropertyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetIntegrationTablePropertiesRequestRequestTypeDef

```python
# GetIntegrationTablePropertiesRequestRequestTypeDef definition

class GetIntegrationTablePropertiesRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TableName: str,
```

## SourceTableConfigOutputTypeDef

```python
# SourceTableConfigOutputTypeDef definition

class SourceTableConfigOutputTypeDef(TypedDict):
    Fields: NotRequired[List[str]],
    FilterPredicate: NotRequired[str],
    PrimaryKey: NotRequired[List[str]],
    RecordUpdateField: NotRequired[str],
```

## GetJobBookmarkRequestRequestTypeDef

```python
# GetJobBookmarkRequestRequestTypeDef definition

class GetJobBookmarkRequestRequestTypeDef(TypedDict):
    JobName: str,
    RunId: NotRequired[str],
```

## JobBookmarkEntryTypeDef

```python
# JobBookmarkEntryTypeDef definition

class JobBookmarkEntryTypeDef(TypedDict):
    JobName: NotRequired[str],
    Version: NotRequired[int],
    Run: NotRequired[int],
    Attempt: NotRequired[int],
    PreviousRunId: NotRequired[str],
    RunId: NotRequired[str],
    JobBookmark: NotRequired[str],
```

## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    JobName: str,
```

## GetJobRunRequestRequestTypeDef

```python
# GetJobRunRequestRequestTypeDef definition

class GetJobRunRequestRequestTypeDef(TypedDict):
    JobName: str,
    RunId: str,
    PredecessorsIncluded: NotRequired[bool],
```

## GetJobRunsRequestRequestTypeDef

```python
# GetJobRunsRequestRequestTypeDef definition

class GetJobRunsRequestRequestTypeDef(TypedDict):
    JobName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetJobsRequestRequestTypeDef

```python
# GetJobsRequestRequestTypeDef definition

class GetJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetMLTaskRunRequestRequestTypeDef

```python
# GetMLTaskRunRequestRequestTypeDef definition

class GetMLTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
```

## TaskRunSortCriteriaTypeDef

```python
# TaskRunSortCriteriaTypeDef definition

class TaskRunSortCriteriaTypeDef(TypedDict):
    Column: TaskRunSortColumnTypeType,  # (1)
    SortDirection: SortDirectionTypeType,  # (2)
```

1. See [:material-code-brackets: TaskRunSortColumnTypeType](./literals.md#taskrunsortcolumntypetype) 
2. See [:material-code-brackets: SortDirectionTypeType](./literals.md#sortdirectiontypetype) 
## GetMLTransformRequestRequestTypeDef

```python
# GetMLTransformRequestRequestTypeDef definition

class GetMLTransformRequestRequestTypeDef(TypedDict):
    TransformId: str,
```

## SchemaColumnTypeDef

```python
# SchemaColumnTypeDef definition

class SchemaColumnTypeDef(TypedDict):
    Name: NotRequired[str],
    DataType: NotRequired[str],
```

## TransformSortCriteriaTypeDef

```python
# TransformSortCriteriaTypeDef definition

class TransformSortCriteriaTypeDef(TypedDict):
    Column: TransformSortColumnTypeType,  # (1)
    SortDirection: SortDirectionTypeType,  # (2)
```

1. See [:material-code-brackets: TransformSortColumnTypeType](./literals.md#transformsortcolumntypetype) 
2. See [:material-code-brackets: SortDirectionTypeType](./literals.md#sortdirectiontypetype) 
## MappingEntryTypeDef

```python
# MappingEntryTypeDef definition

class MappingEntryTypeDef(TypedDict):
    SourceTable: NotRequired[str],
    SourcePath: NotRequired[str],
    SourceType: NotRequired[str],
    TargetTable: NotRequired[str],
    TargetPath: NotRequired[str],
    TargetType: NotRequired[str],
```

## GetPartitionIndexesRequestRequestTypeDef

```python
# GetPartitionIndexesRequestRequestTypeDef definition

class GetPartitionIndexesRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
```

## GetPartitionRequestRequestTypeDef

```python
# GetPartitionRequestRequestTypeDef definition

class GetPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    CatalogId: NotRequired[str],
```

## SegmentTypeDef

```python
# SegmentTypeDef definition

class SegmentTypeDef(TypedDict):
    SegmentNumber: int,
    TotalSegments: int,
```

## GetResourcePoliciesRequestRequestTypeDef

```python
# GetResourcePoliciesRequestRequestTypeDef definition

class GetResourcePoliciesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GluePolicyTypeDef

```python
# GluePolicyTypeDef definition

class GluePolicyTypeDef(TypedDict):
    PolicyInJson: NotRequired[str],
    PolicyHash: NotRequired[str],
    CreateTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
```

## SchemaVersionNumberTypeDef

```python
# SchemaVersionNumberTypeDef definition

class SchemaVersionNumberTypeDef(TypedDict):
    LatestVersion: NotRequired[bool],
    VersionNumber: NotRequired[int],
```

## GetSecurityConfigurationRequestRequestTypeDef

```python
# GetSecurityConfigurationRequestRequestTypeDef definition

class GetSecurityConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetSecurityConfigurationsRequestRequestTypeDef

```python
# GetSecurityConfigurationsRequestRequestTypeDef definition

class GetSecurityConfigurationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetSessionRequestRequestTypeDef

```python
# GetSessionRequestRequestTypeDef definition

class GetSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    RequestOrigin: NotRequired[str],
```

## GetStatementRequestRequestTypeDef

```python
# GetStatementRequestRequestTypeDef definition

class GetStatementRequestRequestTypeDef(TypedDict):
    SessionId: str,
    Id: int,
    RequestOrigin: NotRequired[str],
```

## GetTableOptimizerRequestRequestTypeDef

```python
# GetTableOptimizerRequestRequestTypeDef definition

class GetTableOptimizerRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
## GetTableVersionRequestRequestTypeDef

```python
# GetTableVersionRequestRequestTypeDef definition

class GetTableVersionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    VersionId: NotRequired[str],
```

## GetTableVersionsRequestRequestTypeDef

```python
# GetTableVersionsRequestRequestTypeDef definition

class GetTableVersionsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetTagsRequestRequestTypeDef

```python
# GetTagsRequestRequestTypeDef definition

class GetTagsRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetTriggerRequestRequestTypeDef

```python
# GetTriggerRequestRequestTypeDef definition

class GetTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetTriggersRequestRequestTypeDef

```python
# GetTriggersRequestRequestTypeDef definition

class GetTriggersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    DependentJobName: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SupportedDialectTypeDef

```python
# SupportedDialectTypeDef definition

class SupportedDialectTypeDef(TypedDict):
    Dialect: NotRequired[ViewDialectType],  # (1)
    DialectVersion: NotRequired[str],
```

1. See [:material-code-brackets: ViewDialectType](./literals.md#viewdialecttype) 
## GetUsageProfileRequestRequestTypeDef

```python
# GetUsageProfileRequestRequestTypeDef definition

class GetUsageProfileRequestRequestTypeDef(TypedDict):
    Name: str,
```

## GetUserDefinedFunctionRequestRequestTypeDef

```python
# GetUserDefinedFunctionRequestRequestTypeDef definition

class GetUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionName: str,
    CatalogId: NotRequired[str],
```

## GetUserDefinedFunctionsRequestRequestTypeDef

```python
# GetUserDefinedFunctionsRequestRequestTypeDef definition

class GetUserDefinedFunctionsRequestRequestTypeDef(TypedDict):
    Pattern: str,
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetWorkflowRequestRequestTypeDef

```python
# GetWorkflowRequestRequestTypeDef definition

class GetWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
    IncludeGraph: NotRequired[bool],
```

## GetWorkflowRunPropertiesRequestRequestTypeDef

```python
# GetWorkflowRunPropertiesRequestRequestTypeDef definition

class GetWorkflowRunPropertiesRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
```

## GetWorkflowRunRequestRequestTypeDef

```python
# GetWorkflowRunRequestRequestTypeDef definition

class GetWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
    IncludeGraph: NotRequired[bool],
```

## GetWorkflowRunsRequestRequestTypeDef

```python
# GetWorkflowRunsRequestRequestTypeDef definition

class GetWorkflowRunsRequestRequestTypeDef(TypedDict):
    Name: str,
    IncludeGraph: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GlueStudioSchemaColumnTypeDef

```python
# GlueStudioSchemaColumnTypeDef definition

class GlueStudioSchemaColumnTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[str],
```

## GlueTableTypeDef

```python
# GlueTableTypeDef definition

class GlueTableTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    ConnectionName: NotRequired[str],
    AdditionalOptions: NotRequired[Mapping[str, str]],
```

## S3SourceAdditionalOptionsTypeDef

```python
# S3SourceAdditionalOptionsTypeDef definition

class S3SourceAdditionalOptionsTypeDef(TypedDict):
    BoundedSize: NotRequired[int],
    BoundedFiles: NotRequired[int],
```

## HudiTargetTypeDef

```python
# HudiTargetTypeDef definition

class HudiTargetTypeDef(TypedDict):
    Paths: NotRequired[Sequence[str]],
    ConnectionName: NotRequired[str],
    Exclusions: NotRequired[Sequence[str]],
    MaximumTraversalDepth: NotRequired[int],
```

## IcebergInputTypeDef

```python
# IcebergInputTypeDef definition

class IcebergInputTypeDef(TypedDict):
    MetadataOperation: MetadataOperationType,  # (1)
    Version: NotRequired[str],
```

1. See [:material-code-brackets: MetadataOperationType](./literals.md#metadataoperationtype) 
## IcebergOrphanFileDeletionConfigurationTypeDef

```python
# IcebergOrphanFileDeletionConfigurationTypeDef definition

class IcebergOrphanFileDeletionConfigurationTypeDef(TypedDict):
    orphanFileRetentionPeriodInDays: NotRequired[int],
    location: NotRequired[str],
```

## IcebergOrphanFileDeletionMetricsTypeDef

```python
# IcebergOrphanFileDeletionMetricsTypeDef definition

class IcebergOrphanFileDeletionMetricsTypeDef(TypedDict):
    NumberOfOrphanFilesDeleted: NotRequired[int],
    NumberOfDpus: NotRequired[int],
    JobDurationInHour: NotRequired[float],
```

## IcebergRetentionConfigurationTypeDef

```python
# IcebergRetentionConfigurationTypeDef definition

class IcebergRetentionConfigurationTypeDef(TypedDict):
    snapshotRetentionPeriodInDays: NotRequired[int],
    numberOfSnapshotsToRetain: NotRequired[int],
    cleanExpiredFiles: NotRequired[bool],
```

## IcebergRetentionMetricsTypeDef

```python
# IcebergRetentionMetricsTypeDef definition

class IcebergRetentionMetricsTypeDef(TypedDict):
    NumberOfDataFilesDeleted: NotRequired[int],
    NumberOfManifestFilesDeleted: NotRequired[int],
    NumberOfManifestListsDeleted: NotRequired[int],
    NumberOfDpus: NotRequired[int],
    JobDurationInHour: NotRequired[float],
```

## IcebergTargetTypeDef

```python
# IcebergTargetTypeDef definition

class IcebergTargetTypeDef(TypedDict):
    Paths: NotRequired[Sequence[str]],
    ConnectionName: NotRequired[str],
    Exclusions: NotRequired[Sequence[str]],
    MaximumTraversalDepth: NotRequired[int],
```

## ImportCatalogToGlueRequestRequestTypeDef

```python
# ImportCatalogToGlueRequestRequestTypeDef definition

class ImportCatalogToGlueRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
```

## ImportLabelsTaskRunPropertiesTypeDef

```python
# ImportLabelsTaskRunPropertiesTypeDef definition

class ImportLabelsTaskRunPropertiesTypeDef(TypedDict):
    InputS3Path: NotRequired[str],
    Replace: NotRequired[bool],
```

## IntegrationPartitionTypeDef

```python
# IntegrationPartitionTypeDef definition

class IntegrationPartitionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    FunctionSpec: NotRequired[str],
```

## JDBCConnectorOptionsOutputTypeDef

```python
# JDBCConnectorOptionsOutputTypeDef definition

class JDBCConnectorOptionsOutputTypeDef(TypedDict):
    FilterPredicate: NotRequired[str],
    PartitionColumn: NotRequired[str],
    LowerBound: NotRequired[int],
    UpperBound: NotRequired[int],
    NumPartitions: NotRequired[int],
    JobBookmarkKeys: NotRequired[List[str]],
    JobBookmarkKeysSortOrder: NotRequired[str],
    DataTypeMapping: NotRequired[Dict[JDBCDataTypeType, GlueRecordTypeType]],  # (1)
```

1. See [:material-code-brackets: JDBCDataTypeType](./literals.md#jdbcdatatypetype) [:material-code-brackets: GlueRecordTypeType](./literals.md#gluerecordtypetype) 
## JDBCConnectorOptionsTypeDef

```python
# JDBCConnectorOptionsTypeDef definition

class JDBCConnectorOptionsTypeDef(TypedDict):
    FilterPredicate: NotRequired[str],
    PartitionColumn: NotRequired[str],
    LowerBound: NotRequired[int],
    UpperBound: NotRequired[int],
    NumPartitions: NotRequired[int],
    JobBookmarkKeys: NotRequired[Sequence[str]],
    JobBookmarkKeysSortOrder: NotRequired[str],
    DataTypeMapping: NotRequired[Mapping[JDBCDataTypeType, GlueRecordTypeType]],  # (1)
```

1. See [:material-code-brackets: JDBCDataTypeType](./literals.md#jdbcdatatypetype) [:material-code-brackets: GlueRecordTypeType](./literals.md#gluerecordtypetype) 
## JdbcTargetTypeDef

```python
# JdbcTargetTypeDef definition

class JdbcTargetTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    Path: NotRequired[str],
    Exclusions: NotRequired[Sequence[str]],
    EnableAdditionalMetadata: NotRequired[Sequence[JdbcMetadataEntryType]],  # (1)
```

1. See [:material-code-brackets: JdbcMetadataEntryType](./literals.md#jdbcmetadataentrytype) 
## PredecessorTypeDef

```python
# PredecessorTypeDef definition

class PredecessorTypeDef(TypedDict):
    JobName: NotRequired[str],
    RunId: NotRequired[str],
```

## JoinColumnOutputTypeDef

```python
# JoinColumnOutputTypeDef definition

class JoinColumnOutputTypeDef(TypedDict):
    From: str,
    Keys: List[List[str]],
```

## JoinColumnTypeDef

```python
# JoinColumnTypeDef definition

class JoinColumnTypeDef(TypedDict):
    From: str,
    Keys: Sequence[Sequence[str]],
```

## KeySchemaElementTypeDef

```python
# KeySchemaElementTypeDef definition

class KeySchemaElementTypeDef(TypedDict):
    Name: str,
    Type: str,
```

## LabelingSetGenerationTaskRunPropertiesTypeDef

```python
# LabelingSetGenerationTaskRunPropertiesTypeDef definition

class LabelingSetGenerationTaskRunPropertiesTypeDef(TypedDict):
    OutputS3Path: NotRequired[str],
```

## ListBlueprintsRequestRequestTypeDef

```python
# ListBlueprintsRequestRequestTypeDef definition

class ListBlueprintsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListColumnStatisticsTaskRunsRequestRequestTypeDef

```python
# ListColumnStatisticsTaskRunsRequestRequestTypeDef definition

class ListColumnStatisticsTaskRunsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListConnectionTypesRequestRequestTypeDef

```python
# ListConnectionTypesRequestRequestTypeDef definition

class ListConnectionTypesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCrawlersRequestRequestTypeDef

```python
# ListCrawlersRequestRequestTypeDef definition

class ListCrawlersRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## ListCustomEntityTypesRequestRequestTypeDef

```python
# ListCustomEntityTypesRequestRequestTypeDef definition

class ListCustomEntityTypesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListDevEndpointsRequestRequestTypeDef

```python
# ListDevEndpointsRequestRequestTypeDef definition

class ListDevEndpointsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListEntitiesRequestRequestTypeDef

```python
# ListEntitiesRequestRequestTypeDef definition

class ListEntitiesRequestRequestTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    CatalogId: NotRequired[str],
    ParentEntityName: NotRequired[str],
    NextToken: NotRequired[str],
    DataStoreApiVersion: NotRequired[str],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListRegistriesInputRequestTypeDef

```python
# ListRegistriesInputRequestTypeDef definition

class ListRegistriesInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RegistryListItemTypeDef

```python
# RegistryListItemTypeDef definition

class RegistryListItemTypeDef(TypedDict):
    RegistryName: NotRequired[str],
    RegistryArn: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[RegistryStatusType],  # (1)
    CreatedTime: NotRequired[str],
    UpdatedTime: NotRequired[str],
```

1. See [:material-code-brackets: RegistryStatusType](./literals.md#registrystatustype) 
## SchemaVersionListItemTypeDef

```python
# SchemaVersionListItemTypeDef definition

class SchemaVersionListItemTypeDef(TypedDict):
    SchemaArn: NotRequired[str],
    SchemaVersionId: NotRequired[str],
    VersionNumber: NotRequired[int],
    Status: NotRequired[SchemaVersionStatusType],  # (1)
    CreatedTime: NotRequired[str],
```

1. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
## SchemaListItemTypeDef

```python
# SchemaListItemTypeDef definition

class SchemaListItemTypeDef(TypedDict):
    RegistryName: NotRequired[str],
    SchemaName: NotRequired[str],
    SchemaArn: NotRequired[str],
    Description: NotRequired[str],
    SchemaStatus: NotRequired[SchemaStatusType],  # (1)
    CreatedTime: NotRequired[str],
    UpdatedTime: NotRequired[str],
```

1. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
## ListSessionsRequestRequestTypeDef

```python
# ListSessionsRequestRequestTypeDef definition

class ListSessionsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
    RequestOrigin: NotRequired[str],
```

## ListStatementsRequestRequestTypeDef

```python
# ListStatementsRequestRequestTypeDef definition

class ListStatementsRequestRequestTypeDef(TypedDict):
    SessionId: str,
    RequestOrigin: NotRequired[str],
    NextToken: NotRequired[str],
```

## ListTableOptimizerRunsRequestRequestTypeDef

```python
# ListTableOptimizerRunsRequestRequestTypeDef definition

class ListTableOptimizerRunsRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
## ListTriggersRequestRequestTypeDef

```python
# ListTriggersRequestRequestTypeDef definition

class ListTriggersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    DependentJobName: NotRequired[str],
    MaxResults: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
```

## ListUsageProfilesRequestRequestTypeDef

```python
# ListUsageProfilesRequestRequestTypeDef definition

class ListUsageProfilesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## UsageProfileDefinitionTypeDef

```python
# UsageProfileDefinitionTypeDef definition

class UsageProfileDefinitionTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
```

## ListWorkflowsRequestRequestTypeDef

```python
# ListWorkflowsRequestRequestTypeDef definition

class ListWorkflowsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## MLUserDataEncryptionTypeDef

```python
# MLUserDataEncryptionTypeDef definition

class MLUserDataEncryptionTypeDef(TypedDict):
    MlUserDataEncryptionMode: MLUserDataEncryptionModeStringType,  # (1)
    KmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: MLUserDataEncryptionModeStringType](./literals.md#mluserdataencryptionmodestringtype) 
## MappingTypeDef

```python
# MappingTypeDef definition

class MappingTypeDef(TypedDict):
    ToKey: NotRequired[str],
    FromPath: NotRequired[Sequence[str]],
    FromType: NotRequired[str],
    ToType: NotRequired[str],
    Dropped: NotRequired[bool],
    Children: NotRequired[Sequence[Mapping[str, Any]]],
```

## MergeTypeDef

```python
# MergeTypeDef definition

class MergeTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Source: str,
    PrimaryKeys: Sequence[Sequence[str]],
```

## OtherMetadataValueListItemTypeDef

```python
# OtherMetadataValueListItemTypeDef definition

class OtherMetadataValueListItemTypeDef(TypedDict):
    MetadataValue: NotRequired[str],
    CreatedTime: NotRequired[str],
```

## MetadataKeyValuePairTypeDef

```python
# MetadataKeyValuePairTypeDef definition

class MetadataKeyValuePairTypeDef(TypedDict):
    MetadataKey: NotRequired[str],
    MetadataValue: NotRequired[str],
```

## MicrosoftSQLServerCatalogTargetTypeDef

```python
# MicrosoftSQLServerCatalogTargetTypeDef definition

class MicrosoftSQLServerCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Database: str,
    Table: str,
```

## ModifyIntegrationRequestRequestTypeDef

```python
# ModifyIntegrationRequestRequestTypeDef definition

class ModifyIntegrationRequestRequestTypeDef(TypedDict):
    IntegrationIdentifier: str,
    Description: NotRequired[str],
    DataFilter: NotRequired[str],
    IntegrationName: NotRequired[str],
```

## MySQLCatalogTargetTypeDef

```python
# MySQLCatalogTargetTypeDef definition

class MySQLCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Database: str,
    Table: str,
```

## OAuth2ClientApplicationTypeDef

```python
# OAuth2ClientApplicationTypeDef definition

class OAuth2ClientApplicationTypeDef(TypedDict):
    UserManagedClientApplicationClientId: NotRequired[str],
    AWSManagedClientApplicationReference: NotRequired[str],
```

## OAuth2CredentialsTypeDef

```python
# OAuth2CredentialsTypeDef definition

class OAuth2CredentialsTypeDef(TypedDict):
    UserManagedClientApplicationClientSecret: NotRequired[str],
    AccessToken: NotRequired[str],
    RefreshToken: NotRequired[str],
    JwtToken: NotRequired[str],
```

## OracleSQLCatalogTargetTypeDef

```python
# OracleSQLCatalogTargetTypeDef definition

class OracleSQLCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Database: str,
    Table: str,
```

## OrderTypeDef

```python
# OrderTypeDef definition

class OrderTypeDef(TypedDict):
    Column: str,
    SortOrder: int,
```

## PIIDetectionTypeDef

```python
# PIIDetectionTypeDef definition

class PIIDetectionTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    PiiType: PiiTypeType,  # (1)
    EntityTypesToDetect: Sequence[str],
    OutputColumnName: NotRequired[str],
    SampleFraction: NotRequired[float],
    ThresholdFraction: NotRequired[float],
    MaskValue: NotRequired[str],
```

1. See [:material-code-brackets: PiiTypeType](./literals.md#piitypetype) 
## PhysicalConnectionRequirementsTypeDef

```python
# PhysicalConnectionRequirementsTypeDef definition

class PhysicalConnectionRequirementsTypeDef(TypedDict):
    SubnetId: NotRequired[str],
    SecurityGroupIdList: NotRequired[Sequence[str]],
    AvailabilityZone: NotRequired[str],
```

## PostgreSQLCatalogTargetTypeDef

```python
# PostgreSQLCatalogTargetTypeDef definition

class PostgreSQLCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Database: str,
    Table: str,
```

## PropertyPredicateTypeDef

```python
# PropertyPredicateTypeDef definition

class PropertyPredicateTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Comparator: NotRequired[ComparatorType],  # (1)
```

1. See [:material-code-brackets: ComparatorType](./literals.md#comparatortype) 
## PutDataQualityProfileAnnotationRequestRequestTypeDef

```python
# PutDataQualityProfileAnnotationRequestRequestTypeDef definition

class PutDataQualityProfileAnnotationRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    InclusionAnnotation: InclusionAnnotationValueType,  # (1)
```

1. See [:material-code-brackets: InclusionAnnotationValueType](./literals.md#inclusionannotationvaluetype) 
## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    PolicyInJson: str,
    ResourceArn: NotRequired[str],
    PolicyHashCondition: NotRequired[str],
    PolicyExistsCondition: NotRequired[ExistConditionType],  # (1)
    EnableHybrid: NotRequired[EnableHybridValuesType],  # (2)
```

1. See [:material-code-brackets: ExistConditionType](./literals.md#existconditiontype) 
2. See [:material-code-brackets: EnableHybridValuesType](./literals.md#enablehybridvaluestype) 
## PutWorkflowRunPropertiesRequestRequestTypeDef

```python
# PutWorkflowRunPropertiesRequestRequestTypeDef definition

class PutWorkflowRunPropertiesRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
    RunProperties: Mapping[str, str],
```

## RecipeActionOutputTypeDef

```python
# RecipeActionOutputTypeDef definition

class RecipeActionOutputTypeDef(TypedDict):
    Operation: str,
    Parameters: NotRequired[Dict[str, str]],
```

## RecipeActionTypeDef

```python
# RecipeActionTypeDef definition

class RecipeActionTypeDef(TypedDict):
    Operation: str,
    Parameters: NotRequired[Mapping[str, str]],
```

## RecipeReferenceTypeDef

```python
# RecipeReferenceTypeDef definition

class RecipeReferenceTypeDef(TypedDict):
    RecipeArn: str,
    RecipeVersion: str,
```

## UpsertRedshiftTargetOptionsOutputTypeDef

```python
# UpsertRedshiftTargetOptionsOutputTypeDef definition

class UpsertRedshiftTargetOptionsOutputTypeDef(TypedDict):
    TableLocation: NotRequired[str],
    ConnectionName: NotRequired[str],
    UpsertKeys: NotRequired[List[str]],
```

## RenameFieldTypeDef

```python
# RenameFieldTypeDef definition

class RenameFieldTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    SourcePath: Sequence[str],
    TargetPath: Sequence[str],
```

## ResetJobBookmarkRequestRequestTypeDef

```python
# ResetJobBookmarkRequestRequestTypeDef definition

class ResetJobBookmarkRequestRequestTypeDef(TypedDict):
    JobName: str,
    RunId: NotRequired[str],
```

## ResourceUriTypeDef

```python
# ResourceUriTypeDef definition

class ResourceUriTypeDef(TypedDict):
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    Uri: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResumeWorkflowRunRequestRequestTypeDef

```python
# ResumeWorkflowRunRequestRequestTypeDef definition

class ResumeWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
    NodeIds: Sequence[str],
```

## RunIdentifierTypeDef

```python
# RunIdentifierTypeDef definition

class RunIdentifierTypeDef(TypedDict):
    RunId: NotRequired[str],
    JobRunId: NotRequired[str],
```

## RunMetricsTypeDef

```python
# RunMetricsTypeDef definition

class RunMetricsTypeDef(TypedDict):
    NumberOfBytesCompacted: NotRequired[str],
    NumberOfFilesCompacted: NotRequired[str],
    NumberOfDpus: NotRequired[str],
    JobDurationInHour: NotRequired[str],
```

## RunStatementRequestRequestTypeDef

```python
# RunStatementRequestRequestTypeDef definition

class RunStatementRequestRequestTypeDef(TypedDict):
    SessionId: str,
    Code: str,
    RequestOrigin: NotRequired[str],
```

## S3DirectSourceAdditionalOptionsTypeDef

```python
# S3DirectSourceAdditionalOptionsTypeDef definition

class S3DirectSourceAdditionalOptionsTypeDef(TypedDict):
    BoundedSize: NotRequired[int],
    BoundedFiles: NotRequired[int],
    EnableSamplePath: NotRequired[bool],
    SamplePath: NotRequired[str],
```

## S3TargetTypeDef

```python
# S3TargetTypeDef definition

class S3TargetTypeDef(TypedDict):
    Path: NotRequired[str],
    Exclusions: NotRequired[Sequence[str]],
    ConnectionName: NotRequired[str],
    SampleSize: NotRequired[int],
    EventQueueArn: NotRequired[str],
    DlqEventQueueArn: NotRequired[str],
```

## SortCriterionTypeDef

```python
# SortCriterionTypeDef definition

class SortCriterionTypeDef(TypedDict):
    FieldName: NotRequired[str],
    Sort: NotRequired[SortType],  # (1)
```

1. See [:material-code-brackets: SortType](./literals.md#sorttype) 
## SelectFieldsTypeDef

```python
# SelectFieldsTypeDef definition

class SelectFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Paths: Sequence[Sequence[str]],
```

## SelectFromCollectionTypeDef

```python
# SelectFromCollectionTypeDef definition

class SelectFromCollectionTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Index: int,
```

## SerDeInfoOutputTypeDef

```python
# SerDeInfoOutputTypeDef definition

class SerDeInfoOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    SerializationLibrary: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
```

## SerDeInfoTypeDef

```python
# SerDeInfoTypeDef definition

class SerDeInfoTypeDef(TypedDict):
    Name: NotRequired[str],
    SerializationLibrary: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
```

## SkewedInfoOutputTypeDef

```python
# SkewedInfoOutputTypeDef definition

class SkewedInfoOutputTypeDef(TypedDict):
    SkewedColumnNames: NotRequired[List[str]],
    SkewedColumnValues: NotRequired[List[str]],
    SkewedColumnValueLocationMaps: NotRequired[Dict[str, str]],
```

## SkewedInfoTypeDef

```python
# SkewedInfoTypeDef definition

class SkewedInfoTypeDef(TypedDict):
    SkewedColumnNames: NotRequired[Sequence[str]],
    SkewedColumnValues: NotRequired[Sequence[str]],
    SkewedColumnValueLocationMaps: NotRequired[Mapping[str, str]],
```

## SqlAliasTypeDef

```python
# SqlAliasTypeDef definition

class SqlAliasTypeDef(TypedDict):
    From: str,
    Alias: str,
```

## SpigotTypeDef

```python
# SpigotTypeDef definition

class SpigotTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Path: str,
    Topk: NotRequired[int],
    Prob: NotRequired[float],
```

## SplitFieldsTypeDef

```python
# SplitFieldsTypeDef definition

class SplitFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Paths: Sequence[Sequence[str]],
```

## StartBlueprintRunRequestRequestTypeDef

```python
# StartBlueprintRunRequestRequestTypeDef definition

class StartBlueprintRunRequestRequestTypeDef(TypedDict):
    BlueprintName: str,
    RoleArn: str,
    Parameters: NotRequired[str],
```

## StartColumnStatisticsTaskRunRequestRequestTypeDef

```python
# StartColumnStatisticsTaskRunRequestRequestTypeDef definition

class StartColumnStatisticsTaskRunRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    Role: str,
    ColumnNameList: NotRequired[Sequence[str]],
    SampleSize: NotRequired[float],
    CatalogID: NotRequired[str],
    SecurityConfiguration: NotRequired[str],
```

## StartColumnStatisticsTaskRunScheduleRequestRequestTypeDef

```python
# StartColumnStatisticsTaskRunScheduleRequestRequestTypeDef definition

class StartColumnStatisticsTaskRunScheduleRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## StartCrawlerRequestRequestTypeDef

```python
# StartCrawlerRequestRequestTypeDef definition

class StartCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartCrawlerScheduleRequestRequestTypeDef

```python
# StartCrawlerScheduleRequestRequestTypeDef definition

class StartCrawlerScheduleRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
```

## StartExportLabelsTaskRunRequestRequestTypeDef

```python
# StartExportLabelsTaskRunRequestRequestTypeDef definition

class StartExportLabelsTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    OutputS3Path: str,
```

## StartImportLabelsTaskRunRequestRequestTypeDef

```python
# StartImportLabelsTaskRunRequestRequestTypeDef definition

class StartImportLabelsTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    InputS3Path: str,
    ReplaceAllLabels: NotRequired[bool],
```

## StartMLEvaluationTaskRunRequestRequestTypeDef

```python
# StartMLEvaluationTaskRunRequestRequestTypeDef definition

class StartMLEvaluationTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
```

## StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef

```python
# StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef definition

class StartMLLabelingSetGenerationTaskRunRequestRequestTypeDef(TypedDict):
    TransformId: str,
    OutputS3Path: str,
```

## StartTriggerRequestRequestTypeDef

```python
# StartTriggerRequestRequestTypeDef definition

class StartTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StartWorkflowRunRequestRequestTypeDef

```python
# StartWorkflowRunRequestRequestTypeDef definition

class StartWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunProperties: NotRequired[Mapping[str, str]],
```

## StartingEventBatchConditionTypeDef

```python
# StartingEventBatchConditionTypeDef definition

class StartingEventBatchConditionTypeDef(TypedDict):
    BatchSize: NotRequired[int],
    BatchWindow: NotRequired[int],
```

## StatementOutputDataTypeDef

```python
# StatementOutputDataTypeDef definition

class StatementOutputDataTypeDef(TypedDict):
    TextPlain: NotRequired[str],
```

## TimestampedInclusionAnnotationTypeDef

```python
# TimestampedInclusionAnnotationTypeDef definition

class TimestampedInclusionAnnotationTypeDef(TypedDict):
    Value: NotRequired[InclusionAnnotationValueType],  # (1)
    LastModifiedOn: NotRequired[datetime],
```

1. See [:material-code-brackets: InclusionAnnotationValueType](./literals.md#inclusionannotationvaluetype) 
## StopColumnStatisticsTaskRunRequestRequestTypeDef

```python
# StopColumnStatisticsTaskRunRequestRequestTypeDef definition

class StopColumnStatisticsTaskRunRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## StopColumnStatisticsTaskRunScheduleRequestRequestTypeDef

```python
# StopColumnStatisticsTaskRunScheduleRequestRequestTypeDef definition

class StopColumnStatisticsTaskRunScheduleRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
```

## StopCrawlerRequestRequestTypeDef

```python
# StopCrawlerRequestRequestTypeDef definition

class StopCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StopCrawlerScheduleRequestRequestTypeDef

```python
# StopCrawlerScheduleRequestRequestTypeDef definition

class StopCrawlerScheduleRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
```

## StopSessionRequestRequestTypeDef

```python
# StopSessionRequestRequestTypeDef definition

class StopSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    RequestOrigin: NotRequired[str],
```

## StopTriggerRequestRequestTypeDef

```python
# StopTriggerRequestRequestTypeDef definition

class StopTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
```

## StopWorkflowRunRequestRequestTypeDef

```python
# StopWorkflowRunRequestRequestTypeDef definition

class StopWorkflowRunRequestRequestTypeDef(TypedDict):
    Name: str,
    RunId: str,
```

## TableIdentifierTypeDef

```python
# TableIdentifierTypeDef definition

class TableIdentifierTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    Name: NotRequired[str],
    Region: NotRequired[str],
```

## TableOptimizerVpcConfigurationTypeDef

```python
# TableOptimizerVpcConfigurationTypeDef definition

class TableOptimizerVpcConfigurationTypeDef(TypedDict):
    glueConnectionName: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagsToAdd: Mapping[str, str],
```

## TransformConfigParameterTypeDef

```python
# TransformConfigParameterTypeDef definition

class TransformConfigParameterTypeDef(TypedDict):
    Name: str,
    Type: ParamTypeType,  # (1)
    ValidationRule: NotRequired[str],
    ValidationMessage: NotRequired[str],
    Value: NotRequired[Sequence[str]],
    ListType: NotRequired[ParamTypeType],  # (1)
    IsOptional: NotRequired[bool],
```

1. See [:material-code-brackets: ParamTypeType](./literals.md#paramtypetype) 
2. See [:material-code-brackets: ParamTypeType](./literals.md#paramtypetype) 
## UnionTypeDef

```python
# UnionTypeDef definition

class UnionTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    UnionType: UnionTypeType,  # (1)
```

1. See [:material-code-brackets: UnionTypeType](./literals.md#uniontypetype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagsToRemove: Sequence[str],
```

## UpdateBlueprintRequestRequestTypeDef

```python
# UpdateBlueprintRequestRequestTypeDef definition

class UpdateBlueprintRequestRequestTypeDef(TypedDict):
    Name: str,
    BlueprintLocation: str,
    Description: NotRequired[str],
```

## UpdateCsvClassifierRequestTypeDef

```python
# UpdateCsvClassifierRequestTypeDef definition

class UpdateCsvClassifierRequestTypeDef(TypedDict):
    Name: str,
    Delimiter: NotRequired[str],
    QuoteSymbol: NotRequired[str],
    ContainsHeader: NotRequired[CsvHeaderOptionType],  # (1)
    Header: NotRequired[Sequence[str]],
    DisableValueTrimming: NotRequired[bool],
    AllowSingleColumn: NotRequired[bool],
    CustomDatatypeConfigured: NotRequired[bool],
    CustomDatatypes: NotRequired[Sequence[str]],
    Serde: NotRequired[CsvSerdeOptionType],  # (2)
```

1. See [:material-code-brackets: CsvHeaderOptionType](./literals.md#csvheaderoptiontype) 
2. See [:material-code-brackets: CsvSerdeOptionType](./literals.md#csvserdeoptiontype) 
## UpdateGrokClassifierRequestTypeDef

```python
# UpdateGrokClassifierRequestTypeDef definition

class UpdateGrokClassifierRequestTypeDef(TypedDict):
    Name: str,
    Classification: NotRequired[str],
    GrokPattern: NotRequired[str],
    CustomPatterns: NotRequired[str],
```

## UpdateJsonClassifierRequestTypeDef

```python
# UpdateJsonClassifierRequestTypeDef definition

class UpdateJsonClassifierRequestTypeDef(TypedDict):
    Name: str,
    JsonPath: NotRequired[str],
```

## UpdateXMLClassifierRequestTypeDef

```python
# UpdateXMLClassifierRequestTypeDef definition

class UpdateXMLClassifierRequestTypeDef(TypedDict):
    Name: str,
    Classification: NotRequired[str],
    RowTag: NotRequired[str],
```

## UpdateColumnStatisticsTaskSettingsRequestRequestTypeDef

```python
# UpdateColumnStatisticsTaskSettingsRequestRequestTypeDef definition

class UpdateColumnStatisticsTaskSettingsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    Role: NotRequired[str],
    Schedule: NotRequired[str],
    ColumnNameList: NotRequired[Sequence[str]],
    SampleSize: NotRequired[float],
    CatalogID: NotRequired[str],
    SecurityConfiguration: NotRequired[str],
```

## UpdateCrawlerScheduleRequestRequestTypeDef

```python
# UpdateCrawlerScheduleRequestRequestTypeDef definition

class UpdateCrawlerScheduleRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
    Schedule: NotRequired[str],
```

## UpdateDataQualityRulesetRequestRequestTypeDef

```python
# UpdateDataQualityRulesetRequestRequestTypeDef definition

class UpdateDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Ruleset: NotRequired[str],
```

## UpdateJobFromSourceControlRequestRequestTypeDef

```python
# UpdateJobFromSourceControlRequestRequestTypeDef definition

class UpdateJobFromSourceControlRequestRequestTypeDef(TypedDict):
    JobName: NotRequired[str],
    Provider: NotRequired[SourceControlProviderType],  # (1)
    RepositoryName: NotRequired[str],
    RepositoryOwner: NotRequired[str],
    BranchName: NotRequired[str],
    Folder: NotRequired[str],
    CommitId: NotRequired[str],
    AuthStrategy: NotRequired[SourceControlAuthStrategyType],  # (2)
    AuthToken: NotRequired[str],
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
## UpdateSourceControlFromJobRequestRequestTypeDef

```python
# UpdateSourceControlFromJobRequestRequestTypeDef definition

class UpdateSourceControlFromJobRequestRequestTypeDef(TypedDict):
    JobName: NotRequired[str],
    Provider: NotRequired[SourceControlProviderType],  # (1)
    RepositoryName: NotRequired[str],
    RepositoryOwner: NotRequired[str],
    BranchName: NotRequired[str],
    Folder: NotRequired[str],
    CommitId: NotRequired[str],
    AuthStrategy: NotRequired[SourceControlAuthStrategyType],  # (2)
    AuthToken: NotRequired[str],
```

1. See [:material-code-brackets: SourceControlProviderType](./literals.md#sourcecontrolprovidertype) 
2. See [:material-code-brackets: SourceControlAuthStrategyType](./literals.md#sourcecontrolauthstrategytype) 
## UpdateWorkflowRequestRequestTypeDef

```python
# UpdateWorkflowRequestRequestTypeDef definition

class UpdateWorkflowRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    DefaultRunProperties: NotRequired[Mapping[str, str]],
    MaxConcurrentRuns: NotRequired[int],
```

## UpsertRedshiftTargetOptionsTypeDef

```python
# UpsertRedshiftTargetOptionsTypeDef definition

class UpsertRedshiftTargetOptionsTypeDef(TypedDict):
    TableLocation: NotRequired[str],
    ConnectionName: NotRequired[str],
    UpsertKeys: NotRequired[Sequence[str]],
```

## ViewRepresentationInputTypeDef

```python
# ViewRepresentationInputTypeDef definition

class ViewRepresentationInputTypeDef(TypedDict):
    Dialect: NotRequired[ViewDialectType],  # (1)
    DialectVersion: NotRequired[str],
    ViewOriginalText: NotRequired[str],
    ValidationConnection: NotRequired[str],
    ViewExpandedText: NotRequired[str],
```

1. See [:material-code-brackets: ViewDialectType](./literals.md#viewdialecttype) 
## ViewRepresentationTypeDef

```python
# ViewRepresentationTypeDef definition

class ViewRepresentationTypeDef(TypedDict):
    Dialect: NotRequired[ViewDialectType],  # (1)
    DialectVersion: NotRequired[str],
    ViewOriginalText: NotRequired[str],
    ViewExpandedText: NotRequired[str],
    ValidationConnection: NotRequired[str],
    IsStale: NotRequired[bool],
```

1. See [:material-code-brackets: ViewDialectType](./literals.md#viewdialecttype) 
## WorkflowRunStatisticsTypeDef

```python
# WorkflowRunStatisticsTypeDef definition

class WorkflowRunStatisticsTypeDef(TypedDict):
    TotalActions: NotRequired[int],
    TimeoutActions: NotRequired[int],
    FailedActions: NotRequired[int],
    StoppedActions: NotRequired[int],
    SucceededActions: NotRequired[int],
    RunningActions: NotRequired[int],
    ErroredActions: NotRequired[int],
    WaitingActions: NotRequired[int],
```

## ActionOutputTypeDef

```python
# ActionOutputTypeDef definition

class ActionOutputTypeDef(TypedDict):
    JobName: NotRequired[str],
    Arguments: NotRequired[Dict[str, str]],
    Timeout: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (1)
    CrawlerName: NotRequired[str],
```

1. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    JobName: NotRequired[str],
    Arguments: NotRequired[Mapping[str, str]],
    Timeout: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (1)
    CrawlerName: NotRequired[str],
```

1. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
## StartJobRunRequestRequestTypeDef

```python
# StartJobRunRequestRequestTypeDef definition

class StartJobRunRequestRequestTypeDef(TypedDict):
    JobName: str,
    JobRunQueuingEnabled: NotRequired[bool],
    JobRunId: NotRequired[str],
    Arguments: NotRequired[Mapping[str, str]],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (1)
    WorkerType: NotRequired[WorkerTypeType],  # (2)
    NumberOfWorkers: NotRequired[int],
    ExecutionClass: NotRequired[ExecutionClassType],  # (3)
```

1. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
2. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
3. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
## AggregateOutputTypeDef

```python
# AggregateOutputTypeDef definition

class AggregateOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Groups: List[List[str]],
    Aggs: List[AggregateOperationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AggregateOperationOutputTypeDef](./type_defs.md#aggregateoperationoutputtypedef) 
## PropertyTypeDef

```python
# PropertyTypeDef definition

class PropertyTypeDef(TypedDict):
    Name: str,
    Description: str,
    Required: bool,
    PropertyTypes: List[PropertyTypeType],  # (1)
    DefaultValue: NotRequired[str],
    AllowedValues: NotRequired[List[AllowedValueTypeDef]],  # (2)
    DataOperationScopes: NotRequired[List[DataOperationType]],  # (3)
```

1. See [:material-code-brackets: PropertyTypeType](./literals.md#propertytypetype) 
2. See [:material-code-braces: AllowedValueTypeDef](./type_defs.md#allowedvaluetypedef) 
3. See [:material-code-brackets: DataOperationType](./literals.md#dataoperationtype) 
## AmazonRedshiftNodeDataOutputTypeDef

```python
# AmazonRedshiftNodeDataOutputTypeDef definition

class AmazonRedshiftNodeDataOutputTypeDef(TypedDict):
    AccessType: NotRequired[str],
    SourceType: NotRequired[str],
    Connection: NotRequired[OptionTypeDef],  # (1)
    Schema: NotRequired[OptionTypeDef],  # (1)
    Table: NotRequired[OptionTypeDef],  # (1)
    CatalogDatabase: NotRequired[OptionTypeDef],  # (1)
    CatalogTable: NotRequired[OptionTypeDef],  # (1)
    CatalogRedshiftSchema: NotRequired[str],
    CatalogRedshiftTable: NotRequired[str],
    TempDir: NotRequired[str],
    IamRole: NotRequired[OptionTypeDef],  # (1)
    AdvancedOptions: NotRequired[List[AmazonRedshiftAdvancedOptionTypeDef]],  # (7)
    SampleQuery: NotRequired[str],
    PreAction: NotRequired[str],
    PostAction: NotRequired[str],
    Action: NotRequired[str],
    TablePrefix: NotRequired[str],
    Upsert: NotRequired[bool],
    MergeAction: NotRequired[str],
    MergeWhenMatched: NotRequired[str],
    MergeWhenNotMatched: NotRequired[str],
    MergeClause: NotRequired[str],
    CrawlerConnection: NotRequired[str],
    TableSchema: NotRequired[List[OptionTypeDef]],  # (8)
    StagingTable: NotRequired[str],
    SelectedColumns: NotRequired[List[OptionTypeDef]],  # (8)
```

1. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
2. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
3. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
4. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
5. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
6. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
7. See [:material-code-braces: AmazonRedshiftAdvancedOptionTypeDef](./type_defs.md#amazonredshiftadvancedoptiontypedef) 
8. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
9. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
## AmazonRedshiftNodeDataTypeDef

```python
# AmazonRedshiftNodeDataTypeDef definition

class AmazonRedshiftNodeDataTypeDef(TypedDict):
    AccessType: NotRequired[str],
    SourceType: NotRequired[str],
    Connection: NotRequired[OptionTypeDef],  # (1)
    Schema: NotRequired[OptionTypeDef],  # (1)
    Table: NotRequired[OptionTypeDef],  # (1)
    CatalogDatabase: NotRequired[OptionTypeDef],  # (1)
    CatalogTable: NotRequired[OptionTypeDef],  # (1)
    CatalogRedshiftSchema: NotRequired[str],
    CatalogRedshiftTable: NotRequired[str],
    TempDir: NotRequired[str],
    IamRole: NotRequired[OptionTypeDef],  # (1)
    AdvancedOptions: NotRequired[Sequence[AmazonRedshiftAdvancedOptionTypeDef]],  # (7)
    SampleQuery: NotRequired[str],
    PreAction: NotRequired[str],
    PostAction: NotRequired[str],
    Action: NotRequired[str],
    TablePrefix: NotRequired[str],
    Upsert: NotRequired[bool],
    MergeAction: NotRequired[str],
    MergeWhenMatched: NotRequired[str],
    MergeWhenNotMatched: NotRequired[str],
    MergeClause: NotRequired[str],
    CrawlerConnection: NotRequired[str],
    TableSchema: NotRequired[Sequence[OptionTypeDef]],  # (8)
    StagingTable: NotRequired[str],
    SelectedColumns: NotRequired[Sequence[OptionTypeDef]],  # (8)
```

1. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
2. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
3. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
4. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
5. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
6. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
7. See [:material-code-braces: AmazonRedshiftAdvancedOptionTypeDef](./type_defs.md#amazonredshiftadvancedoptiontypedef) 
8. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
9. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
## SnowflakeNodeDataOutputTypeDef

```python
# SnowflakeNodeDataOutputTypeDef definition

class SnowflakeNodeDataOutputTypeDef(TypedDict):
    SourceType: NotRequired[str],
    Connection: NotRequired[OptionTypeDef],  # (1)
    Schema: NotRequired[str],
    Table: NotRequired[str],
    Database: NotRequired[str],
    TempDir: NotRequired[str],
    IamRole: NotRequired[OptionTypeDef],  # (1)
    AdditionalOptions: NotRequired[Dict[str, str]],
    SampleQuery: NotRequired[str],
    PreAction: NotRequired[str],
    PostAction: NotRequired[str],
    Action: NotRequired[str],
    Upsert: NotRequired[bool],
    MergeAction: NotRequired[str],
    MergeWhenMatched: NotRequired[str],
    MergeWhenNotMatched: NotRequired[str],
    MergeClause: NotRequired[str],
    StagingTable: NotRequired[str],
    SelectedColumns: NotRequired[List[OptionTypeDef]],  # (3)
    AutoPushdown: NotRequired[bool],
    TableSchema: NotRequired[List[OptionTypeDef]],  # (3)
```

1. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
2. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
3. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
4. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
## SnowflakeNodeDataTypeDef

```python
# SnowflakeNodeDataTypeDef definition

class SnowflakeNodeDataTypeDef(TypedDict):
    SourceType: NotRequired[str],
    Connection: NotRequired[OptionTypeDef],  # (1)
    Schema: NotRequired[str],
    Table: NotRequired[str],
    Database: NotRequired[str],
    TempDir: NotRequired[str],
    IamRole: NotRequired[OptionTypeDef],  # (1)
    AdditionalOptions: NotRequired[Mapping[str, str]],
    SampleQuery: NotRequired[str],
    PreAction: NotRequired[str],
    PostAction: NotRequired[str],
    Action: NotRequired[str],
    Upsert: NotRequired[bool],
    MergeAction: NotRequired[str],
    MergeWhenMatched: NotRequired[str],
    MergeWhenNotMatched: NotRequired[str],
    MergeClause: NotRequired[str],
    StagingTable: NotRequired[str],
    SelectedColumns: NotRequired[Sequence[OptionTypeDef]],  # (3)
    AutoPushdown: NotRequired[bool],
    TableSchema: NotRequired[Sequence[OptionTypeDef]],  # (3)
```

1. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
2. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
3. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
4. See [:material-code-braces: OptionTypeDef](./type_defs.md#optiontypedef) 
## ApplyMappingOutputTypeDef

```python
# ApplyMappingOutputTypeDef definition

class ApplyMappingOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Mapping: List[MappingOutputTypeDef],  # (1)
```

1. See [:material-code-braces: MappingOutputTypeDef](./type_defs.md#mappingoutputtypedef) 
## ApplyMappingPaginatorTypeDef

```python
# ApplyMappingPaginatorTypeDef definition

class ApplyMappingPaginatorTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Mapping: List[MappingPaginatorTypeDef],  # (1)
```

1. See [:material-code-braces: MappingPaginatorTypeDef](./type_defs.md#mappingpaginatortypedef) 
## BackfillErrorTypeDef

```python
# BackfillErrorTypeDef definition

class BackfillErrorTypeDef(TypedDict):
    Code: NotRequired[BackfillErrorCodeType],  # (1)
    Partitions: NotRequired[List[PartitionValueListOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: BackfillErrorCodeType](./literals.md#backfillerrorcodetype) 
2. See [:material-code-braces: PartitionValueListOutputTypeDef](./type_defs.md#partitionvaluelistoutputtypedef) 
## BatchPutDataQualityStatisticAnnotationResponseTypeDef

```python
# BatchPutDataQualityStatisticAnnotationResponseTypeDef definition

class BatchPutDataQualityStatisticAnnotationResponseTypeDef(TypedDict):
    FailedInclusionAnnotations: List[AnnotationErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AnnotationErrorTypeDef](./type_defs.md#annotationerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelMLTaskRunResponseTypeDef

```python
# CancelMLTaskRunResponseTypeDef definition

class CancelMLTaskRunResponseTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
    Status: TaskStatusTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckSchemaVersionValidityResponseTypeDef

```python
# CheckSchemaVersionValidityResponseTypeDef definition

class CheckSchemaVersionValidityResponseTypeDef(TypedDict):
    Valid: bool,
    Error: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBlueprintResponseTypeDef

```python
# CreateBlueprintResponseTypeDef definition

class CreateBlueprintResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectionResponseTypeDef

```python
# CreateConnectionResponseTypeDef definition

class CreateConnectionResponseTypeDef(TypedDict):
    CreateConnectionStatus: ConnectionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCustomEntityTypeResponseTypeDef

```python
# CreateCustomEntityTypeResponseTypeDef definition

class CreateCustomEntityTypeResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataQualityRulesetResponseTypeDef

```python
# CreateDataQualityRulesetResponseTypeDef definition

class CreateDataQualityRulesetResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDevEndpointResponseTypeDef

```python
# CreateDevEndpointResponseTypeDef definition

class CreateDevEndpointResponseTypeDef(TypedDict):
    EndpointName: str,
    Status: str,
    SecurityGroupIds: List[str],
    SubnetId: str,
    RoleArn: str,
    YarnEndpointAddress: str,
    ZeppelinRemoteSparkInterpreterPort: int,
    NumberOfNodes: int,
    WorkerType: WorkerTypeType,  # (1)
    GlueVersion: str,
    NumberOfWorkers: int,
    AvailabilityZone: str,
    VpcId: str,
    ExtraPythonLibsS3Path: str,
    ExtraJarsS3Path: str,
    FailureReason: str,
    SecurityConfiguration: str,
    CreatedTimestamp: datetime,
    Arguments: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobResponseTypeDef

```python
# CreateJobResponseTypeDef definition

class CreateJobResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMLTransformResponseTypeDef

```python
# CreateMLTransformResponseTypeDef definition

class CreateMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRegistryResponseTypeDef

```python
# CreateRegistryResponseTypeDef definition

class CreateRegistryResponseTypeDef(TypedDict):
    RegistryArn: str,
    RegistryName: str,
    Description: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSchemaResponseTypeDef

```python
# CreateSchemaResponseTypeDef definition

class CreateSchemaResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    SchemaName: str,
    SchemaArn: str,
    Description: str,
    DataFormat: DataFormatType,  # (1)
    Compatibility: CompatibilityType,  # (2)
    SchemaCheckpoint: int,
    LatestSchemaVersion: int,
    NextSchemaVersion: int,
    SchemaStatus: SchemaStatusType,  # (3)
    Tags: Dict[str, str],
    SchemaVersionId: str,
    SchemaVersionStatus: SchemaVersionStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
3. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
4. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateScriptResponseTypeDef

```python
# CreateScriptResponseTypeDef definition

class CreateScriptResponseTypeDef(TypedDict):
    PythonScript: str,
    ScalaCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSecurityConfigurationResponseTypeDef

```python
# CreateSecurityConfigurationResponseTypeDef definition

class CreateSecurityConfigurationResponseTypeDef(TypedDict):
    Name: str,
    CreatedTimestamp: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTriggerResponseTypeDef

```python
# CreateTriggerResponseTypeDef definition

class CreateTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateUsageProfileResponseTypeDef

```python
# CreateUsageProfileResponseTypeDef definition

class CreateUsageProfileResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateWorkflowResponseTypeDef

```python
# CreateWorkflowResponseTypeDef definition

class CreateWorkflowResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBlueprintResponseTypeDef

```python
# DeleteBlueprintResponseTypeDef definition

class DeleteBlueprintResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCustomEntityTypeResponseTypeDef

```python
# DeleteCustomEntityTypeResponseTypeDef definition

class DeleteCustomEntityTypeResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteJobResponseTypeDef

```python
# DeleteJobResponseTypeDef definition

class DeleteJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteMLTransformResponseTypeDef

```python
# DeleteMLTransformResponseTypeDef definition

class DeleteMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRegistryResponseTypeDef

```python
# DeleteRegistryResponseTypeDef definition

class DeleteRegistryResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    Status: RegistryStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RegistryStatusType](./literals.md#registrystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSchemaResponseTypeDef

```python
# DeleteSchemaResponseTypeDef definition

class DeleteSchemaResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    Status: SchemaStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSessionResponseTypeDef

```python
# DeleteSessionResponseTypeDef definition

class DeleteSessionResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTriggerResponseTypeDef

```python
# DeleteTriggerResponseTypeDef definition

class DeleteTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWorkflowResponseTypeDef

```python
# DeleteWorkflowResponseTypeDef definition

class DeleteWorkflowResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomEntityTypeResponseTypeDef

```python
# GetCustomEntityTypeResponseTypeDef definition

class GetCustomEntityTypeResponseTypeDef(TypedDict):
    Name: str,
    RegexString: str,
    ContextWords: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataQualityModelResponseTypeDef

```python
# GetDataQualityModelResponseTypeDef definition

class GetDataQualityModelResponseTypeDef(TypedDict):
    Status: DataQualityModelStatusType,  # (1)
    StartedOn: datetime,
    CompletedOn: datetime,
    FailureReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataQualityModelStatusType](./literals.md#dataqualitymodelstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEntityRecordsResponseTypeDef

```python
# GetEntityRecordsResponseTypeDef definition

class GetEntityRecordsResponseTypeDef(TypedDict):
    Records: List[Dict[str, Any]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPlanResponseTypeDef

```python
# GetPlanResponseTypeDef definition

class GetPlanResponseTypeDef(TypedDict):
    PythonScript: str,
    ScalaCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRegistryResponseTypeDef

```python
# GetRegistryResponseTypeDef definition

class GetRegistryResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    Description: str,
    Status: RegistryStatusType,  # (1)
    CreatedTime: str,
    UpdatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: RegistryStatusType](./literals.md#registrystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    PolicyInJson: str,
    PolicyHash: str,
    CreateTime: datetime,
    UpdateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaByDefinitionResponseTypeDef

```python
# GetSchemaByDefinitionResponseTypeDef definition

class GetSchemaByDefinitionResponseTypeDef(TypedDict):
    SchemaVersionId: str,
    SchemaArn: str,
    DataFormat: DataFormatType,  # (1)
    Status: SchemaVersionStatusType,  # (2)
    CreatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaResponseTypeDef

```python
# GetSchemaResponseTypeDef definition

class GetSchemaResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    SchemaName: str,
    SchemaArn: str,
    Description: str,
    DataFormat: DataFormatType,  # (1)
    Compatibility: CompatibilityType,  # (2)
    SchemaCheckpoint: int,
    LatestSchemaVersion: int,
    NextSchemaVersion: int,
    SchemaStatus: SchemaStatusType,  # (3)
    CreatedTime: str,
    UpdatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
3. See [:material-code-brackets: SchemaStatusType](./literals.md#schemastatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaVersionResponseTypeDef

```python
# GetSchemaVersionResponseTypeDef definition

class GetSchemaVersionResponseTypeDef(TypedDict):
    SchemaVersionId: str,
    SchemaDefinition: str,
    DataFormat: DataFormatType,  # (1)
    SchemaArn: str,
    VersionNumber: int,
    Status: SchemaVersionStatusType,  # (2)
    CreatedTime: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaVersionsDiffResponseTypeDef

```python
# GetSchemaVersionsDiffResponseTypeDef definition

class GetSchemaVersionsDiffResponseTypeDef(TypedDict):
    Diff: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagsResponseTypeDef

```python
# GetTagsResponseTypeDef definition

class GetTagsResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowRunPropertiesResponseTypeDef

```python
# GetWorkflowRunPropertiesResponseTypeDef definition

class GetWorkflowRunPropertiesResponseTypeDef(TypedDict):
    RunProperties: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBlueprintsResponseTypeDef

```python
# ListBlueprintsResponseTypeDef definition

class ListBlueprintsResponseTypeDef(TypedDict):
    Blueprints: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListColumnStatisticsTaskRunsResponseTypeDef

```python
# ListColumnStatisticsTaskRunsResponseTypeDef definition

class ListColumnStatisticsTaskRunsResponseTypeDef(TypedDict):
    ColumnStatisticsTaskRunIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCrawlersResponseTypeDef

```python
# ListCrawlersResponseTypeDef definition

class ListCrawlersResponseTypeDef(TypedDict):
    CrawlerNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDevEndpointsResponseTypeDef

```python
# ListDevEndpointsResponseTypeDef definition

class ListDevEndpointsResponseTypeDef(TypedDict):
    DevEndpointNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResponseTypeDef

```python
# ListJobsResponseTypeDef definition

class ListJobsResponseTypeDef(TypedDict):
    JobNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMLTransformsResponseTypeDef

```python
# ListMLTransformsResponseTypeDef definition

class ListMLTransformsResponseTypeDef(TypedDict):
    TransformIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTriggersResponseTypeDef

```python
# ListTriggersResponseTypeDef definition

class ListTriggersResponseTypeDef(TypedDict):
    TriggerNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkflowsResponseTypeDef

```python
# ListWorkflowsResponseTypeDef definition

class ListWorkflowsResponseTypeDef(TypedDict):
    Workflows: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    PolicyHash: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSchemaVersionMetadataResponseTypeDef

```python
# PutSchemaVersionMetadataResponseTypeDef definition

class PutSchemaVersionMetadataResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    RegistryName: str,
    LatestVersion: bool,
    VersionNumber: int,
    SchemaVersionId: str,
    MetadataKey: str,
    MetadataValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterSchemaVersionResponseTypeDef

```python
# RegisterSchemaVersionResponseTypeDef definition

class RegisterSchemaVersionResponseTypeDef(TypedDict):
    SchemaVersionId: str,
    VersionNumber: int,
    Status: SchemaVersionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SchemaVersionStatusType](./literals.md#schemaversionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveSchemaVersionMetadataResponseTypeDef

```python
# RemoveSchemaVersionMetadataResponseTypeDef definition

class RemoveSchemaVersionMetadataResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    RegistryName: str,
    LatestVersion: bool,
    VersionNumber: int,
    SchemaVersionId: str,
    MetadataKey: str,
    MetadataValue: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResumeWorkflowRunResponseTypeDef

```python
# ResumeWorkflowRunResponseTypeDef definition

class ResumeWorkflowRunResponseTypeDef(TypedDict):
    RunId: str,
    NodeIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RunStatementResponseTypeDef

```python
# RunStatementResponseTypeDef definition

class RunStatementResponseTypeDef(TypedDict):
    Id: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartBlueprintRunResponseTypeDef

```python
# StartBlueprintRunResponseTypeDef definition

class StartBlueprintRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartColumnStatisticsTaskRunResponseTypeDef

```python
# StartColumnStatisticsTaskRunResponseTypeDef definition

class StartColumnStatisticsTaskRunResponseTypeDef(TypedDict):
    ColumnStatisticsTaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataQualityRuleRecommendationRunResponseTypeDef

```python
# StartDataQualityRuleRecommendationRunResponseTypeDef definition

class StartDataQualityRuleRecommendationRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataQualityRulesetEvaluationRunResponseTypeDef

```python
# StartDataQualityRulesetEvaluationRunResponseTypeDef definition

class StartDataQualityRulesetEvaluationRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartExportLabelsTaskRunResponseTypeDef

```python
# StartExportLabelsTaskRunResponseTypeDef definition

class StartExportLabelsTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartImportLabelsTaskRunResponseTypeDef

```python
# StartImportLabelsTaskRunResponseTypeDef definition

class StartImportLabelsTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartJobRunResponseTypeDef

```python
# StartJobRunResponseTypeDef definition

class StartJobRunResponseTypeDef(TypedDict):
    JobRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLEvaluationTaskRunResponseTypeDef

```python
# StartMLEvaluationTaskRunResponseTypeDef definition

class StartMLEvaluationTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMLLabelingSetGenerationTaskRunResponseTypeDef

```python
# StartMLLabelingSetGenerationTaskRunResponseTypeDef definition

class StartMLLabelingSetGenerationTaskRunResponseTypeDef(TypedDict):
    TaskRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTriggerResponseTypeDef

```python
# StartTriggerResponseTypeDef definition

class StartTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartWorkflowRunResponseTypeDef

```python
# StartWorkflowRunResponseTypeDef definition

class StartWorkflowRunResponseTypeDef(TypedDict):
    RunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopSessionResponseTypeDef

```python
# StopSessionResponseTypeDef definition

class StopSessionResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopTriggerResponseTypeDef

```python
# StopTriggerResponseTypeDef definition

class StopTriggerResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBlueprintResponseTypeDef

```python
# UpdateBlueprintResponseTypeDef definition

class UpdateBlueprintResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataQualityRulesetResponseTypeDef

```python
# UpdateDataQualityRulesetResponseTypeDef definition

class UpdateDataQualityRulesetResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    Ruleset: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobFromSourceControlResponseTypeDef

```python
# UpdateJobFromSourceControlResponseTypeDef definition

class UpdateJobFromSourceControlResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobResponseTypeDef

```python
# UpdateJobResponseTypeDef definition

class UpdateJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMLTransformResponseTypeDef

```python
# UpdateMLTransformResponseTypeDef definition

class UpdateMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRegistryResponseTypeDef

```python
# UpdateRegistryResponseTypeDef definition

class UpdateRegistryResponseTypeDef(TypedDict):
    RegistryName: str,
    RegistryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSchemaResponseTypeDef

```python
# UpdateSchemaResponseTypeDef definition

class UpdateSchemaResponseTypeDef(TypedDict):
    SchemaArn: str,
    SchemaName: str,
    RegistryName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSourceControlFromJobResponseTypeDef

```python
# UpdateSourceControlFromJobResponseTypeDef definition

class UpdateSourceControlFromJobResponseTypeDef(TypedDict):
    JobName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUsageProfileResponseTypeDef

```python
# UpdateUsageProfileResponseTypeDef definition

class UpdateUsageProfileResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWorkflowResponseTypeDef

```python
# UpdateWorkflowResponseTypeDef definition

class UpdateWorkflowResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteConnectionResponseTypeDef

```python
# BatchDeleteConnectionResponseTypeDef definition

class BatchDeleteConnectionResponseTypeDef(TypedDict):
    Succeeded: List[str],
    Errors: Dict[str, ErrorDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetTableOptimizerErrorTypeDef

```python
# BatchGetTableOptimizerErrorTypeDef definition

class BatchGetTableOptimizerErrorTypeDef(TypedDict):
    error: NotRequired[ErrorDetailTypeDef],  # (1)
    catalogId: NotRequired[str],
    databaseName: NotRequired[str],
    tableName: NotRequired[str],
    type: NotRequired[TableOptimizerTypeType],  # (2)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
2. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
## BatchStopJobRunErrorTypeDef

```python
# BatchStopJobRunErrorTypeDef definition

class BatchStopJobRunErrorTypeDef(TypedDict):
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## BatchUpdatePartitionFailureEntryTypeDef

```python
# BatchUpdatePartitionFailureEntryTypeDef definition

class BatchUpdatePartitionFailureEntryTypeDef(TypedDict):
    PartitionValueList: NotRequired[List[str]],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ColumnErrorTypeDef

```python
# ColumnErrorTypeDef definition

class ColumnErrorTypeDef(TypedDict):
    ColumnName: NotRequired[str],
    Error: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## PartitionErrorTypeDef

```python
# PartitionErrorTypeDef definition

class PartitionErrorTypeDef(TypedDict):
    PartitionValues: NotRequired[List[str]],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## TableErrorTypeDef

```python
# TableErrorTypeDef definition

class TableErrorTypeDef(TypedDict):
    TableName: NotRequired[str],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## TableVersionErrorTypeDef

```python
# TableVersionErrorTypeDef definition

class TableVersionErrorTypeDef(TypedDict):
    TableName: NotRequired[str],
    VersionId: NotRequired[str],
    ErrorDetail: NotRequired[ErrorDetailTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ViewValidationTypeDef

```python
# ViewValidationTypeDef definition

class ViewValidationTypeDef(TypedDict):
    Dialect: NotRequired[ViewDialectType],  # (1)
    DialectVersion: NotRequired[str],
    ViewValidationText: NotRequired[str],
    UpdateTime: NotRequired[datetime],
    State: NotRequired[ResourceStateType],  # (2)
    Error: NotRequired[ErrorDetailTypeDef],  # (3)
```

1. See [:material-code-brackets: ViewDialectType](./literals.md#viewdialecttype) 
2. See [:material-code-brackets: ResourceStateType](./literals.md#resourcestatetype) 
3. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## BatchGetCustomEntityTypesResponseTypeDef

```python
# BatchGetCustomEntityTypesResponseTypeDef definition

class BatchGetCustomEntityTypesResponseTypeDef(TypedDict):
    CustomEntityTypes: List[CustomEntityTypeTypeDef],  # (1)
    CustomEntityTypesNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomEntityTypeTypeDef](./type_defs.md#customentitytypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCustomEntityTypesResponseTypeDef

```python
# ListCustomEntityTypesResponseTypeDef definition

class ListCustomEntityTypesResponseTypeDef(TypedDict):
    CustomEntityTypes: List[CustomEntityTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CustomEntityTypeTypeDef](./type_defs.md#customentitytypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetDevEndpointsResponseTypeDef

```python
# BatchGetDevEndpointsResponseTypeDef definition

class BatchGetDevEndpointsResponseTypeDef(TypedDict):
    DevEndpoints: List[DevEndpointTypeDef],  # (1)
    DevEndpointsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevEndpointTypeDef](./type_defs.md#devendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevEndpointResponseTypeDef

```python
# GetDevEndpointResponseTypeDef definition

class GetDevEndpointResponseTypeDef(TypedDict):
    DevEndpoint: DevEndpointTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DevEndpointTypeDef](./type_defs.md#devendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDevEndpointsResponseTypeDef

```python
# GetDevEndpointsResponseTypeDef definition

class GetDevEndpointsResponseTypeDef(TypedDict):
    DevEndpoints: List[DevEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DevEndpointTypeDef](./type_defs.md#devendpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetPartitionRequestRequestTypeDef

```python
# BatchGetPartitionRequestRequestTypeDef definition

class BatchGetPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionsToGet: Sequence[PartitionValueListTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) 
## BatchGetTableOptimizerRequestRequestTypeDef

```python
# BatchGetTableOptimizerRequestRequestTypeDef definition

class BatchGetTableOptimizerRequestRequestTypeDef(TypedDict):
    Entries: Sequence[BatchGetTableOptimizerEntryTypeDef],  # (1)
```

1. See [:material-code-braces: BatchGetTableOptimizerEntryTypeDef](./type_defs.md#batchgettableoptimizerentrytypedef) 
## BatchPutDataQualityStatisticAnnotationRequestRequestTypeDef

```python
# BatchPutDataQualityStatisticAnnotationRequestRequestTypeDef definition

class BatchPutDataQualityStatisticAnnotationRequestRequestTypeDef(TypedDict):
    InclusionAnnotations: Sequence[DatapointInclusionAnnotationTypeDef],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: DatapointInclusionAnnotationTypeDef](./type_defs.md#datapointinclusionannotationtypedef) 
## DecimalNumberTypeDef

```python
# DecimalNumberTypeDef definition

class DecimalNumberTypeDef(TypedDict):
    UnscaledValue: BlobTypeDef,
    Scale: int,
```

## GetBlueprintRunResponseTypeDef

```python
# GetBlueprintRunResponseTypeDef definition

class GetBlueprintRunResponseTypeDef(TypedDict):
    BlueprintRun: BlueprintRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintRunTypeDef](./type_defs.md#blueprintruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlueprintRunsResponseTypeDef

```python
# GetBlueprintRunsResponseTypeDef definition

class GetBlueprintRunsResponseTypeDef(TypedDict):
    BlueprintRuns: List[BlueprintRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BlueprintRunTypeDef](./type_defs.md#blueprintruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BlueprintTypeDef

```python
# BlueprintTypeDef definition

class BlueprintTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    ParameterSpec: NotRequired[str],
    BlueprintLocation: NotRequired[str],
    BlueprintServiceLocation: NotRequired[str],
    Status: NotRequired[BlueprintStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    LastActiveDefinition: NotRequired[LastActiveDefinitionTypeDef],  # (2)
```

1. See [:material-code-brackets: BlueprintStatusType](./literals.md#blueprintstatustype) 
2. See [:material-code-braces: LastActiveDefinitionTypeDef](./type_defs.md#lastactivedefinitiontypedef) 
## ConnectionTypeBriefTypeDef

```python
# ConnectionTypeBriefTypeDef definition

class ConnectionTypeBriefTypeDef(TypedDict):
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
    Description: NotRequired[str],
    Capabilities: NotRequired[CapabilitiesTypeDef],  # (2)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-braces: CapabilitiesTypeDef](./type_defs.md#capabilitiestypedef) 
## GetCatalogImportStatusResponseTypeDef

```python
# GetCatalogImportStatusResponseTypeDef definition

class GetCatalogImportStatusResponseTypeDef(TypedDict):
    ImportStatus: CatalogImportStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CatalogImportStatusTypeDef](./type_defs.md#catalogimportstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CatalogKafkaSourceOutputTypeDef

```python
# CatalogKafkaSourceOutputTypeDef definition

class CatalogKafkaSourceOutputTypeDef(TypedDict):
    Name: str,
    Table: str,
    Database: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KafkaStreamingSourceOptionsOutputTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KafkaStreamingSourceOptionsOutputTypeDef](./type_defs.md#kafkastreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## DirectKafkaSourceOutputTypeDef

```python
# DirectKafkaSourceOutputTypeDef definition

class DirectKafkaSourceOutputTypeDef(TypedDict):
    Name: str,
    StreamingOptions: NotRequired[KafkaStreamingSourceOptionsOutputTypeDef],  # (1)
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KafkaStreamingSourceOptionsOutputTypeDef](./type_defs.md#kafkastreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## CatalogKinesisSourceOutputTypeDef

```python
# CatalogKinesisSourceOutputTypeDef definition

class CatalogKinesisSourceOutputTypeDef(TypedDict):
    Name: str,
    Table: str,
    Database: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KinesisStreamingSourceOptionsOutputTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisStreamingSourceOptionsOutputTypeDef](./type_defs.md#kinesisstreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## DirectKinesisSourceOutputTypeDef

```python
# DirectKinesisSourceOutputTypeDef definition

class DirectKinesisSourceOutputTypeDef(TypedDict):
    Name: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KinesisStreamingSourceOptionsOutputTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisStreamingSourceOptionsOutputTypeDef](./type_defs.md#kinesisstreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## CatalogPropertiesOutputTypeDef

```python
# CatalogPropertiesOutputTypeDef definition

class CatalogPropertiesOutputTypeDef(TypedDict):
    DataLakeAccessProperties: NotRequired[DataLakeAccessPropertiesOutputTypeDef],  # (1)
    CustomProperties: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DataLakeAccessPropertiesOutputTypeDef](./type_defs.md#datalakeaccesspropertiesoutputtypedef) 
## CatalogPropertiesTypeDef

```python
# CatalogPropertiesTypeDef definition

class CatalogPropertiesTypeDef(TypedDict):
    DataLakeAccessProperties: NotRequired[DataLakeAccessPropertiesTypeDef],  # (1)
    CustomProperties: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DataLakeAccessPropertiesTypeDef](./type_defs.md#datalakeaccesspropertiestypedef) 
## GovernedCatalogTargetOutputTypeDef

```python
# GovernedCatalogTargetOutputTypeDef definition

class GovernedCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## GovernedCatalogTargetTypeDef

```python
# GovernedCatalogTargetTypeDef definition

class GovernedCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3CatalogTargetOutputTypeDef

```python
# S3CatalogTargetOutputTypeDef definition

class S3CatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3CatalogTargetTypeDef

```python
# S3CatalogTargetTypeDef definition

class S3CatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3DeltaCatalogTargetOutputTypeDef

```python
# S3DeltaCatalogTargetOutputTypeDef definition

class S3DeltaCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[List[List[str]]],
    AdditionalOptions: NotRequired[Dict[str, str]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3DeltaCatalogTargetTypeDef

```python
# S3DeltaCatalogTargetTypeDef definition

class S3DeltaCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Table: str,
    Database: str,
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    AdditionalOptions: NotRequired[Mapping[str, str]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3HudiCatalogTargetOutputTypeDef

```python
# S3HudiCatalogTargetOutputTypeDef definition

class S3HudiCatalogTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Table: str,
    Database: str,
    AdditionalOptions: Dict[str, str],
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## S3HudiCatalogTargetTypeDef

```python
# S3HudiCatalogTargetTypeDef definition

class S3HudiCatalogTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Table: str,
    Database: str,
    AdditionalOptions: Mapping[str, str],
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    SchemaChangePolicy: NotRequired[CatalogSchemaChangePolicyTypeDef],  # (1)
```

1. See [:material-code-braces: CatalogSchemaChangePolicyTypeDef](./type_defs.md#catalogschemachangepolicytypedef) 
## ClassifierTypeDef

```python
# ClassifierTypeDef definition

class ClassifierTypeDef(TypedDict):
    GrokClassifier: NotRequired[GrokClassifierTypeDef],  # (1)
    XMLClassifier: NotRequired[XMLClassifierTypeDef],  # (2)
    JsonClassifier: NotRequired[JsonClassifierTypeDef],  # (3)
    CsvClassifier: NotRequired[CsvClassifierTypeDef],  # (4)
```

1. See [:material-code-braces: GrokClassifierTypeDef](./type_defs.md#grokclassifiertypedef) 
2. See [:material-code-braces: XMLClassifierTypeDef](./type_defs.md#xmlclassifiertypedef) 
3. See [:material-code-braces: JsonClassifierTypeDef](./type_defs.md#jsonclassifiertypedef) 
4. See [:material-code-braces: CsvClassifierTypeDef](./type_defs.md#csvclassifiertypedef) 
## CodeGenNodeOutputTypeDef

```python
# CodeGenNodeOutputTypeDef definition

class CodeGenNodeOutputTypeDef(TypedDict):
    Id: str,
    NodeType: str,
    Args: List[CodeGenNodeArgTypeDef],  # (1)
    LineNumber: NotRequired[int],
```

1. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
## CodeGenNodeTypeDef

```python
# CodeGenNodeTypeDef definition

class CodeGenNodeTypeDef(TypedDict):
    Id: str,
    NodeType: str,
    Args: Sequence[CodeGenNodeArgTypeDef],  # (1)
    LineNumber: NotRequired[int],
```

1. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
## LocationTypeDef

```python
# LocationTypeDef definition

class LocationTypeDef(TypedDict):
    Jdbc: NotRequired[Sequence[CodeGenNodeArgTypeDef]],  # (1)
    S3: NotRequired[Sequence[CodeGenNodeArgTypeDef]],  # (1)
    DynamoDB: NotRequired[Sequence[CodeGenNodeArgTypeDef]],  # (1)
```

1. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
2. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
3. See [:material-code-braces: CodeGenNodeArgTypeDef](./type_defs.md#codegennodeargtypedef) 
## GetColumnStatisticsTaskRunResponseTypeDef

```python
# GetColumnStatisticsTaskRunResponseTypeDef definition

class GetColumnStatisticsTaskRunResponseTypeDef(TypedDict):
    ColumnStatisticsTaskRun: ColumnStatisticsTaskRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnStatisticsTaskRunTypeDef](./type_defs.md#columnstatisticstaskruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetColumnStatisticsTaskRunsResponseTypeDef

```python
# GetColumnStatisticsTaskRunsResponseTypeDef definition

class GetColumnStatisticsTaskRunsResponseTypeDef(TypedDict):
    ColumnStatisticsTaskRuns: List[ColumnStatisticsTaskRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ColumnStatisticsTaskRunTypeDef](./type_defs.md#columnstatisticstaskruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ColumnStatisticsTaskSettingsTypeDef

```python
# ColumnStatisticsTaskSettingsTypeDef definition

class ColumnStatisticsTaskSettingsTypeDef(TypedDict):
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    Schedule: NotRequired[ScheduleTypeDef],  # (1)
    ColumnNameList: NotRequired[List[str]],
    CatalogID: NotRequired[str],
    Role: NotRequired[str],
    SampleSize: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    ScheduleType: NotRequired[ScheduleTypeType],  # (2)
    SettingSource: NotRequired[SettingSourceType],  # (3)
    LastExecutionAttempt: NotRequired[ExecutionAttemptTypeDef],  # (4)
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-brackets: ScheduleTypeType](./literals.md#scheduletypetype) 
3. See [:material-code-brackets: SettingSourceType](./literals.md#settingsourcetype) 
4. See [:material-code-braces: ExecutionAttemptTypeDef](./type_defs.md#executionattempttypedef) 
## DateColumnStatisticsDataTypeDef

```python
# DateColumnStatisticsDataTypeDef definition

class DateColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[TimestampTypeDef],
    MaximumValue: NotRequired[TimestampTypeDef],
```

## GetTableRequestRequestTypeDef

```python
# GetTableRequestRequestTypeDef definition

class GetTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    Name: str,
    CatalogId: NotRequired[str],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[TimestampTypeDef],
    IncludeStatusDetails: NotRequired[bool],
```

## GetTablesRequestRequestTypeDef

```python
# GetTablesRequestRequestTypeDef definition

class GetTablesRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[TimestampTypeDef],
    IncludeStatusDetails: NotRequired[bool],
    AttributesToGet: NotRequired[Sequence[TableAttributesType]],  # (1)
```

1. See [:material-code-brackets: TableAttributesType](./literals.md#tableattributestype) 
## KafkaStreamingSourceOptionsTypeDef

```python
# KafkaStreamingSourceOptionsTypeDef definition

class KafkaStreamingSourceOptionsTypeDef(TypedDict):
    BootstrapServers: NotRequired[str],
    SecurityProtocol: NotRequired[str],
    ConnectionName: NotRequired[str],
    TopicName: NotRequired[str],
    Assign: NotRequired[str],
    SubscribePattern: NotRequired[str],
    Classification: NotRequired[str],
    Delimiter: NotRequired[str],
    StartingOffsets: NotRequired[str],
    EndingOffsets: NotRequired[str],
    PollTimeoutMs: NotRequired[int],
    NumRetries: NotRequired[int],
    RetryIntervalMs: NotRequired[int],
    MaxOffsetsPerTrigger: NotRequired[int],
    MinPartitions: NotRequired[int],
    IncludeHeaders: NotRequired[bool],
    AddRecordTimestamp: NotRequired[str],
    EmitConsumerLagMetrics: NotRequired[str],
    StartingTimestamp: NotRequired[TimestampTypeDef],
```

## KinesisStreamingSourceOptionsTypeDef

```python
# KinesisStreamingSourceOptionsTypeDef definition

class KinesisStreamingSourceOptionsTypeDef(TypedDict):
    EndpointUrl: NotRequired[str],
    StreamName: NotRequired[str],
    Classification: NotRequired[str],
    Delimiter: NotRequired[str],
    StartingPosition: NotRequired[StartingPositionType],  # (1)
    MaxFetchTimeInMs: NotRequired[int],
    MaxFetchRecordsPerShard: NotRequired[int],
    MaxRecordPerRead: NotRequired[int],
    AddIdleTimeBetweenReads: NotRequired[bool],
    IdleTimeBetweenReadsInMs: NotRequired[int],
    DescribeShardInterval: NotRequired[int],
    NumRetries: NotRequired[int],
    RetryIntervalMs: NotRequired[int],
    MaxRetryIntervalMs: NotRequired[int],
    AvoidEmptyBatches: NotRequired[bool],
    StreamArn: NotRequired[str],
    RoleArn: NotRequired[str],
    RoleSessionName: NotRequired[str],
    AddRecordTimestamp: NotRequired[str],
    EmitConsumerLagMetrics: NotRequired[str],
    StartingTimestamp: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: StartingPositionType](./literals.md#startingpositiontype) 
## QuerySessionContextTypeDef

```python
# QuerySessionContextTypeDef definition

class QuerySessionContextTypeDef(TypedDict):
    QueryId: NotRequired[str],
    QueryStartTime: NotRequired[TimestampTypeDef],
    ClusterId: NotRequired[str],
    QueryAuthorizationId: NotRequired[str],
    AdditionalContext: NotRequired[Mapping[str, str]],
```

## TaskRunFilterCriteriaTypeDef

```python
# TaskRunFilterCriteriaTypeDef definition

class TaskRunFilterCriteriaTypeDef(TypedDict):
    TaskRunType: NotRequired[TaskTypeType],  # (1)
    Status: NotRequired[TaskStatusTypeType],  # (2)
    StartedBefore: NotRequired[TimestampTypeDef],
    StartedAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: TaskTypeType](./literals.md#tasktypetype) 
2. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
## TimestampFilterTypeDef

```python
# TimestampFilterTypeDef definition

class TimestampFilterTypeDef(TypedDict):
    RecordedBefore: NotRequired[TimestampTypeDef],
    RecordedAfter: NotRequired[TimestampTypeDef],
```

## CompactionMetricsTypeDef

```python
# CompactionMetricsTypeDef definition

class CompactionMetricsTypeDef(TypedDict):
    IcebergMetrics: NotRequired[IcebergCompactionMetricsTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergCompactionMetricsTypeDef](./type_defs.md#icebergcompactionmetricstypedef) 
## PredicateOutputTypeDef

```python
# PredicateOutputTypeDef definition

class PredicateOutputTypeDef(TypedDict):
    Logical: NotRequired[LogicalType],  # (1)
    Conditions: NotRequired[List[ConditionTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogicalType](./literals.md#logicaltype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## PredicateTypeDef

```python
# PredicateTypeDef definition

class PredicateTypeDef(TypedDict):
    Logical: NotRequired[LogicalType],  # (1)
    Conditions: NotRequired[Sequence[ConditionTypeDef]],  # (2)
```

1. See [:material-code-brackets: LogicalType](./literals.md#logicaltype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
## ProfileConfigurationOutputTypeDef

```python
# ProfileConfigurationOutputTypeDef definition

class ProfileConfigurationOutputTypeDef(TypedDict):
    SessionConfiguration: NotRequired[Dict[str, ConfigurationObjectOutputTypeDef]],  # (1)
    JobConfiguration: NotRequired[Dict[str, ConfigurationObjectOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfigurationObjectOutputTypeDef](./type_defs.md#configurationobjectoutputtypedef) 
2. See [:material-code-braces: ConfigurationObjectOutputTypeDef](./type_defs.md#configurationobjectoutputtypedef) 
## FindMatchesMetricsTypeDef

```python
# FindMatchesMetricsTypeDef definition

class FindMatchesMetricsTypeDef(TypedDict):
    AreaUnderPRCurve: NotRequired[float],
    Precision: NotRequired[float],
    Recall: NotRequired[float],
    F1: NotRequired[float],
    ConfusionMatrix: NotRequired[ConfusionMatrixTypeDef],  # (1)
    ColumnImportances: NotRequired[List[ColumnImportanceTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfusionMatrixTypeDef](./type_defs.md#confusionmatrixtypedef) 
2. See [:material-code-braces: ColumnImportanceTypeDef](./type_defs.md#columnimportancetypedef) 
## CrawlerNodeDetailsTypeDef

```python
# CrawlerNodeDetailsTypeDef definition

class CrawlerNodeDetailsTypeDef(TypedDict):
    Crawls: NotRequired[List[CrawlTypeDef]],  # (1)
```

1. See [:material-code-braces: CrawlTypeDef](./type_defs.md#crawltypedef) 
## ListCrawlsResponseTypeDef

```python
# ListCrawlsResponseTypeDef definition

class ListCrawlsResponseTypeDef(TypedDict):
    Crawls: List[CrawlerHistoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CrawlerHistoryTypeDef](./type_defs.md#crawlerhistorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCrawlerMetricsResponseTypeDef

```python
# GetCrawlerMetricsResponseTypeDef definition

class GetCrawlerMetricsResponseTypeDef(TypedDict):
    CrawlerMetricsList: List[CrawlerMetricsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CrawlerMetricsTypeDef](./type_defs.md#crawlermetricstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CrawlerTargetsOutputTypeDef

```python
# CrawlerTargetsOutputTypeDef definition

class CrawlerTargetsOutputTypeDef(TypedDict):
    S3Targets: NotRequired[List[S3TargetOutputTypeDef]],  # (1)
    JdbcTargets: NotRequired[List[JdbcTargetOutputTypeDef]],  # (2)
    MongoDBTargets: NotRequired[List[MongoDBTargetTypeDef]],  # (3)
    DynamoDBTargets: NotRequired[List[DynamoDBTargetTypeDef]],  # (4)
    CatalogTargets: NotRequired[List[CatalogTargetOutputTypeDef]],  # (5)
    DeltaTargets: NotRequired[List[DeltaTargetOutputTypeDef]],  # (6)
    IcebergTargets: NotRequired[List[IcebergTargetOutputTypeDef]],  # (7)
    HudiTargets: NotRequired[List[HudiTargetOutputTypeDef]],  # (8)
```

1. See [:material-code-braces: S3TargetOutputTypeDef](./type_defs.md#s3targetoutputtypedef) 
2. See [:material-code-braces: JdbcTargetOutputTypeDef](./type_defs.md#jdbctargetoutputtypedef) 
3. See [:material-code-braces: MongoDBTargetTypeDef](./type_defs.md#mongodbtargettypedef) 
4. See [:material-code-braces: DynamoDBTargetTypeDef](./type_defs.md#dynamodbtargettypedef) 
5. See [:material-code-braces: CatalogTargetOutputTypeDef](./type_defs.md#catalogtargetoutputtypedef) 
6. See [:material-code-braces: DeltaTargetOutputTypeDef](./type_defs.md#deltatargetoutputtypedef) 
7. See [:material-code-braces: IcebergTargetOutputTypeDef](./type_defs.md#icebergtargetoutputtypedef) 
8. See [:material-code-braces: HudiTargetOutputTypeDef](./type_defs.md#huditargetoutputtypedef) 
## ListCrawlsRequestRequestTypeDef

```python
# ListCrawlsRequestRequestTypeDef definition

class ListCrawlsRequestRequestTypeDef(TypedDict):
    CrawlerName: str,
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[CrawlsFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CrawlsFilterTypeDef](./type_defs.md#crawlsfiltertypedef) 
## CreateClassifierRequestRequestTypeDef

```python
# CreateClassifierRequestRequestTypeDef definition

class CreateClassifierRequestRequestTypeDef(TypedDict):
    GrokClassifier: NotRequired[CreateGrokClassifierRequestTypeDef],  # (1)
    XMLClassifier: NotRequired[CreateXMLClassifierRequestTypeDef],  # (2)
    JsonClassifier: NotRequired[CreateJsonClassifierRequestTypeDef],  # (3)
    CsvClassifier: NotRequired[CreateCsvClassifierRequestTypeDef],  # (4)
```

1. See [:material-code-braces: CreateGrokClassifierRequestTypeDef](./type_defs.md#creategrokclassifierrequesttypedef) 
2. See [:material-code-braces: CreateXMLClassifierRequestTypeDef](./type_defs.md#createxmlclassifierrequesttypedef) 
3. See [:material-code-braces: CreateJsonClassifierRequestTypeDef](./type_defs.md#createjsonclassifierrequesttypedef) 
4. See [:material-code-braces: CreateCsvClassifierRequestTypeDef](./type_defs.md#createcsvclassifierrequesttypedef) 
## CreateDataQualityRulesetRequestRequestTypeDef

```python
# CreateDataQualityRulesetRequestRequestTypeDef definition

class CreateDataQualityRulesetRequestRequestTypeDef(TypedDict):
    Name: str,
    Ruleset: str,
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    TargetTable: NotRequired[DataQualityTargetTableTypeDef],  # (1)
    DataQualitySecurityConfiguration: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
## DataQualityRulesetFilterCriteriaTypeDef

```python
# DataQualityRulesetFilterCriteriaTypeDef definition

class DataQualityRulesetFilterCriteriaTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedBefore: NotRequired[TimestampTypeDef],
    CreatedAfter: NotRequired[TimestampTypeDef],
    LastModifiedBefore: NotRequired[TimestampTypeDef],
    LastModifiedAfter: NotRequired[TimestampTypeDef],
    TargetTable: NotRequired[DataQualityTargetTableTypeDef],  # (1)
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
## DataQualityRulesetListDetailsTypeDef

```python
# DataQualityRulesetListDetailsTypeDef definition

class DataQualityRulesetListDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    TargetTable: NotRequired[DataQualityTargetTableTypeDef],  # (1)
    RecommendationRunId: NotRequired[str],
    RuleCount: NotRequired[int],
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
## GetDataQualityRulesetResponseTypeDef

```python
# GetDataQualityRulesetResponseTypeDef definition

class GetDataQualityRulesetResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    Ruleset: str,
    TargetTable: DataQualityTargetTableTypeDef,  # (1)
    CreatedOn: datetime,
    LastModifiedOn: datetime,
    RecommendationRunId: str,
    DataQualitySecurityConfiguration: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityTargetTableTypeDef](./type_defs.md#dataqualitytargettabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationRequestRequestTypeDef

```python
# CreateIntegrationRequestRequestTypeDef definition

class CreateIntegrationRequestRequestTypeDef(TypedDict):
    IntegrationName: str,
    SourceArn: str,
    TargetArn: str,
    Description: NotRequired[str],
    DataFilter: NotRequired[str],
    KmsKeyId: NotRequired[str],
    AdditionalEncryptionContext: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateIntegrationResourcePropertyRequestRequestTypeDef

```python
# CreateIntegrationResourcePropertyRequestRequestTypeDef definition

class CreateIntegrationResourcePropertyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    SourceProcessingProperties: NotRequired[SourceProcessingPropertiesTypeDef],  # (1)
    TargetProcessingProperties: NotRequired[TargetProcessingPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: SourceProcessingPropertiesTypeDef](./type_defs.md#sourceprocessingpropertiestypedef) 
2. See [:material-code-braces: TargetProcessingPropertiesTypeDef](./type_defs.md#targetprocessingpropertiestypedef) 
## CreateIntegrationResourcePropertyResponseTypeDef

```python
# CreateIntegrationResourcePropertyResponseTypeDef definition

class CreateIntegrationResourcePropertyResponseTypeDef(TypedDict):
    ResourceArn: str,
    SourceProcessingProperties: SourceProcessingPropertiesTypeDef,  # (1)
    TargetProcessingProperties: TargetProcessingPropertiesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SourceProcessingPropertiesTypeDef](./type_defs.md#sourceprocessingpropertiestypedef) 
2. See [:material-code-braces: TargetProcessingPropertiesTypeDef](./type_defs.md#targetprocessingpropertiestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIntegrationResourcePropertyResponseTypeDef

```python
# GetIntegrationResourcePropertyResponseTypeDef definition

class GetIntegrationResourcePropertyResponseTypeDef(TypedDict):
    ResourceArn: str,
    SourceProcessingProperties: SourceProcessingPropertiesTypeDef,  # (1)
    TargetProcessingProperties: TargetProcessingPropertiesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SourceProcessingPropertiesTypeDef](./type_defs.md#sourceprocessingpropertiestypedef) 
2. See [:material-code-braces: TargetProcessingPropertiesTypeDef](./type_defs.md#targetprocessingpropertiestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateIntegrationResourcePropertyRequestRequestTypeDef

```python
# UpdateIntegrationResourcePropertyRequestRequestTypeDef definition

class UpdateIntegrationResourcePropertyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    SourceProcessingProperties: NotRequired[SourceProcessingPropertiesTypeDef],  # (1)
    TargetProcessingProperties: NotRequired[TargetProcessingPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: SourceProcessingPropertiesTypeDef](./type_defs.md#sourceprocessingpropertiestypedef) 
2. See [:material-code-braces: TargetProcessingPropertiesTypeDef](./type_defs.md#targetprocessingpropertiestypedef) 
## UpdateIntegrationResourcePropertyResponseTypeDef

```python
# UpdateIntegrationResourcePropertyResponseTypeDef definition

class UpdateIntegrationResourcePropertyResponseTypeDef(TypedDict):
    ResourceArn: str,
    SourceProcessingProperties: SourceProcessingPropertiesTypeDef,  # (1)
    TargetProcessingProperties: TargetProcessingPropertiesTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SourceProcessingPropertiesTypeDef](./type_defs.md#sourceprocessingpropertiestypedef) 
2. See [:material-code-braces: TargetProcessingPropertiesTypeDef](./type_defs.md#targetprocessingpropertiestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationResponseTypeDef

```python
# CreateIntegrationResponseTypeDef definition

class CreateIntegrationResponseTypeDef(TypedDict):
    SourceArn: str,
    TargetArn: str,
    IntegrationName: str,
    Description: str,
    IntegrationArn: str,
    KmsKeyId: str,
    AdditionalEncryptionContext: Dict[str, str],
    Tags: List[TagTypeDef],  # (1)
    Status: IntegrationStatusType,  # (2)
    CreateTime: datetime,
    Errors: List[IntegrationErrorTypeDef],  # (3)
    DataFilter: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
3. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteIntegrationResponseTypeDef

```python
# DeleteIntegrationResponseTypeDef definition

class DeleteIntegrationResponseTypeDef(TypedDict):
    SourceArn: str,
    TargetArn: str,
    IntegrationName: str,
    Description: str,
    IntegrationArn: str,
    KmsKeyId: str,
    AdditionalEncryptionContext: Dict[str, str],
    Tags: List[TagTypeDef],  # (1)
    Status: IntegrationStatusType,  # (2)
    CreateTime: datetime,
    Errors: List[IntegrationErrorTypeDef],  # (3)
    DataFilter: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
3. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## InboundIntegrationTypeDef

```python
# InboundIntegrationTypeDef definition

class InboundIntegrationTypeDef(TypedDict):
    SourceArn: str,
    TargetArn: str,
    IntegrationArn: str,
    Status: IntegrationStatusType,  # (1)
    CreateTime: datetime,
    Errors: NotRequired[List[IntegrationErrorTypeDef]],  # (2)
```

1. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
2. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
## IntegrationTypeDef

```python
# IntegrationTypeDef definition

class IntegrationTypeDef(TypedDict):
    SourceArn: str,
    TargetArn: str,
    IntegrationName: str,
    IntegrationArn: str,
    Status: IntegrationStatusType,  # (2)
    CreateTime: datetime,
    Description: NotRequired[str],
    KmsKeyId: NotRequired[str],
    AdditionalEncryptionContext: NotRequired[Dict[str, str]],
    Tags: NotRequired[List[TagTypeDef]],  # (1)
    Errors: NotRequired[List[IntegrationErrorTypeDef]],  # (3)
    DataFilter: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
3. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
## ModifyIntegrationResponseTypeDef

```python
# ModifyIntegrationResponseTypeDef definition

class ModifyIntegrationResponseTypeDef(TypedDict):
    SourceArn: str,
    TargetArn: str,
    IntegrationName: str,
    Description: str,
    IntegrationArn: str,
    KmsKeyId: str,
    AdditionalEncryptionContext: Dict[str, str],
    Tags: List[TagTypeDef],  # (1)
    Status: IntegrationStatusType,  # (2)
    CreateTime: datetime,
    Errors: List[IntegrationErrorTypeDef],  # (3)
    DataFilter: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: IntegrationStatusType](./literals.md#integrationstatustype) 
3. See [:material-code-braces: IntegrationErrorTypeDef](./type_defs.md#integrationerrortypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePartitionIndexRequestRequestTypeDef

```python
# CreatePartitionIndexRequestRequestTypeDef definition

class CreatePartitionIndexRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionIndex: PartitionIndexTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionIndexTypeDef](./type_defs.md#partitionindextypedef) 
## CreateSchemaInputRequestTypeDef

```python
# CreateSchemaInputRequestTypeDef definition

class CreateSchemaInputRequestTypeDef(TypedDict):
    SchemaName: str,
    DataFormat: DataFormatType,  # (1)
    RegistryId: NotRequired[RegistryIdTypeDef],  # (2)
    Compatibility: NotRequired[CompatibilityType],  # (3)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    SchemaDefinition: NotRequired[str],
```

1. See [:material-code-brackets: DataFormatType](./literals.md#dataformattype) 
2. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
3. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
## DeleteRegistryInputRequestTypeDef

```python
# DeleteRegistryInputRequestTypeDef definition

class DeleteRegistryInputRequestTypeDef(TypedDict):
    RegistryId: RegistryIdTypeDef,  # (1)
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## GetRegistryInputRequestTypeDef

```python
# GetRegistryInputRequestTypeDef definition

class GetRegistryInputRequestTypeDef(TypedDict):
    RegistryId: RegistryIdTypeDef,  # (1)
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## ListSchemasInputRequestTypeDef

```python
# ListSchemasInputRequestTypeDef definition

class ListSchemasInputRequestTypeDef(TypedDict):
    RegistryId: NotRequired[RegistryIdTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## UpdateRegistryInputRequestTypeDef

```python
# UpdateRegistryInputRequestTypeDef definition

class UpdateRegistryInputRequestTypeDef(TypedDict):
    RegistryId: RegistryIdTypeDef,  # (1)
    Description: str,
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
## CreateSessionRequestRequestTypeDef

```python
# CreateSessionRequestRequestTypeDef definition

class CreateSessionRequestRequestTypeDef(TypedDict):
    Id: str,
    Role: str,
    Command: SessionCommandTypeDef,  # (1)
    Description: NotRequired[str],
    Timeout: NotRequired[int],
    IdleTimeout: NotRequired[int],
    DefaultArguments: NotRequired[Mapping[str, str]],
    Connections: NotRequired[ConnectionsListTypeDef],  # (2)
    MaxCapacity: NotRequired[float],
    NumberOfWorkers: NotRequired[int],
    WorkerType: NotRequired[WorkerTypeType],  # (3)
    SecurityConfiguration: NotRequired[str],
    GlueVersion: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    RequestOrigin: NotRequired[str],
```

1. See [:material-code-braces: SessionCommandTypeDef](./type_defs.md#sessioncommandtypedef) 
2. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
3. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    Id: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    Status: NotRequired[SessionStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    Description: NotRequired[str],
    Role: NotRequired[str],
    Command: NotRequired[SessionCommandTypeDef],  # (2)
    DefaultArguments: NotRequired[Dict[str, str]],
    Connections: NotRequired[ConnectionsListOutputTypeDef],  # (3)
    Progress: NotRequired[float],
    MaxCapacity: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    GlueVersion: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    WorkerType: NotRequired[WorkerTypeType],  # (4)
    CompletedOn: NotRequired[datetime],
    ExecutionTime: NotRequired[float],
    DPUSeconds: NotRequired[float],
    IdleTimeout: NotRequired[int],
    ProfileName: NotRequired[str],
```

1. See [:material-code-brackets: SessionStatusType](./literals.md#sessionstatustype) 
2. See [:material-code-braces: SessionCommandTypeDef](./type_defs.md#sessioncommandtypedef) 
3. See [:material-code-braces: ConnectionsListOutputTypeDef](./type_defs.md#connectionslistoutputtypedef) 
4. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## EvaluateDataQualityMultiFrameOutputTypeDef

```python
# EvaluateDataQualityMultiFrameOutputTypeDef definition

class EvaluateDataQualityMultiFrameOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Ruleset: str,
    AdditionalDataSources: NotRequired[Dict[str, str]],
    PublishingOptions: NotRequired[DQResultsPublishingOptionsTypeDef],  # (1)
    AdditionalOptions: NotRequired[Dict[AdditionalOptionKeysType, str]],  # (2)
    StopJobOnFailureOptions: NotRequired[DQStopJobOnFailureOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: DQResultsPublishingOptionsTypeDef](./type_defs.md#dqresultspublishingoptionstypedef) 
2. See [:material-code-brackets: AdditionalOptionKeysType](./literals.md#additionaloptionkeystype) 
3. See [:material-code-braces: DQStopJobOnFailureOptionsTypeDef](./type_defs.md#dqstopjobonfailureoptionstypedef) 
## EvaluateDataQualityMultiFrameTypeDef

```python
# EvaluateDataQualityMultiFrameTypeDef definition

class EvaluateDataQualityMultiFrameTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Ruleset: str,
    AdditionalDataSources: NotRequired[Mapping[str, str]],
    PublishingOptions: NotRequired[DQResultsPublishingOptionsTypeDef],  # (1)
    AdditionalOptions: NotRequired[Mapping[AdditionalOptionKeysType, str]],  # (2)
    StopJobOnFailureOptions: NotRequired[DQStopJobOnFailureOptionsTypeDef],  # (3)
```

1. See [:material-code-braces: DQResultsPublishingOptionsTypeDef](./type_defs.md#dqresultspublishingoptionstypedef) 
2. See [:material-code-brackets: AdditionalOptionKeysType](./literals.md#additionaloptionkeystype) 
3. See [:material-code-braces: DQStopJobOnFailureOptionsTypeDef](./type_defs.md#dqstopjobonfailureoptionstypedef) 
## EvaluateDataQualityOutputTypeDef

```python
# EvaluateDataQualityOutputTypeDef definition

class EvaluateDataQualityOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Ruleset: str,
    Output: NotRequired[DQTransformOutputType],  # (1)
    PublishingOptions: NotRequired[DQResultsPublishingOptionsTypeDef],  # (2)
    StopJobOnFailureOptions: NotRequired[DQStopJobOnFailureOptionsTypeDef],  # (3)
```

1. See [:material-code-brackets: DQTransformOutputType](./literals.md#dqtransformoutputtype) 
2. See [:material-code-braces: DQResultsPublishingOptionsTypeDef](./type_defs.md#dqresultspublishingoptionstypedef) 
3. See [:material-code-braces: DQStopJobOnFailureOptionsTypeDef](./type_defs.md#dqstopjobonfailureoptionstypedef) 
## EvaluateDataQualityTypeDef

```python
# EvaluateDataQualityTypeDef definition

class EvaluateDataQualityTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Ruleset: str,
    Output: NotRequired[DQTransformOutputType],  # (1)
    PublishingOptions: NotRequired[DQResultsPublishingOptionsTypeDef],  # (2)
    StopJobOnFailureOptions: NotRequired[DQStopJobOnFailureOptionsTypeDef],  # (3)
```

1. See [:material-code-brackets: DQTransformOutputType](./literals.md#dqtransformoutputtype) 
2. See [:material-code-braces: DQResultsPublishingOptionsTypeDef](./type_defs.md#dqresultspublishingoptionstypedef) 
3. See [:material-code-braces: DQStopJobOnFailureOptionsTypeDef](./type_defs.md#dqstopjobonfailureoptionstypedef) 
## DataCatalogEncryptionSettingsTypeDef

```python
# DataCatalogEncryptionSettingsTypeDef definition

class DataCatalogEncryptionSettingsTypeDef(TypedDict):
    EncryptionAtRest: NotRequired[EncryptionAtRestTypeDef],  # (1)
    ConnectionPasswordEncryption: NotRequired[ConnectionPasswordEncryptionTypeDef],  # (2)
```

1. See [:material-code-braces: EncryptionAtRestTypeDef](./type_defs.md#encryptionatresttypedef) 
2. See [:material-code-braces: ConnectionPasswordEncryptionTypeDef](./type_defs.md#connectionpasswordencryptiontypedef) 
## PrincipalPermissionsOutputTypeDef

```python
# PrincipalPermissionsOutputTypeDef definition

class PrincipalPermissionsOutputTypeDef(TypedDict):
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Permissions: NotRequired[List[PermissionType]],  # (2)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## PrincipalPermissionsTypeDef

```python
# PrincipalPermissionsTypeDef definition

class PrincipalPermissionsTypeDef(TypedDict):
    Principal: NotRequired[DataLakePrincipalTypeDef],  # (1)
    Permissions: NotRequired[Sequence[PermissionType]],  # (2)
```

1. See [:material-code-braces: DataLakePrincipalTypeDef](./type_defs.md#datalakeprincipaltypedef) 
2. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
## MetricBasedObservationTypeDef

```python
# MetricBasedObservationTypeDef definition

class MetricBasedObservationTypeDef(TypedDict):
    MetricName: NotRequired[str],
    StatisticId: NotRequired[str],
    MetricValues: NotRequired[DataQualityMetricValuesTypeDef],  # (1)
    NewRules: NotRequired[List[str]],
```

1. See [:material-code-braces: DataQualityMetricValuesTypeDef](./type_defs.md#dataqualitymetricvaluestypedef) 
## DataSourceOutputTypeDef

```python
# DataSourceOutputTypeDef definition

class DataSourceOutputTypeDef(TypedDict):
    GlueTable: GlueTableOutputTypeDef,  # (1)
```

1. See [:material-code-braces: GlueTableOutputTypeDef](./type_defs.md#gluetableoutputtypedef) 
## NullValueFieldTypeDef

```python
# NullValueFieldTypeDef definition

class NullValueFieldTypeDef(TypedDict):
    Value: str,
    Datatype: DatatypeTypeDef,  # (1)
```

1. See [:material-code-braces: DatatypeTypeDef](./type_defs.md#datatypetypedef) 
## DecimalColumnStatisticsDataOutputTypeDef

```python
# DecimalColumnStatisticsDataOutputTypeDef definition

class DecimalColumnStatisticsDataOutputTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[DecimalNumberOutputTypeDef],  # (1)
    MaximumValue: NotRequired[DecimalNumberOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DecimalNumberOutputTypeDef](./type_defs.md#decimalnumberoutputtypedef) 
2. See [:material-code-braces: DecimalNumberOutputTypeDef](./type_defs.md#decimalnumberoutputtypedef) 
## DeleteSchemaInputRequestTypeDef

```python
# DeleteSchemaInputRequestTypeDef definition

class DeleteSchemaInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## DeleteSchemaVersionsInputRequestTypeDef

```python
# DeleteSchemaVersionsInputRequestTypeDef definition

class DeleteSchemaVersionsInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    Versions: str,
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## GetSchemaByDefinitionInputRequestTypeDef

```python
# GetSchemaByDefinitionInputRequestTypeDef definition

class GetSchemaByDefinitionInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaDefinition: str,
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## GetSchemaInputRequestTypeDef

```python
# GetSchemaInputRequestTypeDef definition

class GetSchemaInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## ListSchemaVersionsInputRequestTypeDef

```python
# ListSchemaVersionsInputRequestTypeDef definition

class ListSchemaVersionsInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## RegisterSchemaVersionInputRequestTypeDef

```python
# RegisterSchemaVersionInputRequestTypeDef definition

class RegisterSchemaVersionInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaDefinition: str,
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## SchemaReferenceTypeDef

```python
# SchemaReferenceTypeDef definition

class SchemaReferenceTypeDef(TypedDict):
    SchemaId: NotRequired[SchemaIdTypeDef],  # (1)
    SchemaVersionId: NotRequired[str],
    SchemaVersionNumber: NotRequired[int],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
## DescribeEntityRequestPaginateTypeDef

```python
# DescribeEntityRequestPaginateTypeDef definition

class DescribeEntityRequestPaginateTypeDef(TypedDict):
    ConnectionName: str,
    EntityName: str,
    CatalogId: NotRequired[str],
    DataStoreApiVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetClassifiersRequestPaginateTypeDef

```python
# GetClassifiersRequestPaginateTypeDef definition

class GetClassifiersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCrawlerMetricsRequestPaginateTypeDef

```python
# GetCrawlerMetricsRequestPaginateTypeDef definition

class GetCrawlerMetricsRequestPaginateTypeDef(TypedDict):
    CrawlerNameList: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCrawlersRequestPaginateTypeDef

```python
# GetCrawlersRequestPaginateTypeDef definition

class GetCrawlersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDatabasesRequestPaginateTypeDef

```python
# GetDatabasesRequestPaginateTypeDef definition

class GetDatabasesRequestPaginateTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (1)
    AttributesToGet: NotRequired[Sequence[DatabaseAttributesType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
2. See [:material-code-brackets: DatabaseAttributesType](./literals.md#databaseattributestype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetDevEndpointsRequestPaginateTypeDef

```python
# GetDevEndpointsRequestPaginateTypeDef definition

class GetDevEndpointsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetJobRunsRequestPaginateTypeDef

```python
# GetJobRunsRequestPaginateTypeDef definition

class GetJobRunsRequestPaginateTypeDef(TypedDict):
    JobName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetJobsRequestPaginateTypeDef

```python
# GetJobsRequestPaginateTypeDef definition

class GetJobsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetPartitionIndexesRequestPaginateTypeDef

```python
# GetPartitionIndexesRequestPaginateTypeDef definition

class GetPartitionIndexesRequestPaginateTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourcePoliciesRequestPaginateTypeDef

```python
# GetResourcePoliciesRequestPaginateTypeDef definition

class GetResourcePoliciesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetSecurityConfigurationsRequestPaginateTypeDef

```python
# GetSecurityConfigurationsRequestPaginateTypeDef definition

class GetSecurityConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTableVersionsRequestPaginateTypeDef

```python
# GetTableVersionsRequestPaginateTypeDef definition

class GetTableVersionsRequestPaginateTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTablesRequestPaginateTypeDef

```python
# GetTablesRequestPaginateTypeDef definition

class GetTablesRequestPaginateTypeDef(TypedDict):
    DatabaseName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[TimestampTypeDef],
    IncludeStatusDetails: NotRequired[bool],
    AttributesToGet: NotRequired[Sequence[TableAttributesType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TableAttributesType](./literals.md#tableattributestype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetTriggersRequestPaginateTypeDef

```python
# GetTriggersRequestPaginateTypeDef definition

class GetTriggersRequestPaginateTypeDef(TypedDict):
    DependentJobName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetUserDefinedFunctionsRequestPaginateTypeDef

```python
# GetUserDefinedFunctionsRequestPaginateTypeDef definition

class GetUserDefinedFunctionsRequestPaginateTypeDef(TypedDict):
    Pattern: str,
    CatalogId: NotRequired[str],
    DatabaseName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetWorkflowRunsRequestPaginateTypeDef

```python
# GetWorkflowRunsRequestPaginateTypeDef definition

class GetWorkflowRunsRequestPaginateTypeDef(TypedDict):
    Name: str,
    IncludeGraph: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBlueprintsRequestPaginateTypeDef

```python
# ListBlueprintsRequestPaginateTypeDef definition

class ListBlueprintsRequestPaginateTypeDef(TypedDict):
    Tags: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectionTypesRequestPaginateTypeDef

```python
# ListConnectionTypesRequestPaginateTypeDef definition

class ListConnectionTypesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntitiesRequestPaginateTypeDef

```python
# ListEntitiesRequestPaginateTypeDef definition

class ListEntitiesRequestPaginateTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    CatalogId: NotRequired[str],
    ParentEntityName: NotRequired[str],
    DataStoreApiVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestPaginateTypeDef

```python
# ListJobsRequestPaginateTypeDef definition

class ListJobsRequestPaginateTypeDef(TypedDict):
    Tags: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRegistriesInputPaginateTypeDef

```python
# ListRegistriesInputPaginateTypeDef definition

class ListRegistriesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemaVersionsInputPaginateTypeDef

```python
# ListSchemaVersionsInputPaginateTypeDef definition

class ListSchemaVersionsInputPaginateTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSchemasInputPaginateTypeDef

```python
# ListSchemasInputPaginateTypeDef definition

class ListSchemasInputPaginateTypeDef(TypedDict):
    RegistryId: NotRequired[RegistryIdTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RegistryIdTypeDef](./type_defs.md#registryidtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableOptimizerRunsRequestPaginateTypeDef

```python
# ListTableOptimizerRunsRequestPaginateTypeDef definition

class ListTableOptimizerRunsRequestPaginateTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTriggersRequestPaginateTypeDef

```python
# ListTriggersRequestPaginateTypeDef definition

class ListTriggersRequestPaginateTypeDef(TypedDict):
    DependentJobName: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsageProfilesRequestPaginateTypeDef

```python
# ListUsageProfilesRequestPaginateTypeDef definition

class ListUsageProfilesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkflowsRequestPaginateTypeDef

```python
# ListWorkflowsRequestPaginateTypeDef definition

class ListWorkflowsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeEntityResponseTypeDef

```python
# DescribeEntityResponseTypeDef definition

class DescribeEntityResponseTypeDef(TypedDict):
    Fields: List[FieldTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FieldTypeDef](./type_defs.md#fieldtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIntegrationsRequestRequestTypeDef

```python
# DescribeIntegrationsRequestRequestTypeDef definition

class DescribeIntegrationsRequestRequestTypeDef(TypedDict):
    IntegrationIdentifier: NotRequired[str],
    Marker: NotRequired[str],
    MaxRecords: NotRequired[int],
    Filters: NotRequired[Sequence[IntegrationFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: IntegrationFilterTypeDef](./type_defs.md#integrationfiltertypedef) 
## UpdateDevEndpointRequestRequestTypeDef

```python
# UpdateDevEndpointRequestRequestTypeDef definition

class UpdateDevEndpointRequestRequestTypeDef(TypedDict):
    EndpointName: str,
    PublicKey: NotRequired[str],
    AddPublicKeys: NotRequired[Sequence[str]],
    DeletePublicKeys: NotRequired[Sequence[str]],
    CustomLibraries: NotRequired[DevEndpointCustomLibrariesTypeDef],  # (1)
    UpdateEtlLibraries: NotRequired[bool],
    DeleteArguments: NotRequired[Sequence[str]],
    AddArguments: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DevEndpointCustomLibrariesTypeDef](./type_defs.md#devendpointcustomlibrariestypedef) 
## S3DeltaDirectTargetOutputTypeDef

```python
# S3DeltaDirectTargetOutputTypeDef definition

class S3DeltaDirectTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Compression: DeltaTargetCompressionTypeType,  # (1)
    Format: TargetFormatType,  # (2)
    PartitionKeys: NotRequired[List[List[str]]],
    AdditionalOptions: NotRequired[Dict[str, str]],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: DeltaTargetCompressionTypeType](./literals.md#deltatargetcompressiontypetype) 
2. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
3. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3DeltaDirectTargetTypeDef

```python
# S3DeltaDirectTargetTypeDef definition

class S3DeltaDirectTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Path: str,
    Compression: DeltaTargetCompressionTypeType,  # (1)
    Format: TargetFormatType,  # (2)
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    AdditionalOptions: NotRequired[Mapping[str, str]],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: DeltaTargetCompressionTypeType](./literals.md#deltatargetcompressiontypetype) 
2. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
3. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3DirectTargetOutputTypeDef

```python
# S3DirectTargetOutputTypeDef definition

class S3DirectTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Format: TargetFormatType,  # (1)
    PartitionKeys: NotRequired[List[List[str]]],
    Compression: NotRequired[str],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
2. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3DirectTargetTypeDef

```python
# S3DirectTargetTypeDef definition

class S3DirectTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Path: str,
    Format: TargetFormatType,  # (1)
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    Compression: NotRequired[str],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (2)
```

1. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
2. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3GlueParquetTargetOutputTypeDef

```python
# S3GlueParquetTargetOutputTypeDef definition

class S3GlueParquetTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    PartitionKeys: NotRequired[List[List[str]]],
    Compression: NotRequired[ParquetCompressionTypeType],  # (1)
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (2)
```

1. See [:material-code-brackets: ParquetCompressionTypeType](./literals.md#parquetcompressiontypetype) 
2. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3GlueParquetTargetTypeDef

```python
# S3GlueParquetTargetTypeDef definition

class S3GlueParquetTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Path: str,
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    Compression: NotRequired[ParquetCompressionTypeType],  # (1)
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (2)
```

1. See [:material-code-brackets: ParquetCompressionTypeType](./literals.md#parquetcompressiontypetype) 
2. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3HudiDirectTargetOutputTypeDef

```python
# S3HudiDirectTargetOutputTypeDef definition

class S3HudiDirectTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Path: str,
    Compression: HudiTargetCompressionTypeType,  # (1)
    Format: TargetFormatType,  # (2)
    AdditionalOptions: Dict[str, str],
    PartitionKeys: NotRequired[List[List[str]]],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: HudiTargetCompressionTypeType](./literals.md#huditargetcompressiontypetype) 
2. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
3. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## S3HudiDirectTargetTypeDef

```python
# S3HudiDirectTargetTypeDef definition

class S3HudiDirectTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Path: str,
    Compression: HudiTargetCompressionTypeType,  # (1)
    Format: TargetFormatType,  # (2)
    AdditionalOptions: Mapping[str, str],
    PartitionKeys: NotRequired[Sequence[Sequence[str]]],
    SchemaChangePolicy: NotRequired[DirectSchemaChangePolicyTypeDef],  # (3)
```

1. See [:material-code-brackets: HudiTargetCompressionTypeType](./literals.md#huditargetcompressiontypetype) 
2. See [:material-code-brackets: TargetFormatType](./literals.md#targetformattype) 
3. See [:material-code-braces: DirectSchemaChangePolicyTypeDef](./type_defs.md#directschemachangepolicytypedef) 
## EncryptionConfigurationOutputTypeDef

```python
# EncryptionConfigurationOutputTypeDef definition

class EncryptionConfigurationOutputTypeDef(TypedDict):
    S3Encryption: NotRequired[List[S3EncryptionTypeDef]],  # (1)
    CloudWatchEncryption: NotRequired[CloudWatchEncryptionTypeDef],  # (2)
    JobBookmarksEncryption: NotRequired[JobBookmarksEncryptionTypeDef],  # (3)
    DataQualityEncryption: NotRequired[DataQualityEncryptionTypeDef],  # (4)
```

1. See [:material-code-braces: S3EncryptionTypeDef](./type_defs.md#s3encryptiontypedef) 
2. See [:material-code-braces: CloudWatchEncryptionTypeDef](./type_defs.md#cloudwatchencryptiontypedef) 
3. See [:material-code-braces: JobBookmarksEncryptionTypeDef](./type_defs.md#jobbookmarksencryptiontypedef) 
4. See [:material-code-braces: DataQualityEncryptionTypeDef](./type_defs.md#dataqualityencryptiontypedef) 
## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    S3Encryption: NotRequired[Sequence[S3EncryptionTypeDef]],  # (1)
    CloudWatchEncryption: NotRequired[CloudWatchEncryptionTypeDef],  # (2)
    JobBookmarksEncryption: NotRequired[JobBookmarksEncryptionTypeDef],  # (3)
    DataQualityEncryption: NotRequired[DataQualityEncryptionTypeDef],  # (4)
```

1. See [:material-code-braces: S3EncryptionTypeDef](./type_defs.md#s3encryptiontypedef) 
2. See [:material-code-braces: CloudWatchEncryptionTypeDef](./type_defs.md#cloudwatchencryptiontypedef) 
3. See [:material-code-braces: JobBookmarksEncryptionTypeDef](./type_defs.md#jobbookmarksencryptiontypedef) 
4. See [:material-code-braces: DataQualityEncryptionTypeDef](./type_defs.md#dataqualityencryptiontypedef) 
## ListEntitiesResponseTypeDef

```python
# ListEntitiesResponseTypeDef definition

class ListEntitiesResponseTypeDef(TypedDict):
    Entities: List[EntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SchemaVersionErrorItemTypeDef

```python
# SchemaVersionErrorItemTypeDef definition

class SchemaVersionErrorItemTypeDef(TypedDict):
    VersionNumber: NotRequired[int],
    ErrorDetails: NotRequired[ErrorDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: ErrorDetailsTypeDef](./type_defs.md#errordetailstypedef) 
## FilterExpressionOutputTypeDef

```python
# FilterExpressionOutputTypeDef definition

class FilterExpressionOutputTypeDef(TypedDict):
    Operation: FilterOperationType,  # (1)
    Values: List[FilterValueOutputTypeDef],  # (2)
    Negated: NotRequired[bool],
```

1. See [:material-code-brackets: FilterOperationType](./literals.md#filteroperationtype) 
2. See [:material-code-braces: FilterValueOutputTypeDef](./type_defs.md#filtervalueoutputtypedef) 
## TransformParametersTypeDef

```python
# TransformParametersTypeDef definition

class TransformParametersTypeDef(TypedDict):
    TransformType: TransformTypeType,  # (1)
    FindMatchesParameters: NotRequired[FindMatchesParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: TransformTypeType](./literals.md#transformtypetype) 
2. See [:material-code-braces: FindMatchesParametersTypeDef](./type_defs.md#findmatchesparameterstypedef) 
## GetConnectionsRequestPaginateTypeDef

```python
# GetConnectionsRequestPaginateTypeDef definition

class GetConnectionsRequestPaginateTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    Filter: NotRequired[GetConnectionsFilterTypeDef],  # (1)
    HidePassword: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetConnectionsRequestRequestTypeDef

```python
# GetConnectionsRequestRequestTypeDef definition

class GetConnectionsRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    Filter: NotRequired[GetConnectionsFilterTypeDef],  # (1)
    HidePassword: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: GetConnectionsFilterTypeDef](./type_defs.md#getconnectionsfiltertypedef) 
## GetDataQualityModelResultResponseTypeDef

```python
# GetDataQualityModelResultResponseTypeDef definition

class GetDataQualityModelResultResponseTypeDef(TypedDict):
    CompletedOn: datetime,
    Model: List[StatisticModelResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatisticModelResultTypeDef](./type_defs.md#statisticmodelresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobBookmarkResponseTypeDef

```python
# GetJobBookmarkResponseTypeDef definition

class GetJobBookmarkResponseTypeDef(TypedDict):
    JobBookmarkEntry: JobBookmarkEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobBookmarkEntryTypeDef](./type_defs.md#jobbookmarkentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResetJobBookmarkResponseTypeDef

```python
# ResetJobBookmarkResponseTypeDef definition

class ResetJobBookmarkResponseTypeDef(TypedDict):
    JobBookmarkEntry: JobBookmarkEntryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobBookmarkEntryTypeDef](./type_defs.md#jobbookmarkentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransformFilterCriteriaTypeDef

```python
# TransformFilterCriteriaTypeDef definition

class TransformFilterCriteriaTypeDef(TypedDict):
    Name: NotRequired[str],
    TransformType: NotRequired[TransformTypeType],  # (1)
    Status: NotRequired[TransformStatusTypeType],  # (2)
    GlueVersion: NotRequired[str],
    CreatedBefore: NotRequired[TimestampTypeDef],
    CreatedAfter: NotRequired[TimestampTypeDef],
    LastModifiedBefore: NotRequired[TimestampTypeDef],
    LastModifiedAfter: NotRequired[TimestampTypeDef],
    Schema: NotRequired[Sequence[SchemaColumnTypeDef]],  # (3)
```

1. See [:material-code-brackets: TransformTypeType](./literals.md#transformtypetype) 
2. See [:material-code-brackets: TransformStatusTypeType](./literals.md#transformstatustypetype) 
3. See [:material-code-braces: SchemaColumnTypeDef](./type_defs.md#schemacolumntypedef) 
## GetMappingResponseTypeDef

```python
# GetMappingResponseTypeDef definition

class GetMappingResponseTypeDef(TypedDict):
    Mapping: List[MappingEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MappingEntryTypeDef](./type_defs.md#mappingentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartitionsRequestPaginateTypeDef

```python
# GetPartitionsRequestPaginateTypeDef definition

class GetPartitionsRequestPaginateTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    Segment: NotRequired[SegmentTypeDef],  # (1)
    ExcludeColumnSchema: NotRequired[bool],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetPartitionsRequestRequestTypeDef

```python
# GetPartitionsRequestRequestTypeDef definition

class GetPartitionsRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    CatalogId: NotRequired[str],
    Expression: NotRequired[str],
    NextToken: NotRequired[str],
    Segment: NotRequired[SegmentTypeDef],  # (1)
    MaxResults: NotRequired[int],
    ExcludeColumnSchema: NotRequired[bool],
    TransactionId: NotRequired[str],
    QueryAsOfTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
## GetResourcePoliciesResponseTypeDef

```python
# GetResourcePoliciesResponseTypeDef definition

class GetResourcePoliciesResponseTypeDef(TypedDict):
    GetResourcePoliciesResponseList: List[GluePolicyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GluePolicyTypeDef](./type_defs.md#gluepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSchemaVersionInputRequestTypeDef

```python
# GetSchemaVersionInputRequestTypeDef definition

class GetSchemaVersionInputRequestTypeDef(TypedDict):
    SchemaId: NotRequired[SchemaIdTypeDef],  # (1)
    SchemaVersionId: NotRequired[str],
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (2)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
## GetSchemaVersionsDiffInputRequestTypeDef

```python
# GetSchemaVersionsDiffInputRequestTypeDef definition

class GetSchemaVersionsDiffInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    FirstSchemaVersionNumber: SchemaVersionNumberTypeDef,  # (2)
    SecondSchemaVersionNumber: SchemaVersionNumberTypeDef,  # (2)
    SchemaDiffType: SchemaDiffTypeType,  # (4)
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
4. See [:material-code-brackets: SchemaDiffTypeType](./literals.md#schemadifftypetype) 
## UpdateSchemaInputRequestTypeDef

```python
# UpdateSchemaInputRequestTypeDef definition

class UpdateSchemaInputRequestTypeDef(TypedDict):
    SchemaId: SchemaIdTypeDef,  # (1)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (2)
    Compatibility: NotRequired[CompatibilityType],  # (3)
    Description: NotRequired[str],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-brackets: CompatibilityType](./literals.md#compatibilitytype) 
## GlueSchemaOutputTypeDef

```python
# GlueSchemaOutputTypeDef definition

class GlueSchemaOutputTypeDef(TypedDict):
    Columns: NotRequired[List[GlueStudioSchemaColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueStudioSchemaColumnTypeDef](./type_defs.md#gluestudioschemacolumntypedef) 
## GlueSchemaTypeDef

```python
# GlueSchemaTypeDef definition

class GlueSchemaTypeDef(TypedDict):
    Columns: NotRequired[Sequence[GlueStudioSchemaColumnTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueStudioSchemaColumnTypeDef](./type_defs.md#gluestudioschemacolumntypedef) 
## GovernedCatalogSourceTypeDef

```python
# GovernedCatalogSourceTypeDef definition

class GovernedCatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    PartitionPredicate: NotRequired[str],
    AdditionalOptions: NotRequired[S3SourceAdditionalOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: S3SourceAdditionalOptionsTypeDef](./type_defs.md#s3sourceadditionaloptionstypedef) 
## S3CatalogSourceTypeDef

```python
# S3CatalogSourceTypeDef definition

class S3CatalogSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    PartitionPredicate: NotRequired[str],
    AdditionalOptions: NotRequired[S3SourceAdditionalOptionsTypeDef],  # (1)
```

1. See [:material-code-braces: S3SourceAdditionalOptionsTypeDef](./type_defs.md#s3sourceadditionaloptionstypedef) 
## OpenTableFormatInputTypeDef

```python
# OpenTableFormatInputTypeDef definition

class OpenTableFormatInputTypeDef(TypedDict):
    IcebergInput: NotRequired[IcebergInputTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergInputTypeDef](./type_defs.md#iceberginputtypedef) 
## OrphanFileDeletionConfigurationTypeDef

```python
# OrphanFileDeletionConfigurationTypeDef definition

class OrphanFileDeletionConfigurationTypeDef(TypedDict):
    icebergConfiguration: NotRequired[IcebergOrphanFileDeletionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergOrphanFileDeletionConfigurationTypeDef](./type_defs.md#icebergorphanfiledeletionconfigurationtypedef) 
## OrphanFileDeletionMetricsTypeDef

```python
# OrphanFileDeletionMetricsTypeDef definition

class OrphanFileDeletionMetricsTypeDef(TypedDict):
    IcebergMetrics: NotRequired[IcebergOrphanFileDeletionMetricsTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergOrphanFileDeletionMetricsTypeDef](./type_defs.md#icebergorphanfiledeletionmetricstypedef) 
## RetentionConfigurationTypeDef

```python
# RetentionConfigurationTypeDef definition

class RetentionConfigurationTypeDef(TypedDict):
    icebergConfiguration: NotRequired[IcebergRetentionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergRetentionConfigurationTypeDef](./type_defs.md#icebergretentionconfigurationtypedef) 
## RetentionMetricsTypeDef

```python
# RetentionMetricsTypeDef definition

class RetentionMetricsTypeDef(TypedDict):
    IcebergMetrics: NotRequired[IcebergRetentionMetricsTypeDef],  # (1)
```

1. See [:material-code-braces: IcebergRetentionMetricsTypeDef](./type_defs.md#icebergretentionmetricstypedef) 
## TargetTableConfigOutputTypeDef

```python
# TargetTableConfigOutputTypeDef definition

class TargetTableConfigOutputTypeDef(TypedDict):
    UnnestSpec: NotRequired[UnnestSpecType],  # (1)
    PartitionSpec: NotRequired[List[IntegrationPartitionTypeDef]],  # (2)
    TargetTableName: NotRequired[str],
```

1. See [:material-code-brackets: UnnestSpecType](./literals.md#unnestspectype) 
2. See [:material-code-braces: IntegrationPartitionTypeDef](./type_defs.md#integrationpartitiontypedef) 
## TargetTableConfigTypeDef

```python
# TargetTableConfigTypeDef definition

class TargetTableConfigTypeDef(TypedDict):
    UnnestSpec: NotRequired[UnnestSpecType],  # (1)
    PartitionSpec: NotRequired[Sequence[IntegrationPartitionTypeDef]],  # (2)
    TargetTableName: NotRequired[str],
```

1. See [:material-code-brackets: UnnestSpecType](./literals.md#unnestspectype) 
2. See [:material-code-braces: IntegrationPartitionTypeDef](./type_defs.md#integrationpartitiontypedef) 
## JobRunTypeDef

```python
# JobRunTypeDef definition

class JobRunTypeDef(TypedDict):
    Id: NotRequired[str],
    Attempt: NotRequired[int],
    PreviousRunId: NotRequired[str],
    TriggerName: NotRequired[str],
    JobName: NotRequired[str],
    JobMode: NotRequired[JobModeType],  # (1)
    JobRunQueuingEnabled: NotRequired[bool],
    StartedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    JobRunState: NotRequired[JobRunStateType],  # (2)
    Arguments: NotRequired[Dict[str, str]],
    ErrorMessage: NotRequired[str],
    PredecessorRuns: NotRequired[List[PredecessorTypeDef]],  # (3)
    AllocatedCapacity: NotRequired[int],
    ExecutionTime: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (4)
    NumberOfWorkers: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    LogGroupName: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (5)
    GlueVersion: NotRequired[str],
    DPUSeconds: NotRequired[float],
    ExecutionClass: NotRequired[ExecutionClassType],  # (6)
    MaintenanceWindow: NotRequired[str],
    ProfileName: NotRequired[str],
    StateDetail: NotRequired[str],
```

1. See [:material-code-brackets: JobModeType](./literals.md#jobmodetype) 
2. See [:material-code-brackets: JobRunStateType](./literals.md#jobrunstatetype) 
3. See [:material-code-braces: PredecessorTypeDef](./type_defs.md#predecessortypedef) 
4. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
5. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
6. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
## JoinOutputTypeDef

```python
# JoinOutputTypeDef definition

class JoinOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    JoinType: JoinTypeType,  # (1)
    Columns: List[JoinColumnOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: JoinTypeType](./literals.md#jointypetype) 
2. See [:material-code-braces: JoinColumnOutputTypeDef](./type_defs.md#joincolumnoutputtypedef) 
## TaskRunPropertiesTypeDef

```python
# TaskRunPropertiesTypeDef definition

class TaskRunPropertiesTypeDef(TypedDict):
    TaskType: NotRequired[TaskTypeType],  # (1)
    ImportLabelsTaskRunProperties: NotRequired[ImportLabelsTaskRunPropertiesTypeDef],  # (2)
    ExportLabelsTaskRunProperties: NotRequired[ExportLabelsTaskRunPropertiesTypeDef],  # (3)
    LabelingSetGenerationTaskRunProperties: NotRequired[LabelingSetGenerationTaskRunPropertiesTypeDef],  # (4)
    FindMatchesTaskRunProperties: NotRequired[FindMatchesTaskRunPropertiesTypeDef],  # (5)
```

1. See [:material-code-brackets: TaskTypeType](./literals.md#tasktypetype) 
2. See [:material-code-braces: ImportLabelsTaskRunPropertiesTypeDef](./type_defs.md#importlabelstaskrunpropertiestypedef) 
3. See [:material-code-braces: ExportLabelsTaskRunPropertiesTypeDef](./type_defs.md#exportlabelstaskrunpropertiestypedef) 
4. See [:material-code-braces: LabelingSetGenerationTaskRunPropertiesTypeDef](./type_defs.md#labelingsetgenerationtaskrunpropertiestypedef) 
5. See [:material-code-braces: FindMatchesTaskRunPropertiesTypeDef](./type_defs.md#findmatchestaskrunpropertiestypedef) 
## ListRegistriesResponseTypeDef

```python
# ListRegistriesResponseTypeDef definition

class ListRegistriesResponseTypeDef(TypedDict):
    Registries: List[RegistryListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RegistryListItemTypeDef](./type_defs.md#registrylistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemaVersionsResponseTypeDef

```python
# ListSchemaVersionsResponseTypeDef definition

class ListSchemaVersionsResponseTypeDef(TypedDict):
    Schemas: List[SchemaVersionListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaVersionListItemTypeDef](./type_defs.md#schemaversionlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSchemasResponseTypeDef

```python
# ListSchemasResponseTypeDef definition

class ListSchemasResponseTypeDef(TypedDict):
    Schemas: List[SchemaListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaListItemTypeDef](./type_defs.md#schemalistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsageProfilesResponseTypeDef

```python
# ListUsageProfilesResponseTypeDef definition

class ListUsageProfilesResponseTypeDef(TypedDict):
    Profiles: List[UsageProfileDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UsageProfileDefinitionTypeDef](./type_defs.md#usageprofiledefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransformEncryptionTypeDef

```python
# TransformEncryptionTypeDef definition

class TransformEncryptionTypeDef(TypedDict):
    MlUserDataEncryption: NotRequired[MLUserDataEncryptionTypeDef],  # (1)
    TaskRunSecurityConfigurationName: NotRequired[str],
```

1. See [:material-code-braces: MLUserDataEncryptionTypeDef](./type_defs.md#mluserdataencryptiontypedef) 
## MetadataInfoTypeDef

```python
# MetadataInfoTypeDef definition

class MetadataInfoTypeDef(TypedDict):
    MetadataValue: NotRequired[str],
    CreatedTime: NotRequired[str],
    OtherMetadataValueList: NotRequired[List[OtherMetadataValueListItemTypeDef]],  # (1)
```

1. See [:material-code-braces: OtherMetadataValueListItemTypeDef](./type_defs.md#othermetadatavaluelistitemtypedef) 
## PutSchemaVersionMetadataInputRequestTypeDef

```python
# PutSchemaVersionMetadataInputRequestTypeDef definition

class PutSchemaVersionMetadataInputRequestTypeDef(TypedDict):
    MetadataKeyValue: MetadataKeyValuePairTypeDef,  # (1)
    SchemaId: NotRequired[SchemaIdTypeDef],  # (2)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (3)
    SchemaVersionId: NotRequired[str],
```

1. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
2. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
## QuerySchemaVersionMetadataInputRequestTypeDef

```python
# QuerySchemaVersionMetadataInputRequestTypeDef definition

class QuerySchemaVersionMetadataInputRequestTypeDef(TypedDict):
    SchemaId: NotRequired[SchemaIdTypeDef],  # (1)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (2)
    SchemaVersionId: NotRequired[str],
    MetadataList: NotRequired[Sequence[MetadataKeyValuePairTypeDef]],  # (3)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
2. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
3. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
## RemoveSchemaVersionMetadataInputRequestTypeDef

```python
# RemoveSchemaVersionMetadataInputRequestTypeDef definition

class RemoveSchemaVersionMetadataInputRequestTypeDef(TypedDict):
    MetadataKeyValue: MetadataKeyValuePairTypeDef,  # (1)
    SchemaId: NotRequired[SchemaIdTypeDef],  # (2)
    SchemaVersionNumber: NotRequired[SchemaVersionNumberTypeDef],  # (3)
    SchemaVersionId: NotRequired[str],
```

1. See [:material-code-braces: MetadataKeyValuePairTypeDef](./type_defs.md#metadatakeyvaluepairtypedef) 
2. See [:material-code-braces: SchemaIdTypeDef](./type_defs.md#schemaidtypedef) 
3. See [:material-code-braces: SchemaVersionNumberTypeDef](./type_defs.md#schemaversionnumbertypedef) 
## OAuth2PropertiesTypeDef

```python
# OAuth2PropertiesTypeDef definition

class OAuth2PropertiesTypeDef(TypedDict):
    OAuth2GrantType: NotRequired[OAuth2GrantTypeType],  # (1)
    OAuth2ClientApplication: NotRequired[OAuth2ClientApplicationTypeDef],  # (2)
    TokenUrl: NotRequired[str],
    TokenUrlParametersMap: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: OAuth2GrantTypeType](./literals.md#oauth2granttypetype) 
2. See [:material-code-braces: OAuth2ClientApplicationTypeDef](./type_defs.md#oauth2clientapplicationtypedef) 
## OAuth2PropertiesInputTypeDef

```python
# OAuth2PropertiesInputTypeDef definition

class OAuth2PropertiesInputTypeDef(TypedDict):
    OAuth2GrantType: NotRequired[OAuth2GrantTypeType],  # (1)
    OAuth2ClientApplication: NotRequired[OAuth2ClientApplicationTypeDef],  # (2)
    TokenUrl: NotRequired[str],
    TokenUrlParametersMap: NotRequired[Mapping[str, str]],
    AuthorizationCodeProperties: NotRequired[AuthorizationCodePropertiesTypeDef],  # (3)
    OAuth2Credentials: NotRequired[OAuth2CredentialsTypeDef],  # (4)
```

1. See [:material-code-brackets: OAuth2GrantTypeType](./literals.md#oauth2granttypetype) 
2. See [:material-code-braces: OAuth2ClientApplicationTypeDef](./type_defs.md#oauth2clientapplicationtypedef) 
3. See [:material-code-braces: AuthorizationCodePropertiesTypeDef](./type_defs.md#authorizationcodepropertiestypedef) 
4. See [:material-code-braces: OAuth2CredentialsTypeDef](./type_defs.md#oauth2credentialstypedef) 
## RecipeStepOutputTypeDef

```python
# RecipeStepOutputTypeDef definition

class RecipeStepOutputTypeDef(TypedDict):
    Action: RecipeActionOutputTypeDef,  # (1)
    ConditionExpressions: NotRequired[List[ConditionExpressionTypeDef]],  # (2)
```

1. See [:material-code-braces: RecipeActionOutputTypeDef](./type_defs.md#recipeactionoutputtypedef) 
2. See [:material-code-braces: ConditionExpressionTypeDef](./type_defs.md#conditionexpressiontypedef) 
## RedshiftTargetOutputTypeDef

```python
# RedshiftTargetOutputTypeDef definition

class RedshiftTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Database: str,
    Table: str,
    RedshiftTmpDir: NotRequired[str],
    TmpDirIAMRole: NotRequired[str],
    UpsertRedshiftOptions: NotRequired[UpsertRedshiftTargetOptionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: UpsertRedshiftTargetOptionsOutputTypeDef](./type_defs.md#upsertredshifttargetoptionsoutputtypedef) 
## UserDefinedFunctionInputTypeDef

```python
# UserDefinedFunctionInputTypeDef definition

class UserDefinedFunctionInputTypeDef(TypedDict):
    FunctionName: NotRequired[str],
    ClassName: NotRequired[str],
    OwnerName: NotRequired[str],
    OwnerType: NotRequired[PrincipalTypeType],  # (1)
    ResourceUris: NotRequired[Sequence[ResourceUriTypeDef]],  # (2)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ResourceUriTypeDef](./type_defs.md#resourceuritypedef) 
## UserDefinedFunctionTypeDef

```python
# UserDefinedFunctionTypeDef definition

class UserDefinedFunctionTypeDef(TypedDict):
    FunctionName: NotRequired[str],
    DatabaseName: NotRequired[str],
    ClassName: NotRequired[str],
    OwnerName: NotRequired[str],
    OwnerType: NotRequired[PrincipalTypeType],  # (1)
    CreateTime: NotRequired[datetime],
    ResourceUris: NotRequired[List[ResourceUriTypeDef]],  # (2)
    CatalogId: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-braces: ResourceUriTypeDef](./type_defs.md#resourceuritypedef) 
## SearchTablesRequestRequestTypeDef

```python
# SearchTablesRequestRequestTypeDef definition

class SearchTablesRequestRequestTypeDef(TypedDict):
    CatalogId: NotRequired[str],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[PropertyPredicateTypeDef]],  # (1)
    SearchText: NotRequired[str],
    SortCriteria: NotRequired[Sequence[SortCriterionTypeDef]],  # (2)
    MaxResults: NotRequired[int],
    ResourceShareType: NotRequired[ResourceShareTypeType],  # (3)
    IncludeStatusDetails: NotRequired[bool],
```

1. See [:material-code-braces: PropertyPredicateTypeDef](./type_defs.md#propertypredicatetypedef) 
2. See [:material-code-braces: SortCriterionTypeDef](./type_defs.md#sortcriteriontypedef) 
3. See [:material-code-brackets: ResourceShareTypeType](./literals.md#resourcesharetypetype) 
## StatementOutputTypeDef

```python
# StatementOutputTypeDef definition

class StatementOutputTypeDef(TypedDict):
    Data: NotRequired[StatementOutputDataTypeDef],  # (1)
    ExecutionCount: NotRequired[int],
    Status: NotRequired[StatementStateType],  # (2)
    ErrorName: NotRequired[str],
    ErrorValue: NotRequired[str],
    Traceback: NotRequired[List[str]],
```

1. See [:material-code-braces: StatementOutputDataTypeDef](./type_defs.md#statementoutputdatatypedef) 
2. See [:material-code-brackets: StatementStateType](./literals.md#statementstatetype) 
## StatisticAnnotationTypeDef

```python
# StatisticAnnotationTypeDef definition

class StatisticAnnotationTypeDef(TypedDict):
    ProfileId: NotRequired[str],
    StatisticId: NotRequired[str],
    StatisticRecordedOn: NotRequired[datetime],
    InclusionAnnotation: NotRequired[TimestampedInclusionAnnotationTypeDef],  # (1)
```

1. See [:material-code-braces: TimestampedInclusionAnnotationTypeDef](./type_defs.md#timestampedinclusionannotationtypedef) 
## StatisticSummaryTypeDef

```python
# StatisticSummaryTypeDef definition

class StatisticSummaryTypeDef(TypedDict):
    StatisticId: NotRequired[str],
    ProfileId: NotRequired[str],
    RunIdentifier: NotRequired[RunIdentifierTypeDef],  # (1)
    StatisticName: NotRequired[str],
    DoubleValue: NotRequired[float],
    EvaluationLevel: NotRequired[StatisticEvaluationLevelType],  # (2)
    ColumnsReferenced: NotRequired[List[str]],
    ReferencedDatasets: NotRequired[List[str]],
    StatisticProperties: NotRequired[Dict[str, str]],
    RecordedOn: NotRequired[datetime],
    InclusionAnnotation: NotRequired[TimestampedInclusionAnnotationTypeDef],  # (3)
```

1. See [:material-code-braces: RunIdentifierTypeDef](./type_defs.md#runidentifiertypedef) 
2. See [:material-code-brackets: StatisticEvaluationLevelType](./literals.md#statisticevaluationleveltype) 
3. See [:material-code-braces: TimestampedInclusionAnnotationTypeDef](./type_defs.md#timestampedinclusionannotationtypedef) 
## UpdateClassifierRequestRequestTypeDef

```python
# UpdateClassifierRequestRequestTypeDef definition

class UpdateClassifierRequestRequestTypeDef(TypedDict):
    GrokClassifier: NotRequired[UpdateGrokClassifierRequestTypeDef],  # (1)
    XMLClassifier: NotRequired[UpdateXMLClassifierRequestTypeDef],  # (2)
    JsonClassifier: NotRequired[UpdateJsonClassifierRequestTypeDef],  # (3)
    CsvClassifier: NotRequired[UpdateCsvClassifierRequestTypeDef],  # (4)
```

1. See [:material-code-braces: UpdateGrokClassifierRequestTypeDef](./type_defs.md#updategrokclassifierrequesttypedef) 
2. See [:material-code-braces: UpdateXMLClassifierRequestTypeDef](./type_defs.md#updatexmlclassifierrequesttypedef) 
3. See [:material-code-braces: UpdateJsonClassifierRequestTypeDef](./type_defs.md#updatejsonclassifierrequesttypedef) 
4. See [:material-code-braces: UpdateCsvClassifierRequestTypeDef](./type_defs.md#updatecsvclassifierrequesttypedef) 
## ViewDefinitionInputTypeDef

```python
# ViewDefinitionInputTypeDef definition

class ViewDefinitionInputTypeDef(TypedDict):
    IsProtected: NotRequired[bool],
    Definer: NotRequired[str],
    Representations: NotRequired[Sequence[ViewRepresentationInputTypeDef]],  # (1)
    SubObjects: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ViewRepresentationInputTypeDef](./type_defs.md#viewrepresentationinputtypedef) 
## ViewDefinitionTypeDef

```python
# ViewDefinitionTypeDef definition

class ViewDefinitionTypeDef(TypedDict):
    IsProtected: NotRequired[bool],
    Definer: NotRequired[str],
    SubObjects: NotRequired[List[str]],
    Representations: NotRequired[List[ViewRepresentationTypeDef]],  # (1)
```

1. See [:material-code-braces: ViewRepresentationTypeDef](./type_defs.md#viewrepresentationtypedef) 
## AggregateTypeDef

```python
# AggregateTypeDef definition

class AggregateTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Groups: Sequence[Sequence[str]],
    Aggs: Sequence[AggregateOperationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AggregateOperationTypeDef](./type_defs.md#aggregateoperationtypedef) [:material-code-braces: AggregateOperationOutputTypeDef](./type_defs.md#aggregateoperationoutputtypedef) 
## AuthConfigurationTypeDef

```python
# AuthConfigurationTypeDef definition

class AuthConfigurationTypeDef(TypedDict):
    AuthenticationType: PropertyTypeDef,  # (1)
    SecretArn: NotRequired[PropertyTypeDef],  # (1)
    OAuth2Properties: NotRequired[Dict[str, PropertyTypeDef]],  # (3)
    BasicAuthenticationProperties: NotRequired[Dict[str, PropertyTypeDef]],  # (3)
    CustomAuthenticationProperties: NotRequired[Dict[str, PropertyTypeDef]],  # (3)
```

1. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
2. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
3. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
4. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
5. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
## ComputeEnvironmentConfigurationTypeDef

```python
# ComputeEnvironmentConfigurationTypeDef definition

class ComputeEnvironmentConfigurationTypeDef(TypedDict):
    Name: str,
    Description: str,
    ComputeEnvironment: ComputeEnvironmentType,  # (1)
    SupportedAuthenticationTypes: List[AuthenticationTypeType],  # (2)
    ConnectionOptions: Dict[str, PropertyTypeDef],  # (3)
    ConnectionPropertyNameOverrides: Dict[str, str],
    ConnectionOptionNameOverrides: Dict[str, str],
    ConnectionPropertiesRequiredOverrides: List[str],
    PhysicalConnectionPropertiesRequired: NotRequired[bool],
```

1. See [:material-code-brackets: ComputeEnvironmentType](./literals.md#computeenvironmenttype) 
2. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
3. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
## AmazonRedshiftSourceOutputTypeDef

```python
# AmazonRedshiftSourceOutputTypeDef definition

class AmazonRedshiftSourceOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    Data: NotRequired[AmazonRedshiftNodeDataOutputTypeDef],  # (1)
```

1. See [:material-code-braces: AmazonRedshiftNodeDataOutputTypeDef](./type_defs.md#amazonredshiftnodedataoutputtypedef) 
## AmazonRedshiftTargetOutputTypeDef

```python
# AmazonRedshiftTargetOutputTypeDef definition

class AmazonRedshiftTargetOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    Data: NotRequired[AmazonRedshiftNodeDataOutputTypeDef],  # (1)
    Inputs: NotRequired[List[str]],
```

1. See [:material-code-braces: AmazonRedshiftNodeDataOutputTypeDef](./type_defs.md#amazonredshiftnodedataoutputtypedef) 
## SnowflakeTargetOutputTypeDef

```python
# SnowflakeTargetOutputTypeDef definition

class SnowflakeTargetOutputTypeDef(TypedDict):
    Name: str,
    Data: SnowflakeNodeDataOutputTypeDef,  # (1)
    Inputs: NotRequired[List[str]],
```

1. See [:material-code-braces: SnowflakeNodeDataOutputTypeDef](./type_defs.md#snowflakenodedataoutputtypedef) 
## PartitionIndexDescriptorTypeDef

```python
# PartitionIndexDescriptorTypeDef definition

class PartitionIndexDescriptorTypeDef(TypedDict):
    IndexName: str,
    Keys: List[KeySchemaElementTypeDef],  # (1)
    IndexStatus: PartitionIndexStatusType,  # (2)
    BackfillErrors: NotRequired[List[BackfillErrorTypeDef]],  # (3)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-brackets: PartitionIndexStatusType](./literals.md#partitionindexstatustype) 
3. See [:material-code-braces: BackfillErrorTypeDef](./type_defs.md#backfillerrortypedef) 
## BatchStopJobRunResponseTypeDef

```python
# BatchStopJobRunResponseTypeDef definition

class BatchStopJobRunResponseTypeDef(TypedDict):
    SuccessfulSubmissions: List[BatchStopJobRunSuccessfulSubmissionTypeDef],  # (1)
    Errors: List[BatchStopJobRunErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchStopJobRunSuccessfulSubmissionTypeDef](./type_defs.md#batchstopjobrunsuccessfulsubmissiontypedef) 
2. See [:material-code-braces: BatchStopJobRunErrorTypeDef](./type_defs.md#batchstopjobrunerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdatePartitionResponseTypeDef

```python
# BatchUpdatePartitionResponseTypeDef definition

class BatchUpdatePartitionResponseTypeDef(TypedDict):
    Errors: List[BatchUpdatePartitionFailureEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchUpdatePartitionFailureEntryTypeDef](./type_defs.md#batchupdatepartitionfailureentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreatePartitionResponseTypeDef

```python
# BatchCreatePartitionResponseTypeDef definition

class BatchCreatePartitionResponseTypeDef(TypedDict):
    Errors: List[PartitionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionErrorTypeDef](./type_defs.md#partitionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeletePartitionResponseTypeDef

```python
# BatchDeletePartitionResponseTypeDef definition

class BatchDeletePartitionResponseTypeDef(TypedDict):
    Errors: List[PartitionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionErrorTypeDef](./type_defs.md#partitionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteTableResponseTypeDef

```python
# BatchDeleteTableResponseTypeDef definition

class BatchDeleteTableResponseTypeDef(TypedDict):
    Errors: List[TableErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableErrorTypeDef](./type_defs.md#tableerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteTableVersionResponseTypeDef

```python
# BatchDeleteTableVersionResponseTypeDef definition

class BatchDeleteTableVersionResponseTypeDef(TypedDict):
    Errors: List[TableVersionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableVersionErrorTypeDef](./type_defs.md#tableversionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StatusDetailsPaginatorTypeDef

```python
# StatusDetailsPaginatorTypeDef definition

class StatusDetailsPaginatorTypeDef(TypedDict):
    RequestedChange: NotRequired[Dict[str, Any]],
    ViewValidations: NotRequired[List[ViewValidationTypeDef]],  # (1)
```

1. See [:material-code-braces: ViewValidationTypeDef](./type_defs.md#viewvalidationtypedef) 
## StatusDetailsTypeDef

```python
# StatusDetailsTypeDef definition

class StatusDetailsTypeDef(TypedDict):
    RequestedChange: NotRequired[Dict[str, Any]],
    ViewValidations: NotRequired[List[ViewValidationTypeDef]],  # (1)
```

1. See [:material-code-braces: ViewValidationTypeDef](./type_defs.md#viewvalidationtypedef) 
## BatchDeletePartitionRequestRequestTypeDef

```python
# BatchDeletePartitionRequestRequestTypeDef definition

class BatchDeletePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionsToDelete: Sequence[PartitionValueListUnionTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionValueListTypeDef](./type_defs.md#partitionvaluelisttypedef) [:material-code-braces: PartitionValueListOutputTypeDef](./type_defs.md#partitionvaluelistoutputtypedef) 
## BatchGetBlueprintsResponseTypeDef

```python
# BatchGetBlueprintsResponseTypeDef definition

class BatchGetBlueprintsResponseTypeDef(TypedDict):
    Blueprints: List[BlueprintTypeDef],  # (1)
    MissingBlueprints: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintTypeDef](./type_defs.md#blueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBlueprintResponseTypeDef

```python
# GetBlueprintResponseTypeDef definition

class GetBlueprintResponseTypeDef(TypedDict):
    Blueprint: BlueprintTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BlueprintTypeDef](./type_defs.md#blueprinttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConnectionTypesResponseTypeDef

```python
# ListConnectionTypesResponseTypeDef definition

class ListConnectionTypesResponseTypeDef(TypedDict):
    ConnectionTypes: List[ConnectionTypeBriefTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectionTypeBriefTypeDef](./type_defs.md#connectiontypebrieftypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClassifierResponseTypeDef

```python
# GetClassifierResponseTypeDef definition

class GetClassifierResponseTypeDef(TypedDict):
    Classifier: ClassifierTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ClassifierTypeDef](./type_defs.md#classifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetClassifiersResponseTypeDef

```python
# GetClassifiersResponseTypeDef definition

class GetClassifiersResponseTypeDef(TypedDict):
    Classifiers: List[ClassifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ClassifierTypeDef](./type_defs.md#classifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataflowGraphResponseTypeDef

```python
# GetDataflowGraphResponseTypeDef definition

class GetDataflowGraphResponseTypeDef(TypedDict):
    DagNodes: List[CodeGenNodeOutputTypeDef],  # (1)
    DagEdges: List[CodeGenEdgeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CodeGenNodeOutputTypeDef](./type_defs.md#codegennodeoutputtypedef) 
2. See [:material-code-braces: CodeGenEdgeTypeDef](./type_defs.md#codegenedgetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMappingRequestRequestTypeDef

```python
# GetMappingRequestRequestTypeDef definition

class GetMappingRequestRequestTypeDef(TypedDict):
    Source: CatalogEntryTypeDef,  # (1)
    Sinks: NotRequired[Sequence[CatalogEntryTypeDef]],  # (2)
    Location: NotRequired[LocationTypeDef],  # (3)
```

1. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
2. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
3. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
## GetPlanRequestRequestTypeDef

```python
# GetPlanRequestRequestTypeDef definition

class GetPlanRequestRequestTypeDef(TypedDict):
    Mapping: Sequence[MappingEntryTypeDef],  # (1)
    Source: CatalogEntryTypeDef,  # (2)
    Sinks: NotRequired[Sequence[CatalogEntryTypeDef]],  # (3)
    Location: NotRequired[LocationTypeDef],  # (4)
    Language: NotRequired[LanguageType],  # (5)
    AdditionalPlanOptionsMap: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: MappingEntryTypeDef](./type_defs.md#mappingentrytypedef) 
2. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
3. See [:material-code-braces: CatalogEntryTypeDef](./type_defs.md#catalogentrytypedef) 
4. See [:material-code-braces: LocationTypeDef](./type_defs.md#locationtypedef) 
5. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
## GetColumnStatisticsTaskSettingsResponseTypeDef

```python
# GetColumnStatisticsTaskSettingsResponseTypeDef definition

class GetColumnStatisticsTaskSettingsResponseTypeDef(TypedDict):
    ColumnStatisticsTaskSettings: ColumnStatisticsTaskSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnStatisticsTaskSettingsTypeDef](./type_defs.md#columnstatisticstasksettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUnfilteredPartitionMetadataRequestRequestTypeDef

```python
# GetUnfilteredPartitionMetadataRequestRequestTypeDef definition

class GetUnfilteredPartitionMetadataRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    Region: NotRequired[str],
    AuditContext: NotRequired[AuditContextTypeDef],  # (2)
    QuerySessionContext: NotRequired[QuerySessionContextTypeDef],  # (3)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
## GetUnfilteredPartitionsMetadataRequestRequestTypeDef

```python
# GetUnfilteredPartitionsMetadataRequestRequestTypeDef definition

class GetUnfilteredPartitionsMetadataRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    Region: NotRequired[str],
    Expression: NotRequired[str],
    AuditContext: NotRequired[AuditContextTypeDef],  # (2)
    NextToken: NotRequired[str],
    Segment: NotRequired[SegmentTypeDef],  # (3)
    MaxResults: NotRequired[int],
    QuerySessionContext: NotRequired[QuerySessionContextTypeDef],  # (4)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-braces: SegmentTypeDef](./type_defs.md#segmenttypedef) 
4. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
## GetUnfilteredTableMetadataRequestRequestTypeDef

```python
# GetUnfilteredTableMetadataRequestRequestTypeDef definition

class GetUnfilteredTableMetadataRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    Name: str,
    SupportedPermissionTypes: Sequence[PermissionTypeType],  # (1)
    Region: NotRequired[str],
    AuditContext: NotRequired[AuditContextTypeDef],  # (2)
    ParentResourceArn: NotRequired[str],
    RootResourceArn: NotRequired[str],
    SupportedDialect: NotRequired[SupportedDialectTypeDef],  # (3)
    Permissions: NotRequired[Sequence[PermissionType]],  # (4)
    QuerySessionContext: NotRequired[QuerySessionContextTypeDef],  # (5)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-braces: AuditContextTypeDef](./type_defs.md#auditcontexttypedef) 
3. See [:material-code-braces: SupportedDialectTypeDef](./type_defs.md#supporteddialecttypedef) 
4. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
5. See [:material-code-braces: QuerySessionContextTypeDef](./type_defs.md#querysessioncontexttypedef) 
## GetMLTaskRunsRequestRequestTypeDef

```python
# GetMLTaskRunsRequestRequestTypeDef definition

class GetMLTaskRunsRequestRequestTypeDef(TypedDict):
    TransformId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[TaskRunFilterCriteriaTypeDef],  # (1)
    Sort: NotRequired[TaskRunSortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: TaskRunFilterCriteriaTypeDef](./type_defs.md#taskrunfiltercriteriatypedef) 
2. See [:material-code-braces: TaskRunSortCriteriaTypeDef](./type_defs.md#taskrunsortcriteriatypedef) 
## ListDataQualityStatisticAnnotationsRequestRequestTypeDef

```python
# ListDataQualityStatisticAnnotationsRequestRequestTypeDef definition

class ListDataQualityStatisticAnnotationsRequestRequestTypeDef(TypedDict):
    StatisticId: NotRequired[str],
    ProfileId: NotRequired[str],
    TimestampFilter: NotRequired[TimestampFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimestampFilterTypeDef](./type_defs.md#timestampfiltertypedef) 
## ListDataQualityStatisticsRequestRequestTypeDef

```python
# ListDataQualityStatisticsRequestRequestTypeDef definition

class ListDataQualityStatisticsRequestRequestTypeDef(TypedDict):
    StatisticId: NotRequired[str],
    ProfileId: NotRequired[str],
    TimestampFilter: NotRequired[TimestampFilterTypeDef],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimestampFilterTypeDef](./type_defs.md#timestampfiltertypedef) 
## TriggerTypeDef

```python
# TriggerTypeDef definition

class TriggerTypeDef(TypedDict):
    Name: NotRequired[str],
    WorkflowName: NotRequired[str],
    Id: NotRequired[str],
    Type: NotRequired[TriggerTypeType],  # (1)
    State: NotRequired[TriggerStateType],  # (2)
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    Actions: NotRequired[List[ActionOutputTypeDef]],  # (3)
    Predicate: NotRequired[PredicateOutputTypeDef],  # (4)
    EventBatchingCondition: NotRequired[EventBatchingConditionTypeDef],  # (5)
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
2. See [:material-code-brackets: TriggerStateType](./literals.md#triggerstatetype) 
3. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
4. See [:material-code-braces: PredicateOutputTypeDef](./type_defs.md#predicateoutputtypedef) 
5. See [:material-code-braces: EventBatchingConditionTypeDef](./type_defs.md#eventbatchingconditiontypedef) 
## GetUsageProfileResponseTypeDef

```python
# GetUsageProfileResponseTypeDef definition

class GetUsageProfileResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    Configuration: ProfileConfigurationOutputTypeDef,  # (1)
    CreatedOn: datetime,
    LastModifiedOn: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileConfigurationOutputTypeDef](./type_defs.md#profileconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProfileConfigurationTypeDef

```python
# ProfileConfigurationTypeDef definition

class ProfileConfigurationTypeDef(TypedDict):
    SessionConfiguration: NotRequired[Mapping[str, ConfigurationObjectUnionTypeDef]],  # (1)
    JobConfiguration: NotRequired[Mapping[str, ConfigurationObjectTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfigurationObjectTypeDef](./type_defs.md#configurationobjecttypedef) [:material-code-braces: ConfigurationObjectOutputTypeDef](./type_defs.md#configurationobjectoutputtypedef) 
2. See [:material-code-braces: ConfigurationObjectTypeDef](./type_defs.md#configurationobjecttypedef) 
## EvaluationMetricsTypeDef

```python
# EvaluationMetricsTypeDef definition

class EvaluationMetricsTypeDef(TypedDict):
    TransformType: TransformTypeType,  # (1)
    FindMatchesMetrics: NotRequired[FindMatchesMetricsTypeDef],  # (2)
```

1. See [:material-code-brackets: TransformTypeType](./literals.md#transformtypetype) 
2. See [:material-code-braces: FindMatchesMetricsTypeDef](./type_defs.md#findmatchesmetricstypedef) 
## CrawlerTypeDef

```python
# CrawlerTypeDef definition

class CrawlerTypeDef(TypedDict):
    Name: NotRequired[str],
    Role: NotRequired[str],
    Targets: NotRequired[CrawlerTargetsOutputTypeDef],  # (1)
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Classifiers: NotRequired[List[str]],
    RecrawlPolicy: NotRequired[RecrawlPolicyTypeDef],  # (2)
    SchemaChangePolicy: NotRequired[SchemaChangePolicyTypeDef],  # (3)
    LineageConfiguration: NotRequired[LineageConfigurationTypeDef],  # (4)
    State: NotRequired[CrawlerStateType],  # (5)
    TablePrefix: NotRequired[str],
    Schedule: NotRequired[ScheduleTypeDef],  # (6)
    CrawlElapsedTime: NotRequired[int],
    CreationTime: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    LastCrawl: NotRequired[LastCrawlInfoTypeDef],  # (7)
    Version: NotRequired[int],
    Configuration: NotRequired[str],
    CrawlerSecurityConfiguration: NotRequired[str],
    LakeFormationConfiguration: NotRequired[LakeFormationConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: CrawlerTargetsOutputTypeDef](./type_defs.md#crawlertargetsoutputtypedef) 
2. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
3. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-brackets: CrawlerStateType](./literals.md#crawlerstatetype) 
6. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
7. See [:material-code-braces: LastCrawlInfoTypeDef](./type_defs.md#lastcrawlinfotypedef) 
8. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
## ListDataQualityRulesetsRequestRequestTypeDef

```python
# ListDataQualityRulesetsRequestRequestTypeDef definition

class ListDataQualityRulesetsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[DataQualityRulesetFilterCriteriaTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DataQualityRulesetFilterCriteriaTypeDef](./type_defs.md#dataqualityrulesetfiltercriteriatypedef) 
## ListDataQualityRulesetsResponseTypeDef

```python
# ListDataQualityRulesetsResponseTypeDef definition

class ListDataQualityRulesetsResponseTypeDef(TypedDict):
    Rulesets: List[DataQualityRulesetListDetailsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataQualityRulesetListDetailsTypeDef](./type_defs.md#dataqualityrulesetlistdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeInboundIntegrationsResponseTypeDef

```python
# DescribeInboundIntegrationsResponseTypeDef definition

class DescribeInboundIntegrationsResponseTypeDef(TypedDict):
    InboundIntegrations: List[InboundIntegrationTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InboundIntegrationTypeDef](./type_defs.md#inboundintegrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeIntegrationsResponseTypeDef

```python
# DescribeIntegrationsResponseTypeDef definition

class DescribeIntegrationsResponseTypeDef(TypedDict):
    Integrations: List[IntegrationTypeDef],  # (1)
    Marker: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IntegrationTypeDef](./type_defs.md#integrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSessionResponseTypeDef

```python
# CreateSessionResponseTypeDef definition

class CreateSessionResponseTypeDef(TypedDict):
    Session: SessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionResponseTypeDef

```python
# GetSessionResponseTypeDef definition

class GetSessionResponseTypeDef(TypedDict):
    Session: SessionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSessionsResponseTypeDef

```python
# ListSessionsResponseTypeDef definition

class ListSessionsResponseTypeDef(TypedDict):
    Ids: List[str],
    Sessions: List[SessionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataCatalogEncryptionSettingsResponseTypeDef

```python
# GetDataCatalogEncryptionSettingsResponseTypeDef definition

class GetDataCatalogEncryptionSettingsResponseTypeDef(TypedDict):
    DataCatalogEncryptionSettings: DataCatalogEncryptionSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCatalogEncryptionSettingsTypeDef](./type_defs.md#datacatalogencryptionsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDataCatalogEncryptionSettingsRequestRequestTypeDef

```python
# PutDataCatalogEncryptionSettingsRequestRequestTypeDef definition

class PutDataCatalogEncryptionSettingsRequestRequestTypeDef(TypedDict):
    DataCatalogEncryptionSettings: DataCatalogEncryptionSettingsTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: DataCatalogEncryptionSettingsTypeDef](./type_defs.md#datacatalogencryptionsettingstypedef) 
## CatalogTypeDef

```python
# CatalogTypeDef definition

class CatalogTypeDef(TypedDict):
    Name: str,
    CatalogId: NotRequired[str],
    ResourceArn: NotRequired[str],
    Description: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
    CreateTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
    TargetRedshiftCatalog: NotRequired[TargetRedshiftCatalogTypeDef],  # (1)
    FederatedCatalog: NotRequired[FederatedCatalogTypeDef],  # (2)
    CatalogProperties: NotRequired[CatalogPropertiesOutputTypeDef],  # (3)
    CreateTableDefaultPermissions: NotRequired[List[PrincipalPermissionsOutputTypeDef]],  # (4)
    CreateDatabaseDefaultPermissions: NotRequired[List[PrincipalPermissionsOutputTypeDef]],  # (4)
```

1. See [:material-code-braces: TargetRedshiftCatalogTypeDef](./type_defs.md#targetredshiftcatalogtypedef) 
2. See [:material-code-braces: FederatedCatalogTypeDef](./type_defs.md#federatedcatalogtypedef) 
3. See [:material-code-braces: CatalogPropertiesOutputTypeDef](./type_defs.md#catalogpropertiesoutputtypedef) 
4. See [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
5. See [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
## DatabaseTypeDef

```python
# DatabaseTypeDef definition

class DatabaseTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    LocationUri: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
    CreateTime: NotRequired[datetime],
    CreateTableDefaultPermissions: NotRequired[List[PrincipalPermissionsOutputTypeDef]],  # (1)
    TargetDatabase: NotRequired[DatabaseIdentifierTypeDef],  # (2)
    CatalogId: NotRequired[str],
    FederatedDatabase: NotRequired[FederatedDatabaseTypeDef],  # (3)
```

1. See [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
2. See [:material-code-braces: DatabaseIdentifierTypeDef](./type_defs.md#databaseidentifiertypedef) 
3. See [:material-code-braces: FederatedDatabaseTypeDef](./type_defs.md#federateddatabasetypedef) 
## DataQualityObservationTypeDef

```python
# DataQualityObservationTypeDef definition

class DataQualityObservationTypeDef(TypedDict):
    Description: NotRequired[str],
    MetricBasedObservation: NotRequired[MetricBasedObservationTypeDef],  # (1)
```

1. See [:material-code-braces: MetricBasedObservationTypeDef](./type_defs.md#metricbasedobservationtypedef) 
## DataQualityResultDescriptionTypeDef

```python
# DataQualityResultDescriptionTypeDef definition

class DataQualityResultDescriptionTypeDef(TypedDict):
    ResultId: NotRequired[str],
    DataSource: NotRequired[DataSourceOutputTypeDef],  # (1)
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    StartedOn: NotRequired[datetime],
```

1. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
## DataQualityRuleRecommendationRunDescriptionTypeDef

```python
# DataQualityRuleRecommendationRunDescriptionTypeDef definition

class DataQualityRuleRecommendationRunDescriptionTypeDef(TypedDict):
    RunId: NotRequired[str],
    Status: NotRequired[TaskStatusTypeType],  # (1)
    StartedOn: NotRequired[datetime],
    DataSource: NotRequired[DataSourceOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
## DataQualityRulesetEvaluationRunDescriptionTypeDef

```python
# DataQualityRulesetEvaluationRunDescriptionTypeDef definition

class DataQualityRulesetEvaluationRunDescriptionTypeDef(TypedDict):
    RunId: NotRequired[str],
    Status: NotRequired[TaskStatusTypeType],  # (1)
    StartedOn: NotRequired[datetime],
    DataSource: NotRequired[DataSourceOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
## GetDataQualityRuleRecommendationRunResponseTypeDef

```python
# GetDataQualityRuleRecommendationRunResponseTypeDef definition

class GetDataQualityRuleRecommendationRunResponseTypeDef(TypedDict):
    RunId: str,
    DataSource: DataSourceOutputTypeDef,  # (1)
    Role: str,
    NumberOfWorkers: int,
    Timeout: int,
    Status: TaskStatusTypeType,  # (2)
    ErrorString: str,
    StartedOn: datetime,
    LastModifiedOn: datetime,
    CompletedOn: datetime,
    ExecutionTime: int,
    RecommendedRuleset: str,
    CreatedRulesetName: str,
    DataQualitySecurityConfiguration: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
2. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataQualityRulesetEvaluationRunResponseTypeDef

```python
# GetDataQualityRulesetEvaluationRunResponseTypeDef definition

class GetDataQualityRulesetEvaluationRunResponseTypeDef(TypedDict):
    RunId: str,
    DataSource: DataSourceOutputTypeDef,  # (1)
    Role: str,
    NumberOfWorkers: int,
    Timeout: int,
    AdditionalRunOptions: DataQualityEvaluationRunAdditionalRunOptionsTypeDef,  # (2)
    Status: TaskStatusTypeType,  # (3)
    ErrorString: str,
    StartedOn: datetime,
    LastModifiedOn: datetime,
    CompletedOn: datetime,
    ExecutionTime: int,
    RulesetNames: List[str],
    ResultIds: List[str],
    AdditionalDataSources: Dict[str, DataSourceOutputTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
2. See [:material-code-braces: DataQualityEvaluationRunAdditionalRunOptionsTypeDef](./type_defs.md#dataqualityevaluationrunadditionalrunoptionstypedef) 
3. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
4. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DropNullFieldsOutputTypeDef

```python
# DropNullFieldsOutputTypeDef definition

class DropNullFieldsOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    NullCheckBoxList: NotRequired[NullCheckBoxListTypeDef],  # (1)
    NullTextList: NotRequired[List[NullValueFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: NullCheckBoxListTypeDef](./type_defs.md#nullcheckboxlisttypedef) 
2. See [:material-code-braces: NullValueFieldTypeDef](./type_defs.md#nullvaluefieldtypedef) 
## DropNullFieldsTypeDef

```python
# DropNullFieldsTypeDef definition

class DropNullFieldsTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    NullCheckBoxList: NotRequired[NullCheckBoxListTypeDef],  # (1)
    NullTextList: NotRequired[Sequence[NullValueFieldTypeDef]],  # (2)
```

1. See [:material-code-braces: NullCheckBoxListTypeDef](./type_defs.md#nullcheckboxlisttypedef) 
2. See [:material-code-braces: NullValueFieldTypeDef](./type_defs.md#nullvaluefieldtypedef) 
## ColumnStatisticsDataOutputTypeDef

```python
# ColumnStatisticsDataOutputTypeDef definition

class ColumnStatisticsDataOutputTypeDef(TypedDict):
    Type: ColumnStatisticsTypeType,  # (1)
    BooleanColumnStatisticsData: NotRequired[BooleanColumnStatisticsDataTypeDef],  # (2)
    DateColumnStatisticsData: NotRequired[DateColumnStatisticsDataOutputTypeDef],  # (3)
    DecimalColumnStatisticsData: NotRequired[DecimalColumnStatisticsDataOutputTypeDef],  # (4)
    DoubleColumnStatisticsData: NotRequired[DoubleColumnStatisticsDataTypeDef],  # (5)
    LongColumnStatisticsData: NotRequired[LongColumnStatisticsDataTypeDef],  # (6)
    StringColumnStatisticsData: NotRequired[StringColumnStatisticsDataTypeDef],  # (7)
    BinaryColumnStatisticsData: NotRequired[BinaryColumnStatisticsDataTypeDef],  # (8)
```

1. See [:material-code-brackets: ColumnStatisticsTypeType](./literals.md#columnstatisticstypetype) 
2. See [:material-code-braces: BooleanColumnStatisticsDataTypeDef](./type_defs.md#booleancolumnstatisticsdatatypedef) 
3. See [:material-code-braces: DateColumnStatisticsDataOutputTypeDef](./type_defs.md#datecolumnstatisticsdataoutputtypedef) 
4. See [:material-code-braces: DecimalColumnStatisticsDataOutputTypeDef](./type_defs.md#decimalcolumnstatisticsdataoutputtypedef) 
5. See [:material-code-braces: DoubleColumnStatisticsDataTypeDef](./type_defs.md#doublecolumnstatisticsdatatypedef) 
6. See [:material-code-braces: LongColumnStatisticsDataTypeDef](./type_defs.md#longcolumnstatisticsdatatypedef) 
7. See [:material-code-braces: StringColumnStatisticsDataTypeDef](./type_defs.md#stringcolumnstatisticsdatatypedef) 
8. See [:material-code-braces: BinaryColumnStatisticsDataTypeDef](./type_defs.md#binarycolumnstatisticsdatatypedef) 
## StorageDescriptorOutputTypeDef

```python
# StorageDescriptorOutputTypeDef definition

class StorageDescriptorOutputTypeDef(TypedDict):
    Columns: NotRequired[List[ColumnOutputTypeDef]],  # (1)
    Location: NotRequired[str],
    AdditionalLocations: NotRequired[List[str]],
    InputFormat: NotRequired[str],
    OutputFormat: NotRequired[str],
    Compressed: NotRequired[bool],
    NumberOfBuckets: NotRequired[int],
    SerdeInfo: NotRequired[SerDeInfoOutputTypeDef],  # (2)
    BucketColumns: NotRequired[List[str]],
    SortColumns: NotRequired[List[OrderTypeDef]],  # (3)
    Parameters: NotRequired[Dict[str, str]],
    SkewedInfo: NotRequired[SkewedInfoOutputTypeDef],  # (4)
    StoredAsSubDirectories: NotRequired[bool],
    SchemaReference: NotRequired[SchemaReferenceTypeDef],  # (5)
```

1. See [:material-code-braces: ColumnOutputTypeDef](./type_defs.md#columnoutputtypedef) 
2. See [:material-code-braces: SerDeInfoOutputTypeDef](./type_defs.md#serdeinfooutputtypedef) 
3. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
4. See [:material-code-braces: SkewedInfoOutputTypeDef](./type_defs.md#skewedinfooutputtypedef) 
5. See [:material-code-braces: SchemaReferenceTypeDef](./type_defs.md#schemareferencetypedef) 
## SecurityConfigurationTypeDef

```python
# SecurityConfigurationTypeDef definition

class SecurityConfigurationTypeDef(TypedDict):
    Name: NotRequired[str],
    CreatedTimeStamp: NotRequired[datetime],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: EncryptionConfigurationOutputTypeDef](./type_defs.md#encryptionconfigurationoutputtypedef) 
## CreateSecurityConfigurationRequestRequestTypeDef

```python
# CreateSecurityConfigurationRequestRequestTypeDef definition

class CreateSecurityConfigurationRequestRequestTypeDef(TypedDict):
    Name: str,
    EncryptionConfiguration: EncryptionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
## DeleteSchemaVersionsResponseTypeDef

```python
# DeleteSchemaVersionsResponseTypeDef definition

class DeleteSchemaVersionsResponseTypeDef(TypedDict):
    SchemaVersionErrors: List[SchemaVersionErrorItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SchemaVersionErrorItemTypeDef](./type_defs.md#schemaversionerroritemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FilterOutputTypeDef

```python
# FilterOutputTypeDef definition

class FilterOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    LogicalOperator: FilterLogicalOperatorType,  # (1)
    Filters: List[FilterExpressionOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterLogicalOperatorType](./literals.md#filterlogicaloperatortype) 
2. See [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 
## FilterExpressionTypeDef

```python
# FilterExpressionTypeDef definition

class FilterExpressionTypeDef(TypedDict):
    Operation: FilterOperationType,  # (1)
    Values: Sequence[FilterValueUnionTypeDef],  # (2)
    Negated: NotRequired[bool],
```

1. See [:material-code-brackets: FilterOperationType](./literals.md#filteroperationtype) 
2. See [:material-code-braces: FilterValueTypeDef](./type_defs.md#filtervaluetypedef) [:material-code-braces: FilterValueOutputTypeDef](./type_defs.md#filtervalueoutputtypedef) 
## UpdateMLTransformRequestRequestTypeDef

```python
# UpdateMLTransformRequestRequestTypeDef definition

class UpdateMLTransformRequestRequestTypeDef(TypedDict):
    TransformId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    Parameters: NotRequired[TransformParametersTypeDef],  # (1)
    Role: NotRequired[str],
    GlueVersion: NotRequired[str],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (2)
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    MaxRetries: NotRequired[int],
```

1. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
2. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
## GetMLTransformsRequestRequestTypeDef

```python
# GetMLTransformsRequestRequestTypeDef definition

class GetMLTransformsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[TransformFilterCriteriaTypeDef],  # (1)
    Sort: NotRequired[TransformSortCriteriaTypeDef],  # (2)
```

1. See [:material-code-braces: TransformFilterCriteriaTypeDef](./type_defs.md#transformfiltercriteriatypedef) 
2. See [:material-code-braces: TransformSortCriteriaTypeDef](./type_defs.md#transformsortcriteriatypedef) 
## ListMLTransformsRequestRequestTypeDef

```python
# ListMLTransformsRequestRequestTypeDef definition

class ListMLTransformsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filter: NotRequired[TransformFilterCriteriaTypeDef],  # (1)
    Sort: NotRequired[TransformSortCriteriaTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: TransformFilterCriteriaTypeDef](./type_defs.md#transformfiltercriteriatypedef) 
2. See [:material-code-braces: TransformSortCriteriaTypeDef](./type_defs.md#transformsortcriteriatypedef) 
## AthenaConnectorSourceOutputTypeDef

```python
# AthenaConnectorSourceOutputTypeDef definition

class AthenaConnectorSourceOutputTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    SchemaName: str,
    ConnectionTable: NotRequired[str],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## CatalogDeltaSourceOutputTypeDef

```python
# CatalogDeltaSourceOutputTypeDef definition

class CatalogDeltaSourceOutputTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalDeltaOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## CatalogHudiSourceOutputTypeDef

```python
# CatalogHudiSourceOutputTypeDef definition

class CatalogHudiSourceOutputTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalHudiOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## ConnectorDataSourceOutputTypeDef

```python
# ConnectorDataSourceOutputTypeDef definition

class ConnectorDataSourceOutputTypeDef(TypedDict):
    Name: str,
    ConnectionType: str,
    Data: Dict[str, str],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## CustomCodeOutputTypeDef

```python
# CustomCodeOutputTypeDef definition

class CustomCodeOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    Code: str,
    ClassName: str,
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## DynamicTransformOutputTypeDef

```python
# DynamicTransformOutputTypeDef definition

class DynamicTransformOutputTypeDef(TypedDict):
    Name: str,
    TransformName: str,
    Inputs: List[str],
    FunctionName: str,
    Path: str,
    Parameters: NotRequired[List[TransformConfigParameterOutputTypeDef]],  # (1)
    Version: NotRequired[str],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: TransformConfigParameterOutputTypeDef](./type_defs.md#transformconfigparameteroutputtypedef) 
2. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## JDBCConnectorSourceOutputTypeDef

```python
# JDBCConnectorSourceOutputTypeDef definition

class JDBCConnectorSourceOutputTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[JDBCConnectorOptionsOutputTypeDef],  # (1)
    ConnectionTable: NotRequired[str],
    Query: NotRequired[str],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: JDBCConnectorOptionsOutputTypeDef](./type_defs.md#jdbcconnectoroptionsoutputtypedef) 
2. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## JDBCConnectorTargetOutputTypeDef

```python
# JDBCConnectorTargetOutputTypeDef definition

class JDBCConnectorTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    ConnectionName: str,
    ConnectionTable: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## S3CatalogDeltaSourceOutputTypeDef

```python
# S3CatalogDeltaSourceOutputTypeDef definition

class S3CatalogDeltaSourceOutputTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalDeltaOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## S3CatalogHudiSourceOutputTypeDef

```python
# S3CatalogHudiSourceOutputTypeDef definition

class S3CatalogHudiSourceOutputTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalHudiOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## S3CsvSourceOutputTypeDef

```python
# S3CsvSourceOutputTypeDef definition

class S3CsvSourceOutputTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    Separator: SeparatorType,  # (3)
    QuoteChar: QuoteCharType,  # (4)
    CompressionType: NotRequired[CompressionTypeType],  # (1)
    Exclusions: NotRequired[List[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    Escaper: NotRequired[str],
    Multiline: NotRequired[bool],
    WithHeader: NotRequired[bool],
    WriteHeader: NotRequired[bool],
    SkipFirst: NotRequired[bool],
    OptimizePerformance: NotRequired[bool],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (5)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-brackets: SeparatorType](./literals.md#separatortype) 
4. See [:material-code-brackets: QuoteCharType](./literals.md#quotechartype) 
5. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## S3DeltaSourceOutputTypeDef

```python
# S3DeltaSourceOutputTypeDef definition

class S3DeltaSourceOutputTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    AdditionalDeltaOptions: NotRequired[Dict[str, str]],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
2. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## S3HudiSourceOutputTypeDef

```python
# S3HudiSourceOutputTypeDef definition

class S3HudiSourceOutputTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    AdditionalHudiOptions: NotRequired[Dict[str, str]],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
2. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## S3JsonSourceOutputTypeDef

```python
# S3JsonSourceOutputTypeDef definition

class S3JsonSourceOutputTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    CompressionType: NotRequired[CompressionTypeType],  # (1)
    Exclusions: NotRequired[List[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    JsonPath: NotRequired[str],
    Multiline: NotRequired[bool],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## S3ParquetSourceOutputTypeDef

```python
# S3ParquetSourceOutputTypeDef definition

class S3ParquetSourceOutputTypeDef(TypedDict):
    Name: str,
    Paths: List[str],
    CompressionType: NotRequired[ParquetCompressionTypeType],  # (1)
    Exclusions: NotRequired[List[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: ParquetCompressionTypeType](./literals.md#parquetcompressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## SnowflakeSourceOutputTypeDef

```python
# SnowflakeSourceOutputTypeDef definition

class SnowflakeSourceOutputTypeDef(TypedDict):
    Name: str,
    Data: SnowflakeNodeDataOutputTypeDef,  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: SnowflakeNodeDataOutputTypeDef](./type_defs.md#snowflakenodedataoutputtypedef) 
2. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## SparkConnectorSourceOutputTypeDef

```python
# SparkConnectorSourceOutputTypeDef definition

class SparkConnectorSourceOutputTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## SparkConnectorTargetOutputTypeDef

```python
# SparkConnectorTargetOutputTypeDef definition

class SparkConnectorTargetOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Dict[str, str]],
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## SparkSQLOutputTypeDef

```python
# SparkSQLOutputTypeDef definition

class SparkSQLOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    SqlQuery: str,
    SqlAliases: List[SqlAliasTypeDef],  # (1)
    OutputSchemas: NotRequired[List[GlueSchemaOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: SqlAliasTypeDef](./type_defs.md#sqlaliastypedef) 
2. See [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## AthenaConnectorSourceTypeDef

```python
# AthenaConnectorSourceTypeDef definition

class AthenaConnectorSourceTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    SchemaName: str,
    ConnectionTable: NotRequired[str],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## CatalogDeltaSourceTypeDef

```python
# CatalogDeltaSourceTypeDef definition

class CatalogDeltaSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalDeltaOptions: NotRequired[Mapping[str, str]],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## CatalogHudiSourceTypeDef

```python
# CatalogHudiSourceTypeDef definition

class CatalogHudiSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalHudiOptions: NotRequired[Mapping[str, str]],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## CustomCodeTypeDef

```python
# CustomCodeTypeDef definition

class CustomCodeTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Code: str,
    ClassName: str,
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## JDBCConnectorTargetTypeDef

```python
# JDBCConnectorTargetTypeDef definition

class JDBCConnectorTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    ConnectionName: str,
    ConnectionTable: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Mapping[str, str]],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3CatalogDeltaSourceTypeDef

```python
# S3CatalogDeltaSourceTypeDef definition

class S3CatalogDeltaSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalDeltaOptions: NotRequired[Mapping[str, str]],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3CatalogHudiSourceTypeDef

```python
# S3CatalogHudiSourceTypeDef definition

class S3CatalogHudiSourceTypeDef(TypedDict):
    Name: str,
    Database: str,
    Table: str,
    AdditionalHudiOptions: NotRequired[Mapping[str, str]],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3CsvSourceTypeDef

```python
# S3CsvSourceTypeDef definition

class S3CsvSourceTypeDef(TypedDict):
    Name: str,
    Paths: Sequence[str],
    Separator: SeparatorType,  # (3)
    QuoteChar: QuoteCharType,  # (4)
    CompressionType: NotRequired[CompressionTypeType],  # (1)
    Exclusions: NotRequired[Sequence[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    Escaper: NotRequired[str],
    Multiline: NotRequired[bool],
    WithHeader: NotRequired[bool],
    WriteHeader: NotRequired[bool],
    SkipFirst: NotRequired[bool],
    OptimizePerformance: NotRequired[bool],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (5)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-brackets: SeparatorType](./literals.md#separatortype) 
4. See [:material-code-brackets: QuoteCharType](./literals.md#quotechartype) 
5. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3DeltaSourceTypeDef

```python
# S3DeltaSourceTypeDef definition

class S3DeltaSourceTypeDef(TypedDict):
    Name: str,
    Paths: Sequence[str],
    AdditionalDeltaOptions: NotRequired[Mapping[str, str]],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (1)
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3HudiSourceTypeDef

```python
# S3HudiSourceTypeDef definition

class S3HudiSourceTypeDef(TypedDict):
    Name: str,
    Paths: Sequence[str],
    AdditionalHudiOptions: NotRequired[Mapping[str, str]],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (1)
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3JsonSourceTypeDef

```python
# S3JsonSourceTypeDef definition

class S3JsonSourceTypeDef(TypedDict):
    Name: str,
    Paths: Sequence[str],
    CompressionType: NotRequired[CompressionTypeType],  # (1)
    Exclusions: NotRequired[Sequence[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    JsonPath: NotRequired[str],
    Multiline: NotRequired[bool],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (3)
```

1. See [:material-code-brackets: CompressionTypeType](./literals.md#compressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## S3ParquetSourceTypeDef

```python
# S3ParquetSourceTypeDef definition

class S3ParquetSourceTypeDef(TypedDict):
    Name: str,
    Paths: Sequence[str],
    CompressionType: NotRequired[ParquetCompressionTypeType],  # (1)
    Exclusions: NotRequired[Sequence[str]],
    GroupSize: NotRequired[str],
    GroupFiles: NotRequired[str],
    Recurse: NotRequired[bool],
    MaxBand: NotRequired[int],
    MaxFilesInBand: NotRequired[int],
    AdditionalOptions: NotRequired[S3DirectSourceAdditionalOptionsTypeDef],  # (2)
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (3)
```

1. See [:material-code-brackets: ParquetCompressionTypeType](./literals.md#parquetcompressiontypetype) 
2. See [:material-code-braces: S3DirectSourceAdditionalOptionsTypeDef](./type_defs.md#s3directsourceadditionaloptionstypedef) 
3. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## SparkConnectorSourceTypeDef

```python
# SparkConnectorSourceTypeDef definition

class SparkConnectorSourceTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Mapping[str, str]],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## SparkConnectorTargetTypeDef

```python
# SparkConnectorTargetTypeDef definition

class SparkConnectorTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[Mapping[str, str]],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## SparkSQLTypeDef

```python
# SparkSQLTypeDef definition

class SparkSQLTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    SqlQuery: str,
    SqlAliases: Sequence[SqlAliasTypeDef],  # (1)
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: SqlAliasTypeDef](./type_defs.md#sqlaliastypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    GlueTable: GlueTableUnionTypeDef,  # (1)
```

1. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) [:material-code-braces: GlueTableOutputTypeDef](./type_defs.md#gluetableoutputtypedef) 
## TableOptimizerConfigurationTypeDef

```python
# TableOptimizerConfigurationTypeDef definition

class TableOptimizerConfigurationTypeDef(TypedDict):
    roleArn: NotRequired[str],
    enabled: NotRequired[bool],
    vpcConfiguration: NotRequired[TableOptimizerVpcConfigurationTypeDef],  # (1)
    retentionConfiguration: NotRequired[RetentionConfigurationTypeDef],  # (2)
    orphanFileDeletionConfiguration: NotRequired[OrphanFileDeletionConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: TableOptimizerVpcConfigurationTypeDef](./type_defs.md#tableoptimizervpcconfigurationtypedef) 
2. See [:material-code-braces: RetentionConfigurationTypeDef](./type_defs.md#retentionconfigurationtypedef) 
3. See [:material-code-braces: OrphanFileDeletionConfigurationTypeDef](./type_defs.md#orphanfiledeletionconfigurationtypedef) 
## TableOptimizerRunTypeDef

```python
# TableOptimizerRunTypeDef definition

class TableOptimizerRunTypeDef(TypedDict):
    eventType: NotRequired[TableOptimizerEventTypeType],  # (1)
    startTimestamp: NotRequired[datetime],
    endTimestamp: NotRequired[datetime],
    metrics: NotRequired[RunMetricsTypeDef],  # (2)
    error: NotRequired[str],
    compactionMetrics: NotRequired[CompactionMetricsTypeDef],  # (3)
    retentionMetrics: NotRequired[RetentionMetricsTypeDef],  # (4)
    orphanFileDeletionMetrics: NotRequired[OrphanFileDeletionMetricsTypeDef],  # (5)
```

1. See [:material-code-brackets: TableOptimizerEventTypeType](./literals.md#tableoptimizereventtypetype) 
2. See [:material-code-braces: RunMetricsTypeDef](./type_defs.md#runmetricstypedef) 
3. See [:material-code-braces: CompactionMetricsTypeDef](./type_defs.md#compactionmetricstypedef) 
4. See [:material-code-braces: RetentionMetricsTypeDef](./type_defs.md#retentionmetricstypedef) 
5. See [:material-code-braces: OrphanFileDeletionMetricsTypeDef](./type_defs.md#orphanfiledeletionmetricstypedef) 
## GetIntegrationTablePropertiesResponseTypeDef

```python
# GetIntegrationTablePropertiesResponseTypeDef definition

class GetIntegrationTablePropertiesResponseTypeDef(TypedDict):
    ResourceArn: str,
    TableName: str,
    SourceTableConfig: SourceTableConfigOutputTypeDef,  # (1)
    TargetTableConfig: TargetTableConfigOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SourceTableConfigOutputTypeDef](./type_defs.md#sourcetableconfigoutputtypedef) 
2. See [:material-code-braces: TargetTableConfigOutputTypeDef](./type_defs.md#targettableconfigoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIntegrationTablePropertiesRequestRequestTypeDef

```python
# CreateIntegrationTablePropertiesRequestRequestTypeDef definition

class CreateIntegrationTablePropertiesRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TableName: str,
    SourceTableConfig: NotRequired[SourceTableConfigTypeDef],  # (1)
    TargetTableConfig: NotRequired[TargetTableConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SourceTableConfigTypeDef](./type_defs.md#sourcetableconfigtypedef) 
2. See [:material-code-braces: TargetTableConfigTypeDef](./type_defs.md#targettableconfigtypedef) 
## UpdateIntegrationTablePropertiesRequestRequestTypeDef

```python
# UpdateIntegrationTablePropertiesRequestRequestTypeDef definition

class UpdateIntegrationTablePropertiesRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TableName: str,
    SourceTableConfig: NotRequired[SourceTableConfigTypeDef],  # (1)
    TargetTableConfig: NotRequired[TargetTableConfigTypeDef],  # (2)
```

1. See [:material-code-braces: SourceTableConfigTypeDef](./type_defs.md#sourcetableconfigtypedef) 
2. See [:material-code-braces: TargetTableConfigTypeDef](./type_defs.md#targettableconfigtypedef) 
## JDBCConnectorSourceTypeDef

```python
# JDBCConnectorSourceTypeDef definition

class JDBCConnectorSourceTypeDef(TypedDict):
    Name: str,
    ConnectionName: str,
    ConnectorName: str,
    ConnectionType: str,
    AdditionalOptions: NotRequired[JDBCConnectorOptionsUnionTypeDef],  # (1)
    ConnectionTable: NotRequired[str],
    Query: NotRequired[str],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: JDBCConnectorOptionsTypeDef](./type_defs.md#jdbcconnectoroptionstypedef) [:material-code-braces: JDBCConnectorOptionsOutputTypeDef](./type_defs.md#jdbcconnectoroptionsoutputtypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## GetJobRunResponseTypeDef

```python
# GetJobRunResponseTypeDef definition

class GetJobRunResponseTypeDef(TypedDict):
    JobRun: JobRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobRunsResponseTypeDef

```python
# GetJobRunsResponseTypeDef definition

class GetJobRunsResponseTypeDef(TypedDict):
    JobRuns: List[JobRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobNodeDetailsTypeDef

```python
# JobNodeDetailsTypeDef definition

class JobNodeDetailsTypeDef(TypedDict):
    JobRuns: NotRequired[List[JobRunTypeDef]],  # (1)
```

1. See [:material-code-braces: JobRunTypeDef](./type_defs.md#jobruntypedef) 
## JoinTypeDef

```python
# JoinTypeDef definition

class JoinTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    JoinType: JoinTypeType,  # (1)
    Columns: Sequence[JoinColumnUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: JoinTypeType](./literals.md#jointypetype) 
2. See [:material-code-braces: JoinColumnTypeDef](./type_defs.md#joincolumntypedef) [:material-code-braces: JoinColumnOutputTypeDef](./type_defs.md#joincolumnoutputtypedef) 
## GetMLTaskRunResponseTypeDef

```python
# GetMLTaskRunResponseTypeDef definition

class GetMLTaskRunResponseTypeDef(TypedDict):
    TransformId: str,
    TaskRunId: str,
    Status: TaskStatusTypeType,  # (1)
    LogGroupName: str,
    Properties: TaskRunPropertiesTypeDef,  # (2)
    ErrorString: str,
    StartedOn: datetime,
    LastModifiedOn: datetime,
    CompletedOn: datetime,
    ExecutionTime: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: TaskRunPropertiesTypeDef](./type_defs.md#taskrunpropertiestypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TaskRunTypeDef

```python
# TaskRunTypeDef definition

class TaskRunTypeDef(TypedDict):
    TransformId: NotRequired[str],
    TaskRunId: NotRequired[str],
    Status: NotRequired[TaskStatusTypeType],  # (1)
    LogGroupName: NotRequired[str],
    Properties: NotRequired[TaskRunPropertiesTypeDef],  # (2)
    ErrorString: NotRequired[str],
    StartedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    ExecutionTime: NotRequired[int],
```

1. See [:material-code-brackets: TaskStatusTypeType](./literals.md#taskstatustypetype) 
2. See [:material-code-braces: TaskRunPropertiesTypeDef](./type_defs.md#taskrunpropertiestypedef) 
## CreateMLTransformRequestRequestTypeDef

```python
# CreateMLTransformRequestRequestTypeDef definition

class CreateMLTransformRequestRequestTypeDef(TypedDict):
    Name: str,
    InputRecordTables: Sequence[GlueTableUnionTypeDef],  # (1)
    Parameters: TransformParametersTypeDef,  # (2)
    Role: str,
    Description: NotRequired[str],
    GlueVersion: NotRequired[str],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (3)
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    MaxRetries: NotRequired[int],
    Tags: NotRequired[Mapping[str, str]],
    TransformEncryption: NotRequired[TransformEncryptionTypeDef],  # (4)
```

1. See [:material-code-braces: GlueTableTypeDef](./type_defs.md#gluetabletypedef) [:material-code-braces: GlueTableOutputTypeDef](./type_defs.md#gluetableoutputtypedef) 
2. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
3. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
4. See [:material-code-braces: TransformEncryptionTypeDef](./type_defs.md#transformencryptiontypedef) 
## ApplyMappingTypeDef

```python
# ApplyMappingTypeDef definition

class ApplyMappingTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Mapping: Sequence[MappingUnionTypeDef],  # (1)
```

1. See [:material-code-braces: MappingTypeDef](./type_defs.md#mappingtypedef) [:material-code-braces: MappingOutputTypeDef](./type_defs.md#mappingoutputtypedef) 
## QuerySchemaVersionMetadataResponseTypeDef

```python
# QuerySchemaVersionMetadataResponseTypeDef definition

class QuerySchemaVersionMetadataResponseTypeDef(TypedDict):
    MetadataInfoMap: Dict[str, MetadataInfoTypeDef],  # (1)
    SchemaVersionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MetadataInfoTypeDef](./type_defs.md#metadatainfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuthenticationConfigurationTypeDef

```python
# AuthenticationConfigurationTypeDef definition

class AuthenticationConfigurationTypeDef(TypedDict):
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (1)
    SecretArn: NotRequired[str],
    OAuth2Properties: NotRequired[OAuth2PropertiesTypeDef],  # (2)
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: OAuth2PropertiesTypeDef](./type_defs.md#oauth2propertiestypedef) 
## AuthenticationConfigurationInputTypeDef

```python
# AuthenticationConfigurationInputTypeDef definition

class AuthenticationConfigurationInputTypeDef(TypedDict):
    AuthenticationType: NotRequired[AuthenticationTypeType],  # (1)
    OAuth2Properties: NotRequired[OAuth2PropertiesInputTypeDef],  # (2)
    SecretArn: NotRequired[str],
    KmsKeyArn: NotRequired[str],
    BasicAuthenticationCredentials: NotRequired[BasicAuthenticationCredentialsTypeDef],  # (3)
    CustomAuthenticationCredentials: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: OAuth2PropertiesInputTypeDef](./type_defs.md#oauth2propertiesinputtypedef) 
3. See [:material-code-braces: BasicAuthenticationCredentialsTypeDef](./type_defs.md#basicauthenticationcredentialstypedef) 
## RecipeOutputTypeDef

```python
# RecipeOutputTypeDef definition

class RecipeOutputTypeDef(TypedDict):
    Name: str,
    Inputs: List[str],
    RecipeReference: NotRequired[RecipeReferenceTypeDef],  # (1)
    RecipeSteps: NotRequired[List[RecipeStepOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
2. See [:material-code-braces: RecipeStepOutputTypeDef](./type_defs.md#recipestepoutputtypedef) 
## RecipeStepTypeDef

```python
# RecipeStepTypeDef definition

class RecipeStepTypeDef(TypedDict):
    Action: RecipeActionUnionTypeDef,  # (1)
    ConditionExpressions: NotRequired[Sequence[ConditionExpressionTypeDef]],  # (2)
```

1. See [:material-code-braces: RecipeActionTypeDef](./type_defs.md#recipeactiontypedef) [:material-code-braces: RecipeActionOutputTypeDef](./type_defs.md#recipeactionoutputtypedef) 
2. See [:material-code-braces: ConditionExpressionTypeDef](./type_defs.md#conditionexpressiontypedef) 
## CreateUserDefinedFunctionRequestRequestTypeDef

```python
# CreateUserDefinedFunctionRequestRequestTypeDef definition

class CreateUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionInput: UserDefinedFunctionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: UserDefinedFunctionInputTypeDef](./type_defs.md#userdefinedfunctioninputtypedef) 
## UpdateUserDefinedFunctionRequestRequestTypeDef

```python
# UpdateUserDefinedFunctionRequestRequestTypeDef definition

class UpdateUserDefinedFunctionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    FunctionName: str,
    FunctionInput: UserDefinedFunctionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: UserDefinedFunctionInputTypeDef](./type_defs.md#userdefinedfunctioninputtypedef) 
## GetUserDefinedFunctionResponseTypeDef

```python
# GetUserDefinedFunctionResponseTypeDef definition

class GetUserDefinedFunctionResponseTypeDef(TypedDict):
    UserDefinedFunction: UserDefinedFunctionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UserDefinedFunctionTypeDef](./type_defs.md#userdefinedfunctiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserDefinedFunctionsResponseTypeDef

```python
# GetUserDefinedFunctionsResponseTypeDef definition

class GetUserDefinedFunctionsResponseTypeDef(TypedDict):
    UserDefinedFunctions: List[UserDefinedFunctionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UserDefinedFunctionTypeDef](./type_defs.md#userdefinedfunctiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CrawlerTargetsTypeDef

```python
# CrawlerTargetsTypeDef definition

class CrawlerTargetsTypeDef(TypedDict):
    S3Targets: NotRequired[Sequence[S3TargetUnionTypeDef]],  # (1)
    JdbcTargets: NotRequired[Sequence[JdbcTargetUnionTypeDef]],  # (2)
    MongoDBTargets: NotRequired[Sequence[MongoDBTargetTypeDef]],  # (3)
    DynamoDBTargets: NotRequired[Sequence[DynamoDBTargetTypeDef]],  # (4)
    CatalogTargets: NotRequired[Sequence[CatalogTargetUnionTypeDef]],  # (5)
    DeltaTargets: NotRequired[Sequence[DeltaTargetUnionTypeDef]],  # (6)
    IcebergTargets: NotRequired[Sequence[IcebergTargetUnionTypeDef]],  # (7)
    HudiTargets: NotRequired[Sequence[HudiTargetUnionTypeDef]],  # (8)
```

1. See [:material-code-braces: S3TargetTypeDef](./type_defs.md#s3targettypedef) [:material-code-braces: S3TargetOutputTypeDef](./type_defs.md#s3targetoutputtypedef) 
2. See [:material-code-braces: JdbcTargetTypeDef](./type_defs.md#jdbctargettypedef) [:material-code-braces: JdbcTargetOutputTypeDef](./type_defs.md#jdbctargetoutputtypedef) 
3. See [:material-code-braces: MongoDBTargetTypeDef](./type_defs.md#mongodbtargettypedef) 
4. See [:material-code-braces: DynamoDBTargetTypeDef](./type_defs.md#dynamodbtargettypedef) 
5. See [:material-code-braces: CatalogTargetTypeDef](./type_defs.md#catalogtargettypedef) [:material-code-braces: CatalogTargetOutputTypeDef](./type_defs.md#catalogtargetoutputtypedef) 
6. See [:material-code-braces: DeltaTargetTypeDef](./type_defs.md#deltatargettypedef) [:material-code-braces: DeltaTargetOutputTypeDef](./type_defs.md#deltatargetoutputtypedef) 
7. See [:material-code-braces: IcebergTargetTypeDef](./type_defs.md#icebergtargettypedef) [:material-code-braces: IcebergTargetOutputTypeDef](./type_defs.md#icebergtargetoutputtypedef) 
8. See [:material-code-braces: HudiTargetTypeDef](./type_defs.md#huditargettypedef) [:material-code-braces: HudiTargetOutputTypeDef](./type_defs.md#huditargetoutputtypedef) 
## StorageDescriptorTypeDef

```python
# StorageDescriptorTypeDef definition

class StorageDescriptorTypeDef(TypedDict):
    Columns: NotRequired[Sequence[ColumnUnionTypeDef]],  # (1)
    Location: NotRequired[str],
    AdditionalLocations: NotRequired[Sequence[str]],
    InputFormat: NotRequired[str],
    OutputFormat: NotRequired[str],
    Compressed: NotRequired[bool],
    NumberOfBuckets: NotRequired[int],
    SerdeInfo: NotRequired[SerDeInfoUnionTypeDef],  # (2)
    BucketColumns: NotRequired[Sequence[str]],
    SortColumns: NotRequired[Sequence[OrderTypeDef]],  # (3)
    Parameters: NotRequired[Mapping[str, str]],
    SkewedInfo: NotRequired[SkewedInfoUnionTypeDef],  # (4)
    StoredAsSubDirectories: NotRequired[bool],
    SchemaReference: NotRequired[SchemaReferenceTypeDef],  # (5)
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) [:material-code-braces: ColumnOutputTypeDef](./type_defs.md#columnoutputtypedef) 
2. See [:material-code-braces: SerDeInfoTypeDef](./type_defs.md#serdeinfotypedef) [:material-code-braces: SerDeInfoOutputTypeDef](./type_defs.md#serdeinfooutputtypedef) 
3. See [:material-code-braces: OrderTypeDef](./type_defs.md#ordertypedef) 
4. See [:material-code-braces: SkewedInfoTypeDef](./type_defs.md#skewedinfotypedef) [:material-code-braces: SkewedInfoOutputTypeDef](./type_defs.md#skewedinfooutputtypedef) 
5. See [:material-code-braces: SchemaReferenceTypeDef](./type_defs.md#schemareferencetypedef) 
## StatementTypeDef

```python
# StatementTypeDef definition

class StatementTypeDef(TypedDict):
    Id: NotRequired[int],
    Code: NotRequired[str],
    State: NotRequired[StatementStateType],  # (1)
    Output: NotRequired[StatementOutputTypeDef],  # (2)
    Progress: NotRequired[float],
    StartedOn: NotRequired[int],
    CompletedOn: NotRequired[int],
```

1. See [:material-code-brackets: StatementStateType](./literals.md#statementstatetype) 
2. See [:material-code-braces: StatementOutputTypeDef](./type_defs.md#statementoutputtypedef) 
## ListDataQualityStatisticAnnotationsResponseTypeDef

```python
# ListDataQualityStatisticAnnotationsResponseTypeDef definition

class ListDataQualityStatisticAnnotationsResponseTypeDef(TypedDict):
    Annotations: List[StatisticAnnotationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StatisticAnnotationTypeDef](./type_defs.md#statisticannotationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityStatisticsResponseTypeDef

```python
# ListDataQualityStatisticsResponseTypeDef definition

class ListDataQualityStatisticsResponseTypeDef(TypedDict):
    Statistics: List[StatisticSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StatisticSummaryTypeDef](./type_defs.md#statisticsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DynamicTransformTypeDef

```python
# DynamicTransformTypeDef definition

class DynamicTransformTypeDef(TypedDict):
    Name: str,
    TransformName: str,
    Inputs: Sequence[str],
    FunctionName: str,
    Path: str,
    Parameters: NotRequired[Sequence[TransformConfigParameterUnionTypeDef]],  # (1)
    Version: NotRequired[str],
    OutputSchemas: NotRequired[Sequence[GlueSchemaTypeDef]],  # (2)
```

1. See [:material-code-braces: TransformConfigParameterTypeDef](./type_defs.md#transformconfigparametertypedef) [:material-code-braces: TransformConfigParameterOutputTypeDef](./type_defs.md#transformconfigparameteroutputtypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) 
## RedshiftTargetTypeDef

```python
# RedshiftTargetTypeDef definition

class RedshiftTargetTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    Database: str,
    Table: str,
    RedshiftTmpDir: NotRequired[str],
    TmpDirIAMRole: NotRequired[str],
    UpsertRedshiftOptions: NotRequired[UpsertRedshiftTargetOptionsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: UpsertRedshiftTargetOptionsTypeDef](./type_defs.md#upsertredshifttargetoptionstypedef) [:material-code-braces: UpsertRedshiftTargetOptionsOutputTypeDef](./type_defs.md#upsertredshifttargetoptionsoutputtypedef) 
## CreateTriggerRequestRequestTypeDef

```python
# CreateTriggerRequestRequestTypeDef definition

class CreateTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
    Type: TriggerTypeType,  # (1)
    Actions: Sequence[ActionUnionTypeDef],  # (2)
    WorkflowName: NotRequired[str],
    Schedule: NotRequired[str],
    Predicate: NotRequired[PredicateTypeDef],  # (3)
    Description: NotRequired[str],
    StartOnCreation: NotRequired[bool],
    Tags: NotRequired[Mapping[str, str]],
    EventBatchingCondition: NotRequired[EventBatchingConditionTypeDef],  # (4)
```

1. See [:material-code-brackets: TriggerTypeType](./literals.md#triggertypetype) 
2. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
3. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) 
4. See [:material-code-braces: EventBatchingConditionTypeDef](./type_defs.md#eventbatchingconditiontypedef) 
## DescribeConnectionTypeResponseTypeDef

```python
# DescribeConnectionTypeResponseTypeDef definition

class DescribeConnectionTypeResponseTypeDef(TypedDict):
    ConnectionType: str,
    Description: str,
    Capabilities: CapabilitiesTypeDef,  # (1)
    ConnectionProperties: Dict[str, PropertyTypeDef],  # (2)
    ConnectionOptions: Dict[str, PropertyTypeDef],  # (2)
    AuthenticationConfiguration: AuthConfigurationTypeDef,  # (4)
    ComputeEnvironmentConfigurations: Dict[str, ComputeEnvironmentConfigurationTypeDef],  # (5)
    PhysicalConnectionRequirements: Dict[str, PropertyTypeDef],  # (2)
    AthenaConnectionProperties: Dict[str, PropertyTypeDef],  # (2)
    PythonConnectionProperties: Dict[str, PropertyTypeDef],  # (2)
    SparkConnectionProperties: Dict[str, PropertyTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-braces: CapabilitiesTypeDef](./type_defs.md#capabilitiestypedef) 
2. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
3. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
4. See [:material-code-braces: AuthConfigurationTypeDef](./type_defs.md#authconfigurationtypedef) 
5. See [:material-code-braces: ComputeEnvironmentConfigurationTypeDef](./type_defs.md#computeenvironmentconfigurationtypedef) 
6. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
7. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
8. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
9. See [:material-code-braces: PropertyTypeDef](./type_defs.md#propertytypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AmazonRedshiftSourceTypeDef

```python
# AmazonRedshiftSourceTypeDef definition

class AmazonRedshiftSourceTypeDef(TypedDict):
    Name: NotRequired[str],
    Data: NotRequired[AmazonRedshiftNodeDataUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AmazonRedshiftNodeDataTypeDef](./type_defs.md#amazonredshiftnodedatatypedef) [:material-code-braces: AmazonRedshiftNodeDataOutputTypeDef](./type_defs.md#amazonredshiftnodedataoutputtypedef) 
## AmazonRedshiftTargetTypeDef

```python
# AmazonRedshiftTargetTypeDef definition

class AmazonRedshiftTargetTypeDef(TypedDict):
    Name: NotRequired[str],
    Data: NotRequired[AmazonRedshiftNodeDataUnionTypeDef],  # (1)
    Inputs: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: AmazonRedshiftNodeDataTypeDef](./type_defs.md#amazonredshiftnodedatatypedef) [:material-code-braces: AmazonRedshiftNodeDataOutputTypeDef](./type_defs.md#amazonredshiftnodedataoutputtypedef) 
## SnowflakeTargetTypeDef

```python
# SnowflakeTargetTypeDef definition

class SnowflakeTargetTypeDef(TypedDict):
    Name: str,
    Data: SnowflakeNodeDataUnionTypeDef,  # (1)
    Inputs: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: SnowflakeNodeDataTypeDef](./type_defs.md#snowflakenodedatatypedef) [:material-code-braces: SnowflakeNodeDataOutputTypeDef](./type_defs.md#snowflakenodedataoutputtypedef) 
## GetPartitionIndexesResponseTypeDef

```python
# GetPartitionIndexesResponseTypeDef definition

class GetPartitionIndexesResponseTypeDef(TypedDict):
    PartitionIndexDescriptorList: List[PartitionIndexDescriptorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PartitionIndexDescriptorTypeDef](./type_defs.md#partitionindexdescriptortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableStatusPaginatorTypeDef

```python
# TableStatusPaginatorTypeDef definition

class TableStatusPaginatorTypeDef(TypedDict):
    RequestedBy: NotRequired[str],
    UpdatedBy: NotRequired[str],
    RequestTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
    Action: NotRequired[ResourceActionType],  # (1)
    State: NotRequired[ResourceStateType],  # (2)
    Error: NotRequired[ErrorDetailTypeDef],  # (3)
    Details: NotRequired[StatusDetailsPaginatorTypeDef],  # (4)
```

1. See [:material-code-brackets: ResourceActionType](./literals.md#resourceactiontype) 
2. See [:material-code-brackets: ResourceStateType](./literals.md#resourcestatetype) 
3. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
4. See [:material-code-braces: StatusDetailsPaginatorTypeDef](./type_defs.md#statusdetailspaginatortypedef) 
## TableStatusTypeDef

```python
# TableStatusTypeDef definition

class TableStatusTypeDef(TypedDict):
    RequestedBy: NotRequired[str],
    UpdatedBy: NotRequired[str],
    RequestTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
    Action: NotRequired[ResourceActionType],  # (1)
    State: NotRequired[ResourceStateType],  # (2)
    Error: NotRequired[ErrorDetailTypeDef],  # (3)
    Details: NotRequired[StatusDetailsTypeDef],  # (4)
```

1. See [:material-code-brackets: ResourceActionType](./literals.md#resourceactiontype) 
2. See [:material-code-brackets: ResourceStateType](./literals.md#resourcestatetype) 
3. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
4. See [:material-code-braces: StatusDetailsTypeDef](./type_defs.md#statusdetailstypedef) 
## DecimalColumnStatisticsDataTypeDef

```python
# DecimalColumnStatisticsDataTypeDef definition

class DecimalColumnStatisticsDataTypeDef(TypedDict):
    NumberOfNulls: int,
    NumberOfDistinctValues: int,
    MinimumValue: NotRequired[DecimalNumberUnionTypeDef],  # (1)
    MaximumValue: NotRequired[DecimalNumberUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DecimalNumberTypeDef](./type_defs.md#decimalnumbertypedef) [:material-code-braces: DecimalNumberOutputTypeDef](./type_defs.md#decimalnumberoutputtypedef) 
2. See [:material-code-braces: DecimalNumberTypeDef](./type_defs.md#decimalnumbertypedef) [:material-code-braces: DecimalNumberOutputTypeDef](./type_defs.md#decimalnumberoutputtypedef) 
## CreateScriptRequestRequestTypeDef

```python
# CreateScriptRequestRequestTypeDef definition

class CreateScriptRequestRequestTypeDef(TypedDict):
    DagNodes: NotRequired[Sequence[CodeGenNodeUnionTypeDef]],  # (1)
    DagEdges: NotRequired[Sequence[CodeGenEdgeTypeDef]],  # (2)
    Language: NotRequired[LanguageType],  # (3)
```

1. See [:material-code-braces: CodeGenNodeTypeDef](./type_defs.md#codegennodetypedef) [:material-code-braces: CodeGenNodeOutputTypeDef](./type_defs.md#codegennodeoutputtypedef) 
2. See [:material-code-braces: CodeGenEdgeTypeDef](./type_defs.md#codegenedgetypedef) 
3. See [:material-code-brackets: LanguageType](./literals.md#languagetype) 
## CatalogKafkaSourceTypeDef

```python
# CatalogKafkaSourceTypeDef definition

class CatalogKafkaSourceTypeDef(TypedDict):
    Name: str,
    Table: str,
    Database: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KafkaStreamingSourceOptionsUnionTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KafkaStreamingSourceOptionsTypeDef](./type_defs.md#kafkastreamingsourceoptionstypedef) [:material-code-braces: KafkaStreamingSourceOptionsOutputTypeDef](./type_defs.md#kafkastreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## DirectKafkaSourceTypeDef

```python
# DirectKafkaSourceTypeDef definition

class DirectKafkaSourceTypeDef(TypedDict):
    Name: str,
    StreamingOptions: NotRequired[KafkaStreamingSourceOptionsUnionTypeDef],  # (1)
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KafkaStreamingSourceOptionsTypeDef](./type_defs.md#kafkastreamingsourceoptionstypedef) [:material-code-braces: KafkaStreamingSourceOptionsOutputTypeDef](./type_defs.md#kafkastreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## CatalogKinesisSourceTypeDef

```python
# CatalogKinesisSourceTypeDef definition

class CatalogKinesisSourceTypeDef(TypedDict):
    Name: str,
    Table: str,
    Database: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KinesisStreamingSourceOptionsUnionTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisStreamingSourceOptionsTypeDef](./type_defs.md#kinesisstreamingsourceoptionstypedef) [:material-code-braces: KinesisStreamingSourceOptionsOutputTypeDef](./type_defs.md#kinesisstreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## DirectKinesisSourceTypeDef

```python
# DirectKinesisSourceTypeDef definition

class DirectKinesisSourceTypeDef(TypedDict):
    Name: str,
    WindowSize: NotRequired[int],
    DetectSchema: NotRequired[bool],
    StreamingOptions: NotRequired[KinesisStreamingSourceOptionsUnionTypeDef],  # (1)
    DataPreviewOptions: NotRequired[StreamingDataPreviewOptionsTypeDef],  # (2)
```

1. See [:material-code-braces: KinesisStreamingSourceOptionsTypeDef](./type_defs.md#kinesisstreamingsourceoptionstypedef) [:material-code-braces: KinesisStreamingSourceOptionsOutputTypeDef](./type_defs.md#kinesisstreamingsourceoptionsoutputtypedef) 
2. See [:material-code-braces: StreamingDataPreviewOptionsTypeDef](./type_defs.md#streamingdatapreviewoptionstypedef) 
## BatchGetTriggersResponseTypeDef

```python
# BatchGetTriggersResponseTypeDef definition

class BatchGetTriggersResponseTypeDef(TypedDict):
    Triggers: List[TriggerTypeDef],  # (1)
    TriggersNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTriggerResponseTypeDef

```python
# GetTriggerResponseTypeDef definition

class GetTriggerResponseTypeDef(TypedDict):
    Trigger: TriggerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTriggersResponseTypeDef

```python
# GetTriggersResponseTypeDef definition

class GetTriggersResponseTypeDef(TypedDict):
    Triggers: List[TriggerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TriggerNodeDetailsTypeDef

```python
# TriggerNodeDetailsTypeDef definition

class TriggerNodeDetailsTypeDef(TypedDict):
    Trigger: NotRequired[TriggerTypeDef],  # (1)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
## UpdateTriggerResponseTypeDef

```python
# UpdateTriggerResponseTypeDef definition

class UpdateTriggerResponseTypeDef(TypedDict):
    Trigger: TriggerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TriggerTypeDef](./type_defs.md#triggertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TriggerUpdateTypeDef

```python
# TriggerUpdateTypeDef definition

class TriggerUpdateTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    Actions: NotRequired[Sequence[ActionUnionTypeDef]],  # (1)
    Predicate: NotRequired[PredicateUnionTypeDef],  # (2)
    EventBatchingCondition: NotRequired[EventBatchingConditionTypeDef],  # (3)
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
2. See [:material-code-braces: PredicateTypeDef](./type_defs.md#predicatetypedef) [:material-code-braces: PredicateOutputTypeDef](./type_defs.md#predicateoutputtypedef) 
3. See [:material-code-braces: EventBatchingConditionTypeDef](./type_defs.md#eventbatchingconditiontypedef) 
## CreateUsageProfileRequestRequestTypeDef

```python
# CreateUsageProfileRequestRequestTypeDef definition

class CreateUsageProfileRequestRequestTypeDef(TypedDict):
    Name: str,
    Configuration: ProfileConfigurationTypeDef,  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ProfileConfigurationTypeDef](./type_defs.md#profileconfigurationtypedef) 
## UpdateUsageProfileRequestRequestTypeDef

```python
# UpdateUsageProfileRequestRequestTypeDef definition

class UpdateUsageProfileRequestRequestTypeDef(TypedDict):
    Name: str,
    Configuration: ProfileConfigurationTypeDef,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ProfileConfigurationTypeDef](./type_defs.md#profileconfigurationtypedef) 
## GetMLTransformResponseTypeDef

```python
# GetMLTransformResponseTypeDef definition

class GetMLTransformResponseTypeDef(TypedDict):
    TransformId: str,
    Name: str,
    Description: str,
    Status: TransformStatusTypeType,  # (1)
    CreatedOn: datetime,
    LastModifiedOn: datetime,
    InputRecordTables: List[GlueTableOutputTypeDef],  # (2)
    Parameters: TransformParametersTypeDef,  # (3)
    EvaluationMetrics: EvaluationMetricsTypeDef,  # (4)
    LabelCount: int,
    Schema: List[SchemaColumnTypeDef],  # (5)
    Role: str,
    GlueVersion: str,
    MaxCapacity: float,
    WorkerType: WorkerTypeType,  # (6)
    NumberOfWorkers: int,
    Timeout: int,
    MaxRetries: int,
    TransformEncryption: TransformEncryptionTypeDef,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: TransformStatusTypeType](./literals.md#transformstatustypetype) 
2. See [:material-code-braces: GlueTableOutputTypeDef](./type_defs.md#gluetableoutputtypedef) 
3. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
4. See [:material-code-braces: EvaluationMetricsTypeDef](./type_defs.md#evaluationmetricstypedef) 
5. See [:material-code-braces: SchemaColumnTypeDef](./type_defs.md#schemacolumntypedef) 
6. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
7. See [:material-code-braces: TransformEncryptionTypeDef](./type_defs.md#transformencryptiontypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MLTransformTypeDef

```python
# MLTransformTypeDef definition

class MLTransformTypeDef(TypedDict):
    TransformId: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[TransformStatusTypeType],  # (1)
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    InputRecordTables: NotRequired[List[GlueTableOutputTypeDef]],  # (2)
    Parameters: NotRequired[TransformParametersTypeDef],  # (3)
    EvaluationMetrics: NotRequired[EvaluationMetricsTypeDef],  # (4)
    LabelCount: NotRequired[int],
    Schema: NotRequired[List[SchemaColumnTypeDef]],  # (5)
    Role: NotRequired[str],
    GlueVersion: NotRequired[str],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (6)
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    MaxRetries: NotRequired[int],
    TransformEncryption: NotRequired[TransformEncryptionTypeDef],  # (7)
```

1. See [:material-code-brackets: TransformStatusTypeType](./literals.md#transformstatustypetype) 
2. See [:material-code-braces: GlueTableOutputTypeDef](./type_defs.md#gluetableoutputtypedef) 
3. See [:material-code-braces: TransformParametersTypeDef](./type_defs.md#transformparameterstypedef) 
4. See [:material-code-braces: EvaluationMetricsTypeDef](./type_defs.md#evaluationmetricstypedef) 
5. See [:material-code-braces: SchemaColumnTypeDef](./type_defs.md#schemacolumntypedef) 
6. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
7. See [:material-code-braces: TransformEncryptionTypeDef](./type_defs.md#transformencryptiontypedef) 
## BatchGetCrawlersResponseTypeDef

```python
# BatchGetCrawlersResponseTypeDef definition

class BatchGetCrawlersResponseTypeDef(TypedDict):
    Crawlers: List[CrawlerTypeDef],  # (1)
    CrawlersNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrawlerTypeDef](./type_defs.md#crawlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCrawlerResponseTypeDef

```python
# GetCrawlerResponseTypeDef definition

class GetCrawlerResponseTypeDef(TypedDict):
    Crawler: CrawlerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CrawlerTypeDef](./type_defs.md#crawlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCrawlersResponseTypeDef

```python
# GetCrawlersResponseTypeDef definition

class GetCrawlersResponseTypeDef(TypedDict):
    Crawlers: List[CrawlerTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CrawlerTypeDef](./type_defs.md#crawlertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCatalogResponseTypeDef

```python
# GetCatalogResponseTypeDef definition

class GetCatalogResponseTypeDef(TypedDict):
    Catalog: CatalogTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CatalogTypeDef](./type_defs.md#catalogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCatalogsResponseTypeDef

```python
# GetCatalogsResponseTypeDef definition

class GetCatalogsResponseTypeDef(TypedDict):
    CatalogList: List[CatalogTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CatalogTypeDef](./type_defs.md#catalogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDatabaseResponseTypeDef

```python
# GetDatabaseResponseTypeDef definition

class GetDatabaseResponseTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDatabasesResponseTypeDef

```python
# GetDatabasesResponseTypeDef definition

class GetDatabasesResponseTypeDef(TypedDict):
    DatabaseList: List[DatabaseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CatalogInputTypeDef

```python
# CatalogInputTypeDef definition

class CatalogInputTypeDef(TypedDict):
    Description: NotRequired[str],
    FederatedCatalog: NotRequired[FederatedCatalogTypeDef],  # (1)
    Parameters: NotRequired[Mapping[str, str]],
    TargetRedshiftCatalog: NotRequired[TargetRedshiftCatalogTypeDef],  # (2)
    CatalogProperties: NotRequired[CatalogPropertiesTypeDef],  # (3)
    CreateTableDefaultPermissions: NotRequired[Sequence[PrincipalPermissionsUnionTypeDef]],  # (4)
    CreateDatabaseDefaultPermissions: NotRequired[Sequence[PrincipalPermissionsTypeDef]],  # (5)
```

1. See [:material-code-braces: FederatedCatalogTypeDef](./type_defs.md#federatedcatalogtypedef) 
2. See [:material-code-braces: TargetRedshiftCatalogTypeDef](./type_defs.md#targetredshiftcatalogtypedef) 
3. See [:material-code-braces: CatalogPropertiesTypeDef](./type_defs.md#catalogpropertiestypedef) 
4. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
5. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) 
## DatabaseInputTypeDef

```python
# DatabaseInputTypeDef definition

class DatabaseInputTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    LocationUri: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    CreateTableDefaultPermissions: NotRequired[Sequence[PrincipalPermissionsUnionTypeDef]],  # (1)
    TargetDatabase: NotRequired[DatabaseIdentifierTypeDef],  # (2)
    FederatedDatabase: NotRequired[FederatedDatabaseTypeDef],  # (3)
```

1. See [:material-code-braces: PrincipalPermissionsTypeDef](./type_defs.md#principalpermissionstypedef) [:material-code-braces: PrincipalPermissionsOutputTypeDef](./type_defs.md#principalpermissionsoutputtypedef) 
2. See [:material-code-braces: DatabaseIdentifierTypeDef](./type_defs.md#databaseidentifiertypedef) 
3. See [:material-code-braces: FederatedDatabaseTypeDef](./type_defs.md#federateddatabasetypedef) 
## DataQualityResultTypeDef

```python
# DataQualityResultTypeDef definition

class DataQualityResultTypeDef(TypedDict):
    ResultId: NotRequired[str],
    ProfileId: NotRequired[str],
    Score: NotRequired[float],
    DataSource: NotRequired[DataSourceOutputTypeDef],  # (1)
    RulesetName: NotRequired[str],
    EvaluationContext: NotRequired[str],
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    RulesetEvaluationRunId: NotRequired[str],
    RuleResults: NotRequired[List[DataQualityRuleResultTypeDef]],  # (2)
    AnalyzerResults: NotRequired[List[DataQualityAnalyzerResultTypeDef]],  # (3)
    Observations: NotRequired[List[DataQualityObservationTypeDef]],  # (4)
```

1. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
2. See [:material-code-braces: DataQualityRuleResultTypeDef](./type_defs.md#dataqualityruleresulttypedef) 
3. See [:material-code-braces: DataQualityAnalyzerResultTypeDef](./type_defs.md#dataqualityanalyzerresulttypedef) 
4. See [:material-code-braces: DataQualityObservationTypeDef](./type_defs.md#dataqualityobservationtypedef) 
## GetDataQualityResultResponseTypeDef

```python
# GetDataQualityResultResponseTypeDef definition

class GetDataQualityResultResponseTypeDef(TypedDict):
    ResultId: str,
    ProfileId: str,
    Score: float,
    DataSource: DataSourceOutputTypeDef,  # (1)
    RulesetName: str,
    EvaluationContext: str,
    StartedOn: datetime,
    CompletedOn: datetime,
    JobName: str,
    JobRunId: str,
    RulesetEvaluationRunId: str,
    RuleResults: List[DataQualityRuleResultTypeDef],  # (2)
    AnalyzerResults: List[DataQualityAnalyzerResultTypeDef],  # (3)
    Observations: List[DataQualityObservationTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
2. See [:material-code-braces: DataQualityRuleResultTypeDef](./type_defs.md#dataqualityruleresulttypedef) 
3. See [:material-code-braces: DataQualityAnalyzerResultTypeDef](./type_defs.md#dataqualityanalyzerresulttypedef) 
4. See [:material-code-braces: DataQualityObservationTypeDef](./type_defs.md#dataqualityobservationtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityResultsResponseTypeDef

```python
# ListDataQualityResultsResponseTypeDef definition

class ListDataQualityResultsResponseTypeDef(TypedDict):
    Results: List[DataQualityResultDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataQualityResultDescriptionTypeDef](./type_defs.md#dataqualityresultdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityRuleRecommendationRunsResponseTypeDef

```python
# ListDataQualityRuleRecommendationRunsResponseTypeDef definition

class ListDataQualityRuleRecommendationRunsResponseTypeDef(TypedDict):
    Runs: List[DataQualityRuleRecommendationRunDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataQualityRuleRecommendationRunDescriptionTypeDef](./type_defs.md#dataqualityrulerecommendationrundescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityRulesetEvaluationRunsResponseTypeDef

```python
# ListDataQualityRulesetEvaluationRunsResponseTypeDef definition

class ListDataQualityRulesetEvaluationRunsResponseTypeDef(TypedDict):
    Runs: List[DataQualityRulesetEvaluationRunDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataQualityRulesetEvaluationRunDescriptionTypeDef](./type_defs.md#dataqualityrulesetevaluationrundescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ColumnStatisticsOutputTypeDef

```python
# ColumnStatisticsOutputTypeDef definition

class ColumnStatisticsOutputTypeDef(TypedDict):
    ColumnName: str,
    ColumnType: str,
    AnalyzedTime: datetime,
    StatisticsData: ColumnStatisticsDataOutputTypeDef,  # (1)
```

1. See [:material-code-braces: ColumnStatisticsDataOutputTypeDef](./type_defs.md#columnstatisticsdataoutputtypedef) 
## PartitionTypeDef

```python
# PartitionTypeDef definition

class PartitionTypeDef(TypedDict):
    Values: NotRequired[List[str]],
    DatabaseName: NotRequired[str],
    TableName: NotRequired[str],
    CreationTime: NotRequired[datetime],
    LastAccessTime: NotRequired[datetime],
    StorageDescriptor: NotRequired[StorageDescriptorOutputTypeDef],  # (1)
    Parameters: NotRequired[Dict[str, str]],
    LastAnalyzedTime: NotRequired[datetime],
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: StorageDescriptorOutputTypeDef](./type_defs.md#storagedescriptoroutputtypedef) 
## GetSecurityConfigurationResponseTypeDef

```python
# GetSecurityConfigurationResponseTypeDef definition

class GetSecurityConfigurationResponseTypeDef(TypedDict):
    SecurityConfiguration: SecurityConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SecurityConfigurationTypeDef](./type_defs.md#securityconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSecurityConfigurationsResponseTypeDef

```python
# GetSecurityConfigurationsResponseTypeDef definition

class GetSecurityConfigurationsResponseTypeDef(TypedDict):
    SecurityConfigurations: List[SecurityConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecurityConfigurationTypeDef](./type_defs.md#securityconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectorDataSourceTypeDef

```python
# ConnectorDataSourceTypeDef definition

class ConnectorDataSourceTypeDef(TypedDict):
    Name: str,
    ConnectionType: str,
    Data: Mapping[str, str],
    OutputSchemas: NotRequired[Sequence[GlueSchemaUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## SnowflakeSourceTypeDef

```python
# SnowflakeSourceTypeDef definition

class SnowflakeSourceTypeDef(TypedDict):
    Name: str,
    Data: SnowflakeNodeDataUnionTypeDef,  # (1)
    OutputSchemas: NotRequired[Sequence[GlueSchemaUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: SnowflakeNodeDataTypeDef](./type_defs.md#snowflakenodedatatypedef) [:material-code-braces: SnowflakeNodeDataOutputTypeDef](./type_defs.md#snowflakenodedataoutputtypedef) 
2. See [:material-code-braces: GlueSchemaTypeDef](./type_defs.md#glueschematypedef) [:material-code-braces: GlueSchemaOutputTypeDef](./type_defs.md#glueschemaoutputtypedef) 
## StartDataQualityRuleRecommendationRunRequestRequestTypeDef

```python
# StartDataQualityRuleRecommendationRunRequestRequestTypeDef definition

class StartDataQualityRuleRecommendationRunRequestRequestTypeDef(TypedDict):
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    CreatedRulesetName: NotRequired[str],
    DataQualitySecurityConfiguration: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
## CreateTableOptimizerRequestRequestTypeDef

```python
# CreateTableOptimizerRequestRequestTypeDef definition

class CreateTableOptimizerRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,  # (2)
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: TableOptimizerConfigurationTypeDef](./type_defs.md#tableoptimizerconfigurationtypedef) 
## UpdateTableOptimizerRequestRequestTypeDef

```python
# UpdateTableOptimizerRequestRequestTypeDef definition

class UpdateTableOptimizerRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    Type: TableOptimizerTypeType,  # (1)
    TableOptimizerConfiguration: TableOptimizerConfigurationTypeDef,  # (2)
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: TableOptimizerConfigurationTypeDef](./type_defs.md#tableoptimizerconfigurationtypedef) 
## ListTableOptimizerRunsResponseTypeDef

```python
# ListTableOptimizerRunsResponseTypeDef definition

class ListTableOptimizerRunsResponseTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    TableOptimizerRuns: List[TableOptimizerRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableOptimizerRunTypeDef](./type_defs.md#tableoptimizerruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableOptimizerTypeDef

```python
# TableOptimizerTypeDef definition

class TableOptimizerTypeDef(TypedDict):
    type: NotRequired[TableOptimizerTypeType],  # (1)
    configuration: NotRequired[TableOptimizerConfigurationTypeDef],  # (2)
    lastRun: NotRequired[TableOptimizerRunTypeDef],  # (3)
```

1. See [:material-code-brackets: TableOptimizerTypeType](./literals.md#tableoptimizertypetype) 
2. See [:material-code-braces: TableOptimizerConfigurationTypeDef](./type_defs.md#tableoptimizerconfigurationtypedef) 
3. See [:material-code-braces: TableOptimizerRunTypeDef](./type_defs.md#tableoptimizerruntypedef) 
## GetMLTaskRunsResponseTypeDef

```python
# GetMLTaskRunsResponseTypeDef definition

class GetMLTaskRunsResponseTypeDef(TypedDict):
    TaskRuns: List[TaskRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TaskRunTypeDef](./type_defs.md#taskruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionTypeDef

```python
# ConnectionTypeDef definition

class ConnectionTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    ConnectionType: NotRequired[ConnectionTypeType],  # (1)
    MatchCriteria: NotRequired[List[str]],
    ConnectionProperties: NotRequired[Dict[ConnectionPropertyKeyType, str]],  # (2)
    SparkProperties: NotRequired[Dict[str, str]],
    AthenaProperties: NotRequired[Dict[str, str]],
    PythonProperties: NotRequired[Dict[str, str]],
    PhysicalConnectionRequirements: NotRequired[PhysicalConnectionRequirementsOutputTypeDef],  # (3)
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    LastUpdatedBy: NotRequired[str],
    Status: NotRequired[ConnectionStatusType],  # (4)
    StatusReason: NotRequired[str],
    LastConnectionValidationTime: NotRequired[datetime],
    AuthenticationConfiguration: NotRequired[AuthenticationConfigurationTypeDef],  # (5)
    ConnectionSchemaVersion: NotRequired[int],
    CompatibleComputeEnvironments: NotRequired[List[ComputeEnvironmentType]],  # (6)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ConnectionPropertyKeyType](./literals.md#connectionpropertykeytype) 
3. See [:material-code-braces: PhysicalConnectionRequirementsOutputTypeDef](./type_defs.md#physicalconnectionrequirementsoutputtypedef) 
4. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
5. See [:material-code-braces: AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef) 
6. See [:material-code-brackets: ComputeEnvironmentType](./literals.md#computeenvironmenttype) 
## ConnectionInputTypeDef

```python
# ConnectionInputTypeDef definition

class ConnectionInputTypeDef(TypedDict):
    Name: str,
    ConnectionType: ConnectionTypeType,  # (1)
    ConnectionProperties: Mapping[ConnectionPropertyKeyType, str],  # (2)
    Description: NotRequired[str],
    MatchCriteria: NotRequired[Sequence[str]],
    SparkProperties: NotRequired[Mapping[str, str]],
    AthenaProperties: NotRequired[Mapping[str, str]],
    PythonProperties: NotRequired[Mapping[str, str]],
    PhysicalConnectionRequirements: NotRequired[PhysicalConnectionRequirementsUnionTypeDef],  # (3)
    AuthenticationConfiguration: NotRequired[AuthenticationConfigurationInputTypeDef],  # (4)
    ValidateCredentials: NotRequired[bool],
    ValidateForComputeEnvironments: NotRequired[Sequence[ComputeEnvironmentType]],  # (5)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ConnectionPropertyKeyType](./literals.md#connectionpropertykeytype) 
3. See [:material-code-braces: PhysicalConnectionRequirementsTypeDef](./type_defs.md#physicalconnectionrequirementstypedef) [:material-code-braces: PhysicalConnectionRequirementsOutputTypeDef](./type_defs.md#physicalconnectionrequirementsoutputtypedef) 
4. See [:material-code-braces: AuthenticationConfigurationInputTypeDef](./type_defs.md#authenticationconfigurationinputtypedef) 
5. See [:material-code-brackets: ComputeEnvironmentType](./literals.md#computeenvironmenttype) 
## TestConnectionInputTypeDef

```python
# TestConnectionInputTypeDef definition

class TestConnectionInputTypeDef(TypedDict):
    ConnectionType: ConnectionTypeType,  # (1)
    ConnectionProperties: Mapping[ConnectionPropertyKeyType, str],  # (2)
    AuthenticationConfiguration: NotRequired[AuthenticationConfigurationInputTypeDef],  # (3)
```

1. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
2. See [:material-code-brackets: ConnectionPropertyKeyType](./literals.md#connectionpropertykeytype) 
3. See [:material-code-braces: AuthenticationConfigurationInputTypeDef](./type_defs.md#authenticationconfigurationinputtypedef) 
## CodeGenConfigurationNodeOutputTypeDef

```python
# CodeGenConfigurationNodeOutputTypeDef definition

class CodeGenConfigurationNodeOutputTypeDef(TypedDict):
    AthenaConnectorSource: NotRequired[AthenaConnectorSourceOutputTypeDef],  # (1)
    JDBCConnectorSource: NotRequired[JDBCConnectorSourceOutputTypeDef],  # (2)
    SparkConnectorSource: NotRequired[SparkConnectorSourceOutputTypeDef],  # (3)
    CatalogSource: NotRequired[CatalogSourceTypeDef],  # (4)
    RedshiftSource: NotRequired[RedshiftSourceTypeDef],  # (5)
    S3CatalogSource: NotRequired[S3CatalogSourceTypeDef],  # (6)
    S3CsvSource: NotRequired[S3CsvSourceOutputTypeDef],  # (7)
    S3JsonSource: NotRequired[S3JsonSourceOutputTypeDef],  # (8)
    S3ParquetSource: NotRequired[S3ParquetSourceOutputTypeDef],  # (9)
    RelationalCatalogSource: NotRequired[RelationalCatalogSourceTypeDef],  # (10)
    DynamoDBCatalogSource: NotRequired[DynamoDBCatalogSourceTypeDef],  # (11)
    JDBCConnectorTarget: NotRequired[JDBCConnectorTargetOutputTypeDef],  # (12)
    SparkConnectorTarget: NotRequired[SparkConnectorTargetOutputTypeDef],  # (13)
    CatalogTarget: NotRequired[BasicCatalogTargetOutputTypeDef],  # (14)
    RedshiftTarget: NotRequired[RedshiftTargetOutputTypeDef],  # (15)
    S3CatalogTarget: NotRequired[S3CatalogTargetOutputTypeDef],  # (16)
    S3GlueParquetTarget: NotRequired[S3GlueParquetTargetOutputTypeDef],  # (17)
    S3DirectTarget: NotRequired[S3DirectTargetOutputTypeDef],  # (18)
    ApplyMapping: NotRequired[ApplyMappingOutputTypeDef],  # (19)
    SelectFields: NotRequired[SelectFieldsOutputTypeDef],  # (20)
    DropFields: NotRequired[DropFieldsOutputTypeDef],  # (21)
    RenameField: NotRequired[RenameFieldOutputTypeDef],  # (22)
    Spigot: NotRequired[SpigotOutputTypeDef],  # (23)
    Join: NotRequired[JoinOutputTypeDef],  # (24)
    SplitFields: NotRequired[SplitFieldsOutputTypeDef],  # (25)
    SelectFromCollection: NotRequired[SelectFromCollectionOutputTypeDef],  # (26)
    FillMissingValues: NotRequired[FillMissingValuesOutputTypeDef],  # (27)
    Filter: NotRequired[FilterOutputTypeDef],  # (28)
    CustomCode: NotRequired[CustomCodeOutputTypeDef],  # (29)
    SparkSQL: NotRequired[SparkSQLOutputTypeDef],  # (30)
    DirectKinesisSource: NotRequired[DirectKinesisSourceOutputTypeDef],  # (31)
    DirectKafkaSource: NotRequired[DirectKafkaSourceOutputTypeDef],  # (32)
    CatalogKinesisSource: NotRequired[CatalogKinesisSourceOutputTypeDef],  # (33)
    CatalogKafkaSource: NotRequired[CatalogKafkaSourceOutputTypeDef],  # (34)
    DropNullFields: NotRequired[DropNullFieldsOutputTypeDef],  # (35)
    Merge: NotRequired[MergeOutputTypeDef],  # (36)
    Union: NotRequired[UnionOutputTypeDef],  # (37)
    PIIDetection: NotRequired[PIIDetectionOutputTypeDef],  # (38)
    Aggregate: NotRequired[AggregateOutputTypeDef],  # (39)
    DropDuplicates: NotRequired[DropDuplicatesOutputTypeDef],  # (40)
    GovernedCatalogTarget: NotRequired[GovernedCatalogTargetOutputTypeDef],  # (41)
    GovernedCatalogSource: NotRequired[GovernedCatalogSourceTypeDef],  # (42)
    MicrosoftSQLServerCatalogSource: NotRequired[MicrosoftSQLServerCatalogSourceTypeDef],  # (43)
    MySQLCatalogSource: NotRequired[MySQLCatalogSourceTypeDef],  # (44)
    OracleSQLCatalogSource: NotRequired[OracleSQLCatalogSourceTypeDef],  # (45)
    PostgreSQLCatalogSource: NotRequired[PostgreSQLCatalogSourceTypeDef],  # (46)
    MicrosoftSQLServerCatalogTarget: NotRequired[MicrosoftSQLServerCatalogTargetOutputTypeDef],  # (47)
    MySQLCatalogTarget: NotRequired[MySQLCatalogTargetOutputTypeDef],  # (48)
    OracleSQLCatalogTarget: NotRequired[OracleSQLCatalogTargetOutputTypeDef],  # (49)
    PostgreSQLCatalogTarget: NotRequired[PostgreSQLCatalogTargetOutputTypeDef],  # (50)
    DynamicTransform: NotRequired[DynamicTransformOutputTypeDef],  # (51)
    EvaluateDataQuality: NotRequired[EvaluateDataQualityOutputTypeDef],  # (52)
    S3CatalogHudiSource: NotRequired[S3CatalogHudiSourceOutputTypeDef],  # (53)
    CatalogHudiSource: NotRequired[CatalogHudiSourceOutputTypeDef],  # (54)
    S3HudiSource: NotRequired[S3HudiSourceOutputTypeDef],  # (55)
    S3HudiCatalogTarget: NotRequired[S3HudiCatalogTargetOutputTypeDef],  # (56)
    S3HudiDirectTarget: NotRequired[S3HudiDirectTargetOutputTypeDef],  # (57)
    DirectJDBCSource: NotRequired[DirectJDBCSourceTypeDef],  # (58)
    S3CatalogDeltaSource: NotRequired[S3CatalogDeltaSourceOutputTypeDef],  # (59)
    CatalogDeltaSource: NotRequired[CatalogDeltaSourceOutputTypeDef],  # (60)
    S3DeltaSource: NotRequired[S3DeltaSourceOutputTypeDef],  # (61)
    S3DeltaCatalogTarget: NotRequired[S3DeltaCatalogTargetOutputTypeDef],  # (62)
    S3DeltaDirectTarget: NotRequired[S3DeltaDirectTargetOutputTypeDef],  # (63)
    AmazonRedshiftSource: NotRequired[AmazonRedshiftSourceOutputTypeDef],  # (64)
    AmazonRedshiftTarget: NotRequired[AmazonRedshiftTargetOutputTypeDef],  # (65)
    EvaluateDataQualityMultiFrame: NotRequired[EvaluateDataQualityMultiFrameOutputTypeDef],  # (66)
    Recipe: NotRequired[RecipeOutputTypeDef],  # (67)
    SnowflakeSource: NotRequired[SnowflakeSourceOutputTypeDef],  # (68)
    SnowflakeTarget: NotRequired[SnowflakeTargetOutputTypeDef],  # (69)
    ConnectorDataSource: NotRequired[ConnectorDataSourceOutputTypeDef],  # (70)
    ConnectorDataTarget: NotRequired[ConnectorDataTargetOutputTypeDef],  # (71)
```

1. See [:material-code-braces: AthenaConnectorSourceOutputTypeDef](./type_defs.md#athenaconnectorsourceoutputtypedef) 
2. See [:material-code-braces: JDBCConnectorSourceOutputTypeDef](./type_defs.md#jdbcconnectorsourceoutputtypedef) 
3. See [:material-code-braces: SparkConnectorSourceOutputTypeDef](./type_defs.md#sparkconnectorsourceoutputtypedef) 
4. See [:material-code-braces: CatalogSourceTypeDef](./type_defs.md#catalogsourcetypedef) 
5. See [:material-code-braces: RedshiftSourceTypeDef](./type_defs.md#redshiftsourcetypedef) 
6. See [:material-code-braces: S3CatalogSourceTypeDef](./type_defs.md#s3catalogsourcetypedef) 
7. See [:material-code-braces: S3CsvSourceOutputTypeDef](./type_defs.md#s3csvsourceoutputtypedef) 
8. See [:material-code-braces: S3JsonSourceOutputTypeDef](./type_defs.md#s3jsonsourceoutputtypedef) 
9. See [:material-code-braces: S3ParquetSourceOutputTypeDef](./type_defs.md#s3parquetsourceoutputtypedef) 
10. See [:material-code-braces: RelationalCatalogSourceTypeDef](./type_defs.md#relationalcatalogsourcetypedef) 
11. See [:material-code-braces: DynamoDBCatalogSourceTypeDef](./type_defs.md#dynamodbcatalogsourcetypedef) 
12. See [:material-code-braces: JDBCConnectorTargetOutputTypeDef](./type_defs.md#jdbcconnectortargetoutputtypedef) 
13. See [:material-code-braces: SparkConnectorTargetOutputTypeDef](./type_defs.md#sparkconnectortargetoutputtypedef) 
14. See [:material-code-braces: BasicCatalogTargetOutputTypeDef](./type_defs.md#basiccatalogtargetoutputtypedef) 
15. See [:material-code-braces: RedshiftTargetOutputTypeDef](./type_defs.md#redshifttargetoutputtypedef) 
16. See [:material-code-braces: S3CatalogTargetOutputTypeDef](./type_defs.md#s3catalogtargetoutputtypedef) 
17. See [:material-code-braces: S3GlueParquetTargetOutputTypeDef](./type_defs.md#s3glueparquettargetoutputtypedef) 
18. See [:material-code-braces: S3DirectTargetOutputTypeDef](./type_defs.md#s3directtargetoutputtypedef) 
19. See [:material-code-braces: ApplyMappingOutputTypeDef](./type_defs.md#applymappingoutputtypedef) 
20. See [:material-code-braces: SelectFieldsOutputTypeDef](./type_defs.md#selectfieldsoutputtypedef) 
21. See [:material-code-braces: DropFieldsOutputTypeDef](./type_defs.md#dropfieldsoutputtypedef) 
22. See [:material-code-braces: RenameFieldOutputTypeDef](./type_defs.md#renamefieldoutputtypedef) 
23. See [:material-code-braces: SpigotOutputTypeDef](./type_defs.md#spigotoutputtypedef) 
24. See [:material-code-braces: JoinOutputTypeDef](./type_defs.md#joinoutputtypedef) 
25. See [:material-code-braces: SplitFieldsOutputTypeDef](./type_defs.md#splitfieldsoutputtypedef) 
26. See [:material-code-braces: SelectFromCollectionOutputTypeDef](./type_defs.md#selectfromcollectionoutputtypedef) 
27. See [:material-code-braces: FillMissingValuesOutputTypeDef](./type_defs.md#fillmissingvaluesoutputtypedef) 
28. See [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef) 
29. See [:material-code-braces: CustomCodeOutputTypeDef](./type_defs.md#customcodeoutputtypedef) 
30. See [:material-code-braces: SparkSQLOutputTypeDef](./type_defs.md#sparksqloutputtypedef) 
31. See [:material-code-braces: DirectKinesisSourceOutputTypeDef](./type_defs.md#directkinesissourceoutputtypedef) 
32. See [:material-code-braces: DirectKafkaSourceOutputTypeDef](./type_defs.md#directkafkasourceoutputtypedef) 
33. See [:material-code-braces: CatalogKinesisSourceOutputTypeDef](./type_defs.md#catalogkinesissourceoutputtypedef) 
34. See [:material-code-braces: CatalogKafkaSourceOutputTypeDef](./type_defs.md#catalogkafkasourceoutputtypedef) 
35. See [:material-code-braces: DropNullFieldsOutputTypeDef](./type_defs.md#dropnullfieldsoutputtypedef) 
36. See [:material-code-braces: MergeOutputTypeDef](./type_defs.md#mergeoutputtypedef) 
37. See [:material-code-braces: UnionOutputTypeDef](./type_defs.md#unionoutputtypedef) 
38. See [:material-code-braces: PIIDetectionOutputTypeDef](./type_defs.md#piidetectionoutputtypedef) 
39. See [:material-code-braces: AggregateOutputTypeDef](./type_defs.md#aggregateoutputtypedef) 
40. See [:material-code-braces: DropDuplicatesOutputTypeDef](./type_defs.md#dropduplicatesoutputtypedef) 
41. See [:material-code-braces: GovernedCatalogTargetOutputTypeDef](./type_defs.md#governedcatalogtargetoutputtypedef) 
42. See [:material-code-braces: GovernedCatalogSourceTypeDef](./type_defs.md#governedcatalogsourcetypedef) 
43. See [:material-code-braces: MicrosoftSQLServerCatalogSourceTypeDef](./type_defs.md#microsoftsqlservercatalogsourcetypedef) 
44. See [:material-code-braces: MySQLCatalogSourceTypeDef](./type_defs.md#mysqlcatalogsourcetypedef) 
45. See [:material-code-braces: OracleSQLCatalogSourceTypeDef](./type_defs.md#oraclesqlcatalogsourcetypedef) 
46. See [:material-code-braces: PostgreSQLCatalogSourceTypeDef](./type_defs.md#postgresqlcatalogsourcetypedef) 
47. See [:material-code-braces: MicrosoftSQLServerCatalogTargetOutputTypeDef](./type_defs.md#microsoftsqlservercatalogtargetoutputtypedef) 
48. See [:material-code-braces: MySQLCatalogTargetOutputTypeDef](./type_defs.md#mysqlcatalogtargetoutputtypedef) 
49. See [:material-code-braces: OracleSQLCatalogTargetOutputTypeDef](./type_defs.md#oraclesqlcatalogtargetoutputtypedef) 
50. See [:material-code-braces: PostgreSQLCatalogTargetOutputTypeDef](./type_defs.md#postgresqlcatalogtargetoutputtypedef) 
51. See [:material-code-braces: DynamicTransformOutputTypeDef](./type_defs.md#dynamictransformoutputtypedef) 
52. See [:material-code-braces: EvaluateDataQualityOutputTypeDef](./type_defs.md#evaluatedataqualityoutputtypedef) 
53. See [:material-code-braces: S3CatalogHudiSourceOutputTypeDef](./type_defs.md#s3cataloghudisourceoutputtypedef) 
54. See [:material-code-braces: CatalogHudiSourceOutputTypeDef](./type_defs.md#cataloghudisourceoutputtypedef) 
55. See [:material-code-braces: S3HudiSourceOutputTypeDef](./type_defs.md#s3hudisourceoutputtypedef) 
56. See [:material-code-braces: S3HudiCatalogTargetOutputTypeDef](./type_defs.md#s3hudicatalogtargetoutputtypedef) 
57. See [:material-code-braces: S3HudiDirectTargetOutputTypeDef](./type_defs.md#s3hudidirecttargetoutputtypedef) 
58. See [:material-code-braces: DirectJDBCSourceTypeDef](./type_defs.md#directjdbcsourcetypedef) 
59. See [:material-code-braces: S3CatalogDeltaSourceOutputTypeDef](./type_defs.md#s3catalogdeltasourceoutputtypedef) 
60. See [:material-code-braces: CatalogDeltaSourceOutputTypeDef](./type_defs.md#catalogdeltasourceoutputtypedef) 
61. See [:material-code-braces: S3DeltaSourceOutputTypeDef](./type_defs.md#s3deltasourceoutputtypedef) 
62. See [:material-code-braces: S3DeltaCatalogTargetOutputTypeDef](./type_defs.md#s3deltacatalogtargetoutputtypedef) 
63. See [:material-code-braces: S3DeltaDirectTargetOutputTypeDef](./type_defs.md#s3deltadirecttargetoutputtypedef) 
64. See [:material-code-braces: AmazonRedshiftSourceOutputTypeDef](./type_defs.md#amazonredshiftsourceoutputtypedef) 
65. See [:material-code-braces: AmazonRedshiftTargetOutputTypeDef](./type_defs.md#amazonredshifttargetoutputtypedef) 
66. See [:material-code-braces: EvaluateDataQualityMultiFrameOutputTypeDef](./type_defs.md#evaluatedataqualitymultiframeoutputtypedef) 
67. See [:material-code-braces: RecipeOutputTypeDef](./type_defs.md#recipeoutputtypedef) 
68. See [:material-code-braces: SnowflakeSourceOutputTypeDef](./type_defs.md#snowflakesourceoutputtypedef) 
69. See [:material-code-braces: SnowflakeTargetOutputTypeDef](./type_defs.md#snowflaketargetoutputtypedef) 
70. See [:material-code-braces: ConnectorDataSourceOutputTypeDef](./type_defs.md#connectordatasourceoutputtypedef) 
71. See [:material-code-braces: ConnectorDataTargetOutputTypeDef](./type_defs.md#connectordatatargetoutputtypedef) 
## CodeGenConfigurationNodePaginatorTypeDef

```python
# CodeGenConfigurationNodePaginatorTypeDef definition

class CodeGenConfigurationNodePaginatorTypeDef(TypedDict):
    AthenaConnectorSource: NotRequired[AthenaConnectorSourceOutputTypeDef],  # (1)
    JDBCConnectorSource: NotRequired[JDBCConnectorSourceOutputTypeDef],  # (2)
    SparkConnectorSource: NotRequired[SparkConnectorSourceOutputTypeDef],  # (3)
    CatalogSource: NotRequired[CatalogSourceTypeDef],  # (4)
    RedshiftSource: NotRequired[RedshiftSourceTypeDef],  # (5)
    S3CatalogSource: NotRequired[S3CatalogSourceTypeDef],  # (6)
    S3CsvSource: NotRequired[S3CsvSourceOutputTypeDef],  # (7)
    S3JsonSource: NotRequired[S3JsonSourceOutputTypeDef],  # (8)
    S3ParquetSource: NotRequired[S3ParquetSourceOutputTypeDef],  # (9)
    RelationalCatalogSource: NotRequired[RelationalCatalogSourceTypeDef],  # (10)
    DynamoDBCatalogSource: NotRequired[DynamoDBCatalogSourceTypeDef],  # (11)
    JDBCConnectorTarget: NotRequired[JDBCConnectorTargetOutputTypeDef],  # (12)
    SparkConnectorTarget: NotRequired[SparkConnectorTargetOutputTypeDef],  # (13)
    CatalogTarget: NotRequired[BasicCatalogTargetOutputTypeDef],  # (14)
    RedshiftTarget: NotRequired[RedshiftTargetOutputTypeDef],  # (15)
    S3CatalogTarget: NotRequired[S3CatalogTargetOutputTypeDef],  # (16)
    S3GlueParquetTarget: NotRequired[S3GlueParquetTargetOutputTypeDef],  # (17)
    S3DirectTarget: NotRequired[S3DirectTargetOutputTypeDef],  # (18)
    ApplyMapping: NotRequired[ApplyMappingPaginatorTypeDef],  # (19)
    SelectFields: NotRequired[SelectFieldsOutputTypeDef],  # (20)
    DropFields: NotRequired[DropFieldsOutputTypeDef],  # (21)
    RenameField: NotRequired[RenameFieldOutputTypeDef],  # (22)
    Spigot: NotRequired[SpigotOutputTypeDef],  # (23)
    Join: NotRequired[JoinOutputTypeDef],  # (24)
    SplitFields: NotRequired[SplitFieldsOutputTypeDef],  # (25)
    SelectFromCollection: NotRequired[SelectFromCollectionOutputTypeDef],  # (26)
    FillMissingValues: NotRequired[FillMissingValuesOutputTypeDef],  # (27)
    Filter: NotRequired[FilterOutputTypeDef],  # (28)
    CustomCode: NotRequired[CustomCodeOutputTypeDef],  # (29)
    SparkSQL: NotRequired[SparkSQLOutputTypeDef],  # (30)
    DirectKinesisSource: NotRequired[DirectKinesisSourceOutputTypeDef],  # (31)
    DirectKafkaSource: NotRequired[DirectKafkaSourceOutputTypeDef],  # (32)
    CatalogKinesisSource: NotRequired[CatalogKinesisSourceOutputTypeDef],  # (33)
    CatalogKafkaSource: NotRequired[CatalogKafkaSourceOutputTypeDef],  # (34)
    DropNullFields: NotRequired[DropNullFieldsOutputTypeDef],  # (35)
    Merge: NotRequired[MergeOutputTypeDef],  # (36)
    Union: NotRequired[UnionOutputTypeDef],  # (37)
    PIIDetection: NotRequired[PIIDetectionOutputTypeDef],  # (38)
    Aggregate: NotRequired[AggregateOutputTypeDef],  # (39)
    DropDuplicates: NotRequired[DropDuplicatesOutputTypeDef],  # (40)
    GovernedCatalogTarget: NotRequired[GovernedCatalogTargetOutputTypeDef],  # (41)
    GovernedCatalogSource: NotRequired[GovernedCatalogSourceTypeDef],  # (42)
    MicrosoftSQLServerCatalogSource: NotRequired[MicrosoftSQLServerCatalogSourceTypeDef],  # (43)
    MySQLCatalogSource: NotRequired[MySQLCatalogSourceTypeDef],  # (44)
    OracleSQLCatalogSource: NotRequired[OracleSQLCatalogSourceTypeDef],  # (45)
    PostgreSQLCatalogSource: NotRequired[PostgreSQLCatalogSourceTypeDef],  # (46)
    MicrosoftSQLServerCatalogTarget: NotRequired[MicrosoftSQLServerCatalogTargetOutputTypeDef],  # (47)
    MySQLCatalogTarget: NotRequired[MySQLCatalogTargetOutputTypeDef],  # (48)
    OracleSQLCatalogTarget: NotRequired[OracleSQLCatalogTargetOutputTypeDef],  # (49)
    PostgreSQLCatalogTarget: NotRequired[PostgreSQLCatalogTargetOutputTypeDef],  # (50)
    DynamicTransform: NotRequired[DynamicTransformOutputTypeDef],  # (51)
    EvaluateDataQuality: NotRequired[EvaluateDataQualityOutputTypeDef],  # (52)
    S3CatalogHudiSource: NotRequired[S3CatalogHudiSourceOutputTypeDef],  # (53)
    CatalogHudiSource: NotRequired[CatalogHudiSourceOutputTypeDef],  # (54)
    S3HudiSource: NotRequired[S3HudiSourceOutputTypeDef],  # (55)
    S3HudiCatalogTarget: NotRequired[S3HudiCatalogTargetOutputTypeDef],  # (56)
    S3HudiDirectTarget: NotRequired[S3HudiDirectTargetOutputTypeDef],  # (57)
    DirectJDBCSource: NotRequired[DirectJDBCSourceTypeDef],  # (58)
    S3CatalogDeltaSource: NotRequired[S3CatalogDeltaSourceOutputTypeDef],  # (59)
    CatalogDeltaSource: NotRequired[CatalogDeltaSourceOutputTypeDef],  # (60)
    S3DeltaSource: NotRequired[S3DeltaSourceOutputTypeDef],  # (61)
    S3DeltaCatalogTarget: NotRequired[S3DeltaCatalogTargetOutputTypeDef],  # (62)
    S3DeltaDirectTarget: NotRequired[S3DeltaDirectTargetOutputTypeDef],  # (63)
    AmazonRedshiftSource: NotRequired[AmazonRedshiftSourceOutputTypeDef],  # (64)
    AmazonRedshiftTarget: NotRequired[AmazonRedshiftTargetOutputTypeDef],  # (65)
    EvaluateDataQualityMultiFrame: NotRequired[EvaluateDataQualityMultiFrameOutputTypeDef],  # (66)
    Recipe: NotRequired[RecipeOutputTypeDef],  # (67)
    SnowflakeSource: NotRequired[SnowflakeSourceOutputTypeDef],  # (68)
    SnowflakeTarget: NotRequired[SnowflakeTargetOutputTypeDef],  # (69)
    ConnectorDataSource: NotRequired[ConnectorDataSourceOutputTypeDef],  # (70)
    ConnectorDataTarget: NotRequired[ConnectorDataTargetOutputTypeDef],  # (71)
```

1. See [:material-code-braces: AthenaConnectorSourceOutputTypeDef](./type_defs.md#athenaconnectorsourceoutputtypedef) 
2. See [:material-code-braces: JDBCConnectorSourceOutputTypeDef](./type_defs.md#jdbcconnectorsourceoutputtypedef) 
3. See [:material-code-braces: SparkConnectorSourceOutputTypeDef](./type_defs.md#sparkconnectorsourceoutputtypedef) 
4. See [:material-code-braces: CatalogSourceTypeDef](./type_defs.md#catalogsourcetypedef) 
5. See [:material-code-braces: RedshiftSourceTypeDef](./type_defs.md#redshiftsourcetypedef) 
6. See [:material-code-braces: S3CatalogSourceTypeDef](./type_defs.md#s3catalogsourcetypedef) 
7. See [:material-code-braces: S3CsvSourceOutputTypeDef](./type_defs.md#s3csvsourceoutputtypedef) 
8. See [:material-code-braces: S3JsonSourceOutputTypeDef](./type_defs.md#s3jsonsourceoutputtypedef) 
9. See [:material-code-braces: S3ParquetSourceOutputTypeDef](./type_defs.md#s3parquetsourceoutputtypedef) 
10. See [:material-code-braces: RelationalCatalogSourceTypeDef](./type_defs.md#relationalcatalogsourcetypedef) 
11. See [:material-code-braces: DynamoDBCatalogSourceTypeDef](./type_defs.md#dynamodbcatalogsourcetypedef) 
12. See [:material-code-braces: JDBCConnectorTargetOutputTypeDef](./type_defs.md#jdbcconnectortargetoutputtypedef) 
13. See [:material-code-braces: SparkConnectorTargetOutputTypeDef](./type_defs.md#sparkconnectortargetoutputtypedef) 
14. See [:material-code-braces: BasicCatalogTargetOutputTypeDef](./type_defs.md#basiccatalogtargetoutputtypedef) 
15. See [:material-code-braces: RedshiftTargetOutputTypeDef](./type_defs.md#redshifttargetoutputtypedef) 
16. See [:material-code-braces: S3CatalogTargetOutputTypeDef](./type_defs.md#s3catalogtargetoutputtypedef) 
17. See [:material-code-braces: S3GlueParquetTargetOutputTypeDef](./type_defs.md#s3glueparquettargetoutputtypedef) 
18. See [:material-code-braces: S3DirectTargetOutputTypeDef](./type_defs.md#s3directtargetoutputtypedef) 
19. See [:material-code-braces: ApplyMappingPaginatorTypeDef](./type_defs.md#applymappingpaginatortypedef) 
20. See [:material-code-braces: SelectFieldsOutputTypeDef](./type_defs.md#selectfieldsoutputtypedef) 
21. See [:material-code-braces: DropFieldsOutputTypeDef](./type_defs.md#dropfieldsoutputtypedef) 
22. See [:material-code-braces: RenameFieldOutputTypeDef](./type_defs.md#renamefieldoutputtypedef) 
23. See [:material-code-braces: SpigotOutputTypeDef](./type_defs.md#spigotoutputtypedef) 
24. See [:material-code-braces: JoinOutputTypeDef](./type_defs.md#joinoutputtypedef) 
25. See [:material-code-braces: SplitFieldsOutputTypeDef](./type_defs.md#splitfieldsoutputtypedef) 
26. See [:material-code-braces: SelectFromCollectionOutputTypeDef](./type_defs.md#selectfromcollectionoutputtypedef) 
27. See [:material-code-braces: FillMissingValuesOutputTypeDef](./type_defs.md#fillmissingvaluesoutputtypedef) 
28. See [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef) 
29. See [:material-code-braces: CustomCodeOutputTypeDef](./type_defs.md#customcodeoutputtypedef) 
30. See [:material-code-braces: SparkSQLOutputTypeDef](./type_defs.md#sparksqloutputtypedef) 
31. See [:material-code-braces: DirectKinesisSourceOutputTypeDef](./type_defs.md#directkinesissourceoutputtypedef) 
32. See [:material-code-braces: DirectKafkaSourceOutputTypeDef](./type_defs.md#directkafkasourceoutputtypedef) 
33. See [:material-code-braces: CatalogKinesisSourceOutputTypeDef](./type_defs.md#catalogkinesissourceoutputtypedef) 
34. See [:material-code-braces: CatalogKafkaSourceOutputTypeDef](./type_defs.md#catalogkafkasourceoutputtypedef) 
35. See [:material-code-braces: DropNullFieldsOutputTypeDef](./type_defs.md#dropnullfieldsoutputtypedef) 
36. See [:material-code-braces: MergeOutputTypeDef](./type_defs.md#mergeoutputtypedef) 
37. See [:material-code-braces: UnionOutputTypeDef](./type_defs.md#unionoutputtypedef) 
38. See [:material-code-braces: PIIDetectionOutputTypeDef](./type_defs.md#piidetectionoutputtypedef) 
39. See [:material-code-braces: AggregateOutputTypeDef](./type_defs.md#aggregateoutputtypedef) 
40. See [:material-code-braces: DropDuplicatesOutputTypeDef](./type_defs.md#dropduplicatesoutputtypedef) 
41. See [:material-code-braces: GovernedCatalogTargetOutputTypeDef](./type_defs.md#governedcatalogtargetoutputtypedef) 
42. See [:material-code-braces: GovernedCatalogSourceTypeDef](./type_defs.md#governedcatalogsourcetypedef) 
43. See [:material-code-braces: MicrosoftSQLServerCatalogSourceTypeDef](./type_defs.md#microsoftsqlservercatalogsourcetypedef) 
44. See [:material-code-braces: MySQLCatalogSourceTypeDef](./type_defs.md#mysqlcatalogsourcetypedef) 
45. See [:material-code-braces: OracleSQLCatalogSourceTypeDef](./type_defs.md#oraclesqlcatalogsourcetypedef) 
46. See [:material-code-braces: PostgreSQLCatalogSourceTypeDef](./type_defs.md#postgresqlcatalogsourcetypedef) 
47. See [:material-code-braces: MicrosoftSQLServerCatalogTargetOutputTypeDef](./type_defs.md#microsoftsqlservercatalogtargetoutputtypedef) 
48. See [:material-code-braces: MySQLCatalogTargetOutputTypeDef](./type_defs.md#mysqlcatalogtargetoutputtypedef) 
49. See [:material-code-braces: OracleSQLCatalogTargetOutputTypeDef](./type_defs.md#oraclesqlcatalogtargetoutputtypedef) 
50. See [:material-code-braces: PostgreSQLCatalogTargetOutputTypeDef](./type_defs.md#postgresqlcatalogtargetoutputtypedef) 
51. See [:material-code-braces: DynamicTransformOutputTypeDef](./type_defs.md#dynamictransformoutputtypedef) 
52. See [:material-code-braces: EvaluateDataQualityOutputTypeDef](./type_defs.md#evaluatedataqualityoutputtypedef) 
53. See [:material-code-braces: S3CatalogHudiSourceOutputTypeDef](./type_defs.md#s3cataloghudisourceoutputtypedef) 
54. See [:material-code-braces: CatalogHudiSourceOutputTypeDef](./type_defs.md#cataloghudisourceoutputtypedef) 
55. See [:material-code-braces: S3HudiSourceOutputTypeDef](./type_defs.md#s3hudisourceoutputtypedef) 
56. See [:material-code-braces: S3HudiCatalogTargetOutputTypeDef](./type_defs.md#s3hudicatalogtargetoutputtypedef) 
57. See [:material-code-braces: S3HudiDirectTargetOutputTypeDef](./type_defs.md#s3hudidirecttargetoutputtypedef) 
58. See [:material-code-braces: DirectJDBCSourceTypeDef](./type_defs.md#directjdbcsourcetypedef) 
59. See [:material-code-braces: S3CatalogDeltaSourceOutputTypeDef](./type_defs.md#s3catalogdeltasourceoutputtypedef) 
60. See [:material-code-braces: CatalogDeltaSourceOutputTypeDef](./type_defs.md#catalogdeltasourceoutputtypedef) 
61. See [:material-code-braces: S3DeltaSourceOutputTypeDef](./type_defs.md#s3deltasourceoutputtypedef) 
62. See [:material-code-braces: S3DeltaCatalogTargetOutputTypeDef](./type_defs.md#s3deltacatalogtargetoutputtypedef) 
63. See [:material-code-braces: S3DeltaDirectTargetOutputTypeDef](./type_defs.md#s3deltadirecttargetoutputtypedef) 
64. See [:material-code-braces: AmazonRedshiftSourceOutputTypeDef](./type_defs.md#amazonredshiftsourceoutputtypedef) 
65. See [:material-code-braces: AmazonRedshiftTargetOutputTypeDef](./type_defs.md#amazonredshifttargetoutputtypedef) 
66. See [:material-code-braces: EvaluateDataQualityMultiFrameOutputTypeDef](./type_defs.md#evaluatedataqualitymultiframeoutputtypedef) 
67. See [:material-code-braces: RecipeOutputTypeDef](./type_defs.md#recipeoutputtypedef) 
68. See [:material-code-braces: SnowflakeSourceOutputTypeDef](./type_defs.md#snowflakesourceoutputtypedef) 
69. See [:material-code-braces: SnowflakeTargetOutputTypeDef](./type_defs.md#snowflaketargetoutputtypedef) 
70. See [:material-code-braces: ConnectorDataSourceOutputTypeDef](./type_defs.md#connectordatasourceoutputtypedef) 
71. See [:material-code-braces: ConnectorDataTargetOutputTypeDef](./type_defs.md#connectordatatargetoutputtypedef) 
## CreateCrawlerRequestRequestTypeDef

```python
# CreateCrawlerRequestRequestTypeDef definition

class CreateCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
    Role: str,
    Targets: CrawlerTargetsTypeDef,  # (1)
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    Classifiers: NotRequired[Sequence[str]],
    TablePrefix: NotRequired[str],
    SchemaChangePolicy: NotRequired[SchemaChangePolicyTypeDef],  # (2)
    RecrawlPolicy: NotRequired[RecrawlPolicyTypeDef],  # (3)
    LineageConfiguration: NotRequired[LineageConfigurationTypeDef],  # (4)
    LakeFormationConfiguration: NotRequired[LakeFormationConfigurationTypeDef],  # (5)
    Configuration: NotRequired[str],
    CrawlerSecurityConfiguration: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CrawlerTargetsTypeDef](./type_defs.md#crawlertargetstypedef) 
2. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
3. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
## UpdateCrawlerRequestRequestTypeDef

```python
# UpdateCrawlerRequestRequestTypeDef definition

class UpdateCrawlerRequestRequestTypeDef(TypedDict):
    Name: str,
    Role: NotRequired[str],
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Targets: NotRequired[CrawlerTargetsTypeDef],  # (1)
    Schedule: NotRequired[str],
    Classifiers: NotRequired[Sequence[str]],
    TablePrefix: NotRequired[str],
    SchemaChangePolicy: NotRequired[SchemaChangePolicyTypeDef],  # (2)
    RecrawlPolicy: NotRequired[RecrawlPolicyTypeDef],  # (3)
    LineageConfiguration: NotRequired[LineageConfigurationTypeDef],  # (4)
    LakeFormationConfiguration: NotRequired[LakeFormationConfigurationTypeDef],  # (5)
    Configuration: NotRequired[str],
    CrawlerSecurityConfiguration: NotRequired[str],
```

1. See [:material-code-braces: CrawlerTargetsTypeDef](./type_defs.md#crawlertargetstypedef) 
2. See [:material-code-braces: SchemaChangePolicyTypeDef](./type_defs.md#schemachangepolicytypedef) 
3. See [:material-code-braces: RecrawlPolicyTypeDef](./type_defs.md#recrawlpolicytypedef) 
4. See [:material-code-braces: LineageConfigurationTypeDef](./type_defs.md#lineageconfigurationtypedef) 
5. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
## GetStatementResponseTypeDef

```python
# GetStatementResponseTypeDef definition

class GetStatementResponseTypeDef(TypedDict):
    Statement: StatementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStatementsResponseTypeDef

```python
# ListStatementsResponseTypeDef definition

class ListStatementsResponseTypeDef(TypedDict):
    Statements: List[StatementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StatementTypeDef](./type_defs.md#statementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TablePaginatorTypeDef

```python
# TablePaginatorTypeDef definition

class TablePaginatorTypeDef(TypedDict):
    Name: str,
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Owner: NotRequired[str],
    CreateTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
    LastAccessTime: NotRequired[datetime],
    LastAnalyzedTime: NotRequired[datetime],
    Retention: NotRequired[int],
    StorageDescriptor: NotRequired[StorageDescriptorOutputTypeDef],  # (1)
    PartitionKeys: NotRequired[List[ColumnOutputTypeDef]],  # (2)
    ViewOriginalText: NotRequired[str],
    ViewExpandedText: NotRequired[str],
    TableType: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
    CreatedBy: NotRequired[str],
    IsRegisteredWithLakeFormation: NotRequired[bool],
    TargetTable: NotRequired[TableIdentifierTypeDef],  # (3)
    CatalogId: NotRequired[str],
    VersionId: NotRequired[str],
    FederatedTable: NotRequired[FederatedTableTypeDef],  # (4)
    ViewDefinition: NotRequired[ViewDefinitionTypeDef],  # (5)
    IsMultiDialectView: NotRequired[bool],
    Status: NotRequired[TableStatusPaginatorTypeDef],  # (6)
```

1. See [:material-code-braces: StorageDescriptorOutputTypeDef](./type_defs.md#storagedescriptoroutputtypedef) 
2. See [:material-code-braces: ColumnOutputTypeDef](./type_defs.md#columnoutputtypedef) 
3. See [:material-code-braces: TableIdentifierTypeDef](./type_defs.md#tableidentifiertypedef) 
4. See [:material-code-braces: FederatedTableTypeDef](./type_defs.md#federatedtabletypedef) 
5. See [:material-code-braces: ViewDefinitionTypeDef](./type_defs.md#viewdefinitiontypedef) 
6. See [:material-code-braces: TableStatusPaginatorTypeDef](./type_defs.md#tablestatuspaginatortypedef) 
## TableTypeDef

```python
# TableTypeDef definition

class TableTypeDef(TypedDict):
    Name: str,
    DatabaseName: NotRequired[str],
    Description: NotRequired[str],
    Owner: NotRequired[str],
    CreateTime: NotRequired[datetime],
    UpdateTime: NotRequired[datetime],
    LastAccessTime: NotRequired[datetime],
    LastAnalyzedTime: NotRequired[datetime],
    Retention: NotRequired[int],
    StorageDescriptor: NotRequired[StorageDescriptorOutputTypeDef],  # (1)
    PartitionKeys: NotRequired[List[ColumnOutputTypeDef]],  # (2)
    ViewOriginalText: NotRequired[str],
    ViewExpandedText: NotRequired[str],
    TableType: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
    CreatedBy: NotRequired[str],
    IsRegisteredWithLakeFormation: NotRequired[bool],
    TargetTable: NotRequired[TableIdentifierTypeDef],  # (3)
    CatalogId: NotRequired[str],
    VersionId: NotRequired[str],
    FederatedTable: NotRequired[FederatedTableTypeDef],  # (4)
    ViewDefinition: NotRequired[ViewDefinitionTypeDef],  # (5)
    IsMultiDialectView: NotRequired[bool],
    Status: NotRequired[TableStatusTypeDef],  # (6)
```

1. See [:material-code-braces: StorageDescriptorOutputTypeDef](./type_defs.md#storagedescriptoroutputtypedef) 
2. See [:material-code-braces: ColumnOutputTypeDef](./type_defs.md#columnoutputtypedef) 
3. See [:material-code-braces: TableIdentifierTypeDef](./type_defs.md#tableidentifiertypedef) 
4. See [:material-code-braces: FederatedTableTypeDef](./type_defs.md#federatedtabletypedef) 
5. See [:material-code-braces: ViewDefinitionTypeDef](./type_defs.md#viewdefinitiontypedef) 
6. See [:material-code-braces: TableStatusTypeDef](./type_defs.md#tablestatustypedef) 
## NodeTypeDef

```python
# NodeTypeDef definition

class NodeTypeDef(TypedDict):
    Type: NotRequired[NodeTypeType],  # (1)
    Name: NotRequired[str],
    UniqueId: NotRequired[str],
    TriggerDetails: NotRequired[TriggerNodeDetailsTypeDef],  # (2)
    JobDetails: NotRequired[JobNodeDetailsTypeDef],  # (3)
    CrawlerDetails: NotRequired[CrawlerNodeDetailsTypeDef],  # (4)
```

1. See [:material-code-brackets: NodeTypeType](./literals.md#nodetypetype) 
2. See [:material-code-braces: TriggerNodeDetailsTypeDef](./type_defs.md#triggernodedetailstypedef) 
3. See [:material-code-braces: JobNodeDetailsTypeDef](./type_defs.md#jobnodedetailstypedef) 
4. See [:material-code-braces: CrawlerNodeDetailsTypeDef](./type_defs.md#crawlernodedetailstypedef) 
## UpdateTriggerRequestRequestTypeDef

```python
# UpdateTriggerRequestRequestTypeDef definition

class UpdateTriggerRequestRequestTypeDef(TypedDict):
    Name: str,
    TriggerUpdate: TriggerUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: TriggerUpdateTypeDef](./type_defs.md#triggerupdatetypedef) 
## GetMLTransformsResponseTypeDef

```python
# GetMLTransformsResponseTypeDef definition

class GetMLTransformsResponseTypeDef(TypedDict):
    Transforms: List[MLTransformTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MLTransformTypeDef](./type_defs.md#mltransformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCatalogRequestRequestTypeDef

```python
# CreateCatalogRequestRequestTypeDef definition

class CreateCatalogRequestRequestTypeDef(TypedDict):
    Name: str,
    CatalogInput: CatalogInputTypeDef,  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CatalogInputTypeDef](./type_defs.md#cataloginputtypedef) 
## UpdateCatalogRequestRequestTypeDef

```python
# UpdateCatalogRequestRequestTypeDef definition

class UpdateCatalogRequestRequestTypeDef(TypedDict):
    CatalogId: str,
    CatalogInput: CatalogInputTypeDef,  # (1)
```

1. See [:material-code-braces: CatalogInputTypeDef](./type_defs.md#cataloginputtypedef) 
## CreateDatabaseRequestRequestTypeDef

```python
# CreateDatabaseRequestRequestTypeDef definition

class CreateDatabaseRequestRequestTypeDef(TypedDict):
    DatabaseInput: DatabaseInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DatabaseInputTypeDef](./type_defs.md#databaseinputtypedef) 
## UpdateDatabaseRequestRequestTypeDef

```python
# UpdateDatabaseRequestRequestTypeDef definition

class UpdateDatabaseRequestRequestTypeDef(TypedDict):
    Name: str,
    DatabaseInput: DatabaseInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: DatabaseInputTypeDef](./type_defs.md#databaseinputtypedef) 
## BatchGetDataQualityResultResponseTypeDef

```python
# BatchGetDataQualityResultResponseTypeDef definition

class BatchGetDataQualityResultResponseTypeDef(TypedDict):
    Results: List[DataQualityResultTypeDef],  # (1)
    ResultsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataQualityResultTypeDef](./type_defs.md#dataqualityresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ColumnStatisticsErrorTypeDef

```python
# ColumnStatisticsErrorTypeDef definition

class ColumnStatisticsErrorTypeDef(TypedDict):
    ColumnStatistics: NotRequired[ColumnStatisticsOutputTypeDef],  # (1)
    Error: NotRequired[ErrorDetailTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnStatisticsOutputTypeDef](./type_defs.md#columnstatisticsoutputtypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## GetColumnStatisticsForPartitionResponseTypeDef

```python
# GetColumnStatisticsForPartitionResponseTypeDef definition

class GetColumnStatisticsForPartitionResponseTypeDef(TypedDict):
    ColumnStatisticsList: List[ColumnStatisticsOutputTypeDef],  # (1)
    Errors: List[ColumnErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ColumnStatisticsOutputTypeDef](./type_defs.md#columnstatisticsoutputtypedef) 
2. See [:material-code-braces: ColumnErrorTypeDef](./type_defs.md#columnerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetColumnStatisticsForTableResponseTypeDef

```python
# GetColumnStatisticsForTableResponseTypeDef definition

class GetColumnStatisticsForTableResponseTypeDef(TypedDict):
    ColumnStatisticsList: List[ColumnStatisticsOutputTypeDef],  # (1)
    Errors: List[ColumnErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ColumnStatisticsOutputTypeDef](./type_defs.md#columnstatisticsoutputtypedef) 
2. See [:material-code-braces: ColumnErrorTypeDef](./type_defs.md#columnerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetPartitionResponseTypeDef

```python
# BatchGetPartitionResponseTypeDef definition

class BatchGetPartitionResponseTypeDef(TypedDict):
    Partitions: List[PartitionTypeDef],  # (1)
    UnprocessedKeys: List[PartitionValueListOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: PartitionValueListOutputTypeDef](./type_defs.md#partitionvaluelistoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartitionResponseTypeDef

```python
# GetPartitionResponseTypeDef definition

class GetPartitionResponseTypeDef(TypedDict):
    Partition: PartitionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPartitionsResponseTypeDef

```python
# GetPartitionsResponseTypeDef definition

class GetPartitionsResponseTypeDef(TypedDict):
    Partitions: List[PartitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUnfilteredPartitionMetadataResponseTypeDef

```python
# GetUnfilteredPartitionMetadataResponseTypeDef definition

class GetUnfilteredPartitionMetadataResponseTypeDef(TypedDict):
    Partition: PartitionTypeDef,  # (1)
    AuthorizedColumns: List[str],
    IsRegisteredWithLakeFormation: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnfilteredPartitionTypeDef

```python
# UnfilteredPartitionTypeDef definition

class UnfilteredPartitionTypeDef(TypedDict):
    Partition: NotRequired[PartitionTypeDef],  # (1)
    AuthorizedColumns: NotRequired[List[str]],
    IsRegisteredWithLakeFormation: NotRequired[bool],
```

1. See [:material-code-braces: PartitionTypeDef](./type_defs.md#partitiontypedef) 
## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    LogicalOperator: FilterLogicalOperatorType,  # (1)
    Filters: Sequence[FilterExpressionUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterLogicalOperatorType](./literals.md#filterlogicaloperatortype) 
2. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) [:material-code-braces: FilterExpressionOutputTypeDef](./type_defs.md#filterexpressionoutputtypedef) 
## DataQualityResultFilterCriteriaTypeDef

```python
# DataQualityResultFilterCriteriaTypeDef definition

class DataQualityResultFilterCriteriaTypeDef(TypedDict):
    DataSource: NotRequired[DataSourceUnionTypeDef],  # (1)
    JobName: NotRequired[str],
    JobRunId: NotRequired[str],
    StartedAfter: NotRequired[TimestampTypeDef],
    StartedBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
## DataQualityRuleRecommendationRunFilterTypeDef

```python
# DataQualityRuleRecommendationRunFilterTypeDef definition

class DataQualityRuleRecommendationRunFilterTypeDef(TypedDict):
    DataSource: DataSourceUnionTypeDef,  # (1)
    StartedBefore: NotRequired[TimestampTypeDef],
    StartedAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
## DataQualityRulesetEvaluationRunFilterTypeDef

```python
# DataQualityRulesetEvaluationRunFilterTypeDef definition

class DataQualityRulesetEvaluationRunFilterTypeDef(TypedDict):
    DataSource: DataSourceUnionTypeDef,  # (1)
    StartedBefore: NotRequired[TimestampTypeDef],
    StartedAfter: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
## StartDataQualityRulesetEvaluationRunRequestRequestTypeDef

```python
# StartDataQualityRulesetEvaluationRunRequestRequestTypeDef definition

class StartDataQualityRulesetEvaluationRunRequestRequestTypeDef(TypedDict):
    DataSource: DataSourceTypeDef,  # (1)
    Role: str,
    RulesetNames: Sequence[str],
    NumberOfWorkers: NotRequired[int],
    Timeout: NotRequired[int],
    ClientToken: NotRequired[str],
    AdditionalRunOptions: NotRequired[DataQualityEvaluationRunAdditionalRunOptionsTypeDef],  # (2)
    AdditionalDataSources: NotRequired[Mapping[str, DataSourceUnionTypeDef]],  # (3)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: DataQualityEvaluationRunAdditionalRunOptionsTypeDef](./type_defs.md#dataqualityevaluationrunadditionalrunoptionstypedef) 
3. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) [:material-code-braces: DataSourceOutputTypeDef](./type_defs.md#datasourceoutputtypedef) 
## BatchTableOptimizerTypeDef

```python
# BatchTableOptimizerTypeDef definition

class BatchTableOptimizerTypeDef(TypedDict):
    catalogId: NotRequired[str],
    databaseName: NotRequired[str],
    tableName: NotRequired[str],
    tableOptimizer: NotRequired[TableOptimizerTypeDef],  # (1)
```

1. See [:material-code-braces: TableOptimizerTypeDef](./type_defs.md#tableoptimizertypedef) 
## GetTableOptimizerResponseTypeDef

```python
# GetTableOptimizerResponseTypeDef definition

class GetTableOptimizerResponseTypeDef(TypedDict):
    CatalogId: str,
    DatabaseName: str,
    TableName: str,
    TableOptimizer: TableOptimizerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableOptimizerTypeDef](./type_defs.md#tableoptimizertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectionResponseTypeDef

```python
# GetConnectionResponseTypeDef definition

class GetConnectionResponseTypeDef(TypedDict):
    Connection: ConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectionsResponseTypeDef

```python
# GetConnectionsResponseTypeDef definition

class GetConnectionsResponseTypeDef(TypedDict):
    ConnectionList: List[ConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateConnectionRequestRequestTypeDef

```python
# CreateConnectionRequestRequestTypeDef definition

class CreateConnectionRequestRequestTypeDef(TypedDict):
    ConnectionInput: ConnectionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConnectionInputTypeDef](./type_defs.md#connectioninputtypedef) 
## UpdateConnectionRequestRequestTypeDef

```python
# UpdateConnectionRequestRequestTypeDef definition

class UpdateConnectionRequestRequestTypeDef(TypedDict):
    Name: str,
    ConnectionInput: ConnectionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ConnectionInputTypeDef](./type_defs.md#connectioninputtypedef) 
## TestConnectionRequestRequestTypeDef

```python
# TestConnectionRequestRequestTypeDef definition

class TestConnectionRequestRequestTypeDef(TypedDict):
    ConnectionName: NotRequired[str],
    CatalogId: NotRequired[str],
    TestConnectionInput: NotRequired[TestConnectionInputTypeDef],  # (1)
```

1. See [:material-code-braces: TestConnectionInputTypeDef](./type_defs.md#testconnectioninputtypedef) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    Name: NotRequired[str],
    JobMode: NotRequired[JobModeType],  # (1)
    JobRunQueuingEnabled: NotRequired[bool],
    Description: NotRequired[str],
    LogUri: NotRequired[str],
    Role: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    ExecutionProperty: NotRequired[ExecutionPropertyTypeDef],  # (2)
    Command: NotRequired[JobCommandTypeDef],  # (3)
    DefaultArguments: NotRequired[Dict[str, str]],
    NonOverridableArguments: NotRequired[Dict[str, str]],
    Connections: NotRequired[ConnectionsListOutputTypeDef],  # (4)
    MaxRetries: NotRequired[int],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (5)
    NumberOfWorkers: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (6)
    GlueVersion: NotRequired[str],
    CodeGenConfigurationNodes: NotRequired[Dict[str, CodeGenConfigurationNodeOutputTypeDef]],  # (7)
    ExecutionClass: NotRequired[ExecutionClassType],  # (8)
    SourceControlDetails: NotRequired[SourceControlDetailsTypeDef],  # (9)
    MaintenanceWindow: NotRequired[str],
    ProfileName: NotRequired[str],
```

1. See [:material-code-brackets: JobModeType](./literals.md#jobmodetype) 
2. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
3. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
4. See [:material-code-braces: ConnectionsListOutputTypeDef](./type_defs.md#connectionslistoutputtypedef) 
5. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
6. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
7. See [:material-code-braces: CodeGenConfigurationNodeOutputTypeDef](./type_defs.md#codegenconfigurationnodeoutputtypedef) 
8. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
9. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
## JobPaginatorTypeDef

```python
# JobPaginatorTypeDef definition

class JobPaginatorTypeDef(TypedDict):
    Name: NotRequired[str],
    JobMode: NotRequired[JobModeType],  # (1)
    JobRunQueuingEnabled: NotRequired[bool],
    Description: NotRequired[str],
    LogUri: NotRequired[str],
    Role: NotRequired[str],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    ExecutionProperty: NotRequired[ExecutionPropertyTypeDef],  # (2)
    Command: NotRequired[JobCommandTypeDef],  # (3)
    DefaultArguments: NotRequired[Dict[str, str]],
    NonOverridableArguments: NotRequired[Dict[str, str]],
    Connections: NotRequired[ConnectionsListOutputTypeDef],  # (4)
    MaxRetries: NotRequired[int],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (5)
    NumberOfWorkers: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (6)
    GlueVersion: NotRequired[str],
    CodeGenConfigurationNodes: NotRequired[Dict[str, CodeGenConfigurationNodePaginatorTypeDef]],  # (7)
    ExecutionClass: NotRequired[ExecutionClassType],  # (8)
    SourceControlDetails: NotRequired[SourceControlDetailsTypeDef],  # (9)
    MaintenanceWindow: NotRequired[str],
    ProfileName: NotRequired[str],
```

1. See [:material-code-brackets: JobModeType](./literals.md#jobmodetype) 
2. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
3. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
4. See [:material-code-braces: ConnectionsListOutputTypeDef](./type_defs.md#connectionslistoutputtypedef) 
5. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
6. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
7. See [:material-code-braces: CodeGenConfigurationNodePaginatorTypeDef](./type_defs.md#codegenconfigurationnodepaginatortypedef) 
8. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
9. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
## RecipeTypeDef

```python
# RecipeTypeDef definition

class RecipeTypeDef(TypedDict):
    Name: str,
    Inputs: Sequence[str],
    RecipeReference: NotRequired[RecipeReferenceTypeDef],  # (1)
    RecipeSteps: NotRequired[Sequence[RecipeStepUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: RecipeReferenceTypeDef](./type_defs.md#recipereferencetypedef) 
2. See [:material-code-braces: RecipeStepTypeDef](./type_defs.md#recipesteptypedef) [:material-code-braces: RecipeStepOutputTypeDef](./type_defs.md#recipestepoutputtypedef) 
## PartitionInputTypeDef

```python
# PartitionInputTypeDef definition

class PartitionInputTypeDef(TypedDict):
    Values: NotRequired[Sequence[str]],
    LastAccessTime: NotRequired[TimestampTypeDef],
    StorageDescriptor: NotRequired[StorageDescriptorUnionTypeDef],  # (1)
    Parameters: NotRequired[Mapping[str, str]],
    LastAnalyzedTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: StorageDescriptorTypeDef](./type_defs.md#storagedescriptortypedef) [:material-code-braces: StorageDescriptorOutputTypeDef](./type_defs.md#storagedescriptoroutputtypedef) 
## TableInputTypeDef

```python
# TableInputTypeDef definition

class TableInputTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Owner: NotRequired[str],
    LastAccessTime: NotRequired[TimestampTypeDef],
    LastAnalyzedTime: NotRequired[TimestampTypeDef],
    Retention: NotRequired[int],
    StorageDescriptor: NotRequired[StorageDescriptorUnionTypeDef],  # (1)
    PartitionKeys: NotRequired[Sequence[ColumnUnionTypeDef]],  # (2)
    ViewOriginalText: NotRequired[str],
    ViewExpandedText: NotRequired[str],
    TableType: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    TargetTable: NotRequired[TableIdentifierTypeDef],  # (3)
    ViewDefinition: NotRequired[ViewDefinitionInputTypeDef],  # (4)
```

1. See [:material-code-braces: StorageDescriptorTypeDef](./type_defs.md#storagedescriptortypedef) [:material-code-braces: StorageDescriptorOutputTypeDef](./type_defs.md#storagedescriptoroutputtypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) [:material-code-braces: ColumnOutputTypeDef](./type_defs.md#columnoutputtypedef) 
3. See [:material-code-braces: TableIdentifierTypeDef](./type_defs.md#tableidentifiertypedef) 
4. See [:material-code-braces: ViewDefinitionInputTypeDef](./type_defs.md#viewdefinitioninputtypedef) 
## GetTablesResponsePaginatorTypeDef

```python
# GetTablesResponsePaginatorTypeDef definition

class GetTablesResponsePaginatorTypeDef(TypedDict):
    TableList: List[TablePaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TablePaginatorTypeDef](./type_defs.md#tablepaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableVersionPaginatorTypeDef

```python
# TableVersionPaginatorTypeDef definition

class TableVersionPaginatorTypeDef(TypedDict):
    Table: NotRequired[TablePaginatorTypeDef],  # (1)
    VersionId: NotRequired[str],
```

1. See [:material-code-braces: TablePaginatorTypeDef](./type_defs.md#tablepaginatortypedef) 
## GetTableResponseTypeDef

```python
# GetTableResponseTypeDef definition

class GetTableResponseTypeDef(TypedDict):
    Table: TableTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTablesResponseTypeDef

```python
# GetTablesResponseTypeDef definition

class GetTablesResponseTypeDef(TypedDict):
    TableList: List[TableTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUnfilteredTableMetadataResponseTypeDef

```python
# GetUnfilteredTableMetadataResponseTypeDef definition

class GetUnfilteredTableMetadataResponseTypeDef(TypedDict):
    Table: TableTypeDef,  # (1)
    AuthorizedColumns: List[str],
    IsRegisteredWithLakeFormation: bool,
    CellFilters: List[ColumnRowFilterTypeDef],  # (2)
    QueryAuthorizationId: str,
    IsMultiDialectView: bool,
    ResourceArn: str,
    IsProtected: bool,
    Permissions: List[PermissionType],  # (3)
    RowFilter: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ColumnRowFilterTypeDef](./type_defs.md#columnrowfiltertypedef) 
3. See [:material-code-brackets: PermissionType](./literals.md#permissiontype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchTablesResponseTypeDef

```python
# SearchTablesResponseTypeDef definition

class SearchTablesResponseTypeDef(TypedDict):
    TableList: List[TableTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableVersionTypeDef

```python
# TableVersionTypeDef definition

class TableVersionTypeDef(TypedDict):
    Table: NotRequired[TableTypeDef],  # (1)
    VersionId: NotRequired[str],
```

1. See [:material-code-braces: TableTypeDef](./type_defs.md#tabletypedef) 
## ColumnStatisticsDataTypeDef

```python
# ColumnStatisticsDataTypeDef definition

class ColumnStatisticsDataTypeDef(TypedDict):
    Type: ColumnStatisticsTypeType,  # (1)
    BooleanColumnStatisticsData: NotRequired[BooleanColumnStatisticsDataTypeDef],  # (2)
    DateColumnStatisticsData: NotRequired[DateColumnStatisticsDataUnionTypeDef],  # (3)
    DecimalColumnStatisticsData: NotRequired[DecimalColumnStatisticsDataUnionTypeDef],  # (4)
    DoubleColumnStatisticsData: NotRequired[DoubleColumnStatisticsDataTypeDef],  # (5)
    LongColumnStatisticsData: NotRequired[LongColumnStatisticsDataTypeDef],  # (6)
    StringColumnStatisticsData: NotRequired[StringColumnStatisticsDataTypeDef],  # (7)
    BinaryColumnStatisticsData: NotRequired[BinaryColumnStatisticsDataTypeDef],  # (8)
```

1. See [:material-code-brackets: ColumnStatisticsTypeType](./literals.md#columnstatisticstypetype) 
2. See [:material-code-braces: BooleanColumnStatisticsDataTypeDef](./type_defs.md#booleancolumnstatisticsdatatypedef) 
3. See [:material-code-braces: DateColumnStatisticsDataTypeDef](./type_defs.md#datecolumnstatisticsdatatypedef) [:material-code-braces: DateColumnStatisticsDataOutputTypeDef](./type_defs.md#datecolumnstatisticsdataoutputtypedef) 
4. See [:material-code-braces: DecimalColumnStatisticsDataTypeDef](./type_defs.md#decimalcolumnstatisticsdatatypedef) [:material-code-braces: DecimalColumnStatisticsDataOutputTypeDef](./type_defs.md#decimalcolumnstatisticsdataoutputtypedef) 
5. See [:material-code-braces: DoubleColumnStatisticsDataTypeDef](./type_defs.md#doublecolumnstatisticsdatatypedef) 
6. See [:material-code-braces: LongColumnStatisticsDataTypeDef](./type_defs.md#longcolumnstatisticsdatatypedef) 
7. See [:material-code-braces: StringColumnStatisticsDataTypeDef](./type_defs.md#stringcolumnstatisticsdatatypedef) 
8. See [:material-code-braces: BinaryColumnStatisticsDataTypeDef](./type_defs.md#binarycolumnstatisticsdatatypedef) 
## WorkflowGraphTypeDef

```python
# WorkflowGraphTypeDef definition

class WorkflowGraphTypeDef(TypedDict):
    Nodes: NotRequired[List[NodeTypeDef]],  # (1)
    Edges: NotRequired[List[EdgeTypeDef]],  # (2)
```

1. See [:material-code-braces: NodeTypeDef](./type_defs.md#nodetypedef) 
2. See [:material-code-braces: EdgeTypeDef](./type_defs.md#edgetypedef) 
## UpdateColumnStatisticsForPartitionResponseTypeDef

```python
# UpdateColumnStatisticsForPartitionResponseTypeDef definition

class UpdateColumnStatisticsForPartitionResponseTypeDef(TypedDict):
    Errors: List[ColumnStatisticsErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnStatisticsErrorTypeDef](./type_defs.md#columnstatisticserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateColumnStatisticsForTableResponseTypeDef

```python
# UpdateColumnStatisticsForTableResponseTypeDef definition

class UpdateColumnStatisticsForTableResponseTypeDef(TypedDict):
    Errors: List[ColumnStatisticsErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ColumnStatisticsErrorTypeDef](./type_defs.md#columnstatisticserrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUnfilteredPartitionsMetadataResponseTypeDef

```python
# GetUnfilteredPartitionsMetadataResponseTypeDef definition

class GetUnfilteredPartitionsMetadataResponseTypeDef(TypedDict):
    UnfilteredPartitions: List[UnfilteredPartitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: UnfilteredPartitionTypeDef](./type_defs.md#unfilteredpartitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataQualityResultsRequestRequestTypeDef

```python
# ListDataQualityResultsRequestRequestTypeDef definition

class ListDataQualityResultsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DataQualityResultFilterCriteriaTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataQualityResultFilterCriteriaTypeDef](./type_defs.md#dataqualityresultfiltercriteriatypedef) 
## ListDataQualityRuleRecommendationRunsRequestRequestTypeDef

```python
# ListDataQualityRuleRecommendationRunsRequestRequestTypeDef definition

class ListDataQualityRuleRecommendationRunsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DataQualityRuleRecommendationRunFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataQualityRuleRecommendationRunFilterTypeDef](./type_defs.md#dataqualityrulerecommendationrunfiltertypedef) 
## ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef

```python
# ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef definition

class ListDataQualityRulesetEvaluationRunsRequestRequestTypeDef(TypedDict):
    Filter: NotRequired[DataQualityRulesetEvaluationRunFilterTypeDef],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: DataQualityRulesetEvaluationRunFilterTypeDef](./type_defs.md#dataqualityrulesetevaluationrunfiltertypedef) 
## BatchGetTableOptimizerResponseTypeDef

```python
# BatchGetTableOptimizerResponseTypeDef definition

class BatchGetTableOptimizerResponseTypeDef(TypedDict):
    TableOptimizers: List[BatchTableOptimizerTypeDef],  # (1)
    Failures: List[BatchGetTableOptimizerErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchTableOptimizerTypeDef](./type_defs.md#batchtableoptimizertypedef) 
2. See [:material-code-braces: BatchGetTableOptimizerErrorTypeDef](./type_defs.md#batchgettableoptimizererrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetJobsResponseTypeDef

```python
# BatchGetJobsResponseTypeDef definition

class BatchGetJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    JobsNotFound: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobResponseTypeDef

```python
# GetJobResponseTypeDef definition

class GetJobResponseTypeDef(TypedDict):
    Job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobsResponseTypeDef

```python
# GetJobsResponseTypeDef definition

class GetJobsResponseTypeDef(TypedDict):
    Jobs: List[JobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobsResponsePaginatorTypeDef

```python
# GetJobsResponsePaginatorTypeDef definition

class GetJobsResponsePaginatorTypeDef(TypedDict):
    Jobs: List[JobPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JobPaginatorTypeDef](./type_defs.md#jobpaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreatePartitionRequestRequestTypeDef

```python
# BatchCreatePartitionRequestRequestTypeDef definition

class BatchCreatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionInputList: Sequence[PartitionInputTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## BatchUpdatePartitionRequestEntryTypeDef

```python
# BatchUpdatePartitionRequestEntryTypeDef definition

class BatchUpdatePartitionRequestEntryTypeDef(TypedDict):
    PartitionValueList: Sequence[str],
    PartitionInput: PartitionInputTypeDef,  # (1)
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## CreatePartitionRequestRequestTypeDef

```python
# CreatePartitionRequestRequestTypeDef definition

class CreatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionInput: PartitionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## UpdatePartitionRequestRequestTypeDef

```python
# UpdatePartitionRequestRequestTypeDef definition

class UpdatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValueList: Sequence[str],
    PartitionInput: PartitionInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: PartitionInputTypeDef](./type_defs.md#partitioninputtypedef) 
## CreateTableRequestRequestTypeDef

```python
# CreateTableRequestRequestTypeDef definition

class CreateTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableInput: TableInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    PartitionIndexes: NotRequired[Sequence[PartitionIndexTypeDef]],  # (2)
    TransactionId: NotRequired[str],
    OpenTableFormatInput: NotRequired[OpenTableFormatInputTypeDef],  # (3)
```

1. See [:material-code-braces: TableInputTypeDef](./type_defs.md#tableinputtypedef) 
2. See [:material-code-braces: PartitionIndexTypeDef](./type_defs.md#partitionindextypedef) 
3. See [:material-code-braces: OpenTableFormatInputTypeDef](./type_defs.md#opentableformatinputtypedef) 
## UpdateTableRequestRequestTypeDef

```python
# UpdateTableRequestRequestTypeDef definition

class UpdateTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableInput: TableInputTypeDef,  # (1)
    CatalogId: NotRequired[str],
    SkipArchive: NotRequired[bool],
    TransactionId: NotRequired[str],
    VersionId: NotRequired[str],
    ViewUpdateAction: NotRequired[ViewUpdateActionType],  # (2)
    Force: NotRequired[bool],
```

1. See [:material-code-braces: TableInputTypeDef](./type_defs.md#tableinputtypedef) 
2. See [:material-code-brackets: ViewUpdateActionType](./literals.md#viewupdateactiontype) 
## GetTableVersionsResponsePaginatorTypeDef

```python
# GetTableVersionsResponsePaginatorTypeDef definition

class GetTableVersionsResponsePaginatorTypeDef(TypedDict):
    TableVersions: List[TableVersionPaginatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableVersionPaginatorTypeDef](./type_defs.md#tableversionpaginatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableVersionResponseTypeDef

```python
# GetTableVersionResponseTypeDef definition

class GetTableVersionResponseTypeDef(TypedDict):
    TableVersion: TableVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableVersionTypeDef](./type_defs.md#tableversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableVersionsResponseTypeDef

```python
# GetTableVersionsResponseTypeDef definition

class GetTableVersionsResponseTypeDef(TypedDict):
    TableVersions: List[TableVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TableVersionTypeDef](./type_defs.md#tableversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowRunTypeDef

```python
# WorkflowRunTypeDef definition

class WorkflowRunTypeDef(TypedDict):
    Name: NotRequired[str],
    WorkflowRunId: NotRequired[str],
    PreviousRunId: NotRequired[str],
    WorkflowRunProperties: NotRequired[Dict[str, str]],
    StartedOn: NotRequired[datetime],
    CompletedOn: NotRequired[datetime],
    Status: NotRequired[WorkflowRunStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    Statistics: NotRequired[WorkflowRunStatisticsTypeDef],  # (2)
    Graph: NotRequired[WorkflowGraphTypeDef],  # (3)
    StartingEventBatchCondition: NotRequired[StartingEventBatchConditionTypeDef],  # (4)
```

1. See [:material-code-brackets: WorkflowRunStatusType](./literals.md#workflowrunstatustype) 
2. See [:material-code-braces: WorkflowRunStatisticsTypeDef](./type_defs.md#workflowrunstatisticstypedef) 
3. See [:material-code-braces: WorkflowGraphTypeDef](./type_defs.md#workflowgraphtypedef) 
4. See [:material-code-braces: StartingEventBatchConditionTypeDef](./type_defs.md#startingeventbatchconditiontypedef) 
## CodeGenConfigurationNodeTypeDef

```python
# CodeGenConfigurationNodeTypeDef definition

class CodeGenConfigurationNodeTypeDef(TypedDict):
    AthenaConnectorSource: NotRequired[AthenaConnectorSourceUnionTypeDef],  # (1)
    JDBCConnectorSource: NotRequired[JDBCConnectorSourceUnionTypeDef],  # (2)
    SparkConnectorSource: NotRequired[SparkConnectorSourceUnionTypeDef],  # (3)
    CatalogSource: NotRequired[CatalogSourceTypeDef],  # (4)
    RedshiftSource: NotRequired[RedshiftSourceTypeDef],  # (5)
    S3CatalogSource: NotRequired[S3CatalogSourceTypeDef],  # (6)
    S3CsvSource: NotRequired[S3CsvSourceUnionTypeDef],  # (7)
    S3JsonSource: NotRequired[S3JsonSourceUnionTypeDef],  # (8)
    S3ParquetSource: NotRequired[S3ParquetSourceUnionTypeDef],  # (9)
    RelationalCatalogSource: NotRequired[RelationalCatalogSourceTypeDef],  # (10)
    DynamoDBCatalogSource: NotRequired[DynamoDBCatalogSourceTypeDef],  # (11)
    JDBCConnectorTarget: NotRequired[JDBCConnectorTargetUnionTypeDef],  # (12)
    SparkConnectorTarget: NotRequired[SparkConnectorTargetUnionTypeDef],  # (13)
    CatalogTarget: NotRequired[BasicCatalogTargetUnionTypeDef],  # (14)
    RedshiftTarget: NotRequired[RedshiftTargetUnionTypeDef],  # (15)
    S3CatalogTarget: NotRequired[S3CatalogTargetUnionTypeDef],  # (16)
    S3GlueParquetTarget: NotRequired[S3GlueParquetTargetUnionTypeDef],  # (17)
    S3DirectTarget: NotRequired[S3DirectTargetUnionTypeDef],  # (18)
    ApplyMapping: NotRequired[ApplyMappingUnionTypeDef],  # (19)
    SelectFields: NotRequired[SelectFieldsUnionTypeDef],  # (20)
    DropFields: NotRequired[DropFieldsUnionTypeDef],  # (21)
    RenameField: NotRequired[RenameFieldUnionTypeDef],  # (22)
    Spigot: NotRequired[SpigotUnionTypeDef],  # (23)
    Join: NotRequired[JoinUnionTypeDef],  # (24)
    SplitFields: NotRequired[SplitFieldsUnionTypeDef],  # (25)
    SelectFromCollection: NotRequired[SelectFromCollectionUnionTypeDef],  # (26)
    FillMissingValues: NotRequired[FillMissingValuesUnionTypeDef],  # (27)
    Filter: NotRequired[FilterUnionTypeDef],  # (28)
    CustomCode: NotRequired[CustomCodeUnionTypeDef],  # (29)
    SparkSQL: NotRequired[SparkSQLUnionTypeDef],  # (30)
    DirectKinesisSource: NotRequired[DirectKinesisSourceUnionTypeDef],  # (31)
    DirectKafkaSource: NotRequired[DirectKafkaSourceUnionTypeDef],  # (32)
    CatalogKinesisSource: NotRequired[CatalogKinesisSourceUnionTypeDef],  # (33)
    CatalogKafkaSource: NotRequired[CatalogKafkaSourceUnionTypeDef],  # (34)
    DropNullFields: NotRequired[DropNullFieldsUnionTypeDef],  # (35)
    Merge: NotRequired[MergeUnionTypeDef],  # (36)
    Union: NotRequired[UnionUnionTypeDef],  # (37)
    PIIDetection: NotRequired[PIIDetectionUnionTypeDef],  # (38)
    Aggregate: NotRequired[AggregateUnionTypeDef],  # (39)
    DropDuplicates: NotRequired[DropDuplicatesUnionTypeDef],  # (40)
    GovernedCatalogTarget: NotRequired[GovernedCatalogTargetUnionTypeDef],  # (41)
    GovernedCatalogSource: NotRequired[GovernedCatalogSourceTypeDef],  # (42)
    MicrosoftSQLServerCatalogSource: NotRequired[MicrosoftSQLServerCatalogSourceTypeDef],  # (43)
    MySQLCatalogSource: NotRequired[MySQLCatalogSourceTypeDef],  # (44)
    OracleSQLCatalogSource: NotRequired[OracleSQLCatalogSourceTypeDef],  # (45)
    PostgreSQLCatalogSource: NotRequired[PostgreSQLCatalogSourceTypeDef],  # (46)
    MicrosoftSQLServerCatalogTarget: NotRequired[MicrosoftSQLServerCatalogTargetUnionTypeDef],  # (47)
    MySQLCatalogTarget: NotRequired[MySQLCatalogTargetUnionTypeDef],  # (48)
    OracleSQLCatalogTarget: NotRequired[OracleSQLCatalogTargetUnionTypeDef],  # (49)
    PostgreSQLCatalogTarget: NotRequired[PostgreSQLCatalogTargetUnionTypeDef],  # (50)
    DynamicTransform: NotRequired[DynamicTransformUnionTypeDef],  # (51)
    EvaluateDataQuality: NotRequired[EvaluateDataQualityUnionTypeDef],  # (52)
    S3CatalogHudiSource: NotRequired[S3CatalogHudiSourceUnionTypeDef],  # (53)
    CatalogHudiSource: NotRequired[CatalogHudiSourceUnionTypeDef],  # (54)
    S3HudiSource: NotRequired[S3HudiSourceUnionTypeDef],  # (55)
    S3HudiCatalogTarget: NotRequired[S3HudiCatalogTargetUnionTypeDef],  # (56)
    S3HudiDirectTarget: NotRequired[S3HudiDirectTargetUnionTypeDef],  # (57)
    DirectJDBCSource: NotRequired[DirectJDBCSourceTypeDef],  # (58)
    S3CatalogDeltaSource: NotRequired[S3CatalogDeltaSourceUnionTypeDef],  # (59)
    CatalogDeltaSource: NotRequired[CatalogDeltaSourceUnionTypeDef],  # (60)
    S3DeltaSource: NotRequired[S3DeltaSourceUnionTypeDef],  # (61)
    S3DeltaCatalogTarget: NotRequired[S3DeltaCatalogTargetUnionTypeDef],  # (62)
    S3DeltaDirectTarget: NotRequired[S3DeltaDirectTargetUnionTypeDef],  # (63)
    AmazonRedshiftSource: NotRequired[AmazonRedshiftSourceUnionTypeDef],  # (64)
    AmazonRedshiftTarget: NotRequired[AmazonRedshiftTargetUnionTypeDef],  # (65)
    EvaluateDataQualityMultiFrame: NotRequired[EvaluateDataQualityMultiFrameUnionTypeDef],  # (66)
    Recipe: NotRequired[RecipeUnionTypeDef],  # (67)
    SnowflakeSource: NotRequired[SnowflakeSourceUnionTypeDef],  # (68)
    SnowflakeTarget: NotRequired[SnowflakeTargetUnionTypeDef],  # (69)
    ConnectorDataSource: NotRequired[ConnectorDataSourceUnionTypeDef],  # (70)
    ConnectorDataTarget: NotRequired[ConnectorDataTargetUnionTypeDef],  # (71)
```

1. See [:material-code-braces: AthenaConnectorSourceTypeDef](./type_defs.md#athenaconnectorsourcetypedef) [:material-code-braces: AthenaConnectorSourceOutputTypeDef](./type_defs.md#athenaconnectorsourceoutputtypedef) 
2. See [:material-code-braces: JDBCConnectorSourceTypeDef](./type_defs.md#jdbcconnectorsourcetypedef) [:material-code-braces: JDBCConnectorSourceOutputTypeDef](./type_defs.md#jdbcconnectorsourceoutputtypedef) 
3. See [:material-code-braces: SparkConnectorSourceTypeDef](./type_defs.md#sparkconnectorsourcetypedef) [:material-code-braces: SparkConnectorSourceOutputTypeDef](./type_defs.md#sparkconnectorsourceoutputtypedef) 
4. See [:material-code-braces: CatalogSourceTypeDef](./type_defs.md#catalogsourcetypedef) 
5. See [:material-code-braces: RedshiftSourceTypeDef](./type_defs.md#redshiftsourcetypedef) 
6. See [:material-code-braces: S3CatalogSourceTypeDef](./type_defs.md#s3catalogsourcetypedef) 
7. See [:material-code-braces: S3CsvSourceTypeDef](./type_defs.md#s3csvsourcetypedef) [:material-code-braces: S3CsvSourceOutputTypeDef](./type_defs.md#s3csvsourceoutputtypedef) 
8. See [:material-code-braces: S3JsonSourceTypeDef](./type_defs.md#s3jsonsourcetypedef) [:material-code-braces: S3JsonSourceOutputTypeDef](./type_defs.md#s3jsonsourceoutputtypedef) 
9. See [:material-code-braces: S3ParquetSourceTypeDef](./type_defs.md#s3parquetsourcetypedef) [:material-code-braces: S3ParquetSourceOutputTypeDef](./type_defs.md#s3parquetsourceoutputtypedef) 
10. See [:material-code-braces: RelationalCatalogSourceTypeDef](./type_defs.md#relationalcatalogsourcetypedef) 
11. See [:material-code-braces: DynamoDBCatalogSourceTypeDef](./type_defs.md#dynamodbcatalogsourcetypedef) 
12. See [:material-code-braces: JDBCConnectorTargetTypeDef](./type_defs.md#jdbcconnectortargettypedef) [:material-code-braces: JDBCConnectorTargetOutputTypeDef](./type_defs.md#jdbcconnectortargetoutputtypedef) 
13. See [:material-code-braces: SparkConnectorTargetTypeDef](./type_defs.md#sparkconnectortargettypedef) [:material-code-braces: SparkConnectorTargetOutputTypeDef](./type_defs.md#sparkconnectortargetoutputtypedef) 
14. See [:material-code-braces: BasicCatalogTargetTypeDef](./type_defs.md#basiccatalogtargettypedef) [:material-code-braces: BasicCatalogTargetOutputTypeDef](./type_defs.md#basiccatalogtargetoutputtypedef) 
15. See [:material-code-braces: RedshiftTargetTypeDef](./type_defs.md#redshifttargettypedef) [:material-code-braces: RedshiftTargetOutputTypeDef](./type_defs.md#redshifttargetoutputtypedef) 
16. See [:material-code-braces: S3CatalogTargetTypeDef](./type_defs.md#s3catalogtargettypedef) [:material-code-braces: S3CatalogTargetOutputTypeDef](./type_defs.md#s3catalogtargetoutputtypedef) 
17. See [:material-code-braces: S3GlueParquetTargetTypeDef](./type_defs.md#s3glueparquettargettypedef) [:material-code-braces: S3GlueParquetTargetOutputTypeDef](./type_defs.md#s3glueparquettargetoutputtypedef) 
18. See [:material-code-braces: S3DirectTargetTypeDef](./type_defs.md#s3directtargettypedef) [:material-code-braces: S3DirectTargetOutputTypeDef](./type_defs.md#s3directtargetoutputtypedef) 
19. See [:material-code-braces: ApplyMappingTypeDef](./type_defs.md#applymappingtypedef) [:material-code-braces: ApplyMappingOutputTypeDef](./type_defs.md#applymappingoutputtypedef) 
20. See [:material-code-braces: SelectFieldsTypeDef](./type_defs.md#selectfieldstypedef) [:material-code-braces: SelectFieldsOutputTypeDef](./type_defs.md#selectfieldsoutputtypedef) 
21. See [:material-code-braces: DropFieldsTypeDef](./type_defs.md#dropfieldstypedef) [:material-code-braces: DropFieldsOutputTypeDef](./type_defs.md#dropfieldsoutputtypedef) 
22. See [:material-code-braces: RenameFieldTypeDef](./type_defs.md#renamefieldtypedef) [:material-code-braces: RenameFieldOutputTypeDef](./type_defs.md#renamefieldoutputtypedef) 
23. See [:material-code-braces: SpigotTypeDef](./type_defs.md#spigottypedef) [:material-code-braces: SpigotOutputTypeDef](./type_defs.md#spigotoutputtypedef) 
24. See [:material-code-braces: JoinTypeDef](./type_defs.md#jointypedef) [:material-code-braces: JoinOutputTypeDef](./type_defs.md#joinoutputtypedef) 
25. See [:material-code-braces: SplitFieldsTypeDef](./type_defs.md#splitfieldstypedef) [:material-code-braces: SplitFieldsOutputTypeDef](./type_defs.md#splitfieldsoutputtypedef) 
26. See [:material-code-braces: SelectFromCollectionTypeDef](./type_defs.md#selectfromcollectiontypedef) [:material-code-braces: SelectFromCollectionOutputTypeDef](./type_defs.md#selectfromcollectionoutputtypedef) 
27. See [:material-code-braces: FillMissingValuesTypeDef](./type_defs.md#fillmissingvaluestypedef) [:material-code-braces: FillMissingValuesOutputTypeDef](./type_defs.md#fillmissingvaluesoutputtypedef) 
28. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) [:material-code-braces: FilterOutputTypeDef](./type_defs.md#filteroutputtypedef) 
29. See [:material-code-braces: CustomCodeTypeDef](./type_defs.md#customcodetypedef) [:material-code-braces: CustomCodeOutputTypeDef](./type_defs.md#customcodeoutputtypedef) 
30. See [:material-code-braces: SparkSQLTypeDef](./type_defs.md#sparksqltypedef) [:material-code-braces: SparkSQLOutputTypeDef](./type_defs.md#sparksqloutputtypedef) 
31. See [:material-code-braces: DirectKinesisSourceTypeDef](./type_defs.md#directkinesissourcetypedef) [:material-code-braces: DirectKinesisSourceOutputTypeDef](./type_defs.md#directkinesissourceoutputtypedef) 
32. See [:material-code-braces: DirectKafkaSourceTypeDef](./type_defs.md#directkafkasourcetypedef) [:material-code-braces: DirectKafkaSourceOutputTypeDef](./type_defs.md#directkafkasourceoutputtypedef) 
33. See [:material-code-braces: CatalogKinesisSourceTypeDef](./type_defs.md#catalogkinesissourcetypedef) [:material-code-braces: CatalogKinesisSourceOutputTypeDef](./type_defs.md#catalogkinesissourceoutputtypedef) 
34. See [:material-code-braces: CatalogKafkaSourceTypeDef](./type_defs.md#catalogkafkasourcetypedef) [:material-code-braces: CatalogKafkaSourceOutputTypeDef](./type_defs.md#catalogkafkasourceoutputtypedef) 
35. See [:material-code-braces: DropNullFieldsTypeDef](./type_defs.md#dropnullfieldstypedef) [:material-code-braces: DropNullFieldsOutputTypeDef](./type_defs.md#dropnullfieldsoutputtypedef) 
36. See [:material-code-braces: MergeTypeDef](./type_defs.md#mergetypedef) [:material-code-braces: MergeOutputTypeDef](./type_defs.md#mergeoutputtypedef) 
37. See [:material-code-braces: UnionTypeDef](./type_defs.md#uniontypedef) [:material-code-braces: UnionOutputTypeDef](./type_defs.md#unionoutputtypedef) 
38. See [:material-code-braces: PIIDetectionTypeDef](./type_defs.md#piidetectiontypedef) [:material-code-braces: PIIDetectionOutputTypeDef](./type_defs.md#piidetectionoutputtypedef) 
39. See [:material-code-braces: AggregateTypeDef](./type_defs.md#aggregatetypedef) [:material-code-braces: AggregateOutputTypeDef](./type_defs.md#aggregateoutputtypedef) 
40. See [:material-code-braces: DropDuplicatesTypeDef](./type_defs.md#dropduplicatestypedef) [:material-code-braces: DropDuplicatesOutputTypeDef](./type_defs.md#dropduplicatesoutputtypedef) 
41. See [:material-code-braces: GovernedCatalogTargetTypeDef](./type_defs.md#governedcatalogtargettypedef) [:material-code-braces: GovernedCatalogTargetOutputTypeDef](./type_defs.md#governedcatalogtargetoutputtypedef) 
42. See [:material-code-braces: GovernedCatalogSourceTypeDef](./type_defs.md#governedcatalogsourcetypedef) 
43. See [:material-code-braces: MicrosoftSQLServerCatalogSourceTypeDef](./type_defs.md#microsoftsqlservercatalogsourcetypedef) 
44. See [:material-code-braces: MySQLCatalogSourceTypeDef](./type_defs.md#mysqlcatalogsourcetypedef) 
45. See [:material-code-braces: OracleSQLCatalogSourceTypeDef](./type_defs.md#oraclesqlcatalogsourcetypedef) 
46. See [:material-code-braces: PostgreSQLCatalogSourceTypeDef](./type_defs.md#postgresqlcatalogsourcetypedef) 
47. See [:material-code-braces: MicrosoftSQLServerCatalogTargetTypeDef](./type_defs.md#microsoftsqlservercatalogtargettypedef) [:material-code-braces: MicrosoftSQLServerCatalogTargetOutputTypeDef](./type_defs.md#microsoftsqlservercatalogtargetoutputtypedef) 
48. See [:material-code-braces: MySQLCatalogTargetTypeDef](./type_defs.md#mysqlcatalogtargettypedef) [:material-code-braces: MySQLCatalogTargetOutputTypeDef](./type_defs.md#mysqlcatalogtargetoutputtypedef) 
49. See [:material-code-braces: OracleSQLCatalogTargetTypeDef](./type_defs.md#oraclesqlcatalogtargettypedef) [:material-code-braces: OracleSQLCatalogTargetOutputTypeDef](./type_defs.md#oraclesqlcatalogtargetoutputtypedef) 
50. See [:material-code-braces: PostgreSQLCatalogTargetTypeDef](./type_defs.md#postgresqlcatalogtargettypedef) [:material-code-braces: PostgreSQLCatalogTargetOutputTypeDef](./type_defs.md#postgresqlcatalogtargetoutputtypedef) 
51. See [:material-code-braces: DynamicTransformTypeDef](./type_defs.md#dynamictransformtypedef) [:material-code-braces: DynamicTransformOutputTypeDef](./type_defs.md#dynamictransformoutputtypedef) 
52. See [:material-code-braces: EvaluateDataQualityTypeDef](./type_defs.md#evaluatedataqualitytypedef) [:material-code-braces: EvaluateDataQualityOutputTypeDef](./type_defs.md#evaluatedataqualityoutputtypedef) 
53. See [:material-code-braces: S3CatalogHudiSourceTypeDef](./type_defs.md#s3cataloghudisourcetypedef) [:material-code-braces: S3CatalogHudiSourceOutputTypeDef](./type_defs.md#s3cataloghudisourceoutputtypedef) 
54. See [:material-code-braces: CatalogHudiSourceTypeDef](./type_defs.md#cataloghudisourcetypedef) [:material-code-braces: CatalogHudiSourceOutputTypeDef](./type_defs.md#cataloghudisourceoutputtypedef) 
55. See [:material-code-braces: S3HudiSourceTypeDef](./type_defs.md#s3hudisourcetypedef) [:material-code-braces: S3HudiSourceOutputTypeDef](./type_defs.md#s3hudisourceoutputtypedef) 
56. See [:material-code-braces: S3HudiCatalogTargetTypeDef](./type_defs.md#s3hudicatalogtargettypedef) [:material-code-braces: S3HudiCatalogTargetOutputTypeDef](./type_defs.md#s3hudicatalogtargetoutputtypedef) 
57. See [:material-code-braces: S3HudiDirectTargetTypeDef](./type_defs.md#s3hudidirecttargettypedef) [:material-code-braces: S3HudiDirectTargetOutputTypeDef](./type_defs.md#s3hudidirecttargetoutputtypedef) 
58. See [:material-code-braces: DirectJDBCSourceTypeDef](./type_defs.md#directjdbcsourcetypedef) 
59. See [:material-code-braces: S3CatalogDeltaSourceTypeDef](./type_defs.md#s3catalogdeltasourcetypedef) [:material-code-braces: S3CatalogDeltaSourceOutputTypeDef](./type_defs.md#s3catalogdeltasourceoutputtypedef) 
60. See [:material-code-braces: CatalogDeltaSourceTypeDef](./type_defs.md#catalogdeltasourcetypedef) [:material-code-braces: CatalogDeltaSourceOutputTypeDef](./type_defs.md#catalogdeltasourceoutputtypedef) 
61. See [:material-code-braces: S3DeltaSourceTypeDef](./type_defs.md#s3deltasourcetypedef) [:material-code-braces: S3DeltaSourceOutputTypeDef](./type_defs.md#s3deltasourceoutputtypedef) 
62. See [:material-code-braces: S3DeltaCatalogTargetTypeDef](./type_defs.md#s3deltacatalogtargettypedef) [:material-code-braces: S3DeltaCatalogTargetOutputTypeDef](./type_defs.md#s3deltacatalogtargetoutputtypedef) 
63. See [:material-code-braces: S3DeltaDirectTargetTypeDef](./type_defs.md#s3deltadirecttargettypedef) [:material-code-braces: S3DeltaDirectTargetOutputTypeDef](./type_defs.md#s3deltadirecttargetoutputtypedef) 
64. See [:material-code-braces: AmazonRedshiftSourceTypeDef](./type_defs.md#amazonredshiftsourcetypedef) [:material-code-braces: AmazonRedshiftSourceOutputTypeDef](./type_defs.md#amazonredshiftsourceoutputtypedef) 
65. See [:material-code-braces: AmazonRedshiftTargetTypeDef](./type_defs.md#amazonredshifttargettypedef) [:material-code-braces: AmazonRedshiftTargetOutputTypeDef](./type_defs.md#amazonredshifttargetoutputtypedef) 
66. See [:material-code-braces: EvaluateDataQualityMultiFrameTypeDef](./type_defs.md#evaluatedataqualitymultiframetypedef) [:material-code-braces: EvaluateDataQualityMultiFrameOutputTypeDef](./type_defs.md#evaluatedataqualitymultiframeoutputtypedef) 
67. See [:material-code-braces: RecipeTypeDef](./type_defs.md#recipetypedef) [:material-code-braces: RecipeOutputTypeDef](./type_defs.md#recipeoutputtypedef) 
68. See [:material-code-braces: SnowflakeSourceTypeDef](./type_defs.md#snowflakesourcetypedef) [:material-code-braces: SnowflakeSourceOutputTypeDef](./type_defs.md#snowflakesourceoutputtypedef) 
69. See [:material-code-braces: SnowflakeTargetTypeDef](./type_defs.md#snowflaketargettypedef) [:material-code-braces: SnowflakeTargetOutputTypeDef](./type_defs.md#snowflaketargetoutputtypedef) 
70. See [:material-code-braces: ConnectorDataSourceTypeDef](./type_defs.md#connectordatasourcetypedef) [:material-code-braces: ConnectorDataSourceOutputTypeDef](./type_defs.md#connectordatasourceoutputtypedef) 
71. See [:material-code-braces: ConnectorDataTargetTypeDef](./type_defs.md#connectordatatargettypedef) [:material-code-braces: ConnectorDataTargetOutputTypeDef](./type_defs.md#connectordatatargetoutputtypedef) 
## BatchUpdatePartitionRequestRequestTypeDef

```python
# BatchUpdatePartitionRequestRequestTypeDef definition

class BatchUpdatePartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    Entries: Sequence[BatchUpdatePartitionRequestEntryTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: BatchUpdatePartitionRequestEntryTypeDef](./type_defs.md#batchupdatepartitionrequestentrytypedef) 
## ColumnStatisticsTypeDef

```python
# ColumnStatisticsTypeDef definition

class ColumnStatisticsTypeDef(TypedDict):
    ColumnName: str,
    ColumnType: str,
    AnalyzedTime: TimestampTypeDef,
    StatisticsData: ColumnStatisticsDataUnionTypeDef,  # (1)
```

1. See [:material-code-braces: ColumnStatisticsDataTypeDef](./type_defs.md#columnstatisticsdatatypedef) [:material-code-braces: ColumnStatisticsDataOutputTypeDef](./type_defs.md#columnstatisticsdataoutputtypedef) 
## GetWorkflowRunResponseTypeDef

```python
# GetWorkflowRunResponseTypeDef definition

class GetWorkflowRunResponseTypeDef(TypedDict):
    Run: WorkflowRunTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowRunTypeDef](./type_defs.md#workflowruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowRunsResponseTypeDef

```python
# GetWorkflowRunsResponseTypeDef definition

class GetWorkflowRunsResponseTypeDef(TypedDict):
    Runs: List[WorkflowRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkflowRunTypeDef](./type_defs.md#workflowruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkflowTypeDef

```python
# WorkflowTypeDef definition

class WorkflowTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    DefaultRunProperties: NotRequired[Dict[str, str]],
    CreatedOn: NotRequired[datetime],
    LastModifiedOn: NotRequired[datetime],
    LastRun: NotRequired[WorkflowRunTypeDef],  # (1)
    Graph: NotRequired[WorkflowGraphTypeDef],  # (2)
    MaxConcurrentRuns: NotRequired[int],
    BlueprintDetails: NotRequired[BlueprintDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: WorkflowRunTypeDef](./type_defs.md#workflowruntypedef) 
2. See [:material-code-braces: WorkflowGraphTypeDef](./type_defs.md#workflowgraphtypedef) 
3. See [:material-code-braces: BlueprintDetailsTypeDef](./type_defs.md#blueprintdetailstypedef) 
## UpdateColumnStatisticsForTableRequestRequestTypeDef

```python
# UpdateColumnStatisticsForTableRequestRequestTypeDef definition

class UpdateColumnStatisticsForTableRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    ColumnStatisticsList: Sequence[ColumnStatisticsTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) 
## BatchGetWorkflowsResponseTypeDef

```python
# BatchGetWorkflowsResponseTypeDef definition

class BatchGetWorkflowsResponseTypeDef(TypedDict):
    Workflows: List[WorkflowTypeDef],  # (1)
    MissingWorkflows: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowTypeDef](./type_defs.md#workflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkflowResponseTypeDef

```python
# GetWorkflowResponseTypeDef definition

class GetWorkflowResponseTypeDef(TypedDict):
    Workflow: WorkflowTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkflowTypeDef](./type_defs.md#workflowtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateJobRequestRequestTypeDef

```python
# CreateJobRequestRequestTypeDef definition

class CreateJobRequestRequestTypeDef(TypedDict):
    Name: str,
    Role: str,
    Command: JobCommandTypeDef,  # (1)
    JobMode: NotRequired[JobModeType],  # (2)
    JobRunQueuingEnabled: NotRequired[bool],
    Description: NotRequired[str],
    LogUri: NotRequired[str],
    ExecutionProperty: NotRequired[ExecutionPropertyTypeDef],  # (3)
    DefaultArguments: NotRequired[Mapping[str, str]],
    NonOverridableArguments: NotRequired[Mapping[str, str]],
    Connections: NotRequired[ConnectionsListTypeDef],  # (4)
    MaxRetries: NotRequired[int],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    SecurityConfiguration: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (5)
    GlueVersion: NotRequired[str],
    NumberOfWorkers: NotRequired[int],
    WorkerType: NotRequired[WorkerTypeType],  # (6)
    CodeGenConfigurationNodes: NotRequired[Mapping[str, CodeGenConfigurationNodeUnionTypeDef]],  # (7)
    ExecutionClass: NotRequired[ExecutionClassType],  # (8)
    SourceControlDetails: NotRequired[SourceControlDetailsTypeDef],  # (9)
    MaintenanceWindow: NotRequired[str],
```

1. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
2. See [:material-code-brackets: JobModeType](./literals.md#jobmodetype) 
3. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
4. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) 
5. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
6. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
7. See [:material-code-braces: CodeGenConfigurationNodeTypeDef](./type_defs.md#codegenconfigurationnodetypedef) [:material-code-braces: CodeGenConfigurationNodeOutputTypeDef](./type_defs.md#codegenconfigurationnodeoutputtypedef) 
8. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
9. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
## JobUpdateTypeDef

```python
# JobUpdateTypeDef definition

class JobUpdateTypeDef(TypedDict):
    JobMode: NotRequired[JobModeType],  # (1)
    JobRunQueuingEnabled: NotRequired[bool],
    Description: NotRequired[str],
    LogUri: NotRequired[str],
    Role: NotRequired[str],
    ExecutionProperty: NotRequired[ExecutionPropertyTypeDef],  # (2)
    Command: NotRequired[JobCommandTypeDef],  # (3)
    DefaultArguments: NotRequired[Mapping[str, str]],
    NonOverridableArguments: NotRequired[Mapping[str, str]],
    Connections: NotRequired[ConnectionsListUnionTypeDef],  # (4)
    MaxRetries: NotRequired[int],
    AllocatedCapacity: NotRequired[int],
    Timeout: NotRequired[int],
    MaxCapacity: NotRequired[float],
    WorkerType: NotRequired[WorkerTypeType],  # (5)
    NumberOfWorkers: NotRequired[int],
    SecurityConfiguration: NotRequired[str],
    NotificationProperty: NotRequired[NotificationPropertyTypeDef],  # (6)
    GlueVersion: NotRequired[str],
    CodeGenConfigurationNodes: NotRequired[Mapping[str, CodeGenConfigurationNodeUnionTypeDef]],  # (7)
    ExecutionClass: NotRequired[ExecutionClassType],  # (8)
    SourceControlDetails: NotRequired[SourceControlDetailsTypeDef],  # (9)
    MaintenanceWindow: NotRequired[str],
```

1. See [:material-code-brackets: JobModeType](./literals.md#jobmodetype) 
2. See [:material-code-braces: ExecutionPropertyTypeDef](./type_defs.md#executionpropertytypedef) 
3. See [:material-code-braces: JobCommandTypeDef](./type_defs.md#jobcommandtypedef) 
4. See [:material-code-braces: ConnectionsListTypeDef](./type_defs.md#connectionslisttypedef) [:material-code-braces: ConnectionsListOutputTypeDef](./type_defs.md#connectionslistoutputtypedef) 
5. See [:material-code-brackets: WorkerTypeType](./literals.md#workertypetype) 
6. See [:material-code-braces: NotificationPropertyTypeDef](./type_defs.md#notificationpropertytypedef) 
7. See [:material-code-braces: CodeGenConfigurationNodeTypeDef](./type_defs.md#codegenconfigurationnodetypedef) [:material-code-braces: CodeGenConfigurationNodeOutputTypeDef](./type_defs.md#codegenconfigurationnodeoutputtypedef) 
8. See [:material-code-brackets: ExecutionClassType](./literals.md#executionclasstype) 
9. See [:material-code-braces: SourceControlDetailsTypeDef](./type_defs.md#sourcecontroldetailstypedef) 
## UpdateColumnStatisticsForPartitionRequestRequestTypeDef

```python
# UpdateColumnStatisticsForPartitionRequestRequestTypeDef definition

class UpdateColumnStatisticsForPartitionRequestRequestTypeDef(TypedDict):
    DatabaseName: str,
    TableName: str,
    PartitionValues: Sequence[str],
    ColumnStatisticsList: Sequence[ColumnStatisticsUnionTypeDef],  # (1)
    CatalogId: NotRequired[str],
```

1. See [:material-code-braces: ColumnStatisticsTypeDef](./type_defs.md#columnstatisticstypedef) [:material-code-braces: ColumnStatisticsOutputTypeDef](./type_defs.md#columnstatisticsoutputtypedef) 
## UpdateJobRequestRequestTypeDef

```python
# UpdateJobRequestRequestTypeDef definition

class UpdateJobRequestRequestTypeDef(TypedDict):
    JobName: str,
    JobUpdate: JobUpdateTypeDef,  # (1)
```

1. See [:material-code-braces: JobUpdateTypeDef](./type_defs.md#jobupdatetypedef) 
