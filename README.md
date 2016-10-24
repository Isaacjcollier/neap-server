# NEAP Server-Side

Deployed Website : https://rocky-journey-79261.herokuapp.com/

This is the server-side of our NEAP App. It's a RESTful API. It serves up JSON.

## Development

1. Set up database
  - Create and apply migration
  - Create and apply seed(s)
1. Set up env variables
1. Set up route config
1. Create file in routes folder for that resource
1. Add route handlers for that resource
1. Set up knex queries
1. set up .env file
1. Add controller (optional)


## Deployment

1. Setup Heroku
  - `heroku create`
1. Push to Heroku (do this step everytime you make a change that needs to be applied to the Heroku app)
  - `git add -A`
  - `git commit -m'message goes here'`
  - `git push heroku master`
1. Setup DB : `heroku addons:create heroku-postgresql:hobby-dev`
1. Run Migrations : `heroku run knex migrate:latest --env production`
1. Run Seeds: `heroku run knex seed:run -- env production`
1. Heroku Restart
