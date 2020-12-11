# 

# INTRODUCTION

This is a Technical Test for torre.co.

By: Miguel Alejandro Parra Romero. maparrar@gmail.com


## Table of Contents
1. [Planning](#Planning)
	- [Stage 1](#Stage-1)
	- [Stage 2](#Stage-2)
	- [Stage 3](#Stage-3)
2. [Problem and suggested solution](#Problem-and-suggested-solution)
3. [Third Example](#third-example)
4. [Fourth Example](#fourth-examplehttpwwwfourthexamplecom)




# Planning
The project was divided in 3 stages of 24 hours, each stage with 12 hours of effective working time.

## Stage 1:
### Product tasks:
- Interviews with people that was looking for jobs and ask about things that they wanted
- Think about a creative problem and a solution
- Decide viability, feasibility and scope for the solution
- Define a basic design

### Development tasks:
- Create repositories and branches:
	- Docs repository
	- Front repository
	- ad_server repository
- Define architecture and the deply server

## Stage 2:
- Development of front with basic design
- Development of the mock server (ad_server)




# Problem and suggested solution

## Problem: 
Sometimes there isn't an easy way to know the job that people want to apply for several reasons: 
- there is not an standard for the jobs names between countries, or even companies 
- intersection between abilities for jobs: software developer, web developer, front end developer, needs algorithm skills 
- people are amazingly unique, with skills that usually are not consider for jobs, and could be really useful for some companies, ie:
	- a Social Worker with abilities in logistics => environmental consultation 
	- a Developer with abilities in electronics => software developer in electronics company

## Proposed solution: 
	Visualization system to find jobs or careers that are aligned with current abilities or 
	abilities to learn in the future

### Data flow:
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







==================================================================================================
VERSIONS:

Version 1.0: 
	- Load my Genome with Current Skills and Want to Develop Skills from torre.co 
	- Load the available jobs from torre.co and the skills required 
	- Load from learn_server (mock server) the acedemies to improve the desired skills
	- Basic styling

Version 2.0: 
	- Show my skills, jobs and desired skills graphically

Version 3.0: 
	- Graphical controls
	- Improve styling




									VERSION 1.0 
Load my Genoma with Current Skills and Want to Develop Skills from torre.co
	- 
Load the available jobs from torre.co and the skills required 
Load from learn_server (mock server) the acedemies to improve the desired skills



