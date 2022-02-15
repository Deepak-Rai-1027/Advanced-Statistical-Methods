# Advanced Statistical Methods
My learning about various advanced statistical methods and it's implementation using R or Python.

# Introduction to Sampling Distributions
In real life scenarios we don't know the population parameter <img src="https://latex.codecogs.com/svg.image?\mu&space;" title="\mu " /> and <img src="https://latex.codecogs.com/svg.image?\sigma&space;" title="\sigma " /> , in this case we have to reply on the sample statistics to estimate these population parameters. When we take a single sample and caclutate the sample mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" />   it is called the point estimator of the population mean <img src="https://latex.codecogs.com/svg.image?\mu&space;" title="\mu " /> . The population parameters is always fixed, however a statistics can assume different values depending on the sample from which it is computed. If we repeat the process of selecting a simple random sample of size ***n*** from a population of size ***N*** over and over again, each time computing the values of sample mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> we will have a distribution of sample mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> . This distribution of the statistics is called the sampling distribution.

## Sampling Distribution of Sample Mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" />
If we consider the process of selecting a simple random sample as an experiement, the sample mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> is the numerical description of the outcome of the experiment. Thus, the sample mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> is a random variable and just like any other random variable it has a mean or expected value <img src="https://latex.codecogs.com/svg.image?E(\overline{x})" title="E(\overline{x})" /> , a standard deviation <img src="https://latex.codecogs.com/svg.image?\sigma&space;/&space;\sqrt{n}&space;" title="\sigma / \sqrt{n} " /> , and a probability distribution of all possible values of the sample mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> .

### It is important to understand here What a Simple Random Sample is?
A ***simple random sample*** of size ***n*** from a population of size ***N*** is a sample selected such that each possible sample of size ***n*** has the same probability ***1/N*** of being selected. There are two ways of selecting a unit from a sample - with replacement and without replacement. 

## Shape of the Sampling Distribution of <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" />
* **Population has a normal distribution:** Here, the sampling distribution of <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> is also normal for any sample size. 
* **Population does not have a normal distribution:** Here, the sampling distribution of <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> is non-normal for small samples, but normal for large samples ( <img src="https://latex.codecogs.com/svg.image?n&space;\geq&space;30" title="n \geq 30" /> ). 
In the example below we will use R-programming to illustrate the effect of sampling distribution of <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> . 
* ***Example:*** Suppose we have been asked to develop a profile of the company's all data science managers. The characteristics to be identified include the mean annual salary for the managers. Now suppose using the details of all the managers in the personnel database we could compute the population mean annual salary <img src="https://latex.codecogs.com/svg.image?\mu&space;" title="\mu " /> = $51,800, and population standard deviation <img src="https://latex.codecogs.com/svg.image?\sigma&space;" title="\sigma " /> = $4000. We will use these population parameters as a reference to check how close our sample mean <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> comes close to the population mean <img src="https://latex.codecogs.com/svg.image?\mu&space;" title="\mu " /> . Now, suppose that we don't have the necessary information on all the managers, and the mean annual salary details is not readily available to us.The question now is how we can obtain estimates of the population parameters by using a sample of managers rather than all the managers in the entire population. Suppose that a sample without replacement of 30 managers will be used. Clearly, the time and the cost of developing a profile would be substantially less for 30 managers than for the entire population. We will expect that the largest concentration of the <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> values and the mean of the 500 <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> values is near to the population mean <img src="https://latex.codecogs.com/svg.image?\mu&space;" title="\mu " /> = $51,800. As per the Central Limit Theorem the mean of all possible <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> values, which is referred to as the expected value of <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> is <img src="https://latex.codecogs.com/svg.image?E(\overline{x})" title="E(\overline{x})" /> = <img src="https://latex.codecogs.com/svg.image?\mu&space;" title="\mu " /> , the expected value or mean of the sampling distribution of <img src="https://latex.codecogs.com/svg.image?\overline{x}" title="\overline{x}" /> is equal to the mean of the population. Hence the mean of all possible sample mean for our example is also $51800.

