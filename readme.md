### Test Docker project

simple symfony project created from inside the docker so in our host we need code editor only.

steps to build and run :
<pre>
`sudo docker build --file .docker/Dockerfile -t symfony .`
`sudo docker-compose up --build`
`sudo docker-compose up `
`sudo docker-compose exec app /bin/bash`
`cd /srv/app`
`composer create-project symfony/skeleton test-symfony`
`chmod -R 777 . `
`cp -R test-symfony/* ./`
`rm -R test-symfony`
</pre>

open http://127.0.0.1:8989/

u can connect to mysql db on docker using workbench:
see Screenshot_2018-10-30_12-47-34.png
