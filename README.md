# Case-Study-_-Publicis-Sapient
Case-Study-_-Publicis-Sapient | coding excercise

# problem statmet is attached.
# Design & Implementation approach
1. nature of the application is MVC, (Spring MVC)
   as it needs to cater to different front end clients like web, mobile-app
2. The spring boot web controller will interact with the processing layer
3. depending on the request end point, appropriate DAO layer calls will be made
   can use JDBC-temple here.
3a. every end point will correspond to a serach query, RequestMapping with PathVariable can be used to filter each request.
4. the return type will be marshalled from POJO to JSON/XML 
5. Star schema will be a suitable choice to cater faster lookup
5. cursors and trigger, will be enabled to handle update/insert anomalies from other dimension tables .e.g. seller, distributors etc
