# Strategic Covid19 Testing

Via this project we tried to estimate what would be the minimum number of testing to be done in a pandemic affected small world netwrok to recover from the pandemic. We also analysed 3 forms of testing and compared their results.

## Abstract


## Components

### Epidemiological Compartmental Model

[Compartmental Models](https://en.wikipedia.org/wiki/Compartmental_models_in_epidemiology) are mathematical sets of differential equation used to study an epidemic or pandemic through time. These differential equations may be solvable or may be not. There are many kinds of compartmental model which are used by researchers for their specific research. In this project **S-E-I-R-S** model has been used. Each letter in the model means a compartment that is described in details : 
1. ***Susceptibe        (S) =*** _The compartment of Individuals who can get exposed to the virus._
2. ***Exposed           (E) =*** _The compartment of Individuals who has been exposed to the virus by someone infected. The exposed individuals do not show symptoms and do not expose other susceptible. One in every 5 exposed individuals starts to show symptoms and is moved to Infected._
3. ***Infected          (I) =*** _The compartment of Individuals who turned symptomatic are in this compartment. These individuals can expose the virus to susceptible and make them Exposed._
4. ***Recovered/Removed (R) =*** _The compartment of Individuals who have either cured from the virus and no longer Infectious or Susceptible. This also has the individuals who have died in the pandemic._

The time dependent movement of the people from one compartment to another based on the actions of the virus are goverened by sets of differential equations. Each of this equation tells us the rate of change of population in every compartment. That gives epidemiologists and virologists a solid idea of how the virus is infecting the population and how the healthcare measures needs to be placed to incur minimum damage.

### Watts-Strogatz Small World Network
![](https://github.com/thecrazyphysicist369/Voting-in-a-Small-World-Network/blob/master/swn.png)

This is a special type of graph, a small world, which depicts the human dynamics of real world in a fundamental level without all the real world abstractions.
[Watts-Strogatz](https://en.wikipedia.org/wiki/Watts%E2%80%93Strogatz_model) small world network uses 3 variables to define the network.

1. ***Nodes              =  n***   _The total number of nodes in the Small World._
2. ***Nearest neighbors  =  k***   _The number of nodes each node is connected to. Also called close-contacts._
3. ***Probability        =  p***   _This is the length of connection of the edges._



### Testing Strategies

Few lines about how the testing strategy differs.
Testing strategy referes to how one chooses the test subject. In real world, the governments used different strategies dependent on the time in the pandemic, geographical location, population density, demography of the population, etc. The math used to choose the test subject affects the growth of the infected population significantly. In this project, we removed all the abstractions from these testing strategies and brought it down into bare bone. Here 3 different testing strategies were tested.

#### Random Testing

In random testing every individual to be tested is picked at random from the total population. If the tested subject is _Exposed_ or _Infected_ then he/she would result positive and will be quarantined (all connections cut-off) for the next 15 days. If the testes subject is found to be negative, then nothing is done.
```
Pseudocode for random testing
```


About Random testing

#### Targeted Testing
```
Pseudocode for random testing
```


#### n-Neighbor Testing
```
Pseudocode for random testing
```
About n-Neighbor testing


## Executing the Code

The simulation can be executed in two forms Both the forms are coded into the same Jupyter Notebook. Just read the instruction in the Notebook text section.

### The Simulation

Simulating the hybrid model means running the small world network through the given iteration. That includes intial generation of the network and infection the given number of individuals in the population. Then the virus spread happens and the model runs through iterations saving the compartmental values for later analysis and plotting. The final section can be used in two ways, the first one is simultion through input values and the second one is running the simulation with parameters in sliders.


#### Input Value execution

Explain what these tests test and why


#### Slider execution
```
Give an example
```

## Results

Discuss the results include how the number of tests per day affects the network.
### Random Testing
![](https://github.com/thecrazyphysicist369/strategic-Covid19-testing/blob/main/images/random%2010000%205.png)

### Targeted Testing
![](https://github.com/thecrazyphysicist369/strategic-Covid19-testing/blob/main/images/tar%2010000%205.png)

### n-Neighbor Testing
![](https://github.com/thecrazyphysicist369/strategic-Covid19-testing/blob/main/images/neighbor%2010000%205.png)


## Built With

* [Python-3](https://www.python.org/) - The language.
* [Networkx](https://matplotlib.org/) - The network generating library.
* [Matplotlib](https://networkx.org/) - The plotting-visualising library.


## Contributing


### Authors

* **Shaun** - *Author* - [Twitter](https://twitter.com/thecrzyphysicst), [Google Scholar](https://scholar.google.com/citations?hl=en&user=mxc8IfcAAAAJ)

* **Sayan Mondal** - *Author* - [Twitter](https://twitter.com/sayanmondal2098), [Google Scholar](https://scholar.google.com/...)

* **Ritajit Mojumdar** - *Co-author* - [Google Scholar](https://scholar.google.com/citations?user=eZL1OXcAAAAJ&hl=en)

* **Dr. Kingshuk Chatterjee** - *Co-author* - [Google Scholar](https://scholar.google.com/citations?user=o-WIpn0AAAAJ&hl=en)

* **Dr. Debayan Ganguly** - *Co-author* - [Google Scholar](https://scholar.google.com/citations?user=ikohpY4AAAAJ&hl=en)

## Acknowledgments

