# Steps to run
1. install vagrant and vmware
2. clone the git repository - git clone https://github.com/sai3010/item-catalog.git
3. open terminal 
4. run vagrant up and vagrant ssh
5. cd to shared directory

### Set up a Google Plus auth application.
1. go to https://console.developers.google.com/project and login with Google.
2. Create a new project
3. Name the project
4. Select "API's and Auth-> Credentials-> Create a new OAuth client ID" from the project menu
5. Select Web Application
6. On the consent screen, type in a product name and save.
7. In Authorized javascript origins add:
    * http://0.0.0.0:8080
    * http://localhost:8080/ 
8. Click create client ID
9. Click download JSON and save it into the root director of this project. 
10. Rename the JSON file "client_secret.json"
11. In main.html replace the line "data-clientid="45327562329-c34ejqbu5m8i68h1vkgrkhmcstdqktbs.apps.googleusercontent.com" so that it uses your Client ID from the web applciation. 

### How to use
1. cd/vagrant/catalog
2. run python database_setup.py 
3. run python listofmenus.py to populate the database
4. run python project.py
5. open http://localhost:5000/ to view it in browser
