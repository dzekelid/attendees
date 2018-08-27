---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Reports Attendees
  description: Returns a response of the aggregate attendees data.
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events/{id}/attendees/:attendee_id/:
    get:
      summary: Get Events Attendees Attendee
      description: Returns a single attendee by ID, as the key attendee.
      operationId: getEventsAttendeesAttendee
      x-api-path-slug: eventsidattendeesattendee-id-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Attendees
      - :attendee
  /events/{id}/teams/{id}/attendees/:
    get:
      summary: Get Events Teams Attendees
      description: Returns attendee for a single attendee-team.
      operationId: getEventsTeamsAttendees
      x-api-path-slug: eventsidteamsidattendees-get
      responses:
        200:
          description: OK
      tags:
      - Events
      - Teams
      - Attendees
  /reports/attendees/:
    get:
      summary: Get Reports Attendees
      description: Returns a response of the aggregate attendees data.
      operationId: getReportsAttendees
      x-api-path-slug: reportsattendees-get
      parameters:
      - in: query
        name: date_facet
        description: Optional date aggregation level to return data for
        type: query
      - in: query
        name: end_date
        description: Optional end date to query
        type: query
      - in: query
        name: event_ids
        description: List of public event IDs to report on
        type: query
      - in: query
        name: event_status
        description: 'Event status to filter down results by (Valid choices are: all,
          live, or ended)'
        type: query
      - in: query
        name: filter_by
        description: 'Optional filters for sales/attendees data formatted as: {&#8220;ticket_ids&#8221;:
          [1234, 5678], &#8220;currencies&#8221;: [&#8220;USD&#8221;],'
        type: query
      - in: query
        name: group_by
        description: 'Optional field to group data on (Valid choices are: payment_method,
          payment_method_application, ticket, ticket_application, currency, event_currency,
          reserved_section, event, event_ticket, event_application, country, city,
          state, source, zone, location, access_level, device_name, sales_channel_lvl_1,
          sales_channel_lvl_2, or sales_channel_lvl_3)'
        type: query
      - in: query
        name: period
        description: Time period to provide aggregation for in units of the selected
          date_facet
        type: query
      - in: query
        name: start_date
        description: Optional start date to query
        type: query
      - in: query
        name: timezone
        description: Optional timezone
        type: query
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Attendees
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