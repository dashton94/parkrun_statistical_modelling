# Statistical modelling club performance analysis of 5k races (in parkrun)

## Summary  

Jupyter notebook (`python 3`) showcasing methods including: 
- web scraping
- statistical modelling (linear regression & MCMC methods)
- staistical model selection
- numerical integration 
- data visualisations.

## Full overview

In 2019, as a member of the club committee for Southampton based running club Lordshill Road Runners (LRR), I decided to conduct a population analysis of club members in order to investigate the ideal training group boundaries for the club. Weekly training groups set these boundaries based on 5k performance, such that a runner can move between groups based on their present 5k ability.

The basis of this analysis is formed from 5k times recorded by club runners at the local parkrun event, Southampton parkrun. parkrun offers free 5k events globally every Saturday, and is exceptionally popular in Southampton, often drawing over 1000 partipents per week. parkrun results are recorded such that all historical data are publicly accessible. LRR club runners had recorded >20,000 parkrun times at Southampton parkrun by mid-2019 alone.

This notebook takes the times of all LRR club members up to mid-2019, using this sample of recorded 5k times as a proxy for performance at weekly training sessions. It explores methods such as web scraping, statistical modelling (with MCMC methods), model selection and integration, in order to suggest where idealised group boundaries should be set.

This analysis makes several big assumptions: namely that parkrun performance ties with overall ability -- which may fall down if runners choose to run their parkruns at an easy pace (although this may also be true for their traning). Moreover, in assuming all parkrun times by runners to be unweighted and equal, it introduces a bias weighted towards those club runners who complete Southampton parkruns more often, without a gauge as to how often they attend training. Given these working assumptions, I walk through my methodology in this notebook and show how this dataset proves a useful test case for many techniques I employ here.
