Our design document lays out everything we plan on doing and tested out in advance for our project. We are still planning on meeting all of our #1 priorities, but our #3 priorities will be met if time permits. 

One minor obstacle we encountered was getting an "Error 403 Forbidden" when trying to access the GitLab API, which was resolved by logging into GitLab. There was also an issue with accessing the API from a Jupyter Notebook using Python that was fixed as well. Of course when making API calls via command line or python scripting you can't log in.  This was resolved with a personal access token.

After that, we encountered trouble moving from command line api calling (via curl) to python script calling.  The solution was with urllib2 library and the request.get call, which returns data as a status code (hopefully 200) as well as a .json file.
