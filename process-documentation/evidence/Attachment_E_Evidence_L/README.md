![alt tag](https://github.com/AccentureFed/18FRFQ-Response/blob/master/process-documentation/agile-process-photos/response-images/proposal-header.png?raw=true)

[Back to Attachment E_Evidence Criteria](https://github.com/AccentureFed/18FRFQ-Response/blob/master/process-documentation/evidence/README.md)

|#|criteria|evidence|
|-------|---------------|------------------|
|l|set up or used a continuous integration system to automate the running of tests and continuously deployed their code to their IaaS or PaaS provider |Jenkins was used as our continuous integration system. It was configured to test for code changes every 15 minutes in development. For production, a manual Jenkins build was required triggering the running of unit tests and a manual deployment to the production server. After a new change is pushed, Jenkins checks the "test" folder and runs all Unit tests for the project.  Approximately 30 unit tests are run. If all the tests pass, Jenkins packages the repository into a Web Application Archive (WAR file).  From there, the war file is deployed to our development server.  There have been over 125 builds to development, and over 35 builds to the production server.  If the tests failed for both production and development developers were instantly notified of build failure. For the development and production a separate Amazon Web Service EC2 instance was provisioned. Jenkins was continuously deploying on code commit. The team utilized the GitHub integration. |


[Back to Attachment E_Evidence Criteria](https://github.com/AccentureFed/18FRFQ-Response/blob/master/process-documentation/evidence/README.md)

