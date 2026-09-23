#phd

## What the field has established

Although the understanding of the cooperation impact of AI Cognition in hybrid societies of Humans and autonomous agents (AAs) has seen a significant progress, it is still on its embryonic stage. Only in the past few years researchers have started to contribute to the literature, that has now span the fields of evolutionary game theory, organizational theory and behavioral experiments. 

The current state of the art suggests that artificial agents can significantly impact the cooperative dynamics of human societies, even when employing fixed behaviors [[bookerDiscriminatorySamaritanWhich2023|Booker2023]], [[sharmaSmallBotsBig2023|Sharma2023]], [[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[terruchaArtCompensationHow2024|Terrucha2024]], [[quanHumanMachineCooperation2026|Quan2026]]. However, the direction and magnitude of these effects are highly contingent on the dynamics structure, population structure, agent design, and the cognitive evolution over time. Although these 
Let's look at some in particular.

<!--- Dynamics Structure -->

Starting with the dynamics structure, a core finding is that introducing autonomous agents (AAs) into human populations can facilitate or inhibit cooperation depending on the social dilemma structure. 
Cooperative AAs have limited impact in prisoner's dilemma games but facilitate cooperation in stag hunt games, while defective AAs paradoxically promote complete dominance of cooperation in snowdrift games [[guoFacilitatingCooperationHumanagent2023|Guo2023]].
The dynamics effects depend not only on the game itself, but on the game's configurations. In a mixed spatial prisoner's dilemma environment using reinforcement learning–based machine strategies, it was shown that in low-temptation settings, machines strengthen cooperative stability, whereas in high-temptation environments, cooperation relies more on human strategies [[quanHumanMachineCooperation2026|Quan2026]].

<mark style="background:#ff4d4f">add institutions here</mark>

<!--- Population Structure -->

Population structure introduces further dependencies, at various levels. 
Regarding sub-populational proportionality, it has been suggested that the proportion of AAs to humans in a hybrid society play a critical role on cooperation. While increasing the number of agents can foster cooperation, beyond a certain threshold for instance a significant increase in the number of agents can lead to a cooperation collapse [[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[fuOptimalIntegrationIntelligent2026|Fu2026]].
On another level, the populational infrastructure also has a great impact on the overall cooperation dynamics, whether we consider well-mixed populations or structured networks.
Networked populations maintain enhanced cooperation irrespective of imitation strength, while well-mixed populations require weak imitation for agents to be effective [[guoEngineeringOptimalCooperation2024|Guo2024]]. Even a single bot placed at a high-degree node can foster cooperation by reshaping social connections locally [[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[shiradoLocallyNoisyAutonomous2017|Shirado2017]], [[shiradoNetworkEngineeringUsing2020|Shirado2020]].

<!--- Agent Design -->

Agent design comes as a very complex contingency in the AI impact on humans populations. The whole architecture of agents, internal and external, will dictate how AAs behave in the world, shaping the cooperative dynamics of societies.



Studies on the effects of unconditional versus the conditional action have shown that Samaritan-AI agents (that help everyone unconditionally) promote higher cooperation than Discriminatory AI that only helps those considered worthy/cooperative, especially in slow-moving societies where change based on payoff difference is moderate (small intensities of selection) ([[bookerDiscriminatorySamaritanWhich2023|Booker2023]], [[sharmaSmallBotsBig2023|Sharma2023]], [[zimmaroEmergenceCooperationOneshot2024|Zimmaro2024]], [[shiradoNetworkEngineeringUsing2020|Shirado2020]]).
 
Pro-social agents balancing their own payoffs with opponents' foster the highest cooperation, while extreme altruism or pure individualism hinders it [[guoEngineeringOptimalCooperation2024|Guo2024]]. 




Finally we consider the reasoning mechanism. Here we specifically discuss the architecture of the agents' [[research/notes/cognition/Cognitive Profile|cognitive profile]], i.e., how the agent's reasoning repertoire is organized. 

Cognition in hybrid settings has been richly studied, either at dyadic or small-scale groups. At a dyadic-scale, researchers have been focused on understanding coordination dynamics ([[zhaoRoleAdaptationCollective2025|Zhao2025]],[[carrollUtilityLearningHumans2019|Carroll2019]]]), communication ([[pataranutapornInfluencingHumanAI2023|Pataranutaporn2023]], [[zhangInvestigatingAITeammate2023|Zhang2023]], [[crandallCooperatingMachines2018|Crandall2018]]), perception ([[ishowo-olokoBehaviouralEvidenceTransparency2019|Ishowo-oloko2019]], [[karpusAlgorithmExploitationHumans2021|Karpus2021]]) and trust ([[gliksonHumanTrustArtificial2020|Glikson2020]]).
At small-scale groups, researchers have been paying more attention to collective ([[guptaFosteringCollectiveIntelligence2025|Gupta2025]]) and shared cognitions ([[aggarwalSelfbeliefsTransactiveMemory2025|Aggarwal2025]], [[schelbleLetsThinkTogether2022|Schelble2022]]), trust ([[oneillHumanAutonomyTeaming2022|Oneill2022]], [[georgantaWouldYouTrust2024|Georganta2024]]), and team composition and performance ([[mcneeseWhoWhatMy2021|Mcneese2021]]).

Additionally, some frameworks have been proposed aiming to explore the bridging mechanisms that connect dyads to small groups, by treating trust, memory and cognition as a multi-level mechanism rather than properties of a single interaction scale ([[ulfertShapingMultidisciplinaryUnderstanding2024|Ulfert2024]]). This comes as extremely relevant specially attending to the fact that AI exposure affects shared cognition beyond the immediate human-AI interaction ([[riedlCognitiveSpilloverHuman2026|Riedl2026]]). 






This field is, however, mostly focused on general populations of rational individuals, rather than hybrid populations, but nonetheless we can show how different reasoning profiles can drastically change the cooperative dynamics. 

Hybrid populations _have_ been studied at scale — with cognition abstracted to a fixed policy.
<mark style="background:#ff4d4f">add hybrid populations in EGT</mark>


While imitation (social learning) presents the most rational answer, it is not the most frequent heuristic used by humans, as individuals often regard to different reasoning mechanisms. 

Although the usage of these different reasoning types is highly contingent on social and populational structure, their unique nature can  can have major implications in the cooperative dynamics population-wise. 

For instance, conformity-driven individuals can change the equilibria of the game dynamics in well-mixed populations ([[mollemanEffectsConformismCultural2013|MollemanE2013]]), while enhancing network reciprocity in social dilemmas ([[szolnokiConformityEnhancesNetwork2015|Szolnoki2015]]), namely on spatial public goods game ([[quanRationalConformityBehavior2022|Quan2022]]). While these findings are solid, there are caveats: while the most favorable outcomes emerge if the masses conform, forcing leaders to confirm can significantly worsen the overall cooperative performance ([[szolnokiLeadersShouldNot2016|Szolnoki2016]]).

Aspiration-driven individuals can also have great impacts on the game equilibria: independently on the population structure, in non-dyadic games, aspiration favours different strategies than imitation does ([[duAspirationDynamicsMultiplayer2014|Du2014]]). However, mixing aspiration with imitation can promote cooperation in well-mixed populations, but not in structured populations ([[wangEvolutionaryGameDynamics2019|Wang2019]]).


Moving to more deliberative reasoning mechanisms, counterfactual thinking has too a great impact on social dynamics: while a small fraction of counterfactuals may promote high standards of cooperation ([[pereiraCounterfactualThinkingCooperation2019|Pereira2019]]), this effect has a maximum threshold, from which cooperation starts fail ([[fernandesCounterfactualThinkingStochastic2024|Fernandes2024]]). Additionally, these effects are highly contingent of the nature of the game being played.

<mark style="background:#ff4d4f">add theory of mind here</mark>


<!--- Cognitive Evolution -->

Lastly, we have cognitive evolution. Because time is the unconditional factor, the way that the population cognition evolves over time is essential. Here we can discuss culture (?)

This is the big gap, there's not much work here.




<!--- In fact, some findings suggest that introducing autonomous agents (AAs) into human populations can either facilitate or inhibit cooperative action depending on the social dilemma structure. For instance, while AI agents have limited impact in the prisoner's dilemma, it enables cooperation in coordination games, such as the stag hunt, and, paradoxically, promotes complete dominance of cooperation in co-existence games, such as the snowdrift game. 

In another design, it is shown that, in optional prisoner’s dilemma game, AAs operating under unconditionally cooperative bots induce the emergence of cooperation, in both well-mixed populations and a regular lattice under weak imitation scenarios. However, under different circumstances, such as strong imitation, the results vary significantly. These findings emphasize the significance of bot design in promoting cooperation and offer useful insights for encouraging cooperation in real-world scenarios . -->


<!--- [[hanSocialPhysicsAge2026|Han2026]] for the gap -->

## What has been tried on cognition

Whereas most works on cooperation dynamics focus on social learning, assuming individuals are purely rational [ ], many other works have been done in exploring different types of reasoning. While some works focus on incorporating emotions [ ], such as guilt, anger or regret, others try to focus more on the cognitive side exploring, for instance, different update rules, from imitation biases, such as conformism [ ] or prestige [ ], through individual reinforcement based on aspiration levels [ ], to more deliberative mechanisms, such as counterfactual thinking [ ] and theory of mind [ ].

While some works have been done in exploring the impact of AI in society, as a part of a hybrid human-AI society, they are very limited. Agent-based simulations, multi-agent RL, behavioral experiments, all show greater limitations (explain limitations here...(re-do paragraph)). While EGT provides a simple framework that helps exploring the cooperative effects of having different types of agents, reasoning under different cognitive profiles, hybrid human-AI societies are widely unexplored within an EGT approach. Some works have been done, either generally opinions [ ] or very specific situations [Samaritan] but a more general and profound study is lacking.

## What none of this addresses is...

The biggest gap in the field of AI cognition in hybrid populations is the near-total absence of works that examine how AI cognitive capabilities alter cooperative dynamics. Evolutionary game models overwhelmingly use fixed-behavior agents as proxies for AI, explicitly abstracting away cognitive complexity. 

Not only that, but most works consider an AI just as another evolutionary individual that evolves over time, rather than assuming a different species, with distinct motivations, different cognitive profile, unique attributes and, most importantly, that does not reproduce nor imitate for fitness. This overwhelmingly simplifies the real asymmetry between AI and humans, thus providing possibly inaccurate results.


TODO: Guo2023
Although interesting, these insights are highly limited. The authors only consider the simplest social dilemmas, by the dynamics design. AI-AI interactions are not considered

it remains uncertain how they would perform in more complex
scenarios, such as stochastic games and sequential social dilemma games


#### Limitations that we will not address

While these theoretical findings may provide powerful insights, they are bounded to mathematical models in controlled environments that are yet to be empirically validated. While most behavioral studies bridge these models to reality, most experiments assume human-AI pairs, omitting the group (and large group) processes that generate emergent norm expectations [[mutznerBoundedNormativeEquivalence2026|Mutzner2026]].