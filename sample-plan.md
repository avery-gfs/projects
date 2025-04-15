**Which class are you in?**

CS 3-2
 
**Who are you working with?**

Matt Zippin

**Choose a title for your project (a few words that describe it)**

Metro route planner

**Describe what you'll be working on in detail**

<img src="https://www.stm.info/sites/all/modules/features/stm_metro/theme/images/map-interactive.png" width="500">

We will be making a program that finds a route between Montreal metro stations. The user will enter a starting station name and a destination station name and the program will show the names of the stations in between and the total number of stops.

**Why do you want to work on this project?**

I want to learn how navigation software like Google maps works.

**What new skills / concepts will you need to learn to complete this project?**

I will need to learn how to represent a transit map as a data structure and how to search for a route between two points.

**Development step 1**

Choose a subsection of the subway system to start with. Make a hashmap / dictionary where the keys are station names and the values are lists of stations that each station connects to directly:

```
{
	"beaubien": ["jean-talon", "rosemont"],
	"d'iberville": ["fabre", "saint-michel"],
	"fabre": ["d'iberville", "jean-talon"],
	"jarry": ["cremazie", "jean-talon"],
	"jean-talon": ["beaubien", "de-castelnau", "fabre", "jarry"],
	"rosemont": ["beaubien", "laurier"],
	"saint-michel": ["d'iberville"],
}
```

**Development step 2**

Write code to prompt the user for a starting and ending station. Check to make sure the station names are valid.

**Development step 3**

Write a function that uses breadth-first search to find a route between two stations. Have the function return the path as a list of station objects.

**Development step 4**

Print the names of the stations in the route found by the search algorithm. Display the length of the route.

**Development step 5**

Add more stations to the program.

**What are your non-goals for the project? (problems you aren't going to worry about solving)**

I won't worry about suggesting alternative routes, I'll just go with the first route the search finds.
