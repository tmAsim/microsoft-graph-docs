﻿# termsAndConditions resource type> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.

Terms And Conditions.
### Methods
|Method|Return Type|Description|
|---|---|---|
|[List termsAndConditionss](../api/intune_companyterms_termsandconditions_list.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) collection|List properties and relationships of the [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) objects.|
|[Get termsAndConditions](../api/intune_companyterms_termsandconditions_get.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Read properties and relationships of the [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.|
|[Create termsAndConditions](../api/intune_companyterms_termsandconditions_create.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Create a new [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.|
|[Delete termsAndConditions](../api/intune_companyterms_termsandconditions_delete.md)|None|Deletes a [termsAndConditions](../resources/intune_companyterms_termsandconditions.md).|
|[Update termsAndConditions](../api/intune_companyterms_termsandconditions_update.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Update the properties of a [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.|
|[List termsAndConditionsGroupAssignments](../api/intune_companyterms_termsandconditions_list_termsandconditionsgroupassignment.md)|[termsAndConditionsGroupAssignment](../resources/intune_companyterms_termsandconditionsgroupassignment.md) collection|Get the termsAndConditionsGroupAssignments from the groupAssignments navigation property.|
|[List termsAndConditionsAcceptanceStatuses](../api/intune_companyterms_termsandconditions_list_termsandconditionsacceptancestatus.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatuses from the acceptanceStatuses navigation property.|

### Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|modifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|displayName|String|Admin provided name of the term.|
|description|String|Admin provided description of the term.|
|title|String|Admin provided title of the term.|
|bodyText|String|Admin provided body text of the term.|
|acceptanceStatement|String|Admin provided acceptance statement of the term.|
|version|Int32|Version of the term.|

### Relationships
|Relationship|Type|Description|
|---|---|---|
|groupAssignments|[termsAndConditionsGroupAssignment](../resources/intune_companyterms_termsandconditionsgroupassignment.md) collection|The list of group assignments for this terms and conditions.|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) collection|The list of acceptance statuses for this terms and conditions.|

### JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "title": "String",
  "bodyText": "String",
  "acceptanceStatement": "String",
  "version": 1024
}
```



