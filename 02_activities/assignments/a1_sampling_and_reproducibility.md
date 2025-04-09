# ASSIGNMENT: Sampling and Reproducibility in Python

Read the blog post [Contact tracing can give a biased sample of COVID-19 cases](https://andrewwhitby.com/2020/11/24/contact-tracing-biased/) by Andrew Whitby to understand the context and motivation behind the simulation model we will be examining.

Examine the code in `whitby_covid_tracing.py`. Identify all stages at which sampling is occurring in the model. Describe in words the sampling procedure, referencing the functions used, sample size, sampling frame, any underlying distributions involved, and how these relate to the procedure outlined in the blog post.

Run the Python script file called whitby_covid_tracing.py as is and compare the results to the graphs in the original blog post. Does this code appear to reproduce the graphs from the original blog post?

Modify the number of repetitions in the simulation to 100 (from the original 1000). Run the script multiple times and observe the outputted graphs. Comment on the reproducibility of the results.

Alter the code so that it is reproducible. Describe the changes you made to the code and how they affected the reproducibility of the script file. The output does not need to match Whitby’s original blogpost/graphs, it just needs to produce the same output when run multiple times

# Author: Miyo K. Chatanaka

```
1. Identify all stages at which sampling is occurring in the model based on whitby_covid_tracing.py: 

Sampling is occurring in several places, including line 51 (  ppl.loc[ppl['infected'], 'traced'] = np.random.rand(sum(ppl['infected'])) < TRACE_SUCCESS) and line 56 for secondary contact tracing (  ppl.loc[ppl['event'].isin(events_traced) & ppl['infected'], 'traced'] = True).

2. Describe the sampling procedure, referencing the functions used, sample size, sampling frame, any underlying distributions involved, and how these relate to the procedure outlined in the blog post: 

Our sampling frame is individuals who attended weddings and brunches during COVID 19 in Whitby. 

Our sample size was 1000 people, 200 for weddings and 800 for brunches. 

We performed a Simple Random Sampling with probability sampling, whereby we randomly traced infected individuals with a 20% success rate (primary contact tracing, using the function np.random.rand()), and then selected the traced individuals that attendend a wedding vs a brunch (we needed at least 2 independent cases for each). Here, we stratified them based on the type of event they attended, and only selected the ones that were infected, so we used a purposive sampling technique, which is a non-probability sampling. Because there was a 20% chance of the infected person being traced, only 2 people in weddings were traced, and 13 people in brunches, even though 23 and 77 people were infected respectively. Our probability of wedding infections was 23%.

The underlying distribution was a binomial distribution. Interestingly, the distribution of the infected in weddings versus the traced to weddings is not the same- more people had their infection traced to weddings than the actual infections from weddings.

In the blog post, it mentions that weddings, having a fixed guest list, is easier to trace people from. It takes an example whereby people either went to a wedding (n=2) or a brunch (n=80) exactly 1 time. Supposing that exactly 10% got infected (in our case it was 10% chance of getting infected), 20% of all cases were a result of weddings. If each person has a 10% chance of getting infected, then the distribution was not exactly 20%, as shown in their graph. Unlike in our case, the observed proportion of infections resulting from weddings was closer to 0.5 and had a wide spread, whereas in our case the spread was similar to the true proportion of cases from weddings. Although we used the same probabiliteies, the results were different, perhaps due to the sample size.

3. Does the code appear to reproduce the graphs from the original blog post?

The graphs from the post are quite different from the code. The code true proportion was centered around 23%, whereas in the blog it was around 20%. For the observed proportion in the code, it centered around 20% but in the blog post it centered around 50%. In addition, the spread in the blog post was much larger than in the code. This could be because every time we run the analysis, different random numbers are generated, introducing variability.

4. Modify the number of repetitions in the simulation to 100 (from the original 1000), run the script, comment on the reproducibility of the results:

When we modify the number of repetitions in the simulation to 100, the reproducibility is hindered. This may be due to the law of large numbers, which states that the larger the n is (in this case repetitions of the simulation), the closer the n will be to the true probability of infection. Thus, when n is small, the variability is increased.

5. Describe changes made to the code and how they affected the reproducibility of the script file:

I added the code np.random.seed(123) to the code, because this guarantees that our random numbers will be the same, and thus reproducible.

```


## Criteria

|Criteria|Complete|Incomplete|
|--------|----|----|
|Altercation of the code|The code changes made, made it reproducible.|The code is still not reproducible.|
|Description of changes|The author explained the reasonings for the changes made well.|The author did not explain the reasonings for the changes made well.|

## Submission Information

🚨 **Please review our [Assignment Submission Guide](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md)** 🚨 for detailed instructions on how to format, branch, and submit your work. Following these guidelines is crucial for your submissions to be evaluated correctly.

### Submission Parameters:
* Submission Due Date: `23:59 - 09/04/2025`
* The branch name for your repo should be: `assignment-1`
* What to submit for this assignment:
    * This markdown file (a1_sampling_and_reproducibility.md) should be populated.
    * The `whitby_covid_tracing.py` should be changed.
* What the pull request link should look like for this assignment: `https://github.com/<your_github_username>/sampling/pull/<pr_id>`
    * Open a private window in your browser. Copy and paste the link to your pull request into the address bar. Make sure you can see your pull request properly. This helps the technical facilitator and learning support staff review your submission easily.

Checklist:
- [ ] Create a branch called `assignment-1`.
- [ ] Ensure that the repository is public.
- [ ] Review [the PR description guidelines](https://github.com/UofT-DSI/onboarding/blob/main/onboarding_documents/submissions.md#guidelines-for-pull-request-descriptions) and adhere to them.
- [ ] Verify that the link is accessible in a private browser window.

If you encounter any difficulties or have questions, please don't hesitate to reach out to our team via the help channel in Slack. Our Technical Facilitators and Learning Support staff are here to help you navigate any challenges.
