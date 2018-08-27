---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Attendance Taking
  description: Takes member attendance for an event. Limited for use by administrative
    members.
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /:urlname/events/:id/attendance:
    get:
      summary: Attendance
      description: Lists attendance records for Meetup events. Limited for use by
        administrative members.
      operationId: events
      x-api-path-slug: urlnameeventsidattendance-get
      parameters:
      - in: query
        name: filter
        description: A named filter to apply to the attendance list
        type: string
      - in: query
        name: member
        description: Raw text used to search for member by name
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Attendance
    post:
      summary: Attendance Taking
      description: Takes member attendance for an event. Limited for use by administrative
        members.
      operationId: events
      x-api-path-slug: urlnameeventsidattendance-post
      parameters:
      - in: query
        name: guests
        description: The number of guests accompanying member
        type: string
      - in: query
        name: headcount
        description: Sets the overall headcount for the event
        type: string
      - in: query
        name: member
        description: A comma-delimited list of valid ids associated with members RSVPd
          to the event
        type: string
      - in: query
        name: status
        description: An attendance status for the provided members
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Attendance
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