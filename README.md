# Connection With Multiple Docker Container

## Features

<dl>
  <dt>Install Docker Then </dt>
  <dd><a href="https://docs.docker.com/docker-for-windows/install/">Install Docker
  </a></dd>
  <dt>RUN With Compose File: </dt><dd>docker-compose up --build</dd>

  <dt>Get Data Express Server one To api </dt>
  <dd>http://localhost:3000/users</dd>

   <dt>Response Data Express Server tow </dt>
  <dd>http://localhost:4000/users</dd>

  ## DOCKER COMMAND


  <dt>Login Docker:</dt><dd>docker login </dd>
  <dt>Stop container:</dt><dd>docker stop containerID </dd>
  <dt>remove all image :</dt><dd>docker system prune --all</dd>
  <dt>remove image:</dt><dd> docker rmi image ImageID</dd>
  <dt>remove image force :</dt><dd> docker rmi -f image ImageID</dd>

<dt>Create image:</dt><dd>  docker image save -o IMAGE newmohib/verse_gapminder</dd>
<dt>Build Tar:</dt><dd> docker build -t app/second-app .</dd>
<dt>Create tag :</dt><dd> docker tag  babead534f77 newmohib/forth-app:testTag</dd>
<dt>All Images :</dt><dd> docker images</dd>
<dt>Push Image To Docker :</dt><dd> docker push newmohib/forth-app</dd>
<dt>Pull :</dt><dd> docker pull newmohib/forth-app:testTag</dd>

<dt>Build:</dt><dd> docker build -t newmohib/forth-app .</dd>
<dt>Run :</dt><dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>
<dt>Stop:</dt><dd> docker stop 6ce87495c2f4</dd>
<dt>Create tar :</dt><dd> docker save -o c:/new/forth-app.tar  newmohib/forth-app</dd>
<dt>Load tar:</dt><dd> docker load -i c:/new/forth-app.tar</dd>
<dt>Run :</dt><dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>
<dt>View container:</dt><dd> docker ps</dd>

  # after send ter and run app :

  <dt>Load tar:</dt> <dd>docker load -i c:/new/forth-app.tar</dd>
  <dt>Run :</dt><dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>

  # after update code 

  <dt>Build:</dt>	 <dd>    docker build -t newmohib/forth-app .</dd>
  <dt>Create Tag :</dt><dd> docker tag  babead534f77(image ID) newmohib/forth-app:testTag</dd>
  <dt>Push Image To Docker : </dt><dd>docker push newmohib/forth-app</dd>

  # for build ==>> tar ==>> load run

  <dt>Build:</dt>	 <dd>     docker build -t newmohib/abbvie-piap-api .</dd>
  <dt>Create tar :</dt> <dd> docker save -o  C:/new/project/all/abbvie/Docker/abbvie-piap-api.tar newmohib/abbvie-piap-api</dd>
  <dt>Load tar:</dt> <dd> docker load -i C:/new/project/all/abbvie/Docker/abbvie-piap-api.tar</dd>
 <dt> Run :</dt> <dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>

 <dt> Link:</dt> <dd> docker run -p 3001:3001 --link peaceful_germain -d  newmohib/abbvie-piap-admin</dd>

 <dt> Compose with Build:</dt> <dd>docker-compose up --build</dd>


# Database
 <dt> Database connect :</dt> <dd> docker exec -it demo psql -U postgres</dd>
 <dt> Creat Database:</dt> <dd> test;</dd>
 <dt> Go database:</dt>  <dd>\c test;</dd>
 <dt> Create table:</dt> <dd> CREATE TABLE user(something init);</dd>
 <dt> Insert data:</dt> <dd> INSERT INTO user(something)values (1);</dd>
  \dt
 <dt> Select all:</dt> <dd> select * from user ;</dd>

 <dt> Exit Database:</dt> <dd> \q</dd>

 <dt> Pstgresql install:</dt>  <dd> docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres</dd>

 <dt> Pstgresql link with pgAdmin: </dt>  <dd> docker run -p 80:80 --link some-postgres -e "PGADMIN_DEFAULT_EMAIL=email@domain.com" -e "PGADMIN_DEFAULT_PASSWORD=postgres" -d dpage/pgadmin4</dd>