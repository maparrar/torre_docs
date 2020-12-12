# 

# INTRODUCTION

This is a Technical test for torre.co. By: Miguel Alejandro Parra Romero. maparrar@gmail.com

Stage: [skillsviewer-dev](https://skillsviewer-dev.herokuapp.com/)
Production: [skillsviewer](https://skillsviewer.herokuapp.com/)

## Repositories
- Documents (this repository): [https://github.com/maparrar/torre_docs](https://github.com/maparrar/torre_docs)
- Front: [https://github.com/maparrar/torre_front](https://github.com/maparrar/torre_front)
- Back (ad-server): [https://github.com/maparrar/torre_back](https://github.com/maparrar/torre_back)

## Table of Contents
1. [Planning](#Planning)
1. [Problem and proposed solution](#Problem-and-proposed-solution)
1. [Architecture and technologies](#Architecture-and-technologies)
1. [Development details](#Development-details)
1. [Time Log](#Time-log)
1. [Future work](#Future-work)


# Planning
The project was divided in 3 stages of 24 hours, each stage with 12 hours of effective working time.

## Stage 1 (Planning):
### Product tasks:
- Interviews with people that was looking for jobs and ask about things that they wanted
- Think about a creative problem and a solution
- Decide viability, feasibility and scope for the solution
- Define a basic design

### Development tasks:
- Create repositories and branches
- Define architecture and the deploy server

## Stage 2 (Versions 1.0 and 2.0):
- Development of front with basic design
- Development of the visualisator
- Development of the mock server (ad_server)

## Stage 3 (Version 3.0 and 4.0):
- Development of graphical controls
- Development of skills simulator
- Final deployment

# Problem and proposed solution

## Problem:
Sometimes is difficult for a candidate to know what skills need to be improved to apply for a specific job. Even when she/he can see the list of required skills, is not easy to compare with another jobs' required skills.

## Proposed solution:
**skills viewer**: visualisation system to find the skills that need to be improved for a job and 'advertisement' of academies where can be studied them.

The candidate can look for the available jobs and view graphically and intuitively which of these jobs are 'near' to his/her current skills. The criteria are:
- distance: near means the candidate doesn't need so much skills to be 'good' candidate for that job. Far means need improve more skills
- size: big means a big compensation
- color: type of job: freelance-gigs, full-time-employment, ...


# Architecture and technologies

## Front
- React.js
- Redux
- Redux-persist
- Axios
- Deployed to [Surge](https://surge.sh)

## Back (ad-server)
- NodeJs
- Express
- MongoDB
- Deployed to [Heroku](https://heroku.com)

## Back (torre.co)
- API user (skills)
- API jobs 

## Data flow:
```
  __________	                                         __________
 |          |-----------[current_and_future_skills]---->|          |
 | torre.co |                                           |          |
 |__________|----------------[available_jobs]---------->|          |
                                                        |  Client  |
 ____________                                           |          |
|            |                                          |          |
|learn_server|-------[academies_related_with_skills]--->|__________|
|____________|

```


# Development details

## Versions

### 1.0: 
- Load my Genome with Current Skills and Want to Develop Skills from torre.co 
- Load the available jobs from torre.co and the skills required 
- Load from learn_server (mock server) the acedemies to improve the desired skills
- Basic styling

### 2.0: 
- Show my skills, jobs and desired skills graphically

### 3.0: 
- Graphical controls
- Improve styling

### 4.0.
- Skills simulator


# Time Log

## Stage 1 (day 1)
- [2h] Project planning
- [1h] Interviews with people that was looking for jobs and ask about things that they wanted
- [1h] Define and calculate viability, feasibility and scope for the solution
- [1h] Define a basic design
- [2h] Create repositories and branches:
	- Docs repository
	- Front repository
	- ad_server repository
- [2h] Define architecture, technologies and the deploy server
- [3h] Write base documentation

## Stage 2 (day 2)
- [1h] Initialize React project and start Front end development
- [5h] Cors server creation to avoid Cors restrictions
-  


# Future work

This is just and aproximation to a visualisation tool and can be improve in many ways:
- Standarize skills required by Opportunities and the selectable strengths by candidates
- Unify strengths and retun them with ids by candidate
- Improve the visualisation
- ...