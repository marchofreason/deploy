# MJAK Deployment for vue + Django

## Instructions
**NO NEED TO CLONE THE REPO**

For now to get up and running all you need to do is this:
```
$ npm install -g vue-cli
```
Use sudo if error with installing the package

### Clone from our Private Repo
Go to the path you want to setup the project and then run:

```
vue init marchofreason/deploy projectname --clone
```

Create a Virtual env directory as well

``` 
mdkir _projectname
virtualenv -p python3 --no-site-packages _projectname
source _projectname/bin/activate
```

### Create the Virtualenv for Django + PIP
Make sure you create a virutalenv (See Documentation Repo)
Steps to create this and get the main modules running

```
cd projectname/
pip3 install -r requirements.txt
npm install
```
## Development
Running the Development environment runs a node backend on 8080 but serves the assets with a hot-reload. Something like Gulp+ Browser sync - This is purely for development and productionization will be Django (see below)                
`npm run dev`

## Deployment (DIST via Django)
Make sure to chmod your deploy.sh 
`chmod +x deploy.sh` and then `/.deploy.sh`