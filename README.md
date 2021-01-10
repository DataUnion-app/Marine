# Marine
The ecosystem/repository where all our sea creatures/components come together to form an interface where the contributors can provide input to become a part of our data union.

# Setup

## Inital setup
1. Clone the repository
2. `git submodule init`
3. `git submodule update`
4. python -m pip install --user virtualenv
5. python -m virtualenv env
6. source env/bin/activate
7. Create `properties.ini` in `Crab/` folder and add database credentials.
8. Create `.env` file from `.sample_env` and add database credentials.
9. `cp ./config/Dockerfile_Mantis ./Mantis/Dockerfile`

## Start environment

1. Dev: `docker-compose  -f docker-compose.dev.yml --env-file .env up -d`
2. Test: `docker-compose  -f docker-compose.test.yml --env-file .env up -d`

## Stop environment

1. Dev: `docker-compose -f docker-compose.dev.yml down`
2. Test: `docker-compose -f docker-compose.test.yml down`

