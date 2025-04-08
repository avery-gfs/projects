**Which class are you in?**

CS 3-2
 
**Who are you working with?**

Matt Zippin

**Choose a title for your project (a few words that describe it)**

MBTA route planner

**Describe what you'll be working on in detail**

We will be making a program that finds a subway route between Boston subway stations. The user will enter a starting station name and a destination station name and the program will show the names of the stations in between and the total number of stops.

**Why do you want to work on this project?**

I want to learn how navigation software like Google maps works.

**What new skills / concepts will you need to learn to complete this project?**

I will need to learn how to represent a transit map as a data structure and how to search for a route between two points.

**Development step 1**

Make a list of stations on the Red and Orange lines. For each station, write down the name of the station and the stations that are adjacent to it. For example:

```
stop name: Porter
connects to: Davis, Harvard

stop name: Downtown Crossing
connects to: Park St, South Station, Chinatown, State

... etc
```

**Development step 2**

Make a Station class to represent stations in the transit network, including connection information. Make a Station object for each station.

**Development step 3**

Put these stations into a hashmap / dictionary so that we can look them up by name. Write a function that takes the name of a station and returns the corresponding station object.

**Development step 4**

Write a function that uses depth first search to find a path between two stations. Have the function return the path as a list of station objects.

**Development step 5**

Print the names of the stations in the path found by the search algorithm. Display the length of the route.

**What are your non-goals for the project? (problems you aren't going to worry about solving)**

I won't worry about avoiding infinite loops in the search algorithm. I'll make sure that the stations I include in the network don't form any loops that the search algorithm would have do deal with

**What can we do to keep adding to the project once the initial work is complete?**

Add more stations to the program.