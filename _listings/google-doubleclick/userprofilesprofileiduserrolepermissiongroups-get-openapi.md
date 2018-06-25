---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Get User Role Permission Groups
  version: 1.0.0
  description: Gets a list of all supported user role permission groups.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /userprofiles/{profileId}/accountPermissionGroups:
    get:
      summary: Get Account Permission Groups
      description: Retrieves the list of account permission groups.
      operationId: dfareporting.accountPermissionGroups.list
      x-api-path-slug: userprofilesprofileidaccountpermissiongroups-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions Group
  /userprofiles/{profileId}/accountPermissionGroups/{id}:
    get:
      summary: Get Account Permission Group
      description: Gets one account permission group by ID.
      operationId: dfareporting.accountPermissionGroups.get
      x-api-path-slug: userprofilesprofileidaccountpermissiongroupsid-get
      parameters:
      - in: path
        name: id
        description: Account permission group ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions Group
  /userprofiles/{profileId}/accountPermissions:
    get:
      summary: Get Account Permissions
      description: Retrieves the list of account permissions.
      operationId: dfareporting.accountPermissions.list
      x-api-path-slug: userprofilesprofileidaccountpermissions-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions
  /userprofiles/{profileId}/accountPermissions/{id}:
    get:
      summary: Get Account Permissions
      description: Gets one account permission by ID.
      operationId: dfareporting.accountPermissions.get
      x-api-path-slug: userprofilesprofileidaccountpermissionsid-get
      parameters:
      - in: path
        name: id
        description: Account permission ID
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Permissions
  /userprofiles/{profileId}/userRolePermissionGroups:
    get:
      summary: Get User Role Permission Groups
      description: Gets a list of all supported user role permission groups.
      operationId: dfareporting.userRolePermissionGroups.list
      x-api-path-slug: userprofilesprofileiduserrolepermissiongroups-get
      parameters:
      - in: path
        name: profileId
        description: User profile ID associated with this request
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Users
      - Roles
      - Permissions Group
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---