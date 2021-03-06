---
swagger: "2.0"
x-collection-name: Stack Exchange
x-complete: 1
info:
  title: Stack Exchange
  description: stack-exchange-is-a-network-of-130-qa-communities-including-stack-overflow-
  version: "2.0"
host: api.stackexchange.com
basePath: /2.2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/write-permissions:
    get:
      summary: My Write Permissions
      description: "Returns the write permissions a user has via the api, given an
        access token.\n \nThe Stack Exchange API gives users the ability to create,
        edit, and delete certain types. This method returns whether the passed user
        is capable of performing those actions at all, as well as how many times a
        day they can.\n \nThis method does not consider the user's current quota (ie.
        if they've already exhausted it for today) nor any additional restrictions
        on write access, such as editing deleted comments.\n \nThis method returns
        a list of write_permissions."
      operationId: returns-the-write-permissions-a-user-has-via-the-api-given-an-access-token-the-stack-exchange-api-gi
      x-api-path-slug: mewritepermissions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Write Permissions
  /users/{id}/write-permissions:
    get:
      summary: Get User Write Permissions
      description: "Returns the write permissions a user has via the api.\n \nThe
        Stack Exchange API gives users the ability to create, edit, and delete certain
        types. This method returns whether the passed user is capable of performing
        those actions at all, as well as how many times a day they can.\n \nThis method
        does not consider the user's current quota (ie. if they've already exhausted
        it for today) nor any additional restrictions on write access, such as editing
        deleted comments.\n \nThis method returns a list of write_permissions."
      operationId: returns-the-write-permissions-a-user-has-via-the-api-the-stack-exchange-api-gives-users-the-ability-
      x-api-path-slug: usersidwritepermissions-get
      parameters:
      - in: query
        name: callback
        description: All API responses are JSON, we do support JSONP with the callback
          query parameter
      - in: query
        name: filter
        description: '#DiscussionThe Stack Exchange API allows applications to exclude
          almost every field returned'
      - in: path
        name: id
      - in: query
        name: page
      - in: query
        name: pagesize
      - in: query
        name: site
        description: Each of these methods operates on a single site at a time, identified
          by the site parameter
      responses:
        200:
          description: OK
      tags:
      - Write Permissions
---