﻿# Get windowsPhone81StoreApp> **Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.
Read properties and relationships of the [windowsPhone81StoreApp](../resources/intune_apps_windowsphone81storeapp.md) object.
### Prerequisites
One of the following **scopes** is required to execute this API:

*DeviceManagementApps.ReadWrite.All; DeviceManagementApps.Read.All*
### HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /deviceAppManagement/mobileApps/{id}
GET /deviceAppManagement/mobileApps/{id}/userStatuses/{id}/app/
GET /deviceAppManagement/mobileApps/{id}/deviceStatuses/{id}/app/
GET /deviceAppManagement/mobileApps/{id}/groupAssignments/{id}/app/
```

### Optional query parameters
This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.
### Request headers
|Header|Value|
|---|---|
|Authorization|Bearer &lt;token&gt; Required.|
|Accept|application/json|

### Request body
Do not supply a request body for this method.

### Response
If successful, this method returns a `200 OK` response code and [windowsPhone81StoreApp](../resources/intune_apps_windowsphone81storeapp.md) object in the response body.

### Example
##### Request
Here is an example of the request.
```http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}
```

##### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1159

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsPhone81StoreApp",
    "id": "f68ce6a1-e6a1-f68c-a1e6-8cf6a1e68cf6",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "uploadState": 11,
    "installSummary": {
      "@odata.type": "microsoft.graph.mobileAppInstallSummary",
      "installedDeviceCount": 20,
      "failedDeviceCount": 17,
      "notInstalledDeviceCount": 23,
      "installedUserCount": 18,
      "failedUserCount": 15,
      "notInstalledUserCount": 21
    },
    "appStoreUrl": "https://example.com/appStoreUrl/"
  }
}
```



