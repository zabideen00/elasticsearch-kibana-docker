# READ ME

### Set environment variables
Create a `.env` file at the root of the project and set the following variables in the file
```ELASTICSEARCH_PASSWORD=your-password```
### Run docker-compose
Run the docker-compose.
```docker-compose up -d```

### Configure credentials for elasticsearch user
Get into the shell of the `elasticsearch` container
```docker exec -it elasticsearch bash```
Set the password for default users
```/usr/share/elasticsearch/bin/elasticsearch-setup-passwords interactive```
Set the password for elastic user same as defined in the .env file.
### Open kibana
Now go to the http://localhost:5601 to access kibana. Enter the following credentials to login
```username: elastic```
```password: same as defined in .env file```
