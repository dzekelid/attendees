---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToTraining Get Attendance Details
  description: Get attendance details.
  version: 1.0.0
host: api.getgo.com
basePath: /G2T/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/organizers/{organizerKey}/sessions/{sessionKey}/attendees:
    get:
      summary: Get Attendance Details
      description: Get attendance details.
      operationId: ReportsOrganizersSessionsAttendeesByOrganizerKeyAndSessionKeyGet
      x-api-path-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: sessionKey
      responses:
        200:
          description: OK
      tags:
      - Attendance
      - Details
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