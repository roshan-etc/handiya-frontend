#Hadiya Products Admin Panel

Environment variables
Update the following line in src/environments/environment.prod.ts

apiGatewayURL = 'http://<ALB_HOSTNAME>' 

HOSTNAME will be your backend Alb dns.

NOTE: DO NOT ADD TRAILING SLASH '/' AT THE END OF THE ABOVE ENDPOINT


Update the file location src/app/app.component.ts 

replace "http://localhost:3000" with 'http://<ALB_HOSTNAME>' 

ALB HOSTNAME will be your backend Alb dns.
NOTE: DO NOT ADD TRAILING SLASH '/' AT THE END OF THE ABOVE ENDPOINT


Development server
Run ng serve for a dev server. Navigate to http://localhost:4200/. The application will automatically reload if you change any of the source files.



Build
Run ng build to build the project. The build artifacts will be stored in the dist/ directory.
