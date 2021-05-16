Group 10 Sprint 4
-----------------------------------------------

In our final sprint, we took our working prototype code and integrated it with the schema that Sean provided for us on Slack, and implemented error handling to ensure nothing trips us up as we go about matching contributor information to GitLab information.

The following information is in the documentation of our Jupyter Notebook as well, but is also addressed here for clarity's sake.

We found the databse that Goggins suggested to us, after having had some difficulty last sprint.  However, the credentials we had for the augur-community-reports databases (user chaoss) did not have permission to interact with the schema "sean", and it didn't feel right to attempt to test any student code on the other production databases.  For that reason we set up a new database locally (with the same schema via SQL provided by Sean) and copied the data out of the contributors table into our own.  

We modified the code to accept a config file instead of hardcoded values, so to test this code on your desired environment, be that your own local database or on the augur-community-reports live database, you will need to make relevant changes to the config file to access that database.

As long as you've done that, it should be as simple as running our Jupyter Notebook from beginning to end!