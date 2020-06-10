# A/B TESTING

A/B tests are used to test changes on a web page by running an experiment where a control group sees the old version, while the experiment group sees the new version. A metric is then chosen to measure the level of engagement from users in each group. These results are then used to judge whether one version is more effective than the other. A/B testing is very much like hypothesis testing with the following hypotheses:

* **Null Hypothesis**: The new version is no better, or even worse, than the old version

* **Alternative Hypothesis**: The new version is better than the old version

If we fail to reject the null hypothesis, the results would suggest keeping the old version. If we reject the null hypothesis, the results would suggest launching the change. These tests can be used for a wide variety of changes, from large feature additions to small adjustments in color, to see what change maximizes your metric the most.

A/B testing also has its drawbacks. It can help you compare two options, but it can't tell you about an option you haven’t considered. It can also produce bias results when tested on existing users, due to factors like change aversion and novelty effect.

* **Change Aversion**: Existing users may give an unfair advantage to the old version, simply because they are unhappy with change, even if it’s ultimately for the better.

*  **Novelty Effect**: Existing users may give an unfair advantage to the new version, because they’re excited or drawn to the change, even if it isn’t any better in the long run.

-----

#### List of things we did in this casestudy
- We computed the observed difference between the metric, average reading duration, for the control and experiment group.

- We simulated the sampling distribution for the difference in means (or average reading durations).

- We used this sampling distribution to simulate the distribution under the null hypothesis, by creating a random normal distribution centered at 0 with the same spread and size.

- We computed the p-value by finding the proportion of values in the null distribution that were greater than our observed difference.

- We used this p-value to determine the statistical significance of our observed difference.

-----

#### Difficulties in A/B Testing

Being able to determine the statistical significance of performance differences in A/B test results is valuable. However, there are many other factors to consider to ensure your A/B tests are successful. In the real world, designing, running, and drawing conclusions from an A/B test to lead you to the right decisions can be tricky.

**Scenario #1**
- EXPERIMENT: Audacity tests a new layout in the classroom to see if it would help engage students. After running an A/B test for two weeks, they find that average classroom times and completion rates decrease with the new layout, and decide against launching the change.

- REALITY: What they don't know, is that the classroom times and completion rates actually increase significantly for new students using the new layout. In the long run, the layout would help existing students too, but they are currently experiencing change aversion.

**Scenario #2**
- EXPERIMENT: Audacity tests a new feature on their landing page that guides users through their course selection process and makes recommendations. After running an A/B test for a month, they find that the click through rates on course pages increase (enrollment rates increase) with the new feature, and decide to launch the change.

- REALITY: What they don't know, is that although the number of total enrollments increase with the new feature, the courses they are purchasing are almost exclusively shorter and cheaper courses, which brings down the revenue for Audacity. It turns out the feature is leading more students to choose more courses with smaller commitments.

**Scenario #3**
- EXPERIMENT: Audacity tests a new description for a difficult course that gets very few enrollments. They hope this description is more exciting and motivates students to take it. After running an A/B test for five weeks, they find that the enrollment rate increases with the new description, and decide to launch the change.

- REALITY: What they don't know, is that although the enrollment rate appears to increase with the new description, the results from this A/B test are unreliable and largely due to chance, because fewer than 40 out of thousands of visitors enrolled during this experiment. This makes even one new student for the course substantially impact the results and potentially even the conclusion

To conclude, here are some common ones to consider.

- Novelty effect and change aversion when existing users first experience a change

- Sufficient traffic and conversions to have significant and repeatable results

- Best metric choice for making the ultimate decision (eg. measuring revenue vs. clicks)

- Long enough run time for the experiment to account for changes in behavior based on time of day/week or seasonal events.

- Practical significance of a conversion rate (the cost of launching a new feature vs. the gain from the increase in conversion)

- Consistency among test subjects in the control and experiment group (imbalance in the population represented in each group can lead to situations like Simpson's Paradox).
