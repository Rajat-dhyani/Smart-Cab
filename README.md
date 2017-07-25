# Smart Cab
*Udacity - Machine learning Nano Degree Program : Project-4*

## Project Overview
*This is fifth project in the series of the projects listed in Udacity- Machine Learning Nano Degree Program.*

In the not-so-distant future, taxicab companies across the United States no longer employ human drivers to operate their fleet of vehicles. Instead, the taxicabs are operated by self-driving agents, known as **SmartCabs**, to transport people from one location to another within the cities those companies operate. In major metropolitan areas, such as Chicago, New York City, and San Francisco, an increasing number of people have come to depend on smartcabs to get to where they need to go as safely and reliably as possible. 

*Although smartcabs have become the transport of choice, concerns have arose that a self-driving agent might not be as safe or reliable as human drivers, particularly when considering city traffic lights and other vehicles. To alleviate these concerns, My task as an employee for a national taxicab company is to use reinforcement learning techniques to construct a demonstration of a smartcab operating in real-time to prove that both safety and reliability can be achieved.*

![Smart-Cab](https://github.com/Rajat-dhyani/Smart-Cab/blob/master/rajat-dhyani-smart-cab.png)

## Project Definitions

### Environment
The smartcab operates in an ideal, grid-like city (similar to New York City), with roads going in the North-South and East-West directions. Other vehicles will certainly be present on the road, but there will be no pedestrians to be concerned with. At each intersection there is a traffic light that either allows traffic in the North-South direction or the East-West direction. U.S. Right-of-Way rules apply:
* On a green light, a left turn is permitted if there is no oncoming traffic making a right turn or coming straight through the intersection.
* On a red light, a right turn is permitted if no oncoming traffic is approaching from your left through the intersection. To understand how to correctly yield to oncoming traffic when turning left.

### Inputs and Outputs
For this project I have assumed that the smartcab is assigned a route plan based on the passengers' starting location and destination. The route is split at each intersection into waypoints, and the smartcab, at any instant, is at some intersection in the world. Therefore, the next waypoint to the destination, assuming the destination has not already been reached, is one intersection away in one direction (North, South, East, or West). The smartcab has only an egocentric view of the intersection it is at: It can determine the state of the traffic light for its direction of movement, and whether there is a vehicle at the intersection for each of the oncoming directions. For each action, the smartcab may either idle at the intersection, or drive to the next intersection to the left, right, or ahead of it. Finally, each trip has a time to reach the destination which decreases for each action taken (the passengers want to get there quickly). If the allotted time becomes zero before reaching the destination, the trip has failed.

### Rewards and Goal
The smartcab will receive positive or negative rewards based on the action it has taken. Expectedly, the smartcab will receive a small positive reward when making a good action, and a varying amount of negative reward dependent on the severity of the traffic violation it would have committed. Based on the rewards and penalties the smartcab receives, the self-driving agent implementation should learn an optimal policy for driving on the city roads while obeying traffic rules, avoiding accidents, and reaching passengers' destinations in the allotted time.

### Project Highlights
*In this project i have applied reinforcement learning techniques for a self-driving agent in a simplified world to aid it in effectively reaching its destinations in the allotted time. I have first investigated the environment, the agent operates in, by constructing a very basic driving implementation. Once my agent was successful at operating within the environment, i have then identified each possible state the agent can be in when considering such things as traffic lights and oncoming traffic at each intersection. With states identified, i have then implemented a Q-Learning algorithm for the self-driving agent to guide the agent towards its destination within the allotted time. Finally, i have improved upon the Q-Learning algorithm to find the best configuration of learning and exploration factors to ensure the self-driving agent is reaching its destinations with consistently positive results.*

**Achievements**
* Applied reinforcement learning to build a simulated vehicle navigation agent. 
* Achieved A+ rating in both safety and reliability of smart-cab.

Things i have learnt by completing this project:
* How to apply reinforcement learning techniques: Q-learning algorithms.
* How to investigate the environment and train our agent to operate in the specified environment.
* How to analyze agent's performance in the given environment.
* How to optimise Q-learning algortithm, to ensure increase in postive results.

### Other Related Projects:
* <strong> Project 0 : </strong> *[Titanic Survivals Prediction](https://github.com/Rajat-dhyani/titanic_survival)*
* <strong> Project 1 : </strong> *[Boston's Houses Prediction](https://github.com/Rajat-dhyani/boston_housing)*
* <strong> Project 2 : </strong> *[Charity Donors Prediction](https://github.com/Rajat-dhyani/charity_donors)*
* <strong> Project 3 : </strong> *[Creating Customer Segments](https://github.com/Rajat-dhyani/creating_customer_segments)*
* <strong> Project 5 : </strong> *[ImageNetBot](https://github.com/Rajat-dhyani/ImageNetBot)*
* <strong> Project 6 : </strong> *[Stock Price Predictor](https://github.com/Rajat-dhyani/Stock-Price-Predictor)*

## Software and Libraries
This project uses the following software and Python libraries:

* [Python 2.7](https://www.python.org/download/releases/2.7/)
* [NumPy](http://www.numpy.org/)
* [pandas](http://pandas.pydata.org/)
* [scikit-learn](http://scikit-learn.org/0.17/install.html) (v0.17)
* [matplotlib](http://matplotlib.org/)
* [PyGame](http://pygame.org/)
* [Jupyter Notebook](http://ipython.org/notebook.html)

