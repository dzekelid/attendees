---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Update Attendance Status
  description: Update Attendance Status
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/events/{event-id}/registrants/{registrant-id}/attendancestatus:
    get:
      summary: Get Attendance Status
      description: Get Attendance Status
      operationId: get-attendance-status
      x-api-path-slug: usernameeventseventidregistrantsregistrantidattendancestatus-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Attendance
      - Status
    put:
      summary: Update Attendance Status
      description: Update Attendance Status
      operationId: update-attendance-status
      x-api-path-slug: usernameeventseventidregistrantsregistrantidattendancestatus-put
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Attendance
      - Status
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