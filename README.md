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


  <dt>login:</dt>
  <dd>docker login </dd>
  <dt>stop container:</dt>
  <dd>docker stop containerID </dd>
   
<dt>create image:</dt><dd>  docker image save -o IMAGE newmohib/verse_gapminder</dd>
<dt>remove image:</dt><dd> docker rmi image c7174e6ab181</dd>
remove image force :</dt><dd> docker rmi -f image c7174e6ab181</dd>
<dt>build:</dt><dd> docker build -t app/second-app .</dd>
<dt>create tag :</dt><dd> docker tag  babead534f77 newmohib/forth-app:testTag</dd>
<dt>images :</dt><dd> docker images</dd>
<dt>push :</dt><dd> docker push newmohib/forth-app</dd>
<dt>container stop:</dt><dd> docker stop e33d558a5c46</dd>

<dt>remove all image :</dt><dd>docker system prune --all</dd>
<dt>pull :</dt><dd> docker pull newmohib/forth-app:testTag</dd>
<dt>build:</dt><dd> docker build -t newmohib/forth-app .</dd>
<dt>run :</dt><dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>
<dt>stop:</dt><dd> docker stop 6ce87495c2f4</dd>

  <dt>create tar :</dt><dd> docker save -o c:/new/forth-app.tar  newmohib/forth-app</dd>
  <dt>load tar:</dt><dd> docker load -i c:/new/forth-app.tar</dd>
 <dt> run :</dt><dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>
 <dt> view container:</dt><dd> docker ps</dd>

  <dt>after send ter and run app :</dt>

  <dt>load tar:</dt> <dd>docker load -i c:/new/forth-app.tar</dd>
  <dt>run :</dt><dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>

  # after update code 

  <dt>build:</dt>	 <dd>    docker build -t newmohib/forth-app .</dd>
  <dt>create tag :</dt><dd> docker tag  babead534f77(image ID) newmohib/forth-app:testTag</dd>
  <dt>push : </dt><dd>docker push newmohib/forth-app</dd>

  # for build ==>> tar ==>> load run

  <dt>build:</dt>	 <dd>     docker build -t newmohib/abbvie-piap-api .</dd>
  <dt>create tar :</dt> <dd> docker save -o  C:/new/project/all/abbvie/Docker/abbvie-piap-api.tar newmohib/abbvie-piap-api</dd>
  <dt>load tar:</dt> <dd> docker load -i C:/new/project/all/abbvie/Docker/abbvie-piap-api.tar</dd>
 <dt> run :</dt> <dd> docker run -p 3000:8080 -d newmohib/forth-app</dd>

 <dt> Link:</dt> <dd> docker run -p 3001:3001 --link peaceful_germain -d  newmohib/abbvie-piap-admin</dd>

 <dt> compose with Build:</dt> <dd>docker-compose up --build</dd>


# Database
 <dt> database connect :</dt> <dd> docker exec -it demo psql -U postgres</dd>
 <dt> creat Database:</dt> <dd> test;</dd>
 <dt> go database:</dt>  <dd>\c test;</dd>
 <dt> create table:</dt> <dd> CREATE TABLE user(something init);</dd>
 <dt> insert data:</dt> <dd> INSERT INTO user(something)values (1);</dd>
  \dt
 <dt> select all:</dt> <dd> select * from user ;</dd>

 <dt> exit:</dt> <dd> \q</dd>

 <dt> pstgresql install:</dt>  <dd> docker run --name some-postgres -e POSTGRES_PASSWORD=mysecretpassword -d postgres</dd>

 <dt> pstgresql link with pgAdmin: </dt>  <dd> docker run -p 80:80 --link some-postgres -e "PGADMIN_DEFAULT_EMAIL=email@domain.com" -e "PGADMIN_DEFAULT_PASSWORD=postgres" -d dpage/pgadmin4</dd>