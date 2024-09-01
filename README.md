# react-go-tutorial

A simple CRUD todo list app using
- Go backend
- React frontend
  - [ChakraUI](https://v2.chakra-ui.com/) component library
  - [TanStack Query](https://tanstack.com/query/latest) 
- MongoDB database

Tutorial author: <https://github.com/burakorkmez/react-go-tutorial>

## setup

1. setup Go

    ```bash
    go install github.com/air-verse/air@latest
    go get github.com/gofiber/fiber/v2
    go get github.com/joho/godotenv
    go get go.mongodb.org/mongo-driver/mongo

2. setup React

    ```bash
    cd ./client
    npm install
    ```

## usage

1. create an `.env` file

    ```env
    PORT=<port>
    MONGODB_URI=mongodb+srv://<username>:<password>@<cluster_name>.2feve.mongodb.net/<database_name>?retryWrites=true&w=majority&appName=<cluster_name>
    ```

2. start the Go app using `air` (live reload for Go apps)

    ```bash
    ❯ air
    
      __    _   ___  
     / /\  | | | |_) 
    /_/--\ |_| |_| \_ v1.52.3, built with Go go1.23.0
    
    watching .
    !exclude tmp
    building...
    running...
    hello world
    Connected to MongoDB Atlas
    
    ┌───────────────────────────────────────────────────┐ 
    │                   Fiber v2.52.5                   │ 
    │               http://127.0.0.1:4000               │ 
    │       (bound on host 0.0.0.0 and port 4000)       │ 
    │                                                   │ 
    │ Handlers ............. 5  Processes ........... 1 │ 
    │ Prefork ....... Disabled  PID ............. 44620 │ 
    └───────────────────────────────────────────────────┘ 
    ```

3. start the React app

    ```bash
    cd ./client
    npm run dev
    ```

## database

Hosted in a free MongoDB Atlas cluster: <https://cloud.mongodb.com/v2/66d3cccbe605cd7628bda426#/clusters/detail/Cluster0>
