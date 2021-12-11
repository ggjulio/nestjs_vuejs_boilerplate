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
### RTFM !
- https://docs.nestjs.com/
- https://vuejs.org/v2/guide/
