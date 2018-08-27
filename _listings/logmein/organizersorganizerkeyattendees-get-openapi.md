---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToMeeting Attendees by organizer
  description: Lists all attendees for all meetings within a specified date range
    for a specified organizer. This API call is only available to users with the admin
    role.
  version: 1.0.0
host: api.getgo.com
basePath: /G2M/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /session:
    get:
      summary: Start Attended Session in Browser
      description: "This method allows a partner system to launch an attended support
        session within a browser window. This API does not require authentication,
        so the technician will be prompted to enter their credentials when they run
        the GoToAssist Expert desktop application for the first time. Since the technician
        is not required to navigate to a URL, no API is implemented to create the
        session. Note: This method was formerly named \"Create Attended Session in
        browser,\" but has been renamed.\n\n  Request Parameters                    \n
        \                     \n    field        data type      description    \n
        \   sessionType        string      The type of session to create (only \"SCREEN_SHARING\"
        can be used at this time).    \n    layout*        string      The style of
        HTML that will be displayed when starting the session (e.g., \"iFrame\").
        If this parameter is not present, then the HTML will fill the entire browser
        window.    \n    partnerObject*        string      The ID of object in the
        partner system that this session will be associated with.    \n    partnerObjectUrl*
        \       string      The URL that may be used in the GoToAssist Expert desktop
        application if the technician wants to view the partner object. Note: The
        URL can be used in a popup window or iframe that is 600 pixels wide and 500
        pixels wide. For example, a popup window could be created with HTML code as
        follows: Start Remote Support     \n    sessionStatusCallbackUrl*        string
        \     The URL that will receive a POST when the session status changes. A
        POST will also be made to the sessionStatusCallbackUrl when a customer joins
        the session and when the session ends (whether or not a customer joined).
        The contents of the POST will be similar as the GET /v1/sessions/ API. Note:
        The ID of the session is not known until the session is actually started on
        the endpoint. If the URL is not specified or the session is never started
        (e.g., if the customer cancels the installation of the GoToAssist Customer
        desktop application), then the callback will not be made.    \n                      \n*
        Optional parameters"
      operationId: SessionGet
      x-api-path-slug: session-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: sessionType
      responses:
        200:
          description: OK
      tags:
      - Start
      - Attended
      - Session
      - In
      - Browser
  /meetings/{meetingInstanceKey}/attendees:
    get:
      summary: Attendees by meeting
      description: List all attendees for specified meetingId of historical meeting.
        The historical meetings can be fetched using 'Get historical meetings', 'Get
        historical meetings by organizer', and 'Get historical meetings by group'.
        For users with the admin role this call returns attendees for any meeting.
        For any other user the call will return attendees for meetings on which the
        user is a valid organizer.
      operationId: MeetingsAttendeesByMeetingInstanceKeyGet
      x-api-path-slug: meetingsmeetinginstancekeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: meetingInstanceKey
      responses:
        200:
          description: OK
      tags:
      - Attendees
      - By
      - Meeting
  /organizers/{organizerKey}/attendees:
    get:
      summary: Attendees by organizer
      description: Lists all attendees for all meetings within a specified date range
        for a specified organizer. This API call is only available to users with the
        admin role.
      operationId: OrganizersAttendeesByOrganizerKeyGet
      x-api-path-slug: organizersorganizerkeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: organizerKey
      - in: query
        name: starttime
      responses:
        200:
          description: OK
      tags:
      - Attendees
      - By
      - Organizer
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