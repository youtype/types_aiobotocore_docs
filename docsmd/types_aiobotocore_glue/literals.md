# Literals

> [Index](../README.md) > [Glue](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#Glue)
    type annotations stubs module [types-aiobotocore-glue](https://pypi.org/project/types-aiobotocore-glue/).

## AdditionalOptionKeysType

```python
# AdditionalOptionKeysType usage example

from types_aiobotocore_glue.literals import AdditionalOptionKeysType

def get_value() -> AdditionalOptionKeysType:
    return "performanceTuning.caching"
```

```python
# AdditionalOptionKeysType definition

AdditionalOptionKeysType = Literal[
    "performanceTuning.caching",
]
```
## AggFunctionType

```python
# AggFunctionType usage example

from types_aiobotocore_glue.literals import AggFunctionType

def get_value() -> AggFunctionType:
    return "avg"
```

```python
# AggFunctionType definition

AggFunctionType = Literal[
    "avg",
    "count",
    "countDistinct",
    "first",
    "kurtosis",
    "last",
    "max",
    "min",
    "skewness",
    "stddev_pop",
    "stddev_samp",
    "sum",
    "sumDistinct",
    "var_pop",
    "var_samp",
]
```
## BackfillErrorCodeType

```python
# BackfillErrorCodeType usage example

from types_aiobotocore_glue.literals import BackfillErrorCodeType

def get_value() -> BackfillErrorCodeType:
    return "ENCRYPTED_PARTITION_ERROR"
```

```python
# BackfillErrorCodeType definition

BackfillErrorCodeType = Literal[
    "ENCRYPTED_PARTITION_ERROR",
    "INTERNAL_ERROR",
    "INVALID_PARTITION_TYPE_DATA_ERROR",
    "MISSING_PARTITION_VALUE_ERROR",
    "UNSUPPORTED_PARTITION_CHARACTER_ERROR",
]
```
## BlueprintRunStateType

```python
# BlueprintRunStateType usage example

from types_aiobotocore_glue.literals import BlueprintRunStateType

def get_value() -> BlueprintRunStateType:
    return "FAILED"
```

```python
# BlueprintRunStateType definition

BlueprintRunStateType = Literal[
    "FAILED",
    "ROLLING_BACK",
    "RUNNING",
    "SUCCEEDED",
]
```
## BlueprintStatusType

```python
# BlueprintStatusType usage example

from types_aiobotocore_glue.literals import BlueprintStatusType

def get_value() -> BlueprintStatusType:
    return "ACTIVE"
```

```python
# BlueprintStatusType definition

BlueprintStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "FAILED",
    "UPDATING",
]
```
## CatalogEncryptionModeType

```python
# CatalogEncryptionModeType usage example

from types_aiobotocore_glue.literals import CatalogEncryptionModeType

def get_value() -> CatalogEncryptionModeType:
    return "DISABLED"
```

```python
# CatalogEncryptionModeType definition

CatalogEncryptionModeType = Literal[
    "DISABLED",
    "SSE-KMS",
]
```
## CloudWatchEncryptionModeType

```python
# CloudWatchEncryptionModeType usage example

from types_aiobotocore_glue.literals import CloudWatchEncryptionModeType

def get_value() -> CloudWatchEncryptionModeType:
    return "DISABLED"
```

```python
# CloudWatchEncryptionModeType definition

CloudWatchEncryptionModeType = Literal[
    "DISABLED",
    "SSE-KMS",
]
```
## ColumnStatisticsTypeType

```python
# ColumnStatisticsTypeType usage example

from types_aiobotocore_glue.literals import ColumnStatisticsTypeType

def get_value() -> ColumnStatisticsTypeType:
    return "BINARY"
```

```python
# ColumnStatisticsTypeType definition

ColumnStatisticsTypeType = Literal[
    "BINARY",
    "BOOLEAN",
    "DATE",
    "DECIMAL",
    "DOUBLE",
    "LONG",
    "STRING",
]
```
## ComparatorType

```python
# ComparatorType usage example

from types_aiobotocore_glue.literals import ComparatorType

def get_value() -> ComparatorType:
    return "EQUALS"
```

```python
# ComparatorType definition

ComparatorType = Literal[
    "EQUALS",
    "GREATER_THAN",
    "GREATER_THAN_EQUALS",
    "LESS_THAN",
    "LESS_THAN_EQUALS",
]
```
## CompatibilityType

```python
# CompatibilityType usage example

from types_aiobotocore_glue.literals import CompatibilityType

def get_value() -> CompatibilityType:
    return "BACKWARD"
```

```python
# CompatibilityType definition

CompatibilityType = Literal[
    "BACKWARD",
    "BACKWARD_ALL",
    "DISABLED",
    "FORWARD",
    "FORWARD_ALL",
    "FULL",
    "FULL_ALL",
    "NONE",
]
```
## CompressionTypeType

```python
# CompressionTypeType usage example

from types_aiobotocore_glue.literals import CompressionTypeType

def get_value() -> CompressionTypeType:
    return "bzip2"
```

```python
# CompressionTypeType definition

CompressionTypeType = Literal[
    "bzip2",
    "gzip",
]
```
## ConnectionPropertyKeyType

```python
# ConnectionPropertyKeyType usage example

from types_aiobotocore_glue.literals import ConnectionPropertyKeyType

def get_value() -> ConnectionPropertyKeyType:
    return "CONFIG_FILES"
```

```python
# ConnectionPropertyKeyType definition

ConnectionPropertyKeyType = Literal[
    "CONFIG_FILES",
    "CONNECTION_URL",
    "CONNECTOR_CLASS_NAME",
    "CONNECTOR_TYPE",
    "CONNECTOR_URL",
    "CUSTOM_JDBC_CERT",
    "CUSTOM_JDBC_CERT_STRING",
    "ENCRYPTED_KAFKA_CLIENT_KEY_PASSWORD",
    "ENCRYPTED_KAFKA_CLIENT_KEYSTORE_PASSWORD",
    "ENCRYPTED_KAFKA_SASL_SCRAM_PASSWORD",
    "ENCRYPTED_PASSWORD",
    "HOST",
    "INSTANCE_ID",
    "JDBC_CONNECTION_URL",
    "JDBC_DRIVER_CLASS_NAME",
    "JDBC_DRIVER_JAR_URI",
    "JDBC_ENFORCE_SSL",
    "JDBC_ENGINE",
    "JDBC_ENGINE_VERSION",
    "KAFKA_BOOTSTRAP_SERVERS",
    "KAFKA_CLIENT_KEY_PASSWORD",
    "KAFKA_CLIENT_KEYSTORE",
    "KAFKA_CLIENT_KEYSTORE_PASSWORD",
    "KAFKA_CUSTOM_CERT",
    "KAFKA_SASL_GSSAPI_KEYTAB",
    "KAFKA_SASL_GSSAPI_KRB5_CONF",
    "KAFKA_SASL_GSSAPI_PRINCIPAL",
    "KAFKA_SASL_GSSAPI_SERVICE",
    "KAFKA_SASL_MECHANISM",
    "KAFKA_SASL_SCRAM_PASSWORD",
    "KAFKA_SASL_SCRAM_SECRETS_ARN",
    "KAFKA_SASL_SCRAM_USERNAME",
    "KAFKA_SKIP_CUSTOM_CERT_VALIDATION",
    "KAFKA_SSL_ENABLED",
    "PASSWORD",
    "PORT",
    "SECRET_ID",
    "SKIP_CUSTOM_JDBC_CERT_VALIDATION",
    "USERNAME",
]
```
## ConnectionTypeType

```python
# ConnectionTypeType usage example

from types_aiobotocore_glue.literals import ConnectionTypeType

def get_value() -> ConnectionTypeType:
    return "CUSTOM"
```

```python
# ConnectionTypeType definition

ConnectionTypeType = Literal[
    "CUSTOM",
    "JDBC",
    "KAFKA",
    "MARKETPLACE",
    "MONGODB",
    "NETWORK",
    "SFTP",
]
```
## CrawlStateType

```python
# CrawlStateType usage example

from types_aiobotocore_glue.literals import CrawlStateType

def get_value() -> CrawlStateType:
    return "CANCELLED"
```

```python
# CrawlStateType definition

CrawlStateType = Literal[
    "CANCELLED",
    "CANCELLING",
    "ERROR",
    "FAILED",
    "RUNNING",
    "SUCCEEDED",
]
```
## CrawlerHistoryStateType

```python
# CrawlerHistoryStateType usage example

from types_aiobotocore_glue.literals import CrawlerHistoryStateType

def get_value() -> CrawlerHistoryStateType:
    return "COMPLETED"
```

```python
# CrawlerHistoryStateType definition

CrawlerHistoryStateType = Literal[
    "COMPLETED",
    "FAILED",
    "RUNNING",
    "STOPPED",
]
```
## CrawlerLineageSettingsType

```python
# CrawlerLineageSettingsType usage example

from types_aiobotocore_glue.literals import CrawlerLineageSettingsType

def get_value() -> CrawlerLineageSettingsType:
    return "DISABLE"
```

```python
# CrawlerLineageSettingsType definition

CrawlerLineageSettingsType = Literal[
    "DISABLE",
    "ENABLE",
]
```
## CrawlerStateType

```python
# CrawlerStateType usage example

from types_aiobotocore_glue.literals import CrawlerStateType

def get_value() -> CrawlerStateType:
    return "READY"
```

```python
# CrawlerStateType definition

CrawlerStateType = Literal[
    "READY",
    "RUNNING",
    "STOPPING",
]
```
## CsvHeaderOptionType

```python
# CsvHeaderOptionType usage example

from types_aiobotocore_glue.literals import CsvHeaderOptionType

def get_value() -> CsvHeaderOptionType:
    return "ABSENT"
```

```python
# CsvHeaderOptionType definition

CsvHeaderOptionType = Literal[
    "ABSENT",
    "PRESENT",
    "UNKNOWN",
]
```
## DQStopJobOnFailureTimingType

```python
# DQStopJobOnFailureTimingType usage example

from types_aiobotocore_glue.literals import DQStopJobOnFailureTimingType

def get_value() -> DQStopJobOnFailureTimingType:
    return "AfterDataLoad"
```

```python
# DQStopJobOnFailureTimingType definition

DQStopJobOnFailureTimingType = Literal[
    "AfterDataLoad",
    "Immediate",
]
```
## DQTransformOutputType

```python
# DQTransformOutputType usage example

from types_aiobotocore_glue.literals import DQTransformOutputType

def get_value() -> DQTransformOutputType:
    return "EvaluationResults"
```

```python
# DQTransformOutputType definition

DQTransformOutputType = Literal[
    "EvaluationResults",
    "PrimaryInput",
]
```
## DataFormatType

```python
# DataFormatType usage example

from types_aiobotocore_glue.literals import DataFormatType

def get_value() -> DataFormatType:
    return "AVRO"
```

```python
# DataFormatType definition

DataFormatType = Literal[
    "AVRO",
    "JSON",
    "PROTOBUF",
]
```
## DataQualityRuleResultStatusType

```python
# DataQualityRuleResultStatusType usage example

from types_aiobotocore_glue.literals import DataQualityRuleResultStatusType

def get_value() -> DataQualityRuleResultStatusType:
    return "ERROR"
```

```python
# DataQualityRuleResultStatusType definition

DataQualityRuleResultStatusType = Literal[
    "ERROR",
    "FAIL",
    "PASS",
]
```
## DeleteBehaviorType

```python
# DeleteBehaviorType usage example

from types_aiobotocore_glue.literals import DeleteBehaviorType

def get_value() -> DeleteBehaviorType:
    return "DELETE_FROM_DATABASE"
```

```python
# DeleteBehaviorType definition

DeleteBehaviorType = Literal[
    "DELETE_FROM_DATABASE",
    "DEPRECATE_IN_DATABASE",
    "LOG",
]
```
## DeltaTargetCompressionTypeType

```python
# DeltaTargetCompressionTypeType usage example

from types_aiobotocore_glue.literals import DeltaTargetCompressionTypeType

def get_value() -> DeltaTargetCompressionTypeType:
    return "snappy"
```

```python
# DeltaTargetCompressionTypeType definition

DeltaTargetCompressionTypeType = Literal[
    "snappy",
    "uncompressed",
]
```
## EnableHybridValuesType

```python
# EnableHybridValuesType usage example

from types_aiobotocore_glue.literals import EnableHybridValuesType

def get_value() -> EnableHybridValuesType:
    return "FALSE"
```

```python
# EnableHybridValuesType definition

EnableHybridValuesType = Literal[
    "FALSE",
    "TRUE",
]
```
## ExecutionClassType

```python
# ExecutionClassType usage example

from types_aiobotocore_glue.literals import ExecutionClassType

def get_value() -> ExecutionClassType:
    return "FLEX"
```

```python
# ExecutionClassType definition

ExecutionClassType = Literal[
    "FLEX",
    "STANDARD",
]
```
## ExistConditionType

```python
# ExistConditionType usage example

from types_aiobotocore_glue.literals import ExistConditionType

def get_value() -> ExistConditionType:
    return "MUST_EXIST"
```

```python
# ExistConditionType definition

ExistConditionType = Literal[
    "MUST_EXIST",
    "NONE",
    "NOT_EXIST",
]
```
## FieldNameType

```python
# FieldNameType usage example

from types_aiobotocore_glue.literals import FieldNameType

def get_value() -> FieldNameType:
    return "CRAWL_ID"
```

```python
# FieldNameType definition

FieldNameType = Literal[
    "CRAWL_ID",
    "DPU_HOUR",
    "END_TIME",
    "START_TIME",
    "STATE",
]
```
## FilterLogicalOperatorType

```python
# FilterLogicalOperatorType usage example

from types_aiobotocore_glue.literals import FilterLogicalOperatorType

def get_value() -> FilterLogicalOperatorType:
    return "AND"
```

```python
# FilterLogicalOperatorType definition

FilterLogicalOperatorType = Literal[
    "AND",
    "OR",
]
```
## FilterOperationType

```python
# FilterOperationType usage example

from types_aiobotocore_glue.literals import FilterOperationType

def get_value() -> FilterOperationType:
    return "EQ"
```

```python
# FilterOperationType definition

FilterOperationType = Literal[
    "EQ",
    "GT",
    "GTE",
    "ISNULL",
    "LT",
    "LTE",
    "REGEX",
]
```
## FilterOperatorType

```python
# FilterOperatorType usage example

from types_aiobotocore_glue.literals import FilterOperatorType

def get_value() -> FilterOperatorType:
    return "EQ"
```

```python
# FilterOperatorType definition

FilterOperatorType = Literal[
    "EQ",
    "GE",
    "GT",
    "LE",
    "LT",
    "NE",
]
```
## FilterValueTypeType

```python
# FilterValueTypeType usage example

from types_aiobotocore_glue.literals import FilterValueTypeType

def get_value() -> FilterValueTypeType:
    return "COLUMNEXTRACTED"
```

```python
# FilterValueTypeType definition

FilterValueTypeType = Literal[
    "COLUMNEXTRACTED",
    "CONSTANT",
]
```
## GetClassifiersPaginatorName

```python
# GetClassifiersPaginatorName usage example

from types_aiobotocore_glue.literals import GetClassifiersPaginatorName

def get_value() -> GetClassifiersPaginatorName:
    return "get_classifiers"
```

```python
# GetClassifiersPaginatorName definition

GetClassifiersPaginatorName = Literal[
    "get_classifiers",
]
```
## GetConnectionsPaginatorName

```python
# GetConnectionsPaginatorName usage example

from types_aiobotocore_glue.literals import GetConnectionsPaginatorName

def get_value() -> GetConnectionsPaginatorName:
    return "get_connections"
```

```python
# GetConnectionsPaginatorName definition

GetConnectionsPaginatorName = Literal[
    "get_connections",
]
```
## GetCrawlerMetricsPaginatorName

```python
# GetCrawlerMetricsPaginatorName usage example

from types_aiobotocore_glue.literals import GetCrawlerMetricsPaginatorName

def get_value() -> GetCrawlerMetricsPaginatorName:
    return "get_crawler_metrics"
```

```python
# GetCrawlerMetricsPaginatorName definition

GetCrawlerMetricsPaginatorName = Literal[
    "get_crawler_metrics",
]
```
## GetCrawlersPaginatorName

```python
# GetCrawlersPaginatorName usage example

from types_aiobotocore_glue.literals import GetCrawlersPaginatorName

def get_value() -> GetCrawlersPaginatorName:
    return "get_crawlers"
```

```python
# GetCrawlersPaginatorName definition

GetCrawlersPaginatorName = Literal[
    "get_crawlers",
]
```
## GetDatabasesPaginatorName

```python
# GetDatabasesPaginatorName usage example

from types_aiobotocore_glue.literals import GetDatabasesPaginatorName

def get_value() -> GetDatabasesPaginatorName:
    return "get_databases"
```

```python
# GetDatabasesPaginatorName definition

GetDatabasesPaginatorName = Literal[
    "get_databases",
]
```
## GetDevEndpointsPaginatorName

```python
# GetDevEndpointsPaginatorName usage example

from types_aiobotocore_glue.literals import GetDevEndpointsPaginatorName

def get_value() -> GetDevEndpointsPaginatorName:
    return "get_dev_endpoints"
```

```python
# GetDevEndpointsPaginatorName definition

GetDevEndpointsPaginatorName = Literal[
    "get_dev_endpoints",
]
```
## GetJobRunsPaginatorName

```python
# GetJobRunsPaginatorName usage example

from types_aiobotocore_glue.literals import GetJobRunsPaginatorName

def get_value() -> GetJobRunsPaginatorName:
    return "get_job_runs"
```

```python
# GetJobRunsPaginatorName definition

GetJobRunsPaginatorName = Literal[
    "get_job_runs",
]
```
## GetJobsPaginatorName

```python
# GetJobsPaginatorName usage example

from types_aiobotocore_glue.literals import GetJobsPaginatorName

def get_value() -> GetJobsPaginatorName:
    return "get_jobs"
```

```python
# GetJobsPaginatorName definition

GetJobsPaginatorName = Literal[
    "get_jobs",
]
```
## GetPartitionIndexesPaginatorName

```python
# GetPartitionIndexesPaginatorName usage example

from types_aiobotocore_glue.literals import GetPartitionIndexesPaginatorName

def get_value() -> GetPartitionIndexesPaginatorName:
    return "get_partition_indexes"
```

```python
# GetPartitionIndexesPaginatorName definition

GetPartitionIndexesPaginatorName = Literal[
    "get_partition_indexes",
]
```
## GetPartitionsPaginatorName

```python
# GetPartitionsPaginatorName usage example

from types_aiobotocore_glue.literals import GetPartitionsPaginatorName

def get_value() -> GetPartitionsPaginatorName:
    return "get_partitions"
```

```python
# GetPartitionsPaginatorName definition

GetPartitionsPaginatorName = Literal[
    "get_partitions",
]
```
## GetResourcePoliciesPaginatorName

```python
# GetResourcePoliciesPaginatorName usage example

from types_aiobotocore_glue.literals import GetResourcePoliciesPaginatorName

def get_value() -> GetResourcePoliciesPaginatorName:
    return "get_resource_policies"
```

```python
# GetResourcePoliciesPaginatorName definition

GetResourcePoliciesPaginatorName = Literal[
    "get_resource_policies",
]
```
## GetSecurityConfigurationsPaginatorName

```python
# GetSecurityConfigurationsPaginatorName usage example

from types_aiobotocore_glue.literals import GetSecurityConfigurationsPaginatorName

def get_value() -> GetSecurityConfigurationsPaginatorName:
    return "get_security_configurations"
```

```python
# GetSecurityConfigurationsPaginatorName definition

GetSecurityConfigurationsPaginatorName = Literal[
    "get_security_configurations",
]
```
## GetTableVersionsPaginatorName

```python
# GetTableVersionsPaginatorName usage example

from types_aiobotocore_glue.literals import GetTableVersionsPaginatorName

def get_value() -> GetTableVersionsPaginatorName:
    return "get_table_versions"
```

```python
# GetTableVersionsPaginatorName definition

GetTableVersionsPaginatorName = Literal[
    "get_table_versions",
]
```
## GetTablesPaginatorName

```python
# GetTablesPaginatorName usage example

from types_aiobotocore_glue.literals import GetTablesPaginatorName

def get_value() -> GetTablesPaginatorName:
    return "get_tables"
```

```python
# GetTablesPaginatorName definition

GetTablesPaginatorName = Literal[
    "get_tables",
]
```
## GetTriggersPaginatorName

```python
# GetTriggersPaginatorName usage example

from types_aiobotocore_glue.literals import GetTriggersPaginatorName

def get_value() -> GetTriggersPaginatorName:
    return "get_triggers"
```

```python
# GetTriggersPaginatorName definition

GetTriggersPaginatorName = Literal[
    "get_triggers",
]
```
## GetUserDefinedFunctionsPaginatorName

```python
# GetUserDefinedFunctionsPaginatorName usage example

from types_aiobotocore_glue.literals import GetUserDefinedFunctionsPaginatorName

def get_value() -> GetUserDefinedFunctionsPaginatorName:
    return "get_user_defined_functions"
```

```python
# GetUserDefinedFunctionsPaginatorName definition

GetUserDefinedFunctionsPaginatorName = Literal[
    "get_user_defined_functions",
]
```
## GlueRecordTypeType

```python
# GlueRecordTypeType usage example

from types_aiobotocore_glue.literals import GlueRecordTypeType

def get_value() -> GlueRecordTypeType:
    return "BIGDECIMAL"
```

```python
# GlueRecordTypeType definition

GlueRecordTypeType = Literal[
    "BIGDECIMAL",
    "BYTE",
    "DATE",
    "DOUBLE",
    "FLOAT",
    "INT",
    "LONG",
    "SHORT",
    "STRING",
    "TIMESTAMP",
]
```
## HudiTargetCompressionTypeType

```python
# HudiTargetCompressionTypeType usage example

from types_aiobotocore_glue.literals import HudiTargetCompressionTypeType

def get_value() -> HudiTargetCompressionTypeType:
    return "gzip"
```

```python
# HudiTargetCompressionTypeType definition

HudiTargetCompressionTypeType = Literal[
    "gzip",
    "lzo",
    "snappy",
    "uncompressed",
]
```
## JDBCConnectionTypeType

```python
# JDBCConnectionTypeType usage example

from types_aiobotocore_glue.literals import JDBCConnectionTypeType

def get_value() -> JDBCConnectionTypeType:
    return "mysql"
```

```python
# JDBCConnectionTypeType definition

JDBCConnectionTypeType = Literal[
    "mysql",
    "oracle",
    "postgresql",
    "redshift",
    "sqlserver",
]
```
## JDBCDataTypeType

```python
# JDBCDataTypeType usage example

from types_aiobotocore_glue.literals import JDBCDataTypeType

def get_value() -> JDBCDataTypeType:
    return "ARRAY"
```

```python
# JDBCDataTypeType definition

JDBCDataTypeType = Literal[
    "ARRAY",
    "BIGINT",
    "BINARY",
    "BIT",
    "BLOB",
    "BOOLEAN",
    "CHAR",
    "CLOB",
    "DATALINK",
    "DATE",
    "DECIMAL",
    "DISTINCT",
    "DOUBLE",
    "FLOAT",
    "INTEGER",
    "JAVA_OBJECT",
    "LONGNVARCHAR",
    "LONGVARBINARY",
    "LONGVARCHAR",
    "NCHAR",
    "NCLOB",
    "NULL",
    "NUMERIC",
    "NVARCHAR",
    "OTHER",
    "REAL",
    "REF",
    "REF_CURSOR",
    "ROWID",
    "SMALLINT",
    "SQLXML",
    "STRUCT",
    "TIME",
    "TIME_WITH_TIMEZONE",
    "TIMESTAMP",
    "TIMESTAMP_WITH_TIMEZONE",
    "TINYINT",
    "VARBINARY",
    "VARCHAR",
]
```
## JdbcMetadataEntryType

```python
# JdbcMetadataEntryType usage example

from types_aiobotocore_glue.literals import JdbcMetadataEntryType

def get_value() -> JdbcMetadataEntryType:
    return "COMMENTS"
```

```python
# JdbcMetadataEntryType definition

JdbcMetadataEntryType = Literal[
    "COMMENTS",
    "RAWTYPES",
]
```
## JobBookmarksEncryptionModeType

```python
# JobBookmarksEncryptionModeType usage example

from types_aiobotocore_glue.literals import JobBookmarksEncryptionModeType

def get_value() -> JobBookmarksEncryptionModeType:
    return "CSE-KMS"
```

```python
# JobBookmarksEncryptionModeType definition

JobBookmarksEncryptionModeType = Literal[
    "CSE-KMS",
    "DISABLED",
]
```
## JobRunStateType

```python
# JobRunStateType usage example

from types_aiobotocore_glue.literals import JobRunStateType

def get_value() -> JobRunStateType:
    return "ERROR"
```

```python
# JobRunStateType definition

JobRunStateType = Literal[
    "ERROR",
    "FAILED",
    "RUNNING",
    "STARTING",
    "STOPPED",
    "STOPPING",
    "SUCCEEDED",
    "TIMEOUT",
    "WAITING",
]
```
## JoinTypeType

```python
# JoinTypeType usage example

from types_aiobotocore_glue.literals import JoinTypeType

def get_value() -> JoinTypeType:
    return "equijoin"
```

```python
# JoinTypeType definition

JoinTypeType = Literal[
    "equijoin",
    "left",
    "leftanti",
    "leftsemi",
    "outer",
    "right",
]
```
## LanguageType

```python
# LanguageType usage example

from types_aiobotocore_glue.literals import LanguageType

def get_value() -> LanguageType:
    return "PYTHON"
```

```python
# LanguageType definition

LanguageType = Literal[
    "PYTHON",
    "SCALA",
]
```
## LastCrawlStatusType

```python
# LastCrawlStatusType usage example

from types_aiobotocore_glue.literals import LastCrawlStatusType

def get_value() -> LastCrawlStatusType:
    return "CANCELLED"
```

```python
# LastCrawlStatusType definition

LastCrawlStatusType = Literal[
    "CANCELLED",
    "FAILED",
    "SUCCEEDED",
]
```
## ListRegistriesPaginatorName

```python
# ListRegistriesPaginatorName usage example

from types_aiobotocore_glue.literals import ListRegistriesPaginatorName

def get_value() -> ListRegistriesPaginatorName:
    return "list_registries"
```

```python
# ListRegistriesPaginatorName definition

ListRegistriesPaginatorName = Literal[
    "list_registries",
]
```
## ListSchemaVersionsPaginatorName

```python
# ListSchemaVersionsPaginatorName usage example

from types_aiobotocore_glue.literals import ListSchemaVersionsPaginatorName

def get_value() -> ListSchemaVersionsPaginatorName:
    return "list_schema_versions"
```

```python
# ListSchemaVersionsPaginatorName definition

ListSchemaVersionsPaginatorName = Literal[
    "list_schema_versions",
]
```
## ListSchemasPaginatorName

```python
# ListSchemasPaginatorName usage example

from types_aiobotocore_glue.literals import ListSchemasPaginatorName

def get_value() -> ListSchemasPaginatorName:
    return "list_schemas"
```

```python
# ListSchemasPaginatorName definition

ListSchemasPaginatorName = Literal[
    "list_schemas",
]
```
## LogicalOperatorType

```python
# LogicalOperatorType usage example

from types_aiobotocore_glue.literals import LogicalOperatorType

def get_value() -> LogicalOperatorType:
    return "EQUALS"
```

```python
# LogicalOperatorType definition

LogicalOperatorType = Literal[
    "EQUALS",
]
```
## LogicalType

```python
# LogicalType usage example

from types_aiobotocore_glue.literals import LogicalType

def get_value() -> LogicalType:
    return "AND"
```

```python
# LogicalType definition

LogicalType = Literal[
    "AND",
    "ANY",
]
```
## MLUserDataEncryptionModeStringType

```python
# MLUserDataEncryptionModeStringType usage example

from types_aiobotocore_glue.literals import MLUserDataEncryptionModeStringType

def get_value() -> MLUserDataEncryptionModeStringType:
    return "DISABLED"
```

```python
# MLUserDataEncryptionModeStringType definition

MLUserDataEncryptionModeStringType = Literal[
    "DISABLED",
    "SSE-KMS",
]
```
## MetadataOperationType

```python
# MetadataOperationType usage example

from types_aiobotocore_glue.literals import MetadataOperationType

def get_value() -> MetadataOperationType:
    return "CREATE"
```

```python
# MetadataOperationType definition

MetadataOperationType = Literal[
    "CREATE",
]
```
## NodeTypeType

```python
# NodeTypeType usage example

from types_aiobotocore_glue.literals import NodeTypeType

def get_value() -> NodeTypeType:
    return "CRAWLER"
```

```python
# NodeTypeType definition

NodeTypeType = Literal[
    "CRAWLER",
    "JOB",
    "TRIGGER",
]
```
## ParamTypeType

```python
# ParamTypeType usage example

from types_aiobotocore_glue.literals import ParamTypeType

def get_value() -> ParamTypeType:
    return "bool"
```

```python
# ParamTypeType definition

ParamTypeType = Literal[
    "bool",
    "complex",
    "float",
    "int",
    "list",
    "null",
    "str",
]
```
## ParquetCompressionTypeType

```python
# ParquetCompressionTypeType usage example

from types_aiobotocore_glue.literals import ParquetCompressionTypeType

def get_value() -> ParquetCompressionTypeType:
    return "gzip"
```

```python
# ParquetCompressionTypeType definition

ParquetCompressionTypeType = Literal[
    "gzip",
    "lzo",
    "none",
    "snappy",
    "uncompressed",
]
```
## PartitionIndexStatusType

```python
# PartitionIndexStatusType usage example

from types_aiobotocore_glue.literals import PartitionIndexStatusType

def get_value() -> PartitionIndexStatusType:
    return "ACTIVE"
```

```python
# PartitionIndexStatusType definition

PartitionIndexStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
]
```
## PermissionType

```python
# PermissionType usage example

from types_aiobotocore_glue.literals import PermissionType

def get_value() -> PermissionType:
    return "ALL"
```

```python
# PermissionType definition

PermissionType = Literal[
    "ALL",
    "ALTER",
    "CREATE_DATABASE",
    "CREATE_TABLE",
    "DATA_LOCATION_ACCESS",
    "DELETE",
    "DROP",
    "INSERT",
    "SELECT",
]
```
## PermissionTypeType

```python
# PermissionTypeType usage example

from types_aiobotocore_glue.literals import PermissionTypeType

def get_value() -> PermissionTypeType:
    return "CELL_FILTER_PERMISSION"
```

```python
# PermissionTypeType definition

PermissionTypeType = Literal[
    "CELL_FILTER_PERMISSION",
    "COLUMN_PERMISSION",
    "NESTED_CELL_PERMISSION",
    "NESTED_PERMISSION",
]
```
## PiiTypeType

```python
# PiiTypeType usage example

from types_aiobotocore_glue.literals import PiiTypeType

def get_value() -> PiiTypeType:
    return "ColumnAudit"
```

```python
# PiiTypeType definition

PiiTypeType = Literal[
    "ColumnAudit",
    "ColumnMasking",
    "RowAudit",
    "RowMasking",
]
```
## PrincipalTypeType

```python
# PrincipalTypeType usage example

from types_aiobotocore_glue.literals import PrincipalTypeType

def get_value() -> PrincipalTypeType:
    return "GROUP"
```

```python
# PrincipalTypeType definition

PrincipalTypeType = Literal[
    "GROUP",
    "ROLE",
    "USER",
]
```
## QuoteCharType

```python
# QuoteCharType usage example

from types_aiobotocore_glue.literals import QuoteCharType

def get_value() -> QuoteCharType:
    return "disabled"
```

```python
# QuoteCharType definition

QuoteCharType = Literal[
    "disabled",
    "quillemet",
    "quote",
    "single_quote",
]
```
## RecrawlBehaviorType

```python
# RecrawlBehaviorType usage example

from types_aiobotocore_glue.literals import RecrawlBehaviorType

def get_value() -> RecrawlBehaviorType:
    return "CRAWL_EVENT_MODE"
```

```python
# RecrawlBehaviorType definition

RecrawlBehaviorType = Literal[
    "CRAWL_EVENT_MODE",
    "CRAWL_EVERYTHING",
    "CRAWL_NEW_FOLDERS_ONLY",
]
```
## RegistryStatusType

```python
# RegistryStatusType usage example

from types_aiobotocore_glue.literals import RegistryStatusType

def get_value() -> RegistryStatusType:
    return "AVAILABLE"
```

```python
# RegistryStatusType definition

RegistryStatusType = Literal[
    "AVAILABLE",
    "DELETING",
]
```
## ResourceShareTypeType

```python
# ResourceShareTypeType usage example

from types_aiobotocore_glue.literals import ResourceShareTypeType

def get_value() -> ResourceShareTypeType:
    return "ALL"
```

```python
# ResourceShareTypeType definition

ResourceShareTypeType = Literal[
    "ALL",
    "FEDERATED",
    "FOREIGN",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example

from types_aiobotocore_glue.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "ARCHIVE"
```

```python
# ResourceTypeType definition

ResourceTypeType = Literal[
    "ARCHIVE",
    "FILE",
    "JAR",
]
```
## S3EncryptionModeType

```python
# S3EncryptionModeType usage example

from types_aiobotocore_glue.literals import S3EncryptionModeType

def get_value() -> S3EncryptionModeType:
    return "DISABLED"
```

```python
# S3EncryptionModeType definition

S3EncryptionModeType = Literal[
    "DISABLED",
    "SSE-KMS",
    "SSE-S3",
]
```
## ScheduleStateType

```python
# ScheduleStateType usage example

from types_aiobotocore_glue.literals import ScheduleStateType

def get_value() -> ScheduleStateType:
    return "NOT_SCHEDULED"
```

```python
# ScheduleStateType definition

ScheduleStateType = Literal[
    "NOT_SCHEDULED",
    "SCHEDULED",
    "TRANSITIONING",
]
```
## SchemaDiffTypeType

```python
# SchemaDiffTypeType usage example

from types_aiobotocore_glue.literals import SchemaDiffTypeType

def get_value() -> SchemaDiffTypeType:
    return "SYNTAX_DIFF"
```

```python
# SchemaDiffTypeType definition

SchemaDiffTypeType = Literal[
    "SYNTAX_DIFF",
]
```
## SchemaStatusType

```python
# SchemaStatusType usage example

from types_aiobotocore_glue.literals import SchemaStatusType

def get_value() -> SchemaStatusType:
    return "AVAILABLE"
```

```python
# SchemaStatusType definition

SchemaStatusType = Literal[
    "AVAILABLE",
    "DELETING",
    "PENDING",
]
```
## SchemaVersionStatusType

```python
# SchemaVersionStatusType usage example

from types_aiobotocore_glue.literals import SchemaVersionStatusType

def get_value() -> SchemaVersionStatusType:
    return "AVAILABLE"
```

```python
# SchemaVersionStatusType definition

SchemaVersionStatusType = Literal[
    "AVAILABLE",
    "DELETING",
    "FAILURE",
    "PENDING",
]
```
## SeparatorType

```python
# SeparatorType usage example

from types_aiobotocore_glue.literals import SeparatorType

def get_value() -> SeparatorType:
    return "comma"
```

```python
# SeparatorType definition

SeparatorType = Literal[
    "comma",
    "ctrla",
    "pipe",
    "semicolon",
    "tab",
]
```
## SessionStatusType

```python
# SessionStatusType usage example

from types_aiobotocore_glue.literals import SessionStatusType

def get_value() -> SessionStatusType:
    return "FAILED"
```

```python
# SessionStatusType definition

SessionStatusType = Literal[
    "FAILED",
    "PROVISIONING",
    "READY",
    "STOPPED",
    "STOPPING",
    "TIMEOUT",
]
```
## SortDirectionTypeType

```python
# SortDirectionTypeType usage example

from types_aiobotocore_glue.literals import SortDirectionTypeType

def get_value() -> SortDirectionTypeType:
    return "ASCENDING"
```

```python
# SortDirectionTypeType definition

SortDirectionTypeType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## SortType

```python
# SortType usage example

from types_aiobotocore_glue.literals import SortType

def get_value() -> SortType:
    return "ASC"
```

```python
# SortType definition

SortType = Literal[
    "ASC",
    "DESC",
]
```
## SourceControlAuthStrategyType

```python
# SourceControlAuthStrategyType usage example

from types_aiobotocore_glue.literals import SourceControlAuthStrategyType

def get_value() -> SourceControlAuthStrategyType:
    return "AWS_SECRETS_MANAGER"
```

```python
# SourceControlAuthStrategyType definition

SourceControlAuthStrategyType = Literal[
    "AWS_SECRETS_MANAGER",
    "PERSONAL_ACCESS_TOKEN",
]
```
## SourceControlProviderType

```python
# SourceControlProviderType usage example

from types_aiobotocore_glue.literals import SourceControlProviderType

def get_value() -> SourceControlProviderType:
    return "AWS_CODE_COMMIT"
```

```python
# SourceControlProviderType definition

SourceControlProviderType = Literal[
    "AWS_CODE_COMMIT",
    "GITHUB",
]
```
## StartingPositionType

```python
# StartingPositionType usage example

from types_aiobotocore_glue.literals import StartingPositionType

def get_value() -> StartingPositionType:
    return "earliest"
```

```python
# StartingPositionType definition

StartingPositionType = Literal[
    "earliest",
    "latest",
    "timestamp",
    "trim_horizon",
]
```
## StatementStateType

```python
# StatementStateType usage example

from types_aiobotocore_glue.literals import StatementStateType

def get_value() -> StatementStateType:
    return "AVAILABLE"
```

```python
# StatementStateType definition

StatementStateType = Literal[
    "AVAILABLE",
    "CANCELLED",
    "CANCELLING",
    "ERROR",
    "RUNNING",
    "WAITING",
]
```
## TargetFormatType

```python
# TargetFormatType usage example

from types_aiobotocore_glue.literals import TargetFormatType

def get_value() -> TargetFormatType:
    return "avro"
```

```python
# TargetFormatType definition

TargetFormatType = Literal[
    "avro",
    "csv",
    "delta",
    "hudi",
    "json",
    "orc",
    "parquet",
]
```
## TaskRunSortColumnTypeType

```python
# TaskRunSortColumnTypeType usage example

from types_aiobotocore_glue.literals import TaskRunSortColumnTypeType

def get_value() -> TaskRunSortColumnTypeType:
    return "STARTED"
```

```python
# TaskRunSortColumnTypeType definition

TaskRunSortColumnTypeType = Literal[
    "STARTED",
    "STATUS",
    "TASK_RUN_TYPE",
]
```
## TaskStatusTypeType

```python
# TaskStatusTypeType usage example

from types_aiobotocore_glue.literals import TaskStatusTypeType

def get_value() -> TaskStatusTypeType:
    return "FAILED"
```

```python
# TaskStatusTypeType definition

TaskStatusTypeType = Literal[
    "FAILED",
    "RUNNING",
    "STARTING",
    "STOPPED",
    "STOPPING",
    "SUCCEEDED",
    "TIMEOUT",
]
```
## TaskTypeType

```python
# TaskTypeType usage example

from types_aiobotocore_glue.literals import TaskTypeType

def get_value() -> TaskTypeType:
    return "EVALUATION"
```

```python
# TaskTypeType definition

TaskTypeType = Literal[
    "EVALUATION",
    "EXPORT_LABELS",
    "FIND_MATCHES",
    "IMPORT_LABELS",
    "LABELING_SET_GENERATION",
]
```
## TransformSortColumnTypeType

```python
# TransformSortColumnTypeType usage example

from types_aiobotocore_glue.literals import TransformSortColumnTypeType

def get_value() -> TransformSortColumnTypeType:
    return "CREATED"
```

```python
# TransformSortColumnTypeType definition

TransformSortColumnTypeType = Literal[
    "CREATED",
    "LAST_MODIFIED",
    "NAME",
    "STATUS",
    "TRANSFORM_TYPE",
]
```
## TransformStatusTypeType

```python
# TransformStatusTypeType usage example

from types_aiobotocore_glue.literals import TransformStatusTypeType

def get_value() -> TransformStatusTypeType:
    return "DELETING"
```

```python
# TransformStatusTypeType definition

TransformStatusTypeType = Literal[
    "DELETING",
    "NOT_READY",
    "READY",
]
```
## TransformTypeType

```python
# TransformTypeType usage example

from types_aiobotocore_glue.literals import TransformTypeType

def get_value() -> TransformTypeType:
    return "FIND_MATCHES"
```

```python
# TransformTypeType definition

TransformTypeType = Literal[
    "FIND_MATCHES",
]
```
## TriggerStateType

```python
# TriggerStateType usage example

from types_aiobotocore_glue.literals import TriggerStateType

def get_value() -> TriggerStateType:
    return "ACTIVATED"
```

```python
# TriggerStateType definition

TriggerStateType = Literal[
    "ACTIVATED",
    "ACTIVATING",
    "CREATED",
    "CREATING",
    "DEACTIVATED",
    "DEACTIVATING",
    "DELETING",
    "UPDATING",
]
```
## TriggerTypeType

```python
# TriggerTypeType usage example

from types_aiobotocore_glue.literals import TriggerTypeType

def get_value() -> TriggerTypeType:
    return "CONDITIONAL"
```

```python
# TriggerTypeType definition

TriggerTypeType = Literal[
    "CONDITIONAL",
    "EVENT",
    "ON_DEMAND",
    "SCHEDULED",
]
```
## UnionTypeType

```python
# UnionTypeType usage example

from types_aiobotocore_glue.literals import UnionTypeType

def get_value() -> UnionTypeType:
    return "ALL"
```

```python
# UnionTypeType definition

UnionTypeType = Literal[
    "ALL",
    "DISTINCT",
]
```
## UpdateBehaviorType

```python
# UpdateBehaviorType usage example

from types_aiobotocore_glue.literals import UpdateBehaviorType

def get_value() -> UpdateBehaviorType:
    return "LOG"
```

```python
# UpdateBehaviorType definition

UpdateBehaviorType = Literal[
    "LOG",
    "UPDATE_IN_DATABASE",
]
```
## UpdateCatalogBehaviorType

```python
# UpdateCatalogBehaviorType usage example

from types_aiobotocore_glue.literals import UpdateCatalogBehaviorType

def get_value() -> UpdateCatalogBehaviorType:
    return "LOG"
```

```python
# UpdateCatalogBehaviorType definition

UpdateCatalogBehaviorType = Literal[
    "LOG",
    "UPDATE_IN_DATABASE",
]
```
## WorkerTypeType

```python
# WorkerTypeType usage example

from types_aiobotocore_glue.literals import WorkerTypeType

def get_value() -> WorkerTypeType:
    return "G.025X"
```

```python
# WorkerTypeType definition

WorkerTypeType = Literal[
    "G.025X",
    "G.1X",
    "G.2X",
    "G.4X",
    "G.8X",
    "Standard",
    "Z.2X",
]
```
## WorkflowRunStatusType

```python
# WorkflowRunStatusType usage example

from types_aiobotocore_glue.literals import WorkflowRunStatusType

def get_value() -> WorkflowRunStatusType:
    return "COMPLETED"
```

```python
# WorkflowRunStatusType definition

WorkflowRunStatusType = Literal[
    "COMPLETED",
    "ERROR",
    "RUNNING",
    "STOPPED",
    "STOPPING",
]
```
## GlueServiceName

```python
# GlueServiceName usage example

from types_aiobotocore_glue.literals import GlueServiceName

def get_value() -> GlueServiceName:
    return "glue"
```

```python
# GlueServiceName definition

GlueServiceName = Literal[
    "glue",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_glue.literals import ServiceName

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

from types_aiobotocore_glue.literals import ResourceServiceName

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

from types_aiobotocore_glue.literals import PaginatorName

def get_value() -> PaginatorName:
    return "get_classifiers"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "get_classifiers",
    "get_connections",
    "get_crawler_metrics",
    "get_crawlers",
    "get_databases",
    "get_dev_endpoints",
    "get_job_runs",
    "get_jobs",
    "get_partition_indexes",
    "get_partitions",
    "get_resource_policies",
    "get_security_configurations",
    "get_table_versions",
    "get_tables",
    "get_triggers",
    "get_user_defined_functions",
    "list_registries",
    "list_schema_versions",
    "list_schemas",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_glue.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition

RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ap-southeast-4",
    "ca-central-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```
