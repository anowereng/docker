## Docker Use Guide 
````
1) images check
=========
docker images

2) docker build .net core project
===================
E:\Dev-Skill\devskill-dotnetcore-workspace\TaskSystem.Web> docker build -f Tasksystem.Web\Dockerfile -t tasksystem .

3 ) docker images remove  ( not necessary )
doceker rmi 5526363636 -f

4) Create Linux machine on amazon

ssh		tcp	22	custom		0.0.0.0/0
custom TCP 	tcp	80	custom		0.0.0.0/0
mssql 		tcp	1433	custom		0.0.0.0/0

5) puttygen.exe and putty.exe download ( this method pem to ppk convert for connect amazon machine ssh service) 

>puttygen sw open and
	>conversion> import key dockerdeploy.pem( amazon pem file ) 
		>save private key .ppk 

6 ) putty login ( for linux machine ssh port connect ) 
	ubuntu@( your ip) 
 ssh> auth > private key auth ( select file which convert pem to ppk file ) 

7 ) docker use local machine 5000 

8) docker run -it --rm -p 5000:80 -p 1433:1433 --name aspnetcore_sample ecommerce

9) check your site 
	localhost:5000/admin

10 ) docker install in linux machine 

11) create repository in docker hub

12 ) tag use 
	docker tag tasksystem anowerullah/dockercore ( repository name )
13) check taging docker images 
14) docker login
15) after login docker push
	> docker push anowerullah/dockercore
	
16) docker pull on linux machine 
	> docker pull anowerullah/dockercore
17) docker run -it --rm -p 80:80 -p 1433:1433 --name aspnetcore_smaple anowerullah/dockercore


======================== 
docker image rename 
-----------------------
docker image tag 2b410dadcaa1 tasksystem:latestest



