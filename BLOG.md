### Adding Integration Tests to a CI/CD Pipeline 
### (Docker, Drone, Selenium, Pytest) 

This post piggy-backs off a three part tutorial on setting up
a [Drone CI/CD pipeline](https://www.imagescape.com/blog/2017/03/21/integration-Drone-Docker-Django-Gunicorn-Nginx/).  We will continue along the path layed out in that series, with a few changes here and there, and add some basic Behavior Driven Development (BDD) based integration tests.  This tutorial is not meant to proselytize specific testing strategies(BDD) or technologies(Selenium, Drone, Pytest), but rather to provide a basic working instance taken from the dizzying array of potential CI/CD solutions.

**Environment Specs**  
Docker 19.03.1  
Docker-Compose 1.24.1  
Drone 0.8  
Python 3.7  
Django 2.2.5  
pytest-django 3.5.1  
pytest-bdd 3.2.1  
pytest-splinter 2.0.1  

**Project Repo**
```git clone 


First, lets add a basic integration test using `pytest`, `pytest_django`, `pytest_bdd`, and `pytest-splinter` 
This tutorial will use an updated version of Drone, and some different configurations, so there will be a bit of a disconnect with the aforementioned series.
