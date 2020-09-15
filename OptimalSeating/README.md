Finding the optimal seating arrangement at a wedding using operations research models or clustering algorithms.

Given a connection matrix between guests and other parameters such as the number of tables and the tables' seating capacity, we can define a mathematical model to find the optimal seating arrangement of guests at a wedding, meaning that at each table the guests are maximally related. The project was inspired by Bellows, M., & Peterson, J. L. (2012). I implement the authors model in Python, using Gurobi optimization software. As an alternative method, I apply spectral clustering to the connection matrix, as this method can also provide a solution to the seating problem.

After inputing certain parameters about the wedding and a connection matrix $C$, where matrix cell $C_{j,k} indicates some measure of relatedness between guests $j$ and $k$ (e.g. number of common friends or simply how much they like each other) the code can be used to plan any wedding. 

The two methods for finding an optimal seating arrangement are demonstrated on a small example from Bellows, M., & Peterson, J. L. (2012) and on Game of Thrones network data. A number of important characters from Game of Thrones are chosen and seated at four tables according to the two methods.


![Test Image](https://github.com/matevaradi/DataScienceProjects/OptimalSeating/got_example_spectralclustering.png)

![Test Image](https://github.com/matevaradi/DataScienceProjects/OptimalSeating/got_example_lp.png)


Methods used: Zero-one linear programming; Spectral Clustering
Packages used: numpy, pandas, gurobipy, sklearn, networkx

