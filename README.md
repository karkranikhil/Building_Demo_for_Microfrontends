## Microfrontend Demo

### 1) Create react app
    npm install -g create-react-app
    create-react-app header
    cd header/
    npm start
    
### 2) To build transpiled and run the server
    npm run build
    npm run transpile
    npm run start:prod
    
### 3) To run the app inside the Docker image
    docker build . -t header
    docker run -t -e PORT=8080 -p 8080:8080 header
    
### 4) to setup heroku
    heroku create microfrontends-component-one
    git push heroku master
    heroku container:login
    heroku container:push web
    heroku open