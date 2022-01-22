# Springboot-React-Starter
A Basic started code structure with Spring boot backend and React + Webpack frontend

Quickly set up a Spring boot + React + Redux service using this starter code.

Things you get pre-configured
1. Backed code structure for spring boot application along with Open API Swagger api documentation enabled.
2. Webpack configured to Compile a thymeleaf template used by Spring to serve the Single Page Frontend Application.
3. React+Redux along with the directory structure for reducers, selectors, sagas, and actions.
4. Babel plugins configured via webpack.

# Running this project

1. From the project directory





Note: By default all api routes are configured to respond with the webpack compiled html page using thymleaf. To have application API's, make sure to start your api's with the 
prefix 'api', or change the regular expression of the request mapping in the  [Implementation Details](./src/main/java/com/ajsa/template/starter/controller/ui/v1/ApplicationController.java) ApplicationController class.
