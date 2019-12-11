# Connection With Multiple Docker Container

## Features

<dl>
  <dt>Install Docker Then </dt>
  <dd><a href="https://docs.docker.com/docker-for-windows/install/">Install Docker
  </a></dd>
  <dt>RUN : </dt>
  <dd>docker-compose up --build</dd>

  <dt>Get Data Express Server one To api </dt>
  <dd>http://localhost:3000/users</dd>

   <dt>Response Data Express Server tow </dt>
  <dd>http://localhost:4000/users</dd>

  ## DOCKER COMMAND

  <dd>
  stop container: docker stop containerID
login: docker login

create image:  docker image save -o IMAGE newmohib/verse_gapminder
remove image: docker rmi image c7174e6ab181
remove image force : docker rmi -f image c7174e6ab181
build: docker build -t app/second-app .
create tag : docker tag  babead534f77 newmohib/forth-app:testTag
images : docker images
push : docker push newmohib/forth-app
container stop: docker stop e33d558a5c46

remove all image :docker system prune --all
pull : docker pull newmohib/forth-app:testTag
build: docker build -t newmohib/forth-app .
run : docker run -p 3000:8080 -d newmohib/forth-app
stop: docker stop 6ce87495c2f4

create tar : docker save -o c:/new/forth-app.tar  newmohib/forth-app
load tar: docker load -i c:/new/forth-app.tar
run : docker run -p 3000:8080 -d newmohib/forth-app
view container: docker ps


after send ter and run app :

load tar: docker load -i c:/new/forth-app.tar
run : docker run -p 3000:8080 -d newmohib/forth-app


after update code 

build:	     docker build -t newmohib/forth-app .
create tag : docker tag  babead534f77(image ID) newmohib/forth-app:testTag
push : docker push newmohib/forth-app

for build ==>> tar ==>> load run

build:	     docker build -t newmohib/abbvie-piap-api .
create tar : docker save -o  C:/new/project/all/abbvie/Docker/abbvie-piap-api.tar newmohib/abbvie-piap-api
load tar: docker load -i C:/new/project/all/abbvie/Docker/abbvie-piap-api.tar
run : docker run -p 3000:8080 -d newmohib/forth-app

Link: docker run -p 3001:3001 --link peaceful_germain -d  newmohib/abbvie-piap-admin

compose with Build: docker-compose up --build



============Database=====================
database connect : docker exec -it demo psql -U postgres
creat Database: test;
go database: \c test;
create table: CREATE TABLE user(something init);
insert data: INSERT INTO user(something)values (1);
\dt
select all: select * from user ;

exit: \q

pstgresql install:  docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres

pstgresql link with pgAdmin:   docker run -p 80:80 --link some-postgres -e "PGADMIN_DEFAULT_EMAIL=email@domain.com" -e "PGADMIN_DEFAULT_PASSWORD=postgres" -d dpage/pgadmin4

  </dd>