# MBA 511 Final Exam Study Guide
___
### Calculating averages

###### Simple moving average
<a href="https://www.codecogs.com/eqnedit.php?latex=\frac{\sum_{1}^{n}W_i}{n}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\frac{\sum_{1}^{n}W_i}{n}" title="\frac{\sum_{1}^{n}W_i}{n}" /></a>

In other words, the average of the N most recent items

###### Weighted moving average
<a href="https://www.codecogs.com/eqnedit.php?latex=$X_1*W_1&plus;X_2*W_2&plus;X_3*W_3&plus;...&plus;X_n*W_n$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$X_1*W_1&plus;X_2*W_2&plus;X_3*W_3&plus;...&plus;X_n*W_n$" title="$X_1*W_1+X_2*W_2+X_3*W_3+...+X_n*W_n$" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=Where&space;$\sum_{n}W_n&space;=&space;1$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Where&space;$\sum_{n}W_n&space;=&space;1$" title="Where $\sum_{n}W_n = 1$" /></a>

###### Exponential Smoothing
![Exponential Smoothing](./expsmooth.gif)

![](fsubt.gif) The exponentially smoothed forecast for period *t*
![](fsubtmone.gif) The exponentially smoothed forecast made for the prior period	
![](asubtmone.gif) The actual demand in the prior period
![](alpha.gif) The desired response rate, or smoothing constant

###### Little's Law
<a href="https://www.codecogs.com/eqnedit.php?latex=$L&space;=&space;\lambda&space;W$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$L&space;=&space;\lambda&space;W$" title="$L = \lambda W$" /></a>
Where L is Average number of customers in the store
<a href="https://www.codecogs.com/eqnedit.php?latex=$\lambda$" target="_blank"><img src="https://latex.codecogs.com/gif.latex?$\lambda$" title="$\lambda$" /></a> is the effective arrival rate
W is Average time customer spends in store
___
### Chapter 01

<a href="https://www.codecogs.com/eqnedit.php?latex=Receivable&space;Turnover&space;=&space;\frac{Annual&space;Credit&space;Sales}{Average&space;Account&space;Receivable}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Receivable&space;Turnover&space;=&space;\frac{Annual&space;Credit&space;Sales}{Average&space;Account&space;Receivable}" title="Receivable Turnover = \frac{Annual Credit Sales}{Average Account Receivable}" /></a>


<a href="https://www.codecogs.com/eqnedit.php?latex=Inventory&space;Turnover&space;=&space;\frac{Cost&space;of&space;Goods&space;Sold}{Average&space;Inventory&space;Value}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Inventory&space;Turnover&space;=&space;\frac{Cost&space;of&space;Goods&space;Sold}{Average&space;Inventory&space;Value}" title="Inventory Turnover = \frac{Cost of Goods Sold}{Average Inventory Value}" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=Asset&space;Turnover&space;=&space;\frac{Revenue&space;(or&space;Sales)}{Total&space;Assets}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?Asset&space;Turnover&space;=&space;\frac{Revenue&space;(or&space;Sales)}{Total&space;Assets}" title="Asset Turnover = \frac{Revenue (or Sales)}{Total Assets}" /></a>

```Quicker payments will reduce the average amount of accounts receivables, so the receivables turnover ratio will increase.```


______
### Chapter 4 Critical Path Method

* Top left - Early Start
* Top right - Early Finish
* Bottom left - Late Start
* Bottom right - Late Finish

First propagate through the early starts. Once that is calculated, use back propagation to determine late start.

`Late Start - Early Start = Slack Time`

**Any path with 0 slack time is part of the critical path**

![CPM](./cpm.png)

___
### Chapter 10 Waiting Line Analysis and Simulation

#### Phases and Channels
* Single channel, Single phase
	* Only one line, only one station
	* **Typical example is a single chair barbershop**
* Single channel, Multi phase
	* Only one line, multiple stations
	* **Typical example is a car wash**
		* Users move through vacuums, wetting, washing, rinsing, ect.
* Multichannel, single phase
	* Multiple lines to go through, but each station provides only a single stop
	* **Typical example is a bank teller**
		* A bank has multiple tellers, but a customer will only visit a single teller
* Multichannel, multiphase
	* Multiple lines for multiple services. Similar to a bank teller, except multiple stations.
	* **Typical example is a hospital admission.**
		* User must go to triage, insurance, reception, ect. and multiple help desks exist
___
### Chapter 12 Six Sigma
##### Methodology
1. **Define (D)**
	* Identify customers and their priorities.
	* Identify a project suitable for Six Sigma efforts based on business objectives as well as customer needs and feedback.
	* Identify critical-to-quality characteristics (CTQs) that the customer believes have the most impact on quality.
2. **Measure (M)**
	* Determine how to measure the process and how it is performing.
	* Identify the key internal process that influence CTQs and measure the defects currently generated relative to those processes.
3. **Analyze (A)**
	* Determine the most likely causes of defects.
	* Understand why defects are generated by identifying the key variables most likely to create process variation.
4. **Improve (I)**
	* Identify means to remove the cause of defects
	* Confirm the key variables and quantify their effects on the CTQs.
	* Identify the maximum acceptance ranges of the key variables and a system for measuring deviations of the variables.
	* Modify the process to stay within an acceptable range.
5. **Control (C)**
	* Determine how to maintain the improvements
	* Put tools in place to ensure that the key variables remain within the maximum acceptance ranges under the modified process.

##### Six sigma charts
Chart examples are on page 305 of the textbook

* Flow Charts
  * Used in the define stage of a product
* Run charts
  * Depict trends over time and help in the define stage
* Pareto charts
	* These charts help to break down a problem into the relative contributions of its components, based on the idea that 80% of problems are caused by 20% of causes
* Checksheets
	* These are basic forms that help standardize data collections.
* Fishbone (aka Cause and Effect Diagram)
	* To construct, start with a why? question. Why are pizza deliveries late on Friday and Saturday nights?
	* The rest consists of lines drawn across the page, attached to the problem statement, and several lines or "bones" coming out vertically from the main line.
	
	Fishbone diagram example

	![Fishbone](./fishbone.gif)
___
## Chapter 23 Theory of Constraints

Eli Goldratt in his book *The Goal* observed that improving flow time through a resource that was not a bottleneck would not improve over all production time.

Goldratt's Rules of Production Scheduling
1. Do not balance capacity - balance the flow
2. The level of utilization of a nonbottleneck resource is determined not by its own potential but by some other constraint in the system.
3. Utilization and activation of a resource are not the same.
4. An hour lost at a bottleneck is an hour lost for the entire system
5. An hour saved at a nonbottleneck is a mirage.
6. Bottlenecks govern both throughput and inventory in the system.
7. The transfer batch may not, and many times should not, be equal to the process batch.
8. A process batch should be variable both along its route and in time.
9. Priorities can be set only by examining the system's constraints. Lead time is a derivative of the schedule.