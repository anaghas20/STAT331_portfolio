## Revisions and Reflections

#### Lab 4 Question 6 Feeback: 
##### Revision 1: "You should remove the messages from the summarize() function. I want you to pivot your dataframe to obtain the the differences!"

##### Reflection:
- I received a G on Question 6. I had difficulty figuring out how to find the differences of the means. I was able to get the means of each type of avocado in each region and plotted a graph showing these values. However, Dr. Theobold suggested to pivot the dataframe and that allowed me to create a column that calculated the difference in means. I pivoted the types of avocados wider, which placed the mean prices into a separate column. Then I could calculate the differences between the two types of avocados through mutate(). This changed my bar graph to focus on each region and the difference of average price rather than faceting by each region and displaying the average price. I learned that I just needed to pivot the dataframe wider to create a separate column for the values rather than trying to figure out how to find the difference between each row and column at the same time. 

##### Revision 2: "Statisticians have a hard time with barplots for one summary statistic. To us, barplots are for counts of categorical variables. Can you think of a way to reimagine your plot without bars?"

##### Reflection:
- I got a G on Question 6 again where I used the wrong graph to plot the average price differences of avocado prices in the 4 regions. I had used a bar graph to display this summary statistics. Since I am plotting just one statistic of the average price difference for each of the 4 regions, I changed my graph to a scatterplot to better represent the variables. After talking with Dr. Theobold, I understood that when having one summary statistic, it does not make sense to use a bar graph for plotting the difference in average prices. 

I chose this artifact as I had gotten multiple revisions on it. However after fixing this problem, I was able to understand how to solve similar problems in other labs where I had to pivot longer or wider in order to be able to gather certain data and answer the question. I also was able to understand which types of graphs to use dependning on the type of variable available, which helped in future labs deciding what type of graph to use for numerical and categorical variables.

#### Challenge 3 "Published Comparisons" Feeback: 
##### Revision 1: "Great work! You are on the right track! The next step is to find the differences in these means. Could you use another summarize() step to get these differences?"

##### Reflection:
- I got a G on the Published Comparisons where I did not find a difference of the means. I was able to use summarize() to get the means of each genre's reported artists. However, I struggled at finding the difference of means through R and figured out which genre had the highest difference of means by looking at the values. Through Dr. Theobold’s suggestion, I was able to find a difference of means by using another summarize(). First, I split the task into two pipelines, one for getting the mean values by sex/race and one for finding the difference of those mean values. In the first pipeline, I found the mean of the genre’s reported artists and then had to pivot longer to place those values in another column. I had not done that previously, making it difficult to find the difference without having a column with the values separately. In the second pipeline, I incorporated another summarize() and match() to get the matching elements of the difference of mean reported artist values in the sex/race variables inputted. Through using these two functions I was able to get actual values for the differences rather than looking at the columns to see which genres had the highest difference manually. I learned that it is okay to use summarize() multiple times, and to pivot the data in order to be able to calculate the differences of the values. 


##### Revision 2: "This process is rather convoluted and doesn’t use the tools we’re learning in this. Let’s break down what you are trying to do. You want to find the difference between the male and female mean reported artist for each genre. To me, it would be easier if you pivoted sex to a wider format, so Female and Male are columns. With those columns you could take the difference!"

##### Reflection:
- I got a G on the Published Comparisons where I had used methods we had not learned to find
the difference of means in sex and race. After talking with Dr. Theobold, I learned that I could use pivot_wider() to get the mean values of the two columns wanted (female/male and
white/non-white), after the summarize() and pivot_longer() functions applied to get the mean of each genre's reported artists. Then I applied a mutate function to get the difference of the mean of each genre’s reported artists values in the two columns for sex and race. Rather than trying to find the difference of the 2 variables (female/male and white/non-white), by matching the variables and subtracting the rows, by applying pivot_wider(), I could find the difference of the mean values by subtracting the values in two columns for each row. Using these functions instead made it easier to find the differences of the means since I just had to subtract the two columns to get the results.

I chose this artifact as I had also gotten multiple revisions on it. I went to office hours to understand what I was doing wrong and how I could use tools we had learned in class to answer the question. From this I was able to understand what the question was asking and incorporate a double pivot, which helped solidify my understanding in pivot_longer and pivot_wider.

