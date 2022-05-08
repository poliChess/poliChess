## Setup
After cloning, run `git submodule init && git submodule update` to pull all submodules

## Building
Build backend services
`docker-compose -f compose-backend.yml build`

## Running
Start backend (API available on port 3000) 
`docker-compose -f compose-backend.yml up`
