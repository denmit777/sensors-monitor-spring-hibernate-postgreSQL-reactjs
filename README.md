1.Name of project: sensors-monitor-spring-hibernate-postgresql-reactjs

2.Launch of project: 
backend part: mvn run clean tomcat7:run
node modules: sensors-monitor-spring-hibernate-h2-reactjs\src\frontend-react\java-learn-app-main>npm install
frontend part: sensors-monitor-spring-hibernate-h2-reactjs\src\frontend-react\java-learn-app-main>npm start

3.Ports of the project:
backend: http://localhost:8081
frontend: http://localhost:3000

4.Start page: http://localhost:3000

5.Logins/passwords/role of users:

Denis/1234/ROLE_ADMINISTRATOR,
Peter/4321/ROLE_VIEWER,
Asya/5678/ROLE_ADMINISTRATOR,
Jimmy/P@ssword1/ROLE_VIEWER

6.Database scripts: resources/db/data.sql

7.Database properties: resources/db/hibernate.properties

8.Security properties: resources/security/security.properties

9.Rest controllers:

UserController:
registerUser(POST): http://localhost:8081 + body;
authenticationUser(POST): http://localhost:8081/auth + body

SensorController:
save(POST): http://localhost:8081/sensors + body;
getAll(GET): http://localhost:8081/sensors + parameters
getTotalAmount(GET): http://localhost:8081/sensors/total
getById(GET): http://localhost:8081/sensors/{id};
update(PUT): http://localhost:8081/sensors/{id} + body
delete(DELETE): http://localhost:8081/sensors/{id};
