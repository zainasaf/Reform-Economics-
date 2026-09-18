Using the 2024 post-election British Election Study, the script estimates whether economic proximity structures vote choice.
Respondents' self-placements on two 0–10 economic scales (tax-and-spend, and redistribution) are compared with where they place each party, 
and the absolute distance between the two enters a weighted conditional logit  that treats the vote as a single choice among parties
— with a separate proximity coefficient for each party.
Because the quantity of interest is a change in predicted probability rather than a coefficient, the script simulates it directly: it draws 1,000 parameter vectors from the model's sampling distribution, 
and for each party constructs counterfactual datasets in which every voter is placed exactly at that party's position and then moved 1 to 5 points away on the relevant scale, 
averaging the effect across both directions.
The resulting distributions give the average change in each party's vote probability as voter–party distance widens, with 95% intervals, 
