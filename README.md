# Boilerplate: Single repo NestJS + VueJS

## Getting started

###### Build the base image
```bash
docker-compose build
```
###### Create backend Nestjs app :
```bash
docker-compose run --rm backend zsh
```
```bash
nest new . --skip-git
```
```bash
exit
```
###### Create frontend vuejs app:

```bash
docker-compose run --rm frontend zsh
```
```bash
vue create . --no-git # Answer yes to "generate project in current directory" + better choose NPM as package manager 
```
```bash
exit
```
###### Then youre good to go :
```bash
docker-compose up
```
###### Any npm packages can be installed by going in the appropriate container :
Install npm modules in backend (the service must be running -> `docker-compose up`):
```bash
docker-compose exec backend zsh
```
```bash
npm install something
```
Install npm modules in frontend (the service must be running -> `docker-compose up`):
```bash
docker-compose exec frontend zsh
```
```bash
npm install something
```
### RTFM !
- https://docs.nestjs.com/
- https://vuejs.org/v2/guide/
