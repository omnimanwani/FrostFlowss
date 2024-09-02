# **IcyOmni FrostFlow Budget Optimizer**

## **Introduction**
This project focuses on optimizing budget distribution across multiple advertising channels, including Google Ads, Microsoft Ads, and Meta Ads. The primary objective is to allocate the budget in a way that maximizes conversions while minimizing costs.

[Updated Link for colab](https://colab.research.google.com/drive/1QoHyfHExe3NAVgiuFSBlh7DE7MJM_NbB?usp=sharing)

### **Problem Statement**
**AI-Driven Media Investment Plan Across Channels for E-commerce to Maximize Customer Conversion Rate.**

### **Solution**
The project applies the concept of **Multi-Objective Optimization (MOO)** and the **NSGA-II** algorithm for budget allocation. This approach addresses conflicting factors and determines the optimal budget allocation ratio among various media channels.

## **Libraries and Tools**
The project utilizes a range of data analysis and machine learning libraries to process data, perform optimization, and generate results. Such as- 
- NSGA II
- Multi-Objective Optimization
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Numpy
- Deap

## **Approach and Methodology**

### **Data Processing**
The project begins with data cleaning and preprocessing to ensure that the input data is in a usable format. Key steps include handling missing values, encoding categorical variables, and normalizing numerical features.

### **Algorithm**
The budget allocation algorithm is designed to balance several key metrics:
- **Cost per Click (CPC)**
- **Cost per Conversion (CPC)**
- **Revenue**
- **Conversion Rate**

These metrics guide the distribution of the budget across different advertising channels, aligning with the specific goals of each campaign.

### **NSGA-II Optimization**
**NSGA-II (Non-dominated Sorting Genetic Algorithm II)** was employed to optimize the distribution of the budget. The algorithm focuses on:
- Minimizing the Cost per Click (CPC) and Cost per Conversion (CPC)
- Maximizing Revenue and Conversion Rate

### **Assumptions**
- Each advertising channel receives at least 10% of the total budget.
- Conversion rates and revenue data are accurate and reflect real-time performance.
- There is at least one conflicting factor in budget analysis and distribution (e.g., Revenue vs. Cost/Click or Cost/Conversion).

## **Multi-Objective Optimization (MOO) Technique**

### **What is MOO?**
Multi-Objective Optimization (MOO) involves optimizing multiple conflicting objectives simultaneously. In the context of budget allocation, these objectives include minimizing costs while maximizing conversions and revenue. Instead of a single solution, MOO provides a set of optimal solutions known as the Pareto front, where no objective can be improved without negatively impacting another.

### **Why MOO?**
In real-world marketing and budget allocation scenarios, it's common to have conflicting goals. For example, a campaign might aim to minimize the cost per conversion while maximizing total revenue. MOO allows us to balance these competing objectives, offering a more comprehensive and effective solution.

## **NSGA-II (Non-dominated Sorting Genetic Algorithm II)**

### **What is NSGA-II?**
NSGA-II is an evolutionary algorithm designed to solve multi-objective optimization problems. It is widely used due to its ability to efficiently find a diverse set of Pareto-optimal solutions.

### **How NSGA-II Works**
- **Initialization**: Generates a random population of potential solutions.
- **Non-dominated Sorting**: Solutions are ranked based on dominance, with the best solutions forming the first "front."
- **Crowding Distance Calculation**: Ensures diversity among solutions by ranking them based on how close they are to other solutions.
- **Selection, Crossover, and Mutation**: The algorithm selects the best solutions to form a new population, which is then evolved through crossover and mutation.
- **Convergence**: Over time, the algorithm converges towards the Pareto front, providing a set of solutions that balance multiple objectives.

### **Why NSGA-II?**
NSGA-II is particularly effective for budget allocation problems involving multiple conflicting objectives. Its ability to generate a diverse set of optimal solutions allows decision-makers to choose the best budget allocation strategy according to their specific needs.

### **Application in Budget Distribution**
In this project, NSGA-II was used to optimize budget allocation across different advertising channels. The key objectives were to:
- Minimize Cost per Click (CPC) and Cost per Conversion (CPC)
- Maximize Revenue and Conversion Rate

The use of NSGA-II allowed for a balanced approach to budget distribution, resulting in more informed and strategic decision-making.

## **Conclusion**
This project demonstrates the successful application of advanced optimization techniques in budget distribution. By leveraging MOO and NSGA-II, we achieved an optimized budget allocation strategy that balances conflicting objectives, leading to more effective marketing campaigns.

## **References**
- [Gams](https://www.gams.com/latest/docs/T_LIBINCLUDE_MOO.html)
- [GeeksForGeeks](https://www.geeksforgeeks.org/grey-wolf-optimization-introduction/)
- [NPTEL IIT Guwahati](https://www.youtube.com/watch?v=Aq4pwGn5uWY&t=351s)
- [Wikipedia](https://en.wikipedia.org/wiki/Multi-objective_optimization)
