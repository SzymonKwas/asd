##### **Overview of the issue**
I generated a microservice app with :

UAA : uaa
Gateway : gateway
I'm trying to reset password for default user using "Did you forget your password?". Route guard refusing navigation to /reset/request and angular app gets 401 http://localhost/uaa/api/account.

Request:
GET /uaa/api/account HTTP/1.1
Host: localhost:9000
Connection: keep-alive
Accept: application/json, text/plain, */*
User-Agent: Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/64.0.3282.167 Safari/537.36
Referer: http://localhost:9000/
Accept-Encoding: gzip, deflate, br
Accept-Language: pl-PL,pl;q=0.9,en-US;q=0.8,en;q=0.7
Cookie: Idea-4dd094b3=644555e4-12fb-4a76-94d2-9efa5f0a5304; BAMBOO-BUILD-FILTER=ALL_BUILDS; BAMBOO-MAX-DISPLAY-LINES=25; AJS.conglomerate.cookie="|config.sidebar.planNavigator.expanded=true"; bamboo.dash.display.toggles=buildQueueActions-actions-queueControl; _ga=GA1.1.91623415.1507799754; __utma=111872281.91623415.1507799754.1509697702.1510041407.10; __utmz=111872281.1507810479.1.1.utmcsr=(direct)|utmccn=(direct)|utmcmd=(none); iconSize=24x24; XSRF-TOKEN=7c38fb86-e265-45eb-a79a-707a916d7b8f; io=q-mEU5hI20kR3sEJAAAB

Response:
HTTP/1.1 401 Unauthorized
x-powered-by: Express
expires: 0
connection: close
cache-control: no-cache, no-store, max-age=0, must-revalidate
x-xss-protection: 1; mode=block
x-content-type-options: nosniff
pragma: no-cache
content-type: application/json;charset=UTF-8
date: Fri, 16 Feb 2018 09:37:22 GMT
transfer-encoding: chunked

##### **Motivation for or Use Case**

I didn't modified the generated code. User should be able to

##### **Reproduce the error**

<!-- For bug reports, an unambiguous set of steps to reproduce the error -->

##### **Related issues**

<!-- Has a similar issue been reported before? Please search both closed & open issues -->

##### **Suggest a Fix**

<!-- For bug reports, if you can't fix the bug yourself, perhaps you can point to what might be
  causing the problem (line of code or commit) -->

##### **JHipster Version(s)**

jhipsterVersion: 4.14.0

##### **JHipster configuration**

<!--
To provide all information we need, you should run `jhipster info` in the project root folder, and
copy/paste the result here.
The `.yo-rc.json` file generated in the root folder is mandatory for bug reports. This will help us to replicate the scenario.
You should remove any sensitive information like the rememberMe key or the jwtSecretKey key.
-->

##### **Entity configuration(s) `entityName.json` files generated in the `.jhipster` directory**

<!--
If the error is during an entity creation or associated with a specific entity.
If you are using JDL, please share that configuration as well.
-->

##### **Browsers and Operating System**

<!-- What OS are you on? is this a problem with all browsers or only IE8? -->

- [ ] Checking this box is mandatory (this is just to show you read everything)

<!-- Love JHipster? Please consider supporting our collective:
👉  https://opencollective.com/generator-jhipster/donate -->
