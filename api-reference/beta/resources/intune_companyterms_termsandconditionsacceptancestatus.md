﻿# termsAndConditionsAcceptanceStatus resource type> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.

The acceptance status for a user targeted a terms and conditions.
### Methods
|Method|Return Type|Description|
|---|---|---|
|[List termsAndConditionsAcceptanceStatuses](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) collection|List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) objects.|
|[Get termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.|
|[Create termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Create a new [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.|
|[Delete termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|None|Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).|
|[Update termsAndConditionsAcceptanceStatus](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.|
|[Get termsAndConditions](../api/intune_companyterms_termsandconditionsacceptancestatus_get_termsandconditions.md)|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Get the [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) from the termsAndConditions navigation property.|

### Properties
|Property|Type|Description|
|---|---|---|
|id|String|Key of the entity.|
|userDisplayName|String|The name of the user that this acceptance status is for.|
|acceptedVersion|Int32|The version of the terms that were accepted. 0 if never accepted.|
|acceptedDateTime|DateTimeOffset|The date and time that the terms were accepted.|

### Relationships
|Relationship|Type|Description|
|---|---|---|
|termsAndConditions|[termsAndConditions](../resources/intune_companyterms_termsandconditions.md)|Navigation link to the terms and conditions that are assigned.|

### JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
```json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```



