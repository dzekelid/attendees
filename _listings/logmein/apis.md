---
name: LogMeIn
x-slug: logmein
description: LogMeIn, Inc. is a provider of software as a service and cloud-based
  remote connectivity services for collaboration, IT management and customer engagement,
  founded in 2003 and based in Boston, Massachusetts.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
x-kinRank: "7"
x-alexaRank: "7271"
tags: Attendees
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/apis.md
specificationVersion: "0.14"
apis:
- name: GoToAssist Remote Support - Start Attended Session in Browser
  x-api-slug: session-get
  description: "This method allows a partner system to launch an attended support
    session within a browser window. This API does not require authentication, so
    the technician will be prompted to enter their credentials when they run the GoToAssist
    Expert desktop application for the first time. Since the technician is not required
    to navigate to a URL, no API is implemented to create the session. Note: This
    method was formerly named \"Create Attended Session in browser,\" but has been
    renamed.\n\n  Request Parameters                    \n                      \n
    \   field        data type      description    \n    sessionType        string
    \     The type of session to create (only \"SCREEN_SHARING\" can be used at this
    time).    \n    layout*        string      The style of HTML that will be displayed
    when starting the session (e.g., \"iFrame\"). If this parameter is not present,
    then the HTML will fill the entire browser window.    \n    partnerObject*        string
    \     The ID of object in the partner system that this session will be associated
    with.    \n    partnerObjectUrl*        string      The URL that may be used in
    the GoToAssist Expert desktop application if the technician wants to view the
    partner object. Note: The URL can be used in a popup window or iframe that is
    600 pixels wide and 500 pixels wide. For example, a popup window could be created
    with HTML code as follows: Start Remote Support     \n    sessionStatusCallbackUrl*
    \       string      The URL that will receive a POST when the session status changes.
    A POST will also be made to the sessionStatusCallbackUrl when a customer joins
    the session and when the session ends (whether or not a customer joined). The
    contents of the POST will be similar as the GET /v1/sessions/ API. Note: The ID
    of the session is not known until the session is actually started on the endpoint.
    If the URL is not specified or the session is never started (e.g., if the customer
    cancels the installation of the GoToAssist Customer desktop application), then
    the callback will not be made.    \n                      \n* Optional parameters"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/session-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/session-get-openapi.md
- name: GoToAssist Remote Support - Start Attended Session in Browser
  x-api-slug: session-get
  description: "This method allows a partner system to launch an attended support
    session within a browser window. This API does not require authentication, so
    the technician will be prompted to enter their credentials when they run the GoToAssist
    Expert desktop application for the first time. Since the technician is not required
    to navigate to a URL, no API is implemented to create the session. Note: This
    method was formerly named \"Create Attended Session in browser,\" but has been
    renamed.\n\n  Request Parameters                    \n                      \n
    \   field        data type      description    \n    sessionType        string
    \     The type of session to create (only \"SCREEN_SHARING\" can be used at this
    time).    \n    layout*        string      The style of HTML that will be displayed
    when starting the session (e.g., \"iFrame\"). If this parameter is not present,
    then the HTML will fill the entire browser window.    \n    partnerObject*        string
    \     The ID of object in the partner system that this session will be associated
    with.    \n    partnerObjectUrl*        string      The URL that may be used in
    the GoToAssist Expert desktop application if the technician wants to view the
    partner object. Note: The URL can be used in a popup window or iframe that is
    600 pixels wide and 500 pixels wide. For example, a popup window could be created
    with HTML code as follows: Start Remote Support     \n    sessionStatusCallbackUrl*
    \       string      The URL that will receive a POST when the session status changes.
    A POST will also be made to the sessionStatusCallbackUrl when a customer joins
    the session and when the session ends (whether or not a customer joined). The
    contents of the POST will be similar as the GET /v1/sessions/ API. Note: The ID
    of the session is not known until the session is actually started on the endpoint.
    If the URL is not specified or the session is never started (e.g., if the customer
    cancels the installation of the GoToAssist Customer desktop application), then
    the callback will not be made.    \n                      \n* Optional parameters"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/session-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/session-get-openapi.md
- name: GoToAssist Remote Support - Start Attended Session in Browser
  x-api-slug: session-get
  description: "This method allows a partner system to launch an attended support
    session within a browser window. This API does not require authentication, so
    the technician will be prompted to enter their credentials when they run the GoToAssist
    Expert desktop application for the first time. Since the technician is not required
    to navigate to a URL, no API is implemented to create the session. Note: This
    method was formerly named \"Create Attended Session in browser,\" but has been
    renamed.\n\n  Request Parameters                    \n                      \n
    \   field        data type      description    \n    sessionType        string
    \     The type of session to create (only \"SCREEN_SHARING\" can be used at this
    time).    \n    layout*        string      The style of HTML that will be displayed
    when starting the session (e.g., \"iFrame\"). If this parameter is not present,
    then the HTML will fill the entire browser window.    \n    partnerObject*        string
    \     The ID of object in the partner system that this session will be associated
    with.    \n    partnerObjectUrl*        string      The URL that may be used in
    the GoToAssist Expert desktop application if the technician wants to view the
    partner object. Note: The URL can be used in a popup window or iframe that is
    600 pixels wide and 500 pixels wide. For example, a popup window could be created
    with HTML code as follows: Start Remote Support     \n    sessionStatusCallbackUrl*
    \       string      The URL that will receive a POST when the session status changes.
    A POST will also be made to the sessionStatusCallbackUrl when a customer joins
    the session and when the session ends (whether or not a customer joined). The
    contents of the POST will be similar as the GET /v1/sessions/ API. Note: The ID
    of the session is not known until the session is actually started on the endpoint.
    If the URL is not specified or the session is never started (e.g., if the customer
    cancels the installation of the GoToAssist Customer desktop application), then
    the callback will not be made.    \n                      \n* Optional parameters"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2A/rest/v1
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/session-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/session-get-openapi.md
- name: GoToMeeting - Attendees by meeting
  x-api-slug: meetingsmeetinginstancekeyattendees-get
  description: List all attendees for specified meetingId of historical meeting. The
    historical meetings can be fetched using 'Get historical meetings', 'Get historical
    meetings by organizer', and 'Get historical meetings by group'. For users with
    the admin role this call returns attendees for any meeting. For any other user
    the call will return attendees for meetings on which the user is a valid organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/meetingsmeetinginstancekeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/meetingsmeetinginstancekeyattendees-get-openapi.md
- name: GoToMeeting - Attendees by organizer
  x-api-slug: organizersorganizerkeyattendees-get
  description: Lists all attendees for all meetings within a specified date range
    for a specified organizer. This API call is only available to users with the admin
    role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizersorganizerkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizersorganizerkeyattendees-get-openapi.md
- name: GoToMeeting - Attendees by group
  x-api-slug: groupsgroupkeyattendees-get
  description: Returns all attendees for all meetings within specified date range
    held by organizers within the specified group. This API call is only available
    to users with the admin role. This API call can be used only for groups with maximum
    50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2M/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/groupsgroupkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/groupsgroupkeyattendees-get-openapi.md
- name: GoToTraining API - Get Attendance Details
  x-api-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
  description: Get attendance details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-openapi.md
- name: GoToTraining API - Get Attendance Details
  x-api-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
  description: Get attendance details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-openapi.md
- name: GoToTraining API - Get Attendance Details
  x-api-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
  description: Get attendance details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-openapi.md
- name: GoToTraining API - Get Attendance Details
  x-api-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
  description: Get attendance details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2T/rest
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/reportsorganizersorganizerkeysessionssessionkeyattendees-get-openapi.md
- name: GoToWebinar API - Get session attendees
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendees-get
  description: Get session attendees.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendees-get-openapi.md
- name: GoToWebinar API - Get attendees for all webinar sessions
  x-api-slug: organizerkeywebinarswebinarkeyattendees-get
  description: Get attendees for all webinar sessions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeyattendees-get-openapi.md
- name: GoToWebinar API - Get attendee
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Get attendee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
- name: GoToWebinar API - Get attendee questions
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get attendee questions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: GoToWebinar API - Get attendee survey answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Get attendee survey answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
- name: GoToWebinar API - Get attendee poll answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get attendee poll answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: GoToWebinar API - Get attendee
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Get attendee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
- name: GoToWebinar API - Get attendee questions
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get attendee questions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: GoToWebinar API - Get attendee survey answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Get attendee survey answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
- name: GoToWebinar API - Get attendee poll answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get attendee poll answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: GoToWebinar API - Get attendee poll answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get attendee poll answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: GoToWebinar API - Get attendee poll answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get attendee poll answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: GoToWebinar API - Get attendee survey answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Get attendee survey answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
- name: GoToWebinar API - Get attendee survey answers
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Get attendee survey answers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
- name: GoToWebinar API - Get attendee questions
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get attendee questions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: GoToWebinar API - Get attendee questions
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get attendee questions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: GoToWebinar API - Get attendee
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Get attendee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
- name: GoToWebinar API - Get attendee
  x-api-slug: organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Get attendee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28873-www-logmeininc-com.jpg
  humanURL: http://www.LogMeInInc.com
  baseURL: https://api.getgo.com//G2W/rest/organizers
  tags: SaaS, Technology, Enterprise, Voice, Videoconferencing, Audio, Webinars, Relative
    Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/logmein/organizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
x-common:
- type: x-github
  url: https://github.com/logmein
- type: x-openapi
  url: https://www.getpostman.com/collections/94ad52bdc3d954bad52a
- type: x-postman-collection
  url: https://www.getpostman.com/collections/00bf4391e993c3afa7b7
- type: x-postman-collection
  url: https://www.getpostman.com/collections/c35d614484f21e581775
- type: x-postman-collection
  url: https://www.getpostman.com/collections/9c6e067461f45f7faa6b
- type: x-postman-collection
  url: https://drive.google.com/open?id=16WZlBkS1i8cWSfZ3mMKOwlNP-qsE7AWy
- type: x-postman-collection
  url: https://drive.google.com/file/d/1vI11FNCKpv6WJ_70hoqPNMmPAkASiOU_/view?usp=sharing
- type: x-website
  url: http://www.LogMeInInc.com
- type: x-api-gallery
  url: http://loginradius.api.gallery.streamdata.io
- type: x-api-stack
  url: http://logmein.stack.network
- type: x-crunchbase
  url: https://crunchbase.com/organization/logmein
- type: x-developer
  url: https://goto-developer.logmeininc.com/
- type: x-documentation
  url: https://goto-developer.logmeininc.com/apis/apis-overview
- type: x-faq
  url: https://goto-developer.logmeininc.com/faq-page
- type: x-support
  url: https://goto-developer.logmeininc.com/api-support-request-template
- type: x-twitter
  url: https://twitter.com/LogMeIn
- type: x-website
  url: https://www.logmeininc.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---