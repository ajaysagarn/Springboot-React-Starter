# Springboot-React-Starter
A Basic started code structure with Spring boot backend and React + Webpack frontend

Quickly set up a Spring boot + React + Redux service using this starter code.

Things you get pre-configured
1. Backed code structure for spring boot application along with Open API Swagger api documentation enabled.
2. Webpack configured to Compile a thymeleaf template used by Spring to serve the Single Page Frontend Application.
3. React+Redux along with the directory structure for reducers, selectors, sagas, and actions.
4. Babel plugins configured via webpack.

# Running this project

1. navigate to ``src/main/scripts/js`` and run ``npm install`` to fetch all the UI dependencies.
2. run ``npm run prod``. This will generate the required thymleaf html file that will be served by Spring boot.
3. Make sure maven is installed as mentioned here https://maven.apache.org/install.html
4. Next navigate to the project root and run ``mvn clean install``
5. This will compile the project and generate a fat jar in the target folder.
6. Navigate to the target folder and run ``java -jar <jarname_here>``
7. This will start the application in the specified port. Opening the browser and navigating to the localhost port will display the UI of the application.


Note: By default all api routes are configured to respond with the webpack compiled html page using thymleaf. To have application API's, make sure to start your api's with the 
prefix 'api', or change the regular expression of the request mapping in the  [Implementation Details](./src/main/java/com/ajsa/template/starter/controller/ui/v1/ApplicationController.java) ApplicationController class.
