﻿# List remoteActionAudits> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.
List properties and relationships of the [remoteActionAudit](../resources/intune_onboarding_remoteactionaudit.md) objects.
### Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementManagedDevices.Read.All; DeviceManagementManagedDevices.ReadWrite.All*
### HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /deviceManagement/remoteActionAudits/
```

### Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

### Request body
Do not supply a request body for this method.

### Response
If successful, this method returns a `200 OK` response code and a collection of [remoteActionAudit](../resources/intune_onboarding_remoteactionaudit.md) objects in the response body.

### Example
##### Request
Here is an example of the request.
```http
GET https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.remoteActionAudit",
      "id": "477f8d24-8d24-477f-248d-7f47248d7f47",
      "deviceDisplayName": "Device Display Name value",
      "userName": "User Name value",
      "action": "factoryReset",
      "requestDateTime": "2017-01-01T00:03:07.1589002-08:00"
    }
  ]
}
```



