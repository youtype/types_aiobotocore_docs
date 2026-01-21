# Type annotations for aiobotocore

Auto-generated documentation for [aiobotocore](https://pypi.org/project/aiobotocore/)
type annotations package [types-aiobotocore](https://pypi.org/project/types-aiobotocore/).

Generated with [mypy-boto3-builder 8.12.0](https://github.com/youtype/mypy_boto3_builder).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Select services you use in the current project.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` to add type checking for `aiobotocore` package.

```bash
# install type annotations only for aiobotocore
python -m pip install types-aiobotocore

# install aiobotocore type annotations
# for cloudformation, dynamodb, ec2, lambda, rds, s3, sqs
python -m pip install 'types-aiobotocore[essential]'

# or install annotations for services you use
python -m pip install 'types-aiobotocore[acm,apigateway]'

# or install annotations in sync with aiobotocore version
python -m pip install 'types-aiobotocore[aiobotocore]'

# or install all-in-one annotations for all services
python -m pip install 'types-aiobotocore[full]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[essential]'
```



## How to uninstall

```bash
# uninstall types-aiobotocore
python -m pip uninstall -y types-aiobotocore
```

## Packages
- [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) - [aiobotocore](https://pypi.org/project/aiobotocore/) type annotations with `session.create_client` overloads
- [types-aiobotocore-lite](https://pypi.org/project/types-aiobotocore-lite/) - [aiobotocore](https://pypi.org/project/aiobotocore/) type annotations with `session.create_client` overloads
- [types-aiobotocore-full](https://pypi.org/project/types-aiobotocore-full/) - type annotations for all services below in one package

- [types-aiobotocore-accessanalyzer](./types_aiobotocore_accessanalyzer/README.md) - type annotations for [AccessAnalyzer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/accessanalyzer.html#accessanalyzer) service

- [types-aiobotocore-account](./types_aiobotocore_account/README.md) - type annotations for [Account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#account) service

- [types-aiobotocore-acm](./types_aiobotocore_acm/README.md) - type annotations for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#acm) service

- [types-aiobotocore-acm-pca](./types_aiobotocore_acm_pca/README.md) - type annotations for [ACMPCA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#acmpca) service

- [types-aiobotocore-aiops](./types_aiobotocore_aiops/README.md) - type annotations for [AIOps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/aiops.html#aiops) service

- [types-aiobotocore-amp](./types_aiobotocore_amp/README.md) - type annotations for [PrometheusService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amp.html#prometheusservice) service

- [types-aiobotocore-amplify](./types_aiobotocore_amplify/README.md) - type annotations for [Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#amplify) service

- [types-aiobotocore-amplifybackend](./types_aiobotocore_amplifybackend/README.md) - type annotations for [AmplifyBackend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#amplifybackend) service

- [types-aiobotocore-amplifyuibuilder](./types_aiobotocore_amplifyuibuilder/README.md) - type annotations for [AmplifyUIBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#amplifyuibuilder) service

- [types-aiobotocore-apigateway](./types_aiobotocore_apigateway/README.md) - type annotations for [APIGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigateway.html#apigateway) service

- [types-aiobotocore-apigatewaymanagementapi](./types_aiobotocore_apigatewaymanagementapi/README.md) - type annotations for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#apigatewaymanagementapi) service

- [types-aiobotocore-apigatewayv2](./types_aiobotocore_apigatewayv2/README.md) - type annotations for [ApiGatewayV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#apigatewayv2) service

- [types-aiobotocore-appconfig](./types_aiobotocore_appconfig/README.md) - type annotations for [AppConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfig.html#appconfig) service

- [types-aiobotocore-appconfigdata](./types_aiobotocore_appconfigdata/README.md) - type annotations for [AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#appconfigdata) service

- [types-aiobotocore-appfabric](./types_aiobotocore_appfabric/README.md) - type annotations for [AppFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#appfabric) service

- [types-aiobotocore-appflow](./types_aiobotocore_appflow/README.md) - type annotations for [Appflow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appflow.html#appflow) service

- [types-aiobotocore-appintegrations](./types_aiobotocore_appintegrations/README.md) - type annotations for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#appintegrationsservice) service

- [types-aiobotocore-application-autoscaling](./types_aiobotocore_application_autoscaling/README.md) - type annotations for [ApplicationAutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-autoscaling.html#applicationautoscaling) service

- [types-aiobotocore-application-insights](./types_aiobotocore_application_insights/README.md) - type annotations for [ApplicationInsights](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#applicationinsights) service

- [types-aiobotocore-application-signals](./types_aiobotocore_application_signals/README.md) - type annotations for [CloudWatchApplicationSignals](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-signals.html#cloudwatchapplicationsignals) service

- [types-aiobotocore-applicationcostprofiler](./types_aiobotocore_applicationcostprofiler/README.md) - type annotations for [ApplicationCostProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#applicationcostprofiler) service

- [types-aiobotocore-appmesh](./types_aiobotocore_appmesh/README.md) - type annotations for [AppMesh](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#appmesh) service

- [types-aiobotocore-apprunner](./types_aiobotocore_apprunner/README.md) - type annotations for [AppRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#apprunner) service

- [types-aiobotocore-appstream](./types_aiobotocore_appstream/README.md) - type annotations for [AppStream](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appstream.html#appstream) service

- [types-aiobotocore-appsync](./types_aiobotocore_appsync/README.md) - type annotations for [AppSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#appsync) service

- [types-aiobotocore-arc-region-switch](./types_aiobotocore_arc_region_switch/README.md) - type annotations for [ARCRegionswitch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-region-switch.html#arcregionswitch) service

- [types-aiobotocore-arc-zonal-shift](./types_aiobotocore_arc_zonal_shift/README.md) - type annotations for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#arczonalshift) service

- [types-aiobotocore-artifact](./types_aiobotocore_artifact/README.md) - type annotations for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#artifact) service

- [types-aiobotocore-athena](./types_aiobotocore_athena/README.md) - type annotations for [Athena](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#athena) service

- [types-aiobotocore-auditmanager](./types_aiobotocore_auditmanager/README.md) - type annotations for [AuditManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#auditmanager) service

- [types-aiobotocore-autoscaling](./types_aiobotocore_autoscaling/README.md) - type annotations for [AutoScaling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling.html#autoscaling) service

- [types-aiobotocore-autoscaling-plans](./types_aiobotocore_autoscaling_plans/README.md) - type annotations for [AutoScalingPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/autoscaling-plans.html#autoscalingplans) service

- [types-aiobotocore-b2bi](./types_aiobotocore_b2bi/README.md) - type annotations for [B2BI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/b2bi.html#b2bi) service

- [types-aiobotocore-backup](./types_aiobotocore_backup/README.md) - type annotations for [Backup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup.html#backup) service

- [types-aiobotocore-backup-gateway](./types_aiobotocore_backup_gateway/README.md) - type annotations for [BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#backupgateway) service

- [types-aiobotocore-backupsearch](./types_aiobotocore_backupsearch/README.md) - type annotations for [BackupSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupsearch.html#backupsearch) service

- [types-aiobotocore-batch](./types_aiobotocore_batch/README.md) - type annotations for [Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#batch) service

- [types-aiobotocore-bcm-dashboards](./types_aiobotocore_bcm_dashboards/README.md) - type annotations for [BillingandCostManagementDashboards](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-dashboards.html#billingandcostmanagementdashboards) service

- [types-aiobotocore-bcm-data-exports](./types_aiobotocore_bcm_data_exports/README.md) - type annotations for [BillingandCostManagementDataExports](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-data-exports.html#billingandcostmanagementdataexports) service

- [types-aiobotocore-bcm-pricing-calculator](./types_aiobotocore_bcm_pricing_calculator/README.md) - type annotations for [BillingandCostManagementPricingCalculator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-pricing-calculator.html#billingandcostmanagementpricingcalculator) service

- [types-aiobotocore-bcm-recommended-actions](./types_aiobotocore_bcm_recommended_actions/README.md) - type annotations for [BillingandCostManagementRecommendedActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#billingandcostmanagementrecommendedactions) service

- [types-aiobotocore-bedrock](./types_aiobotocore_bedrock/README.md) - type annotations for [Bedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock.html#bedrock) service

- [types-aiobotocore-bedrock-agent](./types_aiobotocore_bedrock_agent/README.md) - type annotations for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#agentsforbedrock) service

- [types-aiobotocore-bedrock-agent-runtime](./types_aiobotocore_bedrock_agent_runtime/README.md) - type annotations for [AgentsforBedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent-runtime.html#agentsforbedrockruntime) service

- [types-aiobotocore-bedrock-agentcore](./types_aiobotocore_bedrock_agentcore/README.md) - type annotations for [BedrockAgentCore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore.html#bedrockagentcore) service

- [types-aiobotocore-bedrock-agentcore-control](./types_aiobotocore_bedrock_agentcore_control/README.md) - type annotations for [BedrockAgentCoreControl](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agentcore-control.html#bedrockagentcorecontrol) service

- [types-aiobotocore-bedrock-data-automation](./types_aiobotocore_bedrock_data_automation/README.md) - type annotations for [DataAutomationforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation.html#dataautomationforbedrock) service

- [types-aiobotocore-bedrock-data-automation-runtime](./types_aiobotocore_bedrock_data_automation_runtime/README.md) - type annotations for [RuntimeforBedrockDataAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-data-automation-runtime.html#runtimeforbedrockdataautomation) service

- [types-aiobotocore-bedrock-runtime](./types_aiobotocore_bedrock_runtime/README.md) - type annotations for [BedrockRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-runtime.html#bedrockruntime) service

- [types-aiobotocore-billing](./types_aiobotocore_billing/README.md) - type annotations for [Billing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billing.html#billing) service

- [types-aiobotocore-billingconductor](./types_aiobotocore_billingconductor/README.md) - type annotations for [BillingConductor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/billingconductor.html#billingconductor) service

- [types-aiobotocore-braket](./types_aiobotocore_braket/README.md) - type annotations for [Braket](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#braket) service

- [types-aiobotocore-budgets](./types_aiobotocore_budgets/README.md) - type annotations for [Budgets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/budgets.html#budgets) service

- [types-aiobotocore-ce](./types_aiobotocore_ce/README.md) - type annotations for [CostExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#costexplorer) service

- [types-aiobotocore-chatbot](./types_aiobotocore_chatbot/README.md) - type annotations for [Chatbot](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chatbot.html#chatbot) service

- [types-aiobotocore-chime](./types_aiobotocore_chime/README.md) - type annotations for [Chime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#chime) service

- [types-aiobotocore-chime-sdk-identity](./types_aiobotocore_chime_sdk_identity/README.md) - type annotations for [ChimeSDKIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#chimesdkidentity) service

- [types-aiobotocore-chime-sdk-media-pipelines](./types_aiobotocore_chime_sdk_media_pipelines/README.md) - type annotations for [ChimeSDKMediaPipelines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-media-pipelines.html#chimesdkmediapipelines) service

- [types-aiobotocore-chime-sdk-meetings](./types_aiobotocore_chime_sdk_meetings/README.md) - type annotations for [ChimeSDKMeetings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-meetings.html#chimesdkmeetings) service

- [types-aiobotocore-chime-sdk-messaging](./types_aiobotocore_chime_sdk_messaging/README.md) - type annotations for [ChimeSDKMessaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#chimesdkmessaging) service

- [types-aiobotocore-chime-sdk-voice](./types_aiobotocore_chime_sdk_voice/README.md) - type annotations for [ChimeSDKVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-voice.html#chimesdkvoice) service

- [types-aiobotocore-cleanrooms](./types_aiobotocore_cleanrooms/README.md) - type annotations for [CleanRoomsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanrooms.html#cleanroomsservice) service

- [types-aiobotocore-cleanroomsml](./types_aiobotocore_cleanroomsml/README.md) - type annotations for [CleanRoomsML](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cleanroomsml.html#cleanroomsml) service

- [types-aiobotocore-cloud9](./types_aiobotocore_cloud9/README.md) - type annotations for [Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#cloud9) service

- [types-aiobotocore-cloudcontrol](./types_aiobotocore_cloudcontrol/README.md) - type annotations for [CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#cloudcontrolapi) service

- [types-aiobotocore-clouddirectory](./types_aiobotocore_clouddirectory/README.md) - type annotations for [CloudDirectory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#clouddirectory) service

- [types-aiobotocore-cloudformation](./types_aiobotocore_cloudformation/README.md) - type annotations for [CloudFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudformation.html#cloudformation) service

- [types-aiobotocore-cloudfront](./types_aiobotocore_cloudfront/README.md) - type annotations for [CloudFront](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront.html#cloudfront) service

- [types-aiobotocore-cloudfront-keyvaluestore](./types_aiobotocore_cloudfront_keyvaluestore/README.md) - type annotations for [CloudFrontKeyValueStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudfront-keyvaluestore.html#cloudfrontkeyvaluestore) service

- [types-aiobotocore-cloudhsm](./types_aiobotocore_cloudhsm/README.md) - type annotations for [CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#cloudhsm) service

- [types-aiobotocore-cloudhsmv2](./types_aiobotocore_cloudhsmv2/README.md) - type annotations for [CloudHSMV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#cloudhsmv2) service

- [types-aiobotocore-cloudsearch](./types_aiobotocore_cloudsearch/README.md) - type annotations for [CloudSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#cloudsearch) service

- [types-aiobotocore-cloudsearchdomain](./types_aiobotocore_cloudsearchdomain/README.md) - type annotations for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#cloudsearchdomain) service

- [types-aiobotocore-cloudtrail](./types_aiobotocore_cloudtrail/README.md) - type annotations for [CloudTrail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#cloudtrail) service

- [types-aiobotocore-cloudtrail-data](./types_aiobotocore_cloudtrail_data/README.md) - type annotations for [CloudTrailDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#cloudtraildataservice) service

- [types-aiobotocore-cloudwatch](./types_aiobotocore_cloudwatch/README.md) - type annotations for [CloudWatch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#cloudwatch) service

- [types-aiobotocore-codeartifact](./types_aiobotocore_codeartifact/README.md) - type annotations for [CodeArtifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeartifact.html#codeartifact) service

- [types-aiobotocore-codebuild](./types_aiobotocore_codebuild/README.md) - type annotations for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#codebuild) service

- [types-aiobotocore-codecatalyst](./types_aiobotocore_codecatalyst/README.md) - type annotations for [CodeCatalyst](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecatalyst.html#codecatalyst) service

- [types-aiobotocore-codecommit](./types_aiobotocore_codecommit/README.md) - type annotations for [CodeCommit](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codecommit.html#codecommit) service

- [types-aiobotocore-codeconnections](./types_aiobotocore_codeconnections/README.md) - type annotations for [CodeConnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeconnections.html#codeconnections) service

- [types-aiobotocore-codedeploy](./types_aiobotocore_codedeploy/README.md) - type annotations for [CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#codedeploy) service

- [types-aiobotocore-codeguru-reviewer](./types_aiobotocore_codeguru_reviewer/README.md) - type annotations for [CodeGuruReviewer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#codegurureviewer) service

- [types-aiobotocore-codeguru-security](./types_aiobotocore_codeguru_security/README.md) - type annotations for [CodeGuruSecurity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-security.html#codegurusecurity) service

- [types-aiobotocore-codeguruprofiler](./types_aiobotocore_codeguruprofiler/README.md) - type annotations for [CodeGuruProfiler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguruprofiler.html#codeguruprofiler) service

- [types-aiobotocore-codepipeline](./types_aiobotocore_codepipeline/README.md) - type annotations for [CodePipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codepipeline.html#codepipeline) service

- [types-aiobotocore-codestar-connections](./types_aiobotocore_codestar_connections/README.md) - type annotations for [CodeStarconnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#codestarconnections) service

- [types-aiobotocore-codestar-notifications](./types_aiobotocore_codestar_notifications/README.md) - type annotations for [CodeStarNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#codestarnotifications) service

- [types-aiobotocore-cognito-identity](./types_aiobotocore_cognito_identity/README.md) - type annotations for [CognitoIdentity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#cognitoidentity) service

- [types-aiobotocore-cognito-idp](./types_aiobotocore_cognito_idp/README.md) - type annotations for [CognitoIdentityProvider](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#cognitoidentityprovider) service

- [types-aiobotocore-cognito-sync](./types_aiobotocore_cognito_sync/README.md) - type annotations for [CognitoSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-sync.html#cognitosync) service

- [types-aiobotocore-comprehend](./types_aiobotocore_comprehend/README.md) - type annotations for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#comprehend) service

- [types-aiobotocore-comprehendmedical](./types_aiobotocore_comprehendmedical/README.md) - type annotations for [ComprehendMedical](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#comprehendmedical) service

- [types-aiobotocore-compute-optimizer](./types_aiobotocore_compute_optimizer/README.md) - type annotations for [ComputeOptimizer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#computeoptimizer) service

- [types-aiobotocore-compute-optimizer-automation](./types_aiobotocore_compute_optimizer_automation/README.md) - type annotations for [ComputeOptimizerAutomation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer-automation.html#computeoptimizerautomation) service

- [types-aiobotocore-config](./types_aiobotocore_config/README.md) - type annotations for [ConfigService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#configservice) service

- [types-aiobotocore-connect](./types_aiobotocore_connect/README.md) - type annotations for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#connect) service

- [types-aiobotocore-connect-contact-lens](./types_aiobotocore_connect_contact_lens/README.md) - type annotations for [ConnectContactLens](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#connectcontactlens) service

- [types-aiobotocore-connectcampaigns](./types_aiobotocore_connectcampaigns/README.md) - type annotations for [ConnectCampaignService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#connectcampaignservice) service

- [types-aiobotocore-connectcampaignsv2](./types_aiobotocore_connectcampaignsv2/README.md) - type annotations for [ConnectCampaignServiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2.html#connectcampaignservicev2) service

- [types-aiobotocore-connectcases](./types_aiobotocore_connectcases/README.md) - type annotations for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases) service

- [types-aiobotocore-connectparticipant](./types_aiobotocore_connectparticipant/README.md) - type annotations for [ConnectParticipant](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#connectparticipant) service

- [types-aiobotocore-controlcatalog](./types_aiobotocore_controlcatalog/README.md) - type annotations for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog) service

- [types-aiobotocore-controltower](./types_aiobotocore_controltower/README.md) - type annotations for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#controltower) service

- [types-aiobotocore-cost-optimization-hub](./types_aiobotocore_cost_optimization_hub/README.md) - type annotations for [CostOptimizationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cost-optimization-hub.html#costoptimizationhub) service

- [types-aiobotocore-cur](./types_aiobotocore_cur/README.md) - type annotations for [CostandUsageReportService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#costandusagereportservice) service

- [types-aiobotocore-customer-profiles](./types_aiobotocore_customer_profiles/README.md) - type annotations for [CustomerProfiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/customer-profiles.html#customerprofiles) service

- [types-aiobotocore-databrew](./types_aiobotocore_databrew/README.md) - type annotations for [GlueDataBrew](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/databrew.html#gluedatabrew) service

- [types-aiobotocore-dataexchange](./types_aiobotocore_dataexchange/README.md) - type annotations for [DataExchange](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dataexchange.html#dataexchange) service

- [types-aiobotocore-datapipeline](./types_aiobotocore_datapipeline/README.md) - type annotations for [DataPipeline](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#datapipeline) service

- [types-aiobotocore-datasync](./types_aiobotocore_datasync/README.md) - type annotations for [DataSync](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datasync.html#datasync) service

- [types-aiobotocore-datazone](./types_aiobotocore_datazone/README.md) - type annotations for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#datazone) service

- [types-aiobotocore-dax](./types_aiobotocore_dax/README.md) - type annotations for [DAX](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#dax) service

- [types-aiobotocore-deadline](./types_aiobotocore_deadline/README.md) - type annotations for [DeadlineCloud](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/deadline.html#deadlinecloud) service

- [types-aiobotocore-detective](./types_aiobotocore_detective/README.md) - type annotations for [Detective](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/detective.html#detective) service

- [types-aiobotocore-devicefarm](./types_aiobotocore_devicefarm/README.md) - type annotations for [DeviceFarm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devicefarm.html#devicefarm) service

- [types-aiobotocore-devops-guru](./types_aiobotocore_devops_guru/README.md) - type annotations for [DevOpsGuru](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#devopsguru) service

- [types-aiobotocore-directconnect](./types_aiobotocore_directconnect/README.md) - type annotations for [DirectConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#directconnect) service

- [types-aiobotocore-discovery](./types_aiobotocore_discovery/README.md) - type annotations for [ApplicationDiscoveryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#applicationdiscoveryservice) service

- [types-aiobotocore-dlm](./types_aiobotocore_dlm/README.md) - type annotations for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#dlm) service

- [types-aiobotocore-dms](./types_aiobotocore_dms/README.md) - type annotations for [DatabaseMigrationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dms.html#databasemigrationservice) service

- [types-aiobotocore-docdb](./types_aiobotocore_docdb/README.md) - type annotations for [DocDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#docdb) service

- [types-aiobotocore-docdb-elastic](./types_aiobotocore_docdb_elastic/README.md) - type annotations for [DocDBElastic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#docdbelastic) service

- [types-aiobotocore-drs](./types_aiobotocore_drs/README.md) - type annotations for [Drs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/drs.html#drs) service

- [types-aiobotocore-ds](./types_aiobotocore_ds/README.md) - type annotations for [DirectoryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#directoryservice) service

- [types-aiobotocore-ds-data](./types_aiobotocore_ds_data/README.md) - type annotations for [DirectoryServiceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#directoryservicedata) service

- [types-aiobotocore-dsql](./types_aiobotocore_dsql/README.md) - type annotations for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql) service

- [types-aiobotocore-dynamodb](./types_aiobotocore_dynamodb/README.md) - type annotations for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#dynamodb) service

- [types-aiobotocore-dynamodbstreams](./types_aiobotocore_dynamodbstreams/README.md) - type annotations for [DynamoDBStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#dynamodbstreams) service

- [types-aiobotocore-ebs](./types_aiobotocore_ebs/README.md) - type annotations for [EBS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#ebs) service

- [types-aiobotocore-ec2](./types_aiobotocore_ec2/README.md) - type annotations for [EC2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#ec2) service

- [types-aiobotocore-ec2-instance-connect](./types_aiobotocore_ec2_instance_connect/README.md) - type annotations for [EC2InstanceConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2-instance-connect.html#ec2instanceconnect) service

- [types-aiobotocore-ecr](./types_aiobotocore_ecr/README.md) - type annotations for [ECR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr.html#ecr) service

- [types-aiobotocore-ecr-public](./types_aiobotocore_ecr_public/README.md) - type annotations for [ECRPublic](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ecrpublic) service

- [types-aiobotocore-ecs](./types_aiobotocore_ecs/README.md) - type annotations for [ECS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecs.html#ecs) service

- [types-aiobotocore-efs](./types_aiobotocore_efs/README.md) - type annotations for [EFS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#efs) service

- [types-aiobotocore-eks](./types_aiobotocore_eks/README.md) - type annotations for [EKS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks.html#eks) service

- [types-aiobotocore-eks-auth](./types_aiobotocore_eks_auth/README.md) - type annotations for [EKSAuth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#eksauth) service

- [types-aiobotocore-elasticache](./types_aiobotocore_elasticache/README.md) - type annotations for [ElastiCache](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticache.html#elasticache) service

- [types-aiobotocore-elasticbeanstalk](./types_aiobotocore_elasticbeanstalk/README.md) - type annotations for [ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#elasticbeanstalk) service

- [types-aiobotocore-elb](./types_aiobotocore_elb/README.md) - type annotations for [ElasticLoadBalancing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elb.html#elasticloadbalancing) service

- [types-aiobotocore-elbv2](./types_aiobotocore_elbv2/README.md) - type annotations for [ElasticLoadBalancingv2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elbv2.html#elasticloadbalancingv2) service

- [types-aiobotocore-emr](./types_aiobotocore_emr/README.md) - type annotations for [EMR](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#emr) service

- [types-aiobotocore-emr-containers](./types_aiobotocore_emr_containers/README.md) - type annotations for [EMRContainers](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-containers.html#emrcontainers) service

- [types-aiobotocore-emr-serverless](./types_aiobotocore_emr_serverless/README.md) - type annotations for [EMRServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr-serverless.html#emrserverless) service

- [types-aiobotocore-entityresolution](./types_aiobotocore_entityresolution/README.md) - type annotations for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#entityresolution) service

- [types-aiobotocore-es](./types_aiobotocore_es/README.md) - type annotations for [ElasticsearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/es.html#elasticsearchservice) service

- [types-aiobotocore-events](./types_aiobotocore_events/README.md) - type annotations for [EventBridge](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#eventbridge) service

- [types-aiobotocore-evidently](./types_aiobotocore_evidently/README.md) - type annotations for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently) service

- [types-aiobotocore-evs](./types_aiobotocore_evs/README.md) - type annotations for [EVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evs.html#evs) service

- [types-aiobotocore-finspace](./types_aiobotocore_finspace/README.md) - type annotations for [Finspace](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace) service

- [types-aiobotocore-finspace-data](./types_aiobotocore_finspace_data/README.md) - type annotations for [FinSpaceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#finspacedata) service

- [types-aiobotocore-firehose](./types_aiobotocore_firehose/README.md) - type annotations for [Firehose](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/firehose.html#firehose) service

- [types-aiobotocore-fis](./types_aiobotocore_fis/README.md) - type annotations for [FIS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#fis) service

- [types-aiobotocore-fms](./types_aiobotocore_fms/README.md) - type annotations for [FMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#fms) service

- [types-aiobotocore-forecast](./types_aiobotocore_forecast/README.md) - type annotations for [ForecastService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#forecastservice) service

- [types-aiobotocore-forecastquery](./types_aiobotocore_forecastquery/README.md) - type annotations for [ForecastQueryService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#forecastqueryservice) service

- [types-aiobotocore-frauddetector](./types_aiobotocore_frauddetector/README.md) - type annotations for [FraudDetector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/frauddetector.html#frauddetector) service

- [types-aiobotocore-freetier](./types_aiobotocore_freetier/README.md) - type annotations for [FreeTier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/freetier.html#freetier) service

- [types-aiobotocore-fsx](./types_aiobotocore_fsx/README.md) - type annotations for [FSx](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fsx.html#fsx) service

- [types-aiobotocore-gamelift](./types_aiobotocore_gamelift/README.md) - type annotations for [GameLift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamelift.html#gamelift) service

- [types-aiobotocore-gameliftstreams](./types_aiobotocore_gameliftstreams/README.md) - type annotations for [GameLiftStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gameliftstreams.html#gameliftstreams) service

- [types-aiobotocore-geo-maps](./types_aiobotocore_geo_maps/README.md) - type annotations for [LocationServiceMapsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-maps.html#locationservicemapsv2) service

- [types-aiobotocore-geo-places](./types_aiobotocore_geo_places/README.md) - type annotations for [LocationServicePlacesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-places.html#locationserviceplacesv2) service

- [types-aiobotocore-geo-routes](./types_aiobotocore_geo_routes/README.md) - type annotations for [LocationServiceRoutesV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/geo-routes.html#locationserviceroutesv2) service

- [types-aiobotocore-glacier](./types_aiobotocore_glacier/README.md) - type annotations for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#glacier) service

- [types-aiobotocore-globalaccelerator](./types_aiobotocore_globalaccelerator/README.md) - type annotations for [GlobalAccelerator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#globalaccelerator) service

- [types-aiobotocore-glue](./types_aiobotocore_glue/README.md) - type annotations for [Glue](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glue.html#glue) service

- [types-aiobotocore-grafana](./types_aiobotocore_grafana/README.md) - type annotations for [ManagedGrafana](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/grafana.html#managedgrafana) service

- [types-aiobotocore-greengrass](./types_aiobotocore_greengrass/README.md) - type annotations for [Greengrass](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrass.html#greengrass) service

- [types-aiobotocore-greengrassv2](./types_aiobotocore_greengrassv2/README.md) - type annotations for [GreengrassV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/greengrassv2.html#greengrassv2) service

- [types-aiobotocore-groundstation](./types_aiobotocore_groundstation/README.md) - type annotations for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#groundstation) service

- [types-aiobotocore-guardduty](./types_aiobotocore_guardduty/README.md) - type annotations for [GuardDuty](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#guardduty) service

- [types-aiobotocore-health](./types_aiobotocore_health/README.md) - type annotations for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#health) service

- [types-aiobotocore-healthlake](./types_aiobotocore_healthlake/README.md) - type annotations for [HealthLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#healthlake) service

- [types-aiobotocore-iam](./types_aiobotocore_iam/README.md) - type annotations for [IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#iam) service

- [types-aiobotocore-identitystore](./types_aiobotocore_identitystore/README.md) - type annotations for [IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#identitystore) service

- [types-aiobotocore-imagebuilder](./types_aiobotocore_imagebuilder/README.md) - type annotations for [Imagebuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/imagebuilder.html#imagebuilder) service

- [types-aiobotocore-importexport](./types_aiobotocore_importexport/README.md) - type annotations for [ImportExport](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#importexport) service

- [types-aiobotocore-inspector](./types_aiobotocore_inspector/README.md) - type annotations for [Inspector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#inspector) service

- [types-aiobotocore-inspector-scan](./types_aiobotocore_inspector_scan/README.md) - type annotations for [Inspectorscan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan) service

- [types-aiobotocore-inspector2](./types_aiobotocore_inspector2/README.md) - type annotations for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#inspector2) service

- [types-aiobotocore-internetmonitor](./types_aiobotocore_internetmonitor/README.md) - type annotations for [CloudWatchInternetMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/internetmonitor.html#cloudwatchinternetmonitor) service

- [types-aiobotocore-invoicing](./types_aiobotocore_invoicing/README.md) - type annotations for [Invoicing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/invoicing.html#invoicing) service

- [types-aiobotocore-iot](./types_aiobotocore_iot/README.md) - type annotations for [IoT](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#iot) service

- [types-aiobotocore-iot-data](./types_aiobotocore_iot_data/README.md) - type annotations for [IoTDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-data.html#iotdataplane) service

- [types-aiobotocore-iot-jobs-data](./types_aiobotocore_iot_jobs_data/README.md) - type annotations for [IoTJobsDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#iotjobsdataplane) service

- [types-aiobotocore-iot-managed-integrations](./types_aiobotocore_iot_managed_integrations/README.md) - type annotations for [ManagedintegrationsforIoTDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations.html#managedintegrationsforiotdevicemanagement) service

- [types-aiobotocore-iotanalytics](./types_aiobotocore_iotanalytics/README.md) - type annotations for [IoTAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotanalytics.html#iotanalytics) service

- [types-aiobotocore-iotdeviceadvisor](./types_aiobotocore_iotdeviceadvisor/README.md) - type annotations for [IoTDeviceAdvisor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotdeviceadvisor.html#iotdeviceadvisor) service

- [types-aiobotocore-iotevents](./types_aiobotocore_iotevents/README.md) - type annotations for [IoTEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#iotevents) service

- [types-aiobotocore-iotevents-data](./types_aiobotocore_iotevents_data/README.md) - type annotations for [IoTEventsData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents-data.html#ioteventsdata) service

- [types-aiobotocore-iotfleetwise](./types_aiobotocore_iotfleetwise/README.md) - type annotations for [IoTFleetWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#iotfleetwise) service

- [types-aiobotocore-iotsecuretunneling](./types_aiobotocore_iotsecuretunneling/README.md) - type annotations for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#iotsecuretunneling) service

- [types-aiobotocore-iotsitewise](./types_aiobotocore_iotsitewise/README.md) - type annotations for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#iotsitewise) service

- [types-aiobotocore-iotthingsgraph](./types_aiobotocore_iotthingsgraph/README.md) - type annotations for [IoTThingsGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#iotthingsgraph) service

- [types-aiobotocore-iottwinmaker](./types_aiobotocore_iottwinmaker/README.md) - type annotations for [IoTTwinMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#iottwinmaker) service

- [types-aiobotocore-iotwireless](./types_aiobotocore_iotwireless/README.md) - type annotations for [IoTWireless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#iotwireless) service

- [types-aiobotocore-ivs](./types_aiobotocore_ivs/README.md) - type annotations for [IVS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs.html#ivs) service

- [types-aiobotocore-ivs-realtime](./types_aiobotocore_ivs_realtime/README.md) - type annotations for [Ivsrealtime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime) service

- [types-aiobotocore-ivschat](./types_aiobotocore_ivschat/README.md) - type annotations for [Ivschat](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat) service

- [types-aiobotocore-kafka](./types_aiobotocore_kafka/README.md) - type annotations for [Kafka](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#kafka) service

- [types-aiobotocore-kafkaconnect](./types_aiobotocore_kafkaconnect/README.md) - type annotations for [KafkaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafkaconnect.html#kafkaconnect) service

- [types-aiobotocore-kendra](./types_aiobotocore_kendra/README.md) - type annotations for [Kendra](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra) service

- [types-aiobotocore-kendra-ranking](./types_aiobotocore_kendra_ranking/README.md) - type annotations for [KendraRanking](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#kendraranking) service

- [types-aiobotocore-keyspaces](./types_aiobotocore_keyspaces/README.md) - type annotations for [Keyspaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#keyspaces) service

- [types-aiobotocore-keyspacesstreams](./types_aiobotocore_keyspacesstreams/README.md) - type annotations for [KeyspacesStreams](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspacesstreams.html#keyspacesstreams) service

- [types-aiobotocore-kinesis](./types_aiobotocore_kinesis/README.md) - type annotations for [Kinesis](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis.html#kinesis) service

- [types-aiobotocore-kinesis-video-archived-media](./types_aiobotocore_kinesis_video_archived_media/README.md) - type annotations for [KinesisVideoArchivedMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#kinesisvideoarchivedmedia) service

- [types-aiobotocore-kinesis-video-media](./types_aiobotocore_kinesis_video_media/README.md) - type annotations for [KinesisVideoMedia](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#kinesisvideomedia) service

- [types-aiobotocore-kinesis-video-signaling](./types_aiobotocore_kinesis_video_signaling/README.md) - type annotations for [KinesisVideoSignalingChannels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#kinesisvideosignalingchannels) service

- [types-aiobotocore-kinesis-video-webrtc-storage](./types_aiobotocore_kinesis_video_webrtc_storage/README.md) - type annotations for [KinesisVideoWebRTCStorage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#kinesisvideowebrtcstorage) service

- [types-aiobotocore-kinesisanalytics](./types_aiobotocore_kinesisanalytics/README.md) - type annotations for [KinesisAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#kinesisanalytics) service

- [types-aiobotocore-kinesisanalyticsv2](./types_aiobotocore_kinesisanalyticsv2/README.md) - type annotations for [KinesisAnalyticsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalyticsv2.html#kinesisanalyticsv2) service

- [types-aiobotocore-kinesisvideo](./types_aiobotocore_kinesisvideo/README.md) - type annotations for [KinesisVideo](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#kinesisvideo) service

- [types-aiobotocore-kms](./types_aiobotocore_kms/README.md) - type annotations for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#kms) service

- [types-aiobotocore-lakeformation](./types_aiobotocore_lakeformation/README.md) - type annotations for [LakeFormation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lakeformation.html#lakeformation) service

- [types-aiobotocore-lambda](./types_aiobotocore_lambda/README.md) - type annotations for [Lambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#lambda) service

- [types-aiobotocore-launch-wizard](./types_aiobotocore_launch_wizard/README.md) - type annotations for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#launchwizard) service

- [types-aiobotocore-lex-models](./types_aiobotocore_lex_models/README.md) - type annotations for [LexModelBuildingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#lexmodelbuildingservice) service

- [types-aiobotocore-lex-runtime](./types_aiobotocore_lex_runtime/README.md) - type annotations for [LexRuntimeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#lexruntimeservice) service

- [types-aiobotocore-lexv2-models](./types_aiobotocore_lexv2_models/README.md) - type annotations for [LexModelsV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-models.html#lexmodelsv2) service

- [types-aiobotocore-lexv2-runtime](./types_aiobotocore_lexv2_runtime/README.md) - type annotations for [LexRuntimeV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#lexruntimev2) service

- [types-aiobotocore-license-manager](./types_aiobotocore_license_manager/README.md) - type annotations for [LicenseManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#licensemanager) service

- [types-aiobotocore-license-manager-linux-subscriptions](./types_aiobotocore_license_manager_linux_subscriptions/README.md) - type annotations for [LicenseManagerLinuxSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#licensemanagerlinuxsubscriptions) service

- [types-aiobotocore-license-manager-user-subscriptions](./types_aiobotocore_license_manager_user_subscriptions/README.md) - type annotations for [LicenseManagerUserSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#licensemanagerusersubscriptions) service

- [types-aiobotocore-lightsail](./types_aiobotocore_lightsail/README.md) - type annotations for [Lightsail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#lightsail) service

- [types-aiobotocore-location](./types_aiobotocore_location/README.md) - type annotations for [LocationService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#locationservice) service

- [types-aiobotocore-logs](./types_aiobotocore_logs/README.md) - type annotations for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#cloudwatchlogs) service

- [types-aiobotocore-lookoutequipment](./types_aiobotocore_lookoutequipment/README.md) - type annotations for [LookoutEquipment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutequipment.html#lookoutequipment) service

- [types-aiobotocore-m2](./types_aiobotocore_m2/README.md) - type annotations for [MainframeModernization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/m2.html#mainframemodernization) service

- [types-aiobotocore-machinelearning](./types_aiobotocore_machinelearning/README.md) - type annotations for [MachineLearning](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#machinelearning) service

- [types-aiobotocore-macie2](./types_aiobotocore_macie2/README.md) - type annotations for [Macie2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#macie2) service

- [types-aiobotocore-mailmanager](./types_aiobotocore_mailmanager/README.md) - type annotations for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager) service

- [types-aiobotocore-managedblockchain](./types_aiobotocore_managedblockchain/README.md) - type annotations for [ManagedBlockchain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#managedblockchain) service

- [types-aiobotocore-managedblockchain-query](./types_aiobotocore_managedblockchain_query/README.md) - type annotations for [ManagedBlockchainQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain-query.html#managedblockchainquery) service

- [types-aiobotocore-marketplace-agreement](./types_aiobotocore_marketplace_agreement/README.md) - type annotations for [AgreementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-agreement.html#agreementservice) service

- [types-aiobotocore-marketplace-catalog](./types_aiobotocore_marketplace_catalog/README.md) - type annotations for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#marketplacecatalog) service

- [types-aiobotocore-marketplace-deployment](./types_aiobotocore_marketplace_deployment/README.md) - type annotations for [MarketplaceDeploymentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-deployment.html#marketplacedeploymentservice) service

- [types-aiobotocore-marketplace-entitlement](./types_aiobotocore_marketplace_entitlement/README.md) - type annotations for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#marketplaceentitlementservice) service

- [types-aiobotocore-marketplace-reporting](./types_aiobotocore_marketplace_reporting/README.md) - type annotations for [MarketplaceReportingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#marketplacereportingservice) service

- [types-aiobotocore-marketplacecommerceanalytics](./types_aiobotocore_marketplacecommerceanalytics/README.md) - type annotations for [MarketplaceCommerceAnalytics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplacecommerceanalytics.html#marketplacecommerceanalytics) service

- [types-aiobotocore-mediaconnect](./types_aiobotocore_mediaconnect/README.md) - type annotations for [MediaConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconnect.html#mediaconnect) service

- [types-aiobotocore-mediaconvert](./types_aiobotocore_mediaconvert/README.md) - type annotations for [MediaConvert](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#mediaconvert) service

- [types-aiobotocore-medialive](./types_aiobotocore_medialive/README.md) - type annotations for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#medialive) service

- [types-aiobotocore-mediapackage](./types_aiobotocore_mediapackage/README.md) - type annotations for [MediaPackage](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage.html#mediapackage) service

- [types-aiobotocore-mediapackage-vod](./types_aiobotocore_mediapackage_vod/README.md) - type annotations for [MediaPackageVod](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackage-vod.html#mediapackagevod) service

- [types-aiobotocore-mediapackagev2](./types_aiobotocore_mediapackagev2/README.md) - type annotations for [Mediapackagev2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediapackagev2.html#mediapackagev2) service

- [types-aiobotocore-mediastore](./types_aiobotocore_mediastore/README.md) - type annotations for [MediaStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#mediastore) service

- [types-aiobotocore-mediastore-data](./types_aiobotocore_mediastore_data/README.md) - type annotations for [MediaStoreData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#mediastoredata) service

- [types-aiobotocore-mediatailor](./types_aiobotocore_mediatailor/README.md) - type annotations for [MediaTailor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#mediatailor) service

- [types-aiobotocore-medical-imaging](./types_aiobotocore_medical_imaging/README.md) - type annotations for [HealthImaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#healthimaging) service

- [types-aiobotocore-memorydb](./types_aiobotocore_memorydb/README.md) - type annotations for [MemoryDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/memorydb.html#memorydb) service

- [types-aiobotocore-meteringmarketplace](./types_aiobotocore_meteringmarketplace/README.md) - type annotations for [MarketplaceMetering](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#marketplacemetering) service

- [types-aiobotocore-mgh](./types_aiobotocore_mgh/README.md) - type annotations for [MigrationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#migrationhub) service

- [types-aiobotocore-mgn](./types_aiobotocore_mgn/README.md) - type annotations for [Mgn](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgn.html#mgn) service

- [types-aiobotocore-migration-hub-refactor-spaces](./types_aiobotocore_migration_hub_refactor_spaces/README.md) - type annotations for [MigrationHubRefactorSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#migrationhubrefactorspaces) service

- [types-aiobotocore-migrationhub-config](./types_aiobotocore_migrationhub_config/README.md) - type annotations for [MigrationHubConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#migrationhubconfig) service

- [types-aiobotocore-migrationhuborchestrator](./types_aiobotocore_migrationhuborchestrator/README.md) - type annotations for [MigrationHubOrchestrator](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhuborchestrator.html#migrationhuborchestrator) service

- [types-aiobotocore-migrationhubstrategy](./types_aiobotocore_migrationhubstrategy/README.md) - type annotations for [MigrationHubStrategyRecommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#migrationhubstrategyrecommendations) service

- [types-aiobotocore-mpa](./types_aiobotocore_mpa/README.md) - type annotations for [MultipartyApproval](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mpa.html#multipartyapproval) service

- [types-aiobotocore-mq](./types_aiobotocore_mq/README.md) - type annotations for [MQ](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mq.html#mq) service

- [types-aiobotocore-mturk](./types_aiobotocore_mturk/README.md) - type annotations for [MTurk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#mturk) service

- [types-aiobotocore-mwaa](./types_aiobotocore_mwaa/README.md) - type annotations for [MWAA](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#mwaa) service

- [types-aiobotocore-mwaa-serverless](./types_aiobotocore_mwaa_serverless/README.md) - type annotations for [MWAAServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa-serverless.html#mwaaserverless) service

- [types-aiobotocore-neptune](./types_aiobotocore_neptune/README.md) - type annotations for [Neptune](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune.html#neptune) service

- [types-aiobotocore-neptune-graph](./types_aiobotocore_neptune_graph/README.md) - type annotations for [NeptuneGraph](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptune-graph.html#neptunegraph) service

- [types-aiobotocore-neptunedata](./types_aiobotocore_neptunedata/README.md) - type annotations for [NeptuneData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/neptunedata.html#neptunedata) service

- [types-aiobotocore-network-firewall](./types_aiobotocore_network_firewall/README.md) - type annotations for [NetworkFirewall](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/network-firewall.html#networkfirewall) service

- [types-aiobotocore-networkflowmonitor](./types_aiobotocore_networkflowmonitor/README.md) - type annotations for [NetworkFlowMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkflowmonitor.html#networkflowmonitor) service

- [types-aiobotocore-networkmanager](./types_aiobotocore_networkmanager/README.md) - type annotations for [NetworkManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#networkmanager) service

- [types-aiobotocore-networkmonitor](./types_aiobotocore_networkmonitor/README.md) - type annotations for [CloudWatchNetworkMonitor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmonitor.html#cloudwatchnetworkmonitor) service

- [types-aiobotocore-notifications](./types_aiobotocore_notifications/README.md) - type annotations for [UserNotifications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notifications.html#usernotifications) service

- [types-aiobotocore-notificationscontacts](./types_aiobotocore_notificationscontacts/README.md) - type annotations for [UserNotificationsContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#usernotificationscontacts) service

- [types-aiobotocore-nova-act](./types_aiobotocore_nova_act/README.md) - type annotations for [NovaActService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nova-act.html#novaactservice) service

- [types-aiobotocore-oam](./types_aiobotocore_oam/README.md) - type annotations for [CloudWatchObservabilityAccessManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#cloudwatchobservabilityaccessmanager) service

- [types-aiobotocore-observabilityadmin](./types_aiobotocore_observabilityadmin/README.md) - type annotations for [CloudWatchObservabilityAdminService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/observabilityadmin.html#cloudwatchobservabilityadminservice) service

- [types-aiobotocore-odb](./types_aiobotocore_odb/README.md) - type annotations for [Odb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/odb.html#odb) service

- [types-aiobotocore-omics](./types_aiobotocore_omics/README.md) - type annotations for [Omics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/omics.html#omics) service

- [types-aiobotocore-opensearch](./types_aiobotocore_opensearch/README.md) - type annotations for [OpenSearchService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#opensearchservice) service

- [types-aiobotocore-opensearchserverless](./types_aiobotocore_opensearchserverless/README.md) - type annotations for [OpenSearchServiceServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearchserverless.html#opensearchserviceserverless) service

- [types-aiobotocore-organizations](./types_aiobotocore_organizations/README.md) - type annotations for [Organizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/organizations.html#organizations) service

- [types-aiobotocore-osis](./types_aiobotocore_osis/README.md) - type annotations for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion) service

- [types-aiobotocore-outposts](./types_aiobotocore_outposts/README.md) - type annotations for [Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/outposts.html#outposts) service

- [types-aiobotocore-panorama](./types_aiobotocore_panorama/README.md) - type annotations for [Panorama](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/panorama.html#panorama) service

- [types-aiobotocore-partnercentral-account](./types_aiobotocore_partnercentral_account/README.md) - type annotations for [PartnerCentralAccountAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-account.html#partnercentralaccountapi) service

- [types-aiobotocore-partnercentral-benefits](./types_aiobotocore_partnercentral_benefits/README.md) - type annotations for [PartnerCentralBenefits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-benefits.html#partnercentralbenefits) service

- [types-aiobotocore-partnercentral-channel](./types_aiobotocore_partnercentral_channel/README.md) - type annotations for [PartnerCentralChannelAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-channel.html#partnercentralchannelapi) service

- [types-aiobotocore-partnercentral-selling](./types_aiobotocore_partnercentral_selling/README.md) - type annotations for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi) service

- [types-aiobotocore-payment-cryptography](./types_aiobotocore_payment_cryptography/README.md) - type annotations for [PaymentCryptographyControlPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography.html#paymentcryptographycontrolplane) service

- [types-aiobotocore-payment-cryptography-data](./types_aiobotocore_payment_cryptography_data/README.md) - type annotations for [PaymentCryptographyDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/payment-cryptography-data.html#paymentcryptographydataplane) service

- [types-aiobotocore-pca-connector-ad](./types_aiobotocore_pca_connector_ad/README.md) - type annotations for [PcaConnectorAd](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-ad.html#pcaconnectorad) service

- [types-aiobotocore-pca-connector-scep](./types_aiobotocore_pca_connector_scep/README.md) - type annotations for [PrivateCAConnectorforSCEP](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pca-connector-scep.html#privatecaconnectorforscep) service

- [types-aiobotocore-pcs](./types_aiobotocore_pcs/README.md) - type annotations for [ParallelComputingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pcs.html#parallelcomputingservice) service

- [types-aiobotocore-personalize](./types_aiobotocore_personalize/README.md) - type annotations for [Personalize](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize.html#personalize) service

- [types-aiobotocore-personalize-events](./types_aiobotocore_personalize_events/README.md) - type annotations for [PersonalizeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-events.html#personalizeevents) service

- [types-aiobotocore-personalize-runtime](./types_aiobotocore_personalize_runtime/README.md) - type annotations for [PersonalizeRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#personalizeruntime) service

- [types-aiobotocore-pi](./types_aiobotocore_pi/README.md) - type annotations for [PI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#pi) service

- [types-aiobotocore-pinpoint](./types_aiobotocore_pinpoint/README.md) - type annotations for [Pinpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#pinpoint) service

- [types-aiobotocore-pinpoint-email](./types_aiobotocore_pinpoint_email/README.md) - type annotations for [PinpointEmail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#pinpointemail) service

- [types-aiobotocore-pinpoint-sms-voice](./types_aiobotocore_pinpoint_sms_voice/README.md) - type annotations for [PinpointSMSVoice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice.html#pinpointsmsvoice) service

- [types-aiobotocore-pinpoint-sms-voice-v2](./types_aiobotocore_pinpoint_sms_voice_v2/README.md) - type annotations for [PinpointSMSVoiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#pinpointsmsvoicev2) service

- [types-aiobotocore-pipes](./types_aiobotocore_pipes/README.md) - type annotations for [EventBridgePipes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pipes.html#eventbridgepipes) service

- [types-aiobotocore-polly](./types_aiobotocore_polly/README.md) - type annotations for [Polly](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#polly) service

- [types-aiobotocore-pricing](./types_aiobotocore_pricing/README.md) - type annotations for [Pricing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pricing.html#pricing) service

- [types-aiobotocore-proton](./types_aiobotocore_proton/README.md) - type annotations for [Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#proton) service

- [types-aiobotocore-qapps](./types_aiobotocore_qapps/README.md) - type annotations for [QApps](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qapps.html#qapps) service

- [types-aiobotocore-qbusiness](./types_aiobotocore_qbusiness/README.md) - type annotations for [QBusiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qbusiness.html#qbusiness) service

- [types-aiobotocore-qconnect](./types_aiobotocore_qconnect/README.md) - type annotations for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#qconnect) service

- [types-aiobotocore-quicksight](./types_aiobotocore_quicksight/README.md) - type annotations for [QuickSight](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#quicksight) service

- [types-aiobotocore-ram](./types_aiobotocore_ram/README.md) - type annotations for [RAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#ram) service

- [types-aiobotocore-rbin](./types_aiobotocore_rbin/README.md) - type annotations for [RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#recyclebin) service

- [types-aiobotocore-rds](./types_aiobotocore_rds/README.md) - type annotations for [RDS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds.html#rds) service

- [types-aiobotocore-rds-data](./types_aiobotocore_rds_data/README.md) - type annotations for [RDSDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rds-data.html#rdsdataservice) service

- [types-aiobotocore-redshift](./types_aiobotocore_redshift/README.md) - type annotations for [Redshift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#redshift) service

- [types-aiobotocore-redshift-data](./types_aiobotocore_redshift_data/README.md) - type annotations for [RedshiftDataAPIService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#redshiftdataapiservice) service

- [types-aiobotocore-redshift-serverless](./types_aiobotocore_redshift_serverless/README.md) - type annotations for [RedshiftServerless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#redshiftserverless) service

- [types-aiobotocore-rekognition](./types_aiobotocore_rekognition/README.md) - type annotations for [Rekognition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#rekognition) service

- [types-aiobotocore-repostspace](./types_aiobotocore_repostspace/README.md) - type annotations for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate) service

- [types-aiobotocore-resiliencehub](./types_aiobotocore_resiliencehub/README.md) - type annotations for [ResilienceHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resiliencehub.html#resiliencehub) service

- [types-aiobotocore-resource-explorer-2](./types_aiobotocore_resource_explorer_2/README.md) - type annotations for [ResourceExplorer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#resourceexplorer) service

- [types-aiobotocore-resource-groups](./types_aiobotocore_resource_groups/README.md) - type annotations for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#resourcegroups) service

- [types-aiobotocore-resourcegroupstaggingapi](./types_aiobotocore_resourcegroupstaggingapi/README.md) - type annotations for [ResourceGroupsTaggingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#resourcegroupstaggingapi) service

- [types-aiobotocore-rolesanywhere](./types_aiobotocore_rolesanywhere/README.md) - type annotations for [IAMRolesAnywhere](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#iamrolesanywhere) service

- [types-aiobotocore-route53](./types_aiobotocore_route53/README.md) - type annotations for [Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#route53) service

- [types-aiobotocore-route53-recovery-cluster](./types_aiobotocore_route53_recovery_cluster/README.md) - type annotations for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#route53recoverycluster) service

- [types-aiobotocore-route53-recovery-control-config](./types_aiobotocore_route53_recovery_control_config/README.md) - type annotations for [Route53RecoveryControlConfig](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-control-config.html#route53recoverycontrolconfig) service

- [types-aiobotocore-route53-recovery-readiness](./types_aiobotocore_route53_recovery_readiness/README.md) - type annotations for [Route53RecoveryReadiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#route53recoveryreadiness) service

- [types-aiobotocore-route53domains](./types_aiobotocore_route53domains/README.md) - type annotations for [Route53Domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#route53domains) service

- [types-aiobotocore-route53globalresolver](./types_aiobotocore_route53globalresolver/README.md) - type annotations for [Route53GlobalResolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53globalresolver.html#route53globalresolver) service

- [types-aiobotocore-route53profiles](./types_aiobotocore_route53profiles/README.md) - type annotations for [Route53Profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#route53profiles) service

- [types-aiobotocore-route53resolver](./types_aiobotocore_route53resolver/README.md) - type annotations for [Route53Resolver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53resolver.html#route53resolver) service

- [types-aiobotocore-rtbfabric](./types_aiobotocore_rtbfabric/README.md) - type annotations for [RTBFabric](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rtbfabric.html#rtbfabric) service

- [types-aiobotocore-rum](./types_aiobotocore_rum/README.md) - type annotations for [CloudWatchRUM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#cloudwatchrum) service

- [types-aiobotocore-s3](./types_aiobotocore_s3/README.md) - type annotations for [S3](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#s3) service

- [types-aiobotocore-s3control](./types_aiobotocore_s3control/README.md) - type annotations for [S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#s3control) service

- [types-aiobotocore-s3outposts](./types_aiobotocore_s3outposts/README.md) - type annotations for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#s3outposts) service

- [types-aiobotocore-s3tables](./types_aiobotocore_s3tables/README.md) - type annotations for [S3Tables](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3tables.html#s3tables) service

- [types-aiobotocore-s3vectors](./types_aiobotocore_s3vectors/README.md) - type annotations for [S3Vectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3vectors.html#s3vectors) service

- [types-aiobotocore-sagemaker](./types_aiobotocore_sagemaker/README.md) - type annotations for [SageMaker](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker.html#sagemaker) service

- [types-aiobotocore-sagemaker-a2i-runtime](./types_aiobotocore_sagemaker_a2i_runtime/README.md) - type annotations for [AugmentedAIRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#augmentedairuntime) service

- [types-aiobotocore-sagemaker-edge](./types_aiobotocore_sagemaker_edge/README.md) - type annotations for [SagemakerEdgeManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#sagemakeredgemanager) service

- [types-aiobotocore-sagemaker-featurestore-runtime](./types_aiobotocore_sagemaker_featurestore_runtime/README.md) - type annotations for [SageMakerFeatureStoreRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-featurestore-runtime.html#sagemakerfeaturestoreruntime) service

- [types-aiobotocore-sagemaker-geospatial](./types_aiobotocore_sagemaker_geospatial/README.md) - type annotations for [SageMakergeospatialcapabilities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#sagemakergeospatialcapabilities) service

- [types-aiobotocore-sagemaker-metrics](./types_aiobotocore_sagemaker_metrics/README.md) - type annotations for [SageMakerMetrics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#sagemakermetrics) service

- [types-aiobotocore-sagemaker-runtime](./types_aiobotocore_sagemaker_runtime/README.md) - type annotations for [SageMakerRuntime](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-runtime.html#sagemakerruntime) service

- [types-aiobotocore-savingsplans](./types_aiobotocore_savingsplans/README.md) - type annotations for [SavingsPlans](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/savingsplans.html#savingsplans) service

- [types-aiobotocore-scheduler](./types_aiobotocore_scheduler/README.md) - type annotations for [EventBridgeScheduler](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/scheduler.html#eventbridgescheduler) service

- [types-aiobotocore-schemas](./types_aiobotocore_schemas/README.md) - type annotations for [Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#schemas) service

- [types-aiobotocore-sdb](./types_aiobotocore_sdb/README.md) - type annotations for [SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#simpledb) service

- [types-aiobotocore-secretsmanager](./types_aiobotocore_secretsmanager/README.md) - type annotations for [SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#secretsmanager) service

- [types-aiobotocore-security-ir](./types_aiobotocore_security_ir/README.md) - type annotations for [SecurityIncidentResponse](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#securityincidentresponse) service

- [types-aiobotocore-securityhub](./types_aiobotocore_securityhub/README.md) - type annotations for [SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#securityhub) service

- [types-aiobotocore-securitylake](./types_aiobotocore_securitylake/README.md) - type annotations for [SecurityLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securitylake.html#securitylake) service

- [types-aiobotocore-serverlessrepo](./types_aiobotocore_serverlessrepo/README.md) - type annotations for [ServerlessApplicationRepository](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#serverlessapplicationrepository) service

- [types-aiobotocore-service-quotas](./types_aiobotocore_service_quotas/README.md) - type annotations for [ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#servicequotas) service

- [types-aiobotocore-servicecatalog](./types_aiobotocore_servicecatalog/README.md) - type annotations for [ServiceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#servicecatalog) service

- [types-aiobotocore-servicecatalog-appregistry](./types_aiobotocore_servicecatalog_appregistry/README.md) - type annotations for [AppRegistry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#appregistry) service

- [types-aiobotocore-servicediscovery](./types_aiobotocore_servicediscovery/README.md) - type annotations for [ServiceDiscovery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicediscovery.html#servicediscovery) service

- [types-aiobotocore-ses](./types_aiobotocore_ses/README.md) - type annotations for [SES](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#ses) service

- [types-aiobotocore-sesv2](./types_aiobotocore_sesv2/README.md) - type annotations for [SESV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sesv2.html#sesv2) service

- [types-aiobotocore-shield](./types_aiobotocore_shield/README.md) - type annotations for [Shield](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/shield.html#shield) service

- [types-aiobotocore-signer](./types_aiobotocore_signer/README.md) - type annotations for [Signer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer) service

- [types-aiobotocore-signin](./types_aiobotocore_signin/README.md) - type annotations for [SignInService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#signinservice) service

- [types-aiobotocore-simspaceweaver](./types_aiobotocore_simspaceweaver/README.md) - type annotations for [SimSpaceWeaver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#simspaceweaver) service

- [types-aiobotocore-snow-device-management](./types_aiobotocore_snow_device_management/README.md) - type annotations for [SnowDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#snowdevicemanagement) service

- [types-aiobotocore-snowball](./types_aiobotocore_snowball/README.md) - type annotations for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#snowball) service

- [types-aiobotocore-sns](./types_aiobotocore_sns/README.md) - type annotations for [SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#sns) service

- [types-aiobotocore-socialmessaging](./types_aiobotocore_socialmessaging/README.md) - type annotations for [EndUserMessagingSocial](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/socialmessaging.html#endusermessagingsocial) service

- [types-aiobotocore-sqs](./types_aiobotocore_sqs/README.md) - type annotations for [SQS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#sqs) service

- [types-aiobotocore-ssm](./types_aiobotocore_ssm/README.md) - type annotations for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#ssm) service

- [types-aiobotocore-ssm-contacts](./types_aiobotocore_ssm_contacts/README.md) - type annotations for [SSMContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#ssmcontacts) service

- [types-aiobotocore-ssm-guiconnect](./types_aiobotocore_ssm_guiconnect/README.md) - type annotations for [SSMGUIConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-guiconnect.html#ssmguiconnect) service

- [types-aiobotocore-ssm-incidents](./types_aiobotocore_ssm_incidents/README.md) - type annotations for [SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#ssmincidents) service

- [types-aiobotocore-ssm-quicksetup](./types_aiobotocore_ssm_quicksetup/README.md) - type annotations for [SystemsManagerQuickSetup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#systemsmanagerquicksetup) service

- [types-aiobotocore-ssm-sap](./types_aiobotocore_ssm_sap/README.md) - type annotations for [SsmSap](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-sap.html#ssmsap) service

- [types-aiobotocore-sso](./types_aiobotocore_sso/README.md) - type annotations for [SSO](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#sso) service

- [types-aiobotocore-sso-admin](./types_aiobotocore_sso_admin/README.md) - type annotations for [SSOAdmin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#ssoadmin) service

- [types-aiobotocore-sso-oidc](./types_aiobotocore_sso_oidc/README.md) - type annotations for [SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#ssooidc) service

- [types-aiobotocore-stepfunctions](./types_aiobotocore_stepfunctions/README.md) - type annotations for [SFN](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#sfn) service

- [types-aiobotocore-storagegateway](./types_aiobotocore_storagegateway/README.md) - type annotations for [StorageGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/storagegateway.html#storagegateway) service

- [types-aiobotocore-sts](./types_aiobotocore_sts/README.md) - type annotations for [STS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#sts) service

- [types-aiobotocore-supplychain](./types_aiobotocore_supplychain/README.md) - type annotations for [SupplyChain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/supplychain.html#supplychain) service

- [types-aiobotocore-support](./types_aiobotocore_support/README.md) - type annotations for [Support](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#support) service

- [types-aiobotocore-support-app](./types_aiobotocore_support_app/README.md) - type annotations for [SupportApp](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#supportapp) service

- [types-aiobotocore-swf](./types_aiobotocore_swf/README.md) - type annotations for [SWF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/swf.html#swf) service

- [types-aiobotocore-synthetics](./types_aiobotocore_synthetics/README.md) - type annotations for [Synthetics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#synthetics) service

- [types-aiobotocore-taxsettings](./types_aiobotocore_taxsettings/README.md) - type annotations for [TaxSettings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/taxsettings.html#taxsettings) service

- [types-aiobotocore-textract](./types_aiobotocore_textract/README.md) - type annotations for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#textract) service

- [types-aiobotocore-timestream-influxdb](./types_aiobotocore_timestream_influxdb/README.md) - type annotations for [TimestreamInfluxDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-influxdb.html#timestreaminfluxdb) service

- [types-aiobotocore-timestream-query](./types_aiobotocore_timestream_query/README.md) - type annotations for [TimestreamQuery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#timestreamquery) service

- [types-aiobotocore-timestream-write](./types_aiobotocore_timestream_write/README.md) - type annotations for [TimestreamWrite](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#timestreamwrite) service

- [types-aiobotocore-tnb](./types_aiobotocore_tnb/README.md) - type annotations for [TelcoNetworkBuilder](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/tnb.html#telconetworkbuilder) service

- [types-aiobotocore-transcribe](./types_aiobotocore_transcribe/README.md) - type annotations for [TranscribeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#transcribeservice) service

- [types-aiobotocore-transfer](./types_aiobotocore_transfer/README.md) - type annotations for [Transfer](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#transfer) service

- [types-aiobotocore-translate](./types_aiobotocore_translate/README.md) - type annotations for [Translate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/translate.html#translate) service

- [types-aiobotocore-trustedadvisor](./types_aiobotocore_trustedadvisor/README.md) - type annotations for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#trustedadvisorpublicapi) service

- [types-aiobotocore-verifiedpermissions](./types_aiobotocore_verifiedpermissions/README.md) - type annotations for [VerifiedPermissions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#verifiedpermissions) service

- [types-aiobotocore-voice-id](./types_aiobotocore_voice_id/README.md) - type annotations for [VoiceID](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#voiceid) service

- [types-aiobotocore-vpc-lattice](./types_aiobotocore_vpc_lattice/README.md) - type annotations for [VPCLattice](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#vpclattice) service

- [types-aiobotocore-waf](./types_aiobotocore_waf/README.md) - type annotations for [WAF](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf.html#waf) service

- [types-aiobotocore-waf-regional](./types_aiobotocore_waf_regional/README.md) - type annotations for [WAFRegional](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/waf-regional.html#wafregional) service

- [types-aiobotocore-wafv2](./types_aiobotocore_wafv2/README.md) - type annotations for [WAFV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wafv2.html#wafv2) service

- [types-aiobotocore-wellarchitected](./types_aiobotocore_wellarchitected/README.md) - type annotations for [WellArchitected](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wellarchitected.html#wellarchitected) service

- [types-aiobotocore-wickr](./types_aiobotocore_wickr/README.md) - type annotations for [WickrAdminAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wickr.html#wickradminapi) service

- [types-aiobotocore-wisdom](./types_aiobotocore_wisdom/README.md) - type annotations for [ConnectWisdomService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#connectwisdomservice) service

- [types-aiobotocore-workdocs](./types_aiobotocore_workdocs/README.md) - type annotations for [WorkDocs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workdocs.html#workdocs) service

- [types-aiobotocore-workmail](./types_aiobotocore_workmail/README.md) - type annotations for [WorkMail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmail.html#workmail) service

- [types-aiobotocore-workmailmessageflow](./types_aiobotocore_workmailmessageflow/README.md) - type annotations for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#workmailmessageflow) service

- [types-aiobotocore-workspaces](./types_aiobotocore_workspaces/README.md) - type annotations for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#workspaces) service

- [types-aiobotocore-workspaces-instances](./types_aiobotocore_workspaces_instances/README.md) - type annotations for [WorkspacesInstances](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-instances.html#workspacesinstances) service

- [types-aiobotocore-workspaces-thin-client](./types_aiobotocore_workspaces_thin_client/README.md) - type annotations for [WorkSpacesThinClient](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-thin-client.html#workspacesthinclient) service

- [types-aiobotocore-workspaces-web](./types_aiobotocore_workspaces_web/README.md) - type annotations for [WorkSpacesWeb](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces-web.html#workspacesweb) service

- [types-aiobotocore-xray](./types_aiobotocore_xray/README.md) - type annotations for [XRay](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#xray) service
