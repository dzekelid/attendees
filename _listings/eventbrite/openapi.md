---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 1
info:
  title: Eventbrite
  description: create-manage--promote-events--add-eventmanagement-features-to-your-site--show-the-world-what-exciting-things-are-happening-around-them-
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
  /users/{id}/owned_event_attendees/:
    get:
      summary: Get Users Owned Event Attendees
      description: |-
        Returns a paginated response of attendees,
        under the key attendees, of attendees visiting any of the events the user owns
        (events that would be returned from /users/:id/owned_events/)
      operationId: getUsersOwnedEventAttendees
      x-api-path-slug: usersidowned-event-attendees-get
      parameters:
      - in: query
        name: changed_since
        description: Only return resource changed on or after the time given
        type: query
      - in: query
        name: status
        description: Limits results to either confirmed attendees or cancelled/refunded/etc
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Owned
      - Event
      - Attendees
  /event_list_attendees:
    get:
      summary: Get Event List Attendees
      description: This method returns a list of attendees for a given event. If no
        authentication is passed, only publicly available attendee records will be
        returned.
      operationId: Get_event_list_attendees_
      x-api-path-slug: event-list-attendees-get
      parameters:
      - in: query
        name: count
        description: Limit the number of attendees returned
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: do_not_display
        description: Comma separated list without spaces that leaves out certain data
          returned
      - in: query
        name: event_id
        description: The ID of the event
      - in: query
        name: page
        description: Allows for paging through the results of a query
      - in: query
        name: show_full_barcodes
        description: If set to ???true???, it will return all barcodes associates
          with the attendee, plus the barcode status, device used, attendee_id, and
          barcode number
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
      - Attendees
---