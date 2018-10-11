# uber-dispatch-algorithm
  
  I am interested in how to design and optimise a uber-like taxi dispatch algorithm so that passenger waiting time is minimized.

  Suppose that we think of the street network of a city as a graph, whose nodes are locations, and whose edges are labelled with the time it takes to traverse them.

  There are requests to the system which include a start location and a finish location, and a time stamp. Uber drivers fulfill requests in the order of their start time stamp, moves to the pickup location (one of the nodes, for simplicity), and then takes the passenger to the finish location they requested; and then fulfills the next outstanding request, and so on.

  Assume that (a) the static data describing the city layout and street level transit times, and (b) a sequence of requests for service are given. The output of  algorithm is the total length of time that passengers spent waiting (i.e. a request start time was earlier than the arrival time of the Uber driver) and I want to make it as small as possible.

  I will start by assuming there are 2 Uber drivers, then I will discuss how the code (and results) would change if the number of drivers becomes an input to the system.
