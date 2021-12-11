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
nest new .
```
```bash
exit
```
###### Create frontend vuejs app:

```bash
docker-compose run --rm backend zsh
```
```bash
vue create .
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
