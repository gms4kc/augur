1. Identify GitLab’s API
   1. [https://gitlab.com/api/v4/users?search=$email](https://gitlab.com/api/v4/users?search=$email)

   2. 1. curl -XGET "[https://gitlab.com/api/v4/users?search=brossn7@gmail.com](https://gitlab.com/api/v4/users?search=$email)" -H "private-token: $[Personal access token]"

   3. Must be logged in to GitLab to access their API

   4. 1. Command line/scripts can use access tokens generated by GitLab

2. Parse returned data by searching for "username" token

3. Test to see how user email works
   1. If searching by email fails, then search by name

4. Test to see how user name works
   1. If searching by name fails, move onto next user

5. Query table and iterate through all emails 

6. If time, create user interface that allows users to input their email to check the connected user
    1. Simple HTML form with textareas and a button to submit inputted data
    2. Output textarea to show information

7. If time, sort data 
   1. Implement sorting algorithm
