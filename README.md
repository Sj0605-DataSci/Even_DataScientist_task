# Even_DataScientist_task

## Instructions:

Please provide python code in this notebook answering the 3 questions outlined below to the best of your ability.
Along with this file, you should have received a file called `data_science_task_dataset.csv` containing all the relevant data for this task.

- It should be possible to run the notebook you send back without any local/external dependencies (though feel free to use any python package which can be pip-installed).

- Make sure the notebook is broken up in sections so that it won't be too difficult to read or to know where each question is being answered. Extra points for tidiness and readability!

- Feel free to use any libraries you are comfortable with (as long as they are freely available through pip) for plotting, importing and manipulating data, etc.

- You are encouraged to leave in your thought process and any explorations you did, to show how you went about answering the questions.


## Data structure:

We have given you a (fake) dataset (in `.csv` format), simulating user sign ups to the Even website.

- Each row represents a sign up. However, any person signing up can add their family members, meaning that a row can contain information about multiple individuals. Fields containing commas (i.e. `ages`, `genders`, and `plans`), provide comma-separated information for each person who has been added. So, in the `plans` field: `PLUS, LITE, PLUS` means the person who originally signed up chose the Plus plan, the second person to be added picked Lite, and the third Plus again. This format applies to all fields containing individual level information. Other fields contain a single value which you can assume applies to the whole account/family (i.e. is not on an individual basis).


- Some rows are for users who have simply signed up but not paid whereas others will be for users who have also paid. You can tell who is which, since paid users will have non-blank values for `payment_time`.


- Fields have been labelled in a way that makes their contents easily understood. If something is not clear/unknown you can state whichever assumptions you have made in a "Preamble" in the notebook.


## Questions:

1. After playing around with the data a bit (please leave in a rough "Exploration" section showing how you did that :)), what do you think are 2 crucial data breakdowns or plots to be shown if you were presenting this data to the wider team? If you think multiple options are possible, feel free to say why you picked those 2.


2. Consider the fields `signup_time` and `payment_time`. They stand for the time a given user (who then may add multiple family members) signed up and then paid, respectively. In a single plot, how can you best show the distribution of time "deltas" between the sign up time and payment time (i.e. how long it takes for people to pay once they have signed up)? What is the best way to condense the relevant information and insights? Remember it needs to be a single, static plot, which ideally should not need to be magnified to make sense.


3. You are given the payment amounts but you don't know what the underlying price function is, and what its inputs are (though you can assume they are a subset of the given fields). If you had to treat this as a prediction problem, what kind of model would you use? **PLEASE DO NOT ACTUALLY ATTEMPT MODELLING**. Base your answer on any data exploration you did (and feel free to show plots/stats), but what we are looking is simply a discussion of what may be some of the modelling challenges here and how to pick a model which can overcome them.
