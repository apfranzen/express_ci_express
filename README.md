# Continuous Integration and Deplyment with GitHub, Travis and Heroku

## Deploy to Heroku

1. `heroku create`
1. `git push heroku master`
1. Create db
1. Set up the db on Heroku: `heroku addons:create
heroku-postgresql:hobby-dev`
1. Update *knexfile.js* with production config
1. Push to Heroku after you commit
1. Add any necessary environment variables
1. Create migrations (if necessary)
1. Apply migrations: `heroku run knex migrate:latest --env=produciton`
1. Apply seeds: `Heroku run knex seed:run --env=production`
1. Restart Heroku app: `heroku restart`

## Push to GitHub
