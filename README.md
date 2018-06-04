# Now.sh

To install Now.sh
```
nom install -g now
```
Test repositories
```
https://github.com/platzi/invie-responsive

https://github.com/platzi/now-course.git
```
To deploy, we go to the folder and put
```
now
```
To change the url, we add an alias
```
now alias url_antigua url_nueva
```
In now.json we place the necessary configuration to perform deploy, as well as the necessary environment variables

To test the backend with the db we use elephant sql that are instances of postgres

To hide the passwords and use them, we use secret
```
now secret add valor_alias valor_password
```
Suppose that the new variable is: platzi_now_db_user, we replace it in now.json

To see the code we access with
```
http://xxxxxx.now.sh/_src
```
To see the logs we access with
```
http://xxxxxx.now.sh/_log
```
to list all the deployds we use
```
now ls
```
To run all our applications under the same domain we create rule.json in the root of the project, and to set the rules to now we do:
```
now alias index_path.now.sh -r rules.json
```
To deploy from github
```
now repository/name
```
