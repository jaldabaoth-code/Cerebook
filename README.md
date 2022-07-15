<h1>Cerebook (Project 3, WCS CDA Java)</h1>

### Create a site web (social network) for superheroes by using Java Spring


---

### Prerequisites

* PostgreSQL (<a href="https://phoenixnap.com/kb/how-to-install-postgresql-on-ubuntu">Link for how to install <b>PostgreSQL</b></a>)
    #### Install PostgreSQL from PostgreSQL Apt Repository
1. `sudo apt-get install wget ca-certificates`
2. `wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -`
3. `sudo sh -c 'echo "deb http://apt.postgresql.org/pub/repos/apt $(lsb_release -cs)-pgdg main" > /etc/apt/sources.list.d/pgdg.list'`
4. `sudo apt-get update`
5. `sudo apt-get install postgresql postgresql-contrib`
   #### Install PostgreSQL from Local Ubuntu Repository
6. `apt show postgresql`
7. `sudo apt install postgresql postgresql-contrib`
   #### Connect to PostgreSQL
8. `sudo su - postgres`
9. `psql`
   #### Check Connection Information
10. `\conninfo`


### Other postgreSQL commands
1. Create new user : `create user user_name with encrypted password 'mypassword';`
2. Grant privileges : `grant all privileges on database database_name to user_name;`
3. Connect to new user : `psql -d database_name -U user_name -h localhost`
4. Delete a user : `sudo su - postgres` -> `psql` -> `DROP OWNED BY user_name;` -> `DROP ROLE user_name;`
5. Connect to database : `\c database_name`
6. List all Users in PostgreSQL  : `\du`
7. List all Databases in PostgreSQL  : `\l`
8. List all Tables in PostgreSQL  : `\dt`

### Steps

1. Clone the repo from Github
2. Create the database
3. Create <b>.env</b> file from <b>.env.model</b> and add your Database parameters
4. Run `mvn install`
5. Run the server with `sh ./env_spring_boot_run.sh`
6. Import the last version of the <b>dataVx.sql</b> file in your SQL server
7. Go to <b>localhost:8080</b> on your browser
8. For login You can use :

    Username = deadpool<br/>
    Password = 123456789<br/>
    <b>OR</b><br/>
    Username = domino<br/>
    Password = 123456789<br/>

---

## The Links

<a href="https://github.com/RaphaelBS-WCS/Cerebook">Link to the repository of project where we worked during <b>WCS CDA Project 3</b></a>
