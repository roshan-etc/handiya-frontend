#Hadiya Products Angular Frontend

Update the following line in src/environments/environment.prod.ts with
apiGatewayURL = 'http://<ALB_HOSTNAME>' 

#HOSTNAME will be your backend Alb DNS.
NOTE: DO NOT ADD TRAILING SLASH '/' AT THE END OF THE ABOVE ENDPOINT

Update the file location src/app/app.component.ts by replacing "http://localhost:3000" with 'http://<ALB_HOSTNAME>' 

#HOSTNAME will be your backend Alb DNS.
NOTE: DO NOT ADD TRAILING SLASH '/' AT THE END OF THE ABOVE ENDPOINT

# To install packages
npm install 
# To build the application
ng build or npm run build
# The build artifacts will be stored in the dist/ directory.
# This dist/ directory needs to be copied to s3 bucket where you enabled static website hosting.
# Optional, If you want to run locally to check how it's behaving
Run ng serve for a dev server. Navigate to http://localhost:4200/. The application will automatically reload if you change any of the source files.
