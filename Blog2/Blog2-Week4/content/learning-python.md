Title: My First Story
Date: 2016-12-07 11:10
Category: Python

Learning python:

python is a very powerful programming language. In this blog I am going to share some of cool stuff I learn during the GA program about python.

One of the cool things I learn was about .copydeepcopy(). In the following paragraphs I will tak about how and when we need to use this command.

Consider you generate a list of data. 

df = [1,2,3,4,5]

Then, you would like to generate a new list which has all the elements of the previous list except the first element. You probably do this steps.

df_new= df[1:]

Although, you did not change the original variable, when you print it, the original data also changes. 
So, what is the solution?

maybe the first solution come to your mind is like this:

df_copy = df

df_new= df_copy[1:]

It is interesting that this solution does not work. The solution I found for it is importing a library with the name "copy" and use it to make a copy of my original data.

import copy
df_copy = copy.deepcopy(df)

df_new= df_copy[1:]

In this way you can make a copy from your data, modify the copy version without being worry about the original data. 


