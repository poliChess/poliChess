# poliChess
Online Chess platform
* local games, no account required
* Account creation or Google Sign-In
* Player vs player or player vs computer
* Matchmaking
* Rating and stats
* Profile inspection


## Project for learning full stack development
This is the master repository containing all the services and frontend

Backend Features:
* service-oriented architecture
* graphql for main API, websockets for games and REST for intra-service communication
* JWT authentication
* using Redis to cache service calls
* Google Sing-In integration
* fully containerized with Docker

Frontend Features:
* React + Redux and Tailwind for styling
* clean, minimalist and responsive design
* optimised for both desktop and mobile


## Setup
After cloning, run `git submodule init && git submodule update` to pull all submodules

## Building
 Build backend services
`docker-compose -f compose-backend.yml build`

 Build backend services + frontend
`docker-compose -f compose-all.yml build`

## Running
 Start backend 
`docker-compose -f compose-backend.yml up`

 Start backend + frontend
`docker-compose -f compose-all.yml up`
 
By default, the ports are:
 - 3000: graphql API
 - 3001: websockets
 - 3002: frontend app
