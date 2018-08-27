---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 0
info:
  title: Go To Webinar Get session attendees
  description: Retrieve details for all attendees of a specific webinar session. For
    technical reasons, this call cannot be executed from this documentation. Please
    use the curl command to execute it.
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2W/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{groupKey}/attendees:
    get:
      summary: Get attendees by group
      description: Returns all attendees for all meetings within specified date range
        held by organizers within the specified group. This API call is only available
        to users with the admin role. This API call can be used only for groups with
        maximum 50 organizers.
      operationId: returns-all-attendees-for-all-meetings-within-specified-date-range-held-by-organizers-within-the-spe
      x-api-path-slug: groupsgroupkeyattendees-get
      parameters:
      - in: query
        name: endDate
        description: End of date range, in ISO8601 UTC format, e
      - in: query
        name: No Name
      - in: query
        name: startDate
        description: Start of date range, in ISO8601 UTC format, e
      responses:
        200:
          description: OK
      tags:
      - Groups
      - GroupKey
      - Attendees
  /meetings/{meetingId}/attendees:
    get:
      summary: Get attendees by meeting
      description: List all attendees for specified meetingId of historical meeting.
        The historical meetings can be fetched using 'Get historical meetings', 'Get
        historical meetings by organizer', and 'Get historical meetings by group'.
        For users with the admin role this call returns attendees for any meeting.
        For any other user the call will return attendees for meetings on which the
        user is a valid organizer.
      operationId: list-all-attendees-for-specified-meetingid-of-historical-meeting--the-historical-meetings-can-be-fet
      x-api-path-slug: meetingsmeetingidattendees-get
      parameters:
      - in: path
        name: meetingId
        description: The meeting ID
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Meetings
      - MeetingId
      - Attendees
  /organizers/{organizerKey}/attendees:
    get:
      summary: Get attendees by organizer
      description: Lists all attendees for all meetings within a specified date range
        for a specified organizer. This API call is only available to users with the
        admin role.
      operationId: lists-all-attendees-for-all-meetings-within-a-specified-date-range-for-a-specified-organizer--this-a
      x-api-path-slug: organizersorganizerkeyattendees-get
      parameters:
      - in: query
        name: endDate
        description: A required end of date range in ISO8601 UTC format, e
      - in: query
        name: No Name
      - in: query
        name: startDate
        description: A required start of date range in ISO8601 UTC format, e
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Attendees
  /reports/organizers/{organizerKey}/sessions/{sessionKey}/attendees:
    get:
      summary: Get Attendance Details
      description: This call retrieves a list of registrants from a specific completed
        training session. The response includes the registrants' email addresses,
        and if they attended, it includes the duration of each period of their attendance
        in minutes, and the times at which they joined and left. If a registrant does
        not attend, they appear at the bottom of the listing with timeInSession =
        0.
      operationId: getAttendanceDetails
      x-api-path-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: sessionKey
        description: The key of the training session
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Organizers
      - OrganizerKey
      - Sessions
      - SessionKey
      - Attendees
  /organizers/{organizerKey}/webinars/{webinarKey}/attendees:
    get:
      summary: Get attendees for all webinar sessions
      description: Returns all attendees for all sessions of the specified webinar.
      operationId: getAttendeesForAllWebinarSessions
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeyattendees-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Attendees
  /organizers/{organizerKey}/webinars/{webinarKey}/sessions/{sessionKey}/attendees:
    get:
      summary: Get session attendees
      description: Retrieve details for all attendees of a specific webinar session.
        For technical reasons, this call cannot be executed from this documentation.
        Please use the curl command to execute it.
      operationId: getAttendees
      x-api-path-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendees-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - Webinars
      - WebinarKey
      - Sessions
      - SessionKey
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