# Inferring-efficacy-with-RJAGS
On March 22, 2021, Astrazeneca released the results of the phase III trial of their vaccine. From their analysis, it turned out that the vaccine efficacy at preventing symptomatic COVID-19 is 79% and the efficacy against severe or critical disease and hospitalisation is 100% [1]. The results were presented with no uncertainty and, because of how efficacy is defined, do not indicate the likelihood that the next patient will be protected by the vaccine. This created confusion not only in the media, but more importantly about how people interpreted these results, even those with specialized backgrounds. For this reason, I attempted to extrapolate, from the few published data, the full probability density (pdf) of efficacy. The work is based on a previous one concerning the early stages of vaccine trials [2], and through the implementation of a simple model based on a Bayesian Network, processed through Markov Chain Monte Carlo techniques. For inferred efficacy I found (78.0 ± 4.0)% (mean ± standard dev) at preventing symptomatic COVID-19. On the other hand, as far as severe disease is concerned, from the published data, it is impossible to determine a definite conclusion for the efficacy of the vaccine. In particular, I studied how the lack of information on the number of severe placebos drastically changes our knowledge of vaccine efficacy pdf. The results published by Asrazeneca are in agreement with the modal values of the distributions obtained, and this leads us to believe that the method used is consistent with their analysis, however, statements about efficacy against severe cases have been sloppy and have led to important misunderstanding.


Bayesian Network for Symptomatic:

<img width="425" alt="Schermata 2021-05-10 alle 17 39 45" src="https://user-images.githubusercontent.com/83967142/117687593-3c60ae80-b1b8-11eb-928c-b71d45d766fb.png">

Bayesian Network for Severe: 

<img width="533" alt="Schermata 2021-05-10 alle 17 39 26" src="https://user-images.githubusercontent.com/83967142/117687525-2a7f0b80-b1b8-11eb-8e8e-a4096c2bb097.png">

[1] AstraZeneca PLC, News Release, 22 March 2021,https://www.astrazeneca.com/media-centre/press-releases/2021/astrazeneca-us-vaccine-trial-met-primary-endpoint.html

[2] G. D’Agostini and A. Esposito, “What is the probability that a vaccinated person is shielded from Covid-19? A Bayesian MCMC based reanalysis of published data with emphasis on what should be reported as ‘efficacy”’, https://arxiv.org/abs/2102.11022v1
