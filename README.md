# 

# INTRODUCTION

This is a Technical Test for torre.co.

By: Miguel Alejandro Parra Romero. maparrar@gmail.com


## Table of Contents
1. [Planning](#Planning)
	- [Stage 1](#Stage-1)
	- [Stage 2](#Stage-2)
	- [Stage 3](#Stage-3)
1. [Problem and suggested solution](#Problem-and-suggested-solution)
1. [Time Log](#Time-log)




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



# Problem and proposed solution

## Problem:
Sometimes is difficult for a candidate to know what skills need to be improved to apply for a specific job. Even when she/he can see the list of required skills, is not easy to compare with another jobs' required skills.

## Proposed solution:
**skills viewer**: visualisation system to find the skills that need to be improved for a job and 'advertisement' of academies where can be studied them.

The candidate can look for the available jobs and view graphically and intuitively which of these jobs are 'near' to his/her current skills. The criteria are:
- distance: near means the candidate doesn't need so much skills to be 'good' candidate for that job. Far means need improve more skills
- size: big means a big compensation
- color: type of job: freelance-gigs, full-time-employment, ...


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

Version 4.0.
	- 



VERSION 1.0 
Load my Genoma with Current Skills and Want to Develop Skills from torre.co
	- 
Load the available jobs from torre.co and the skills required 
Load from learn_server (mock server) the acedemies to improve the desired skills



# Time Log