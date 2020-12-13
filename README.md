# 

# INTRODUCTION

This is a Technical test for torre.co. By: Miguel Alejandro Parra Romero. maparrar@gmail.com. 

Tool for compare jobs' skills required with the strengths of a torre.co user. (mobile, web).

This tool works better with users that have strenghts registered in torre.co. As example, you can use:
- maparrar (my username)
- torrenegra
- larpa
- kc
- georgecarretto

The working apps are in the links:
- Stage: [skillsviewer-dev](https://skillsviewer-dev.herokuapp.com/)
- Production: [skillsviewer](https://skillsviewer.herokuapp.com/)

Note: Can be delays in the app because these are free servers. Also the CORS-restrictions-avoid-server can add millseconds to the response.


## Repositories
The repositories are public, but I can change the visibility to private if required.
- Documents (this repository): [https://github.com/maparrar/torre_docs](https://github.com/maparrar/torre_docs)
- App: [https://github.com/maparrar/torre_front](https://github.com/maparrar/torre_front)

## Table of Contents
1. [Planning](#Planning)
1. [Problem and proposed solution](#Problem-and-proposed-solution)
1. [Architecture and technologies](#Architecture-and-technologies)
1. [Development details](#Development-details)
1. [Time Log](#Time-log)
1. [Future work](#Future-work)


# Planning
The project was divided in 3 stages of 24 hours, each stage with 10 hours of effective working time.

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

## Stage 3 (Version 3.0 and 4.0):
- Development of graphical controls
- Development of skills simulator
- Final deployment

# Problem and proposed solution

## Problem:
Sometimes is difficult for a candidate to know what skills need to be improved to apply for a specific job. Even when she/he can see the list of required skills, is not easy to compare with another jobs' required skills.

## Proposed solution:
**skills viewer**: visualisation system to find the skills that need to be improved for a job.

The candidate can look for the available jobs and view graphically and intuitively which of these jobs are 'near' to his/her current skills. The criteria are:
- distance: near means the candidate doesn't need so much skills to be 'good' candidate for that job. Far means need improve more skills
- size: big means a big compensation


# Architecture and technologies

## Front
- React.js
- Redux
- Axios
- Deployed to [skillsviewer](https://skillsviewer.herokuapp.com/)

## Back (torre.co)
- API user (skills)
- API jobs 

## Data flow:
```
  __________	                                         __________
 |          |-----------[current_and_future_skills]---->|          |
 | torre.co |                                           |  Client  |
 |__________|----------------[available_jobs]---------->|          |
                                                        |__________|

```


# Development details

## Versions

### 1.0: 
- Load my Genome with Current stregths from torre.co 
- Load the available jobs from torre.co and the skills required 
- Basic styling

### 2.0: 
- Show my stregths and jobs' skills

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
- [1h] Write base documentation

## Stage 2 (day 2)
- [1h] Initialize React project and start Front end development
- [7h] Cors server creation to avoid Cors restrictions
- [3h] Tests with graphical library

## Stage 3 (day 3)
- [4h] Create functions to transform input data to graphical data
- [6h] Create the visualisation tool
- [2h] Final styling and minor improvements



# Future work

This is just and aproximation to a visualisation tool and can be improve in many ways:
- Standarize skills required by Opportunities and the selectable strengths by candidates
- This tool uses 200 jobs for testing puposes, but the graphical system supports thousands of nodes, so can be used with the available jobs
-  