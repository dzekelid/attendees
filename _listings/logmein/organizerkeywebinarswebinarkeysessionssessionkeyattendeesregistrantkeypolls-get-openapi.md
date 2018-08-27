---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToWebinar Get attendee poll answers
  description: Get attendee poll answers.
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
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
  /groups/{groupkey}/attendees:
    get:
      summary: Attendees by group
      description: Returns all attendees for all meetings within specified date range
        held by organizers within the specified group. This API call is only available
        to users with the admin role. This API call can be used only for groups with
        maximum 50 organizers.
      operationId: GroupsAttendeesByGroupkeyGet
      x-api-path-slug: groupsgroupkeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: groupkey
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Attendees
      - By
      - Group
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
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees:
    get:
      summary: Get session attendees
      description: Get session attendees.
      operationId: WebinarsSessionsSessionKeyAttendeesByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Session
      - Attendees
  /{organizerKey}/webinars/{webinarKey}/attendees:
    get:
      summary: Get attendees for all webinar sessions
      description: Get attendees for all webinar sessions.
      operationId: WebinarsAttendeesByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeyattendees-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendees
      - Webinar
      - Sessions
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}:
    get:
      summary: Get attendee
      description: Get attendee.
      operationId: WebinarsSessionsSessionKeyAttendeesRegistrantKeyByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendee
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/questions:
    get:
      summary: Get attendee questions
      description: Get attendee questions.
      operationId: WebinarsSessionsSessionKeyAttendeesRegistrantKeyQuestionsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendee
      - Questions
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/surveys:
    get:
      summary: Get attendee survey answers
      description: Get attendee survey answers.
      operationId: WebinarsSessionsSessionKeyAttendeesRegistrantKeySurveysByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendee
      - Survey
      - Answers
  /{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees/{registrantKey}/polls:
    get:
      summary: Get attendee poll answers
      description: Get attendee poll answers.
      operationId: WebinarsSessionsSessionKeyAttendeesRegistrantKeyPollsByOrganizerKeyAndWebinarKeyGet
      x-api-path-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: organizerKey
      - in: path
        name: registrantKey
      - in: path
        name: sessionKey
      - in: path
        name: webinarKey
      responses:
        200:
          description: OK
      tags:
      - Attendee
      - Poll
      - Answers
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