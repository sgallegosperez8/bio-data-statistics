# bio-data-statistics 

Attached are associated projects included in biological data

## [gut-microbiome-stat-analysis](https://github.com/sgallegosperez8/bio-data-statistics/tree/main/Projects/gut-data)

Breath H2 emissions were analyzed using a general linear regression model which included years on oral contraceptives as a continuous independent variable, prune diet as a categorical independent variable, and their interaction. The model was run using the anova() function in The R Stats Package. The summary() function of the same package was used to build the linear equations from the model. All analyses were done in R 4.5.2 (R Development Core Team 2025).

Diet (F=4.05; df=1;p=0.052) and the interaction of diet and years on OC (F=2.21; df=1; p=0.146) were not statistically significant in their effect on H2 breath emissions with a significance threshold of 0.05. However, diet is only ~0.02 over this value, so it can be considered slightly significant. Additionally, Years on OC (F=5.51; df=1; p=0.025) did have a significant effect on H2 breath emissions.


## [microbial-comm-stat-analysis](https://github.com/sgallegosperez8/bio-data-statistics/tree/main/microbial-comm-data)

Bacterial relative abundance using a linear mixed model with the lme() function in the “nlme” package (Lindstrom and Bates 1990). Factors including Site, Fire and Season were treated as independent categorical variables and Fire and Season as the interaction. To account for the repeated measures design, Fire and Season were treated as fixed factors and Site as a random factor. The Site variable identified the location where the soil was sampled in or around the Nachusa Grasslands. The Season variable indicated what season the sample was collected and the variable Fire indicated if the Site was burned in the previous season (Mason et al., 2023). The residuals were plotted to assess the model’s assumptions of normality and heteroskedasticity. Because the dataset was unbalanced, the model’s significance was evaluated using the Type III χ ² test through the Anova() function in the “car” package (Fox and Weisberg 2019). Post-Hoc comparisons of the means were evaluated using the emmeans() function from the “emmeans” package (Lenth 2021).  All analyses were done in R 4.5.2 (R Development Core Team 2025).

Based on the Analysis of Deviance Table, there was no significant interaction between fire management and season and how it affects the relative abundance of bacteria (χ = 1.04; df=2; χ ²= 0.592). Independently, Season (χ = 1.35; df=2; χ ²= 0.509) and Fire (χ = 1.40; df=1; χ ²= 0.237) did not show any significant effect on relative abundance either. Bacterial relative abundance was high overall and was not dependent on Season, Fire, or their interaction. With added fire management practices, seasonal abundance rose by 0.05%(Spring), 0.09%(Summer), and 0.17%(Autumn).
