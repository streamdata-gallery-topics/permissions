---
swagger: "2.0"
x-collection-name: Apigee
x-complete: 0
info:
  title: Apigee Edge Get Users User Email Permissions Get
  description: Checks user has particular permission for a resource at global level
  version: 1.0.0
host: api.enterprise.apigee.com
basePath: /v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org_name}/userroles/{role_name}/permissions:
    get:
      summary: Get Organizations Name Userroles Role Name Permissions
      description: Gets a list of permissions associated with the specified resource
        for a single resource.
      operationId: getOrganizationsOrgNameUserrolesRoleNamePermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissions-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
    post:
      summary: Post Organizations Name Userroles Role Name Permissions
      description: Associates permissions for a resource with a user role.
      operationId: postOrganizationsOrgNameUserrolesRoleNamePermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissions-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
  /organizations/{org_name}/userroles/{role_name}/permissions/get:
    get:
      summary: Get Organizations Name Userroles Role Name Permissions Get
      description: Checks the particular userrole permission of a resource at organization
        level.
      operationId: getOrganizationsOrgNameUserrolesRoleNamePermissionsGet
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissionsget-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
      - Get
    delete:
      summary: Delete Organizations Name Userroles Role Name Permissions Get
      description: Deletes particular userrole permission at organization level.
      operationId: deleteOrganizationsOrgNameUserrolesRoleNamePermissionsGet
      x-api-path-slug: organizationsorg-nameuserrolesrole-namepermissionsget-delete
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Permissions
      - Get
  /organizations/{org_name}/userroles/{role_name}/resourcepermissions:
    post:
      summary: Post Organizations Name Userroles Role Name Resourcepermissions
      description: Adds multiple resource permissions for resource at organization
        level.
      operationId: postOrganizationsOrgNameUserrolesRoleNameResourcepermissions
      x-api-path-slug: organizationsorg-nameuserrolesrole-nameresourcepermissions-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: org_name
        description: Mention the organization name
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Userroles
      - Role
      - Resourcepermissions
  /userroles/{role_name}/permissions:
    get:
      summary: Get Userroles Role Name Permissions
      description: Gets permission for a specific resource at global level.
      operationId: getUserrolesRoleNamePermissions
      x-api-path-slug: userrolesrole-namepermissions-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify Content Type
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Permissions
    post:
      summary: Post Userroles Role Name Permissions
      description: Adds permissions for resource at global level.
      operationId: postUserrolesRoleNamePermissions
      x-api-path-slug: userrolesrole-namepermissions-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the content type
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Permissions
  /userroles/{role_name}/permissions/get:
    get:
      summary: Get Userroles Role Name Permissions Get
      description: Checks particular userrole permission for a resource at global
        level.
      operationId: getUserrolesRoleNamePermissionsGet
      x-api-path-slug: userrolesrole-namepermissionsget-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Permissions
      - Get
    delete:
      summary: Delete Userroles Role Name Permissions Get
      description: Deletes particular userrole permission for a resource at global
        level
      operationId: deleteUserrolesRoleNamePermissionsGet
      x-api-path-slug: userrolesrole-namepermissionsget-delete
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Permissions
      - Get
  /userroles/{role_name}/resourcepermissions:
    post:
      summary: Post Userroles Role Name Resourcepermissions
      description: Adds multiple resource permissions for resource at global level.
      operationId: postUserrolesRoleNameResourcepermissions
      x-api-path-slug: userrolesrole-nameresourcepermissions-post
      parameters:
      - in: query
        name: Content-Type
        description: Specify the Content Type
      - in: path
        name: role_name
        description: Mention the role name
      responses:
        200:
          description: OK
      tags:
      - Userroles
      - Role
      - Resourcepermissions
  /users/{user_name}/permissions:
    get:
      summary: Get Users User Name Permissions
      description: Gets permissions for a user at global level
      operationId: getUsersUserNamePermissions
      x-api-path-slug: usersuser-namepermissions-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource path
      - in: path
        name: user_name
        description: Mention the user name
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Permissions
  /users/{user_email}permissions/get:
    get:
      summary: Get Users User Email Permissions Get
      description: Checks user has particular permission for a resource at global
        level
      operationId: getUsersUserEmailPermissionsGet
      x-api-path-slug: usersuser-emailpermissionsget-get
      parameters:
      - in: query
        name: Content-Type
        description: Specify content type
      - in: query
        name: path
        description: Specify the resource path
      - in: query
        name: userEmail
        description: Mention the user name
      responses:
        200:
          description: OK
      tags:
      - Users
      - User
      - Emailpermissions
      - Get
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