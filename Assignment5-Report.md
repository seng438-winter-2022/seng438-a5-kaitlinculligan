**SENG 438- Software Testing, Reliability, and Quality**

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:      |  8   |
| -------------- | --- |
| Student Names: |  Kaitlin Culligan   |
|                |  Kunal Dhawan   |
|                |  Chloe Bouchard   |
|                |  Jacob Lansang   |

# Introduction
This lab had the purpose of teaching us how to use an integration testing system to analyze the reliability of a system given the failure data of the system, including the time between failures, the failure count, and the execution time of the system. For our lab, we used a combination of CASRE and SRTAT to accomplish these tests. Reliability assessment of a software will be done using a tool called a Reliability Demonstration Chart in Microsoft Excel.
# 

# Assessment Using Reliability Growth Testing 

We used the negative binomial and IFR Salvia & Bollinger models for our graphs. As determined by the results of our model comparison as shown below:
![alt text](https://github.com/seng438-winter-2022/seng438-a5-kaitlinculligan/blob/main/media/mean_comparison_a5.png?raw=true)

Here is our time-between-failures graph:
![alt text](https://github.com/seng438-winter-2022/seng438-a5-kaitlinculligan/blob/main/media/DW3_a5.png?raw=true)

Here is our failure intensity graph:
![alt text](https://github.com/seng438-winter-2022/seng438-a5-kaitlinculligan/blob/main/media/intensity_graph_a5.png?raw=true)

We were unable to get a reliability graph, but we suspect it would look like a standard reliability graph with all data for reliability falling into acceptable ranges. This is due to the time-between-failures graph and failure intensity graph both displaying data in acceptable ranges.

The acceptable range of failure rate for the SUT was anything below 7, which the SUT reached partway through testing. Therefore, the SUT had reached a failure rate which is acceptable given the circumstances. There are several advantages and disadvantages when it comes to using reliabilty growth testing. For starters, reliability growth testing allows for insight into several different metrics of reliability including MTTF, failure intensity and reliability. A drawback to using reliability growth testing is that because it gives a more indepth view, a higher knowledge of the content is required in order to comprehend what is going on.

# Assessment Using Reliability Demonstration Chart 
![image](https://user-images.githubusercontent.com/82078868/161868540-a3111e88-9d66-41f3-8137-14668f49f34a.png)
As shown by this chart, which has a failure rate of 4 failures per 10000 seconds, we were able to assess the reliability of this system using the RDC. We we able to adjust the parameters of the RDC in order to put all points of the chart in the acceptable range of the Reliability Demonstration chart.

![image](https://user-images.githubusercontent.com/82078868/162260920-27541445-8c7b-44e2-a915-07fd66d5d107.png)
This chart shows a failure rate of 3 failures per 10000 seconds, in which almost all points are within the "continue test" range. 


![image](https://user-images.githubusercontent.com/82078868/162261050-4f311809-a502-4e6a-97af-f32b735a4358.png)
This chart shows a failure rate of 2 failures per 10000 seconds, in which all points are within the reject region.

As shown by these charts, we were able to assess the reliability of this system using the RDC. The RDC was able to be used effectively as we were aware of the number of failures as well as the times of each failure. By inputting this failure data, we were able to analyse the trend that the RDC produced. By setting the MTTF to different variables, we observed that the RDC changes to let us know if the software is ready to be released or if it needs to be tested more. We observed that 4 failures per 10000 seconds resulted in the RDC telling us that the software is ready to be released, while a failure rate of 3 or 2 failures per 10000 seconds result in the RDC telling us to continue testing or that the software has failed. 

Overall, the RDC was very useful for analyzing the reliability of this system, but it is limited in that it can only indicate that the SUT is acceptable or not. 

# Comparison of Results

We were able to use both the C-SFRAT and the RDC to assess the reliability of this system. Using the RDC to assess the reliability of the system, we saw that the software that was tested would be acceptable if we set the failure rate to 4 failures per 10000 unit calls. Any more failures past this point means that the system would be unacceptable, as shown by the chart in the previous section. The results from reliability growth testing supported that over time, the system was becoming more reliable, despite there being some spikes in failure intensity during integration testing.

# Discussion on Similarity and Differences of the Two Techniques

Both the techniques helped us understand and interpret the failure rates of data given to us in regard to the expected value. While Reliability growth testing helped us to envisage the entire dataset over a given time range, the Reliability Demonstration chart allowed us to only differentiate certain accepted and rejected conditions. Both techniques allowed us to analyse trends based on different value and datasets. Apart from this, RGA was dependant on failure count in contrast to RDC, which was not. 

To summarise, where reliability growth testing helped us to expand on the system's reliability by presenting us the certain intervals where the system lacks Reliability Demonstration Chart, on the other hand, was predominately used to verify the systems reliability as a whole.

# How the team work/effort was divided and managed

In order to complete parts 1 and 2, we all joined together on a call and one team member shared their screen. All together, we then went through the work together. We collectively decided what to write for our tests, and the person sharing their screen was in charge of writing down our suggestions. This was very effective, since 4 people were tackling a problem at the same time.

# Difficulties encountered, challenges overcome, and lessons learned

We had difficulty getting the tools to work on our computers. We also had issues reformatting the data to make it acceptable to the tools. In the end, we had several group members who were able to determine the issue and solve the problem. Use of the RDC was somewhat difficult as the RDC only accepted 16 observations, so many different parameters needed to be changed in the Plot Data section of the RDC. Much work on the RDC was done through trial and error, but once you are aware of the all the components of the RDC it becomes relatively simple to use.

# Comments/feedback on the lab itself

This lab was interesting and provided valuable insight into reliability assessment. There was some confusion on how exactly we were expected to use the tools to complete the lab. For some team members, 75% of the recommended tools did not work, which made the lab very difficult to complete. Additionally, the tools did not have any helpful instruction manuals available. More explicit instructions in the lab would have been helpful. The fact that the demonstration was a week before the actual submission also added to the confusion as the TAs did not really answer the doubts due to the time constraint.
