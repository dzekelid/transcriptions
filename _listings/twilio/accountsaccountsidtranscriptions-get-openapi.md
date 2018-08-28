---
swagger: "2.0"
x-collection-name: Twilio
x-complete: 0
info:
  title: Twilio Get Transcriptions
  description: Returns a set of Transcription resource representations that includes
    pagingninformation.n
  termsOfService: https://www.twilio.com/legal/tos
  version: v1
host: api.twilio.com
basePath: /2010-04-01/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Accounts/{AccountSid}/Transcriptions/{TranscriptionSid}.{format}:
    get:
      summary: GetTranscription
      description: GetTranscription
      operationId: gettranscription
      x-api-path-slug: accountsaccountsidtranscriptionstranscriptionsid-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
      - in: path
        name: TranscriptionSid
        description: A 34 character string that uniquely identifies the transcription
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
  /Accounts/{AccountSid}/Transcriptions.{format}:
    get:
      summary: GetTranscriptionList
      description: GetTranscriptionList
      operationId: gettranscriptionlist
      x-api-path-slug: accountsaccountsidtranscriptions-format-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      - in: path
        name: format
        description: By default, Twilios REST API returns XML
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
  /Accounts/{AccountSid}/Transcriptions:
    get:
      summary: Get Transcriptions
      description: Returns a set of Transcription resource representations that includes
        pagingninformation.n
      operationId: returns-a-set-of-transcription-resource-representations-that-includes-paginginformation
      x-api-path-slug: accountsaccountsidtranscriptions-get
      parameters:
      - in: path
        name: AccountSid
        description: The ID for the Twilio account
      responses:
        200:
          description: OK
      tags:
      - Transcriptions
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---