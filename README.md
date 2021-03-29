# Java pirate 2d game sover interview task

### Motivation:

We would like you to implement a solver for a simple 2D game to help a pirate to get to target destination collecting as much treasure as possible.

The inputs are: 
 - 2 dimensional map 
 - pirate start position (x, y)
 - destination position pirate should get to

Given
 	- the pirot can move only up and right 
 	- the amount of treasure he collects is the sum of coins all the way pirot get to the destination point

Expected output is an either an object representing a path and amount of treasure pirot has collected or an error denoting that the target position is out of reach.
 	 
Step 1. A map consists of only coins where each point can contain specific amount.
	
Step 2. Assume we need to adapt this solver to an updated game where new items have been introduced. So instead of coins the map can make up of rocks wich pirot can't get accross and bombs which pirot can use to blew up rocks on his way. 

### Task description:
	
Requirements
 - Candidates should use Java programming language
 - Code should be accompanied with a docker file which can be used to run/test the solution
  
Delivery: 
 1. We expect candidates to provide us with a github link to a repository which has a guidence of how to run and test the code in docker container.
 2. Application run on container should expose REST API with methods to 
 	- load the map
 	- calculate pirate's path

## Some test cases

### Pirate can't reach the destination point
Example
 POST /map 
 [{
    
  }]

  GET /findPath?=startXPosition=2&startYPosition=3&targetXPosition=5&startYPosition=5
  Expected result
  {{
  
  }}

### Pirate collects 5 conins 


### Pirate collects 13 conins 

### Pirate collects 2 conins (has to blew up 2 rocks on his way)
