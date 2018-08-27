---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Attendees
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: Go To Meeting - Get attendees by group
  x-api-slug: groupsgroupkeyattendees-get
  description: Returns all attendees for all meetings within specified date range
    held by organizers within the specified group. This API call is only available
    to users with the admin role. This API call can be used only for groups with maximum
    50 organizers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/groupsgroupkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/groupsgroupkeyattendees-get-openapi.md
- name: Go To Meeting - Get attendees by meeting
  x-api-slug: meetingsmeetingidattendees-get
  description: List all attendees for specified meetingId of historical meeting. The
    historical meetings can be fetched using 'Get historical meetings', 'Get historical
    meetings by organizer', and 'Get historical meetings by group'. For users with
    the admin role this call returns attendees for any meeting. For any other user
    the call will return attendees for meetings on which the user is a valid organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/meetingsmeetingidattendees-get-openapi.md
- name: Go To Meeting - Get attendees by organizer
  x-api-slug: organizersorganizerkeyattendees-get
  description: Lists all attendees for all meetings within a specified date range
    for a specified organizer. This API call is only available to users with the admin
    role.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeyattendees-get-openapi.md
- name: Go To Training - Get Attendance Details
  x-api-slug: reportsorganizersorganizerkeysessionssessionkeyattendees-get
  description: This call retrieves a list of registrants from a specific completed
    training session. The response includes the registrants' email addresses, and
    if they attended, it includes the duration of each period of their attendance
    in minutes, and the times at which they joined and left. If a registrant does
    not attend, they appear at the bottom of the listing with timeInSession = 0.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2T/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/reportsorganizersorganizerkeysessionssessionkeyattendees-get-openapi.md
- name: Go To Webinar - Get attendees for all webinar sessions
  x-api-slug: organizersorganizerkeywebinarswebinarkeyattendees-get
  description: Returns all attendees for all sessions of the specified webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeyattendees-get-openapi.md
- name: Go To Webinar - Get session attendees
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendees-get
  description: Retrieve details for all attendees of a specific webinar session. For
    technical reasons, this call cannot be executed from this documentation. Please
    use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendees-get-openapi.md
- name: Go To Webinar - Get attendee
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get
  description: Retrieve registration details for a particular attendee of a specific
    webinar session. For technical reasons, this call cannot be executed from this
    documentation. Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkey-get-openapi.md
- name: Go To Webinar - Get attendee poll answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get
  description: Get poll answers from a particular attendee of a specific webinar session.
    For technical reasons, this call cannot be executed from this documentation. Please
    use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeypolls-get-openapi.md
- name: Go To Webinar - Get attendee questions
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get
  description: Get questions asked by an attendee during a webinar session. For technical
    reasons, this call cannot be executed from this documentation. Please use the
    curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeyquestions-get-openapi.md
- name: Go To Webinar - Get attendee survey answers
  x-api-slug: organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get
  description: Retrieve survey answers from a particular attendee during a webinar
    session. For technical reasons, this call cannot be executed from this documentation.
    Please use the curl command to execute it.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Office, Meetings, Collaboration, Video Conferencing, Video Conferencing, SaaS,
    Technology, Enterprise, API Provider, Meetings, Profiles, Conferences, Relative
    Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/attendees/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeysessionssessionkeyattendeesregistrantkeysurveys-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.url.shortener.api.gallery.streamdata.io
- type: x-api-stack
  url: http://gotomeeting.stack.network
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---