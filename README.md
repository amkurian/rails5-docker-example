To create the database run **docker-compose run web rake db:create**

To start the application run **docker-compose up** in the project directory

To stop the application run **docker-compose down** in the project directory

If you make changes to the Gemfile or the Compose file to try out some different configurations, you need to rebuild. Some changes require only **docker-compose up --build**, but a full rebuild requires a re-run of **docker-compose run web bundle install** to sync changes in the Gemfile.lock to the host, followed by **docker-compose up --build**.
