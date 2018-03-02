---
title: "Formatting data tables in Spreadsheets"
teaching: 10
exercises: 10
questions:
- "How do we format data in spreadsheets for effective data use?"
objectives:
- "Describe best practices for data entry and formatting in spreadsheets."
- "Apply best practices to arrange variables and observations in a spreadsheet."
keypoints:
- "Never modify your raw data. Always make a copy before making any changes."  
- "Keep track of all of the steps you take to clean your data."  
- "Organize your data according to tidy data principles."  
---

we-Deliver Modifications: **Anelda van der Walt**, **Juan Steyn**<br>
Original Authors: **Christie Bahlai**, **Aleksandra Pawlik**<br>

The most common mistake made is treating treating spreadsheet programs like lab notebooks, that is, 
relying on context, notes in the margin,
spatial layout of data and fields to convey information. As humans, we
can (usually) interpret these things, but computers don't view information the same way, and
unless we explain to the computer what every single thing means (and
that can be hard!), it will not be able to see how our data fit
together.

Using the power of computers, we can manage and analyze data in much more 
effective and faster ways, but to use that power, we have to set up
our data for the computer to be able to understand it (and computers are very 
literal).

This is why it’s extremely important to set up well-formatted
tables from the outset - before you even start entering data from
your very first preliminary experiment. Data organization is the
foundation of your research project. It can make it easier or harder
to work with your data throughout your analysis, so it's worth
thinking about when you're doing your data entry or setting up your
experiment. You can set things up in different ways in spreadsheets,
but some of these choices can limit your ability to work with the data in other programs or
have the you-of-6-months-from-now or your collaborator work with the
data.

> Note: the best layouts/formats (as well as software and
> interfaces) for data entry and data analysis might be
> different. It is important to take this into account, and ideally
> automate the conversion from one to another.

### Keeping track of your analyses

When you're working with spreadsheets, during data clean up or analyses, it's
very easy to end up with a spreadsheet that looks very different from the one
you started with. In order to be able to reproduce your analyses or figure out
what you did when Reviewer #3 asks for a different analysis, you should

- create a new file or tab with your cleaned or analyzed data. Don't modify
the original dataset, or you will never know where you started!
- keep track of the steps you took in your clean up or analysis. You should track 
these steps as you would any step in an experiment. You can
do this in another text file, or a good option is to create a new tab in your spreadsheet
with your notes. This way the notes and data stay together.

This might be an example of a spreadsheet setup:

![spreadsheet setup](../fig/01-format-keeping-notes.png)

Put these principles in to practice today during your Exercises. 


### Structuring data in spreadsheets


The cardinal rules of using spreadsheet programs for data:

1. Put all your variables in columns - the thing you're measuring or that describes your individual
   like 'number_of_twitter_followers' or 'date_collected'.
2. Put each observation in its own row.
3. Don't combine multiple pieces of information in one
   cell. Sometimes it just seems like one thing, but think if that's
   the only way you'll want to be able to use or sort that data.
4. Leave the raw data raw - don't change it!
5. Export the cleaned data to a text-based format like CSV (comma-separated values) format. This
   ensures that anyone can use the data, and is required by
   most data repositories.

For instance, we have data collected from Twitter over different time periods downloaded by different 
student assistants. Each of them collected the data in a slightly different way. 

One of the collected datasets looks like this:

![multiple-info example](../fig/01-format-multiple-values.png)

The problem here is that the handle field also includes the language of the Tweet. So, if we wanted to 
look at the number of languages that were represented in Tweets with the #digitalhumanities hashtag in our dataset, 
it would be hard to extract that information from the spreadsheet in the way that it is currently set up. If instead we created separate columns for the handle and the language of the Tweet, you can see that it would be much easier.  

### Columns for variables and rows for observations

The rule of thumb, when setting up a datasheet, is columns =
variables, rows = observations, cells = data (values).

So, instead we should have:

![single-info example](../fig/01-format-clean-data.png)

> ## Discussion
> If not already discussed, introduce the dataset that will be used in this
> lesson, and in the other digital humanities lessons, the [Summer of #digitalhumanities Twitter data](../Setup). 
>
> This is a real dataset that has been published on Figshare. We’ve simplified it just a little bit for the workshop, but you can download the full dataset and work with it using exactly the same tools we’ll learn about today.  
{: .discussion}


> ## Exercise
> 
> We're going to take a messy version of the Twitter data and describe how we would clean it up.
>
> 1. Download the data by clicking [here](../data/survey_data_spreadsheet_messy.xls) to get it from our repository.
> 2. Open up the data in a spreadsheet program. 
> 3. You can see that there are five tabs. The first tab is a "ReadMe" which you will learn about at the end of the [next episode](02-common-mistakes.md). It describes the data in this document. The second and third tabs were individually collected by our two imaginary student assistants. They both collected the data in their own way. The fourth tab has been created for you to create a copy of the cleaned up data. The fifth tab is where you can keep notes of what you did to clean the data up. 
> Now you're the person in charge of this project and you want to be able to 
> start analyzing the data.   
> 4. With the person next to you, identify what is wrong with this spreadsheet. Also discuss the steps you would need to take to clean up the 2013 and 2014 tabs, and to put them all together in one spreadsheet. 
>
> **Important** Do not forget our first piece of advice, the
> create a new file (or tab) for the cleaned data, never
> modify your original (raw) data.
> 
> After you go through this exercise, we'll discuss as a group what was wrong
> with this data and how you would fix it. 
> 
> > ## Solution
> > - Take about 10 minutes to work on this exercise.
> > - All the mistakes in [02-common-mistakes](../02-common-mistakes) are present in the messy dataset. If
> > exercise is done during a workshop, ask people what they saw as wrong with
> > the data data. As they bring up different points, you can refer to [02-common-mistakes](../02-common-mistakes)
> > or expand a bit on the point they brought up.
> > - If you get a response where they've fixed the date, you can pause and go to the [03-dates-as-data](../03-dates-as-data) lesson. Or you can say you'll come back to dates at the end. 
> {: .solution}
{: .challenge}

An excellent reference, in particular with regard to R scripting is

> Hadley Wickham, *Tidy Data*, Vol. 59, Issue 10, Sep 2014, Journal of
> Statistical Software. [http://www.jstatsoft.org/v59/i10](http://www.jstatsoft.org/v59/i10).


