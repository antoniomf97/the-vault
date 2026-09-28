#phd 

## What the field has established

In the past few years, the understanding of the cooperation impact of AI Cognition in hybrid societies of Humans and autonomous agents (AAs) has seen a significant progress, despite studies at large-scale still being on its embryonic stage. Only in the past few years researchers have started to contribute to the literature, that has now span the fields of evolutionary game theory, organizational theory and behavioral experiments. 

The current state of the art suggests that artificial agents can significantly impact the cooperative dynamics of human societies, even when employing fixed behaviors ([[bookerDiscriminatorySamaritanWhich2023|Booker2023]], [[sharmaSmallBotsBig2023|Sharma2023]], [[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[terruchaArtCompensationHow2024|Terrucha2024]], [[quanHumanMachineCooperation2026|Quan2026]]). However, the direction and magnitude of these effects are highly contingent on all the default dimensions of large-scale simulations: population structure, dynamics structure, agent design, and the cognitive evolution over time. We will now be looking at each of these dimensions in particular.

<!--- ===== Population Structure===== -->

Starting with the foundation, the population structure is the backbone of large-scale simulations, as it describes the basis of the social environment on which agents can act, at different level. Specifically, we'll look into the social structure, that defines who can interact with who, the individuals' intrinsic nature, which specifies who is the agent, and the population composition, which is specific to what is the overall population composition.

<!--- Social Structure -->

On a first level, the social structure of a population has major impacts on its overall cooperation dynamics. Whether modelled as unstructured well-mixed systems, rigid networks, or even an hybrid intermediate configurations between the two systems, topology fundamentally changes how cooperative behaviors emerge, stabilize, or decay ([[randStaticNetworkStructure2014|Rand2014]], [[allenEvolutionaryDynamicsAny2017|Allen2017]]). Researchers have shown that this result remains unaltered even when considering hybrid societies of human and agents: networked populations maintain enhanced cooperation irrespective of imitation strength, while well-mixed populations require weak imitation for agents to be effective ([[guoEngineeringOptimalCooperation2024|Guo2024]]).

<!---  Intrinsic Nature -->

On a second level, the nature of each individual's intrinsic types heavily impacts cooperation. For instance, while adding a single human node does not show significant consequences, a single bot placed at a high-degree node can foster cooperation by reshaping social connections locally ([[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[shiradoLocallyNoisyAutonomous2017|Shirado2017]], [[shiradoNetworkEngineeringUsing2020|Shirado2020]]).

<!--- Population Composition -->

Lastly, we must also consider the population composition, in specific, the sub-population proportionality. The relative proportions, and relative scales of interacting sub-populations directly govern the survival, spread, and phase transitions of cooperation ([[huangEffectHeterogeneousSubpopulations2015|Huang2015]]). The same is true for hybrid societies, where researchers suggest that the proportion of AAs to humans in a hybrid society play a critical role on cooperation. For instance, while increasing the number of agents can foster cooperation, beyond a certain threshold for instance a significant increase in the number of agents can lead to a cooperation collapse ([[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[fuOptimalIntegrationIntelligent2026|Fu2026]]).

<!--- ===== Dynamics Structure ===== -->

Another important core dimension is the dynamics structure, that intends to describe when, how and with whom the different individuals can interact with. It defines the temporal scheduling, public game-theoretic interaction protocols, and matching mechanisms that govern how artificial agents and humans exchange actions. Recent literature has shown that cooperation rates are highly sensitive to these operational rules, hence determining whether prosocial behaviors spread or collapse ([], []).

<!--- Temporal Scheduling -->

 In fact, starting with temporal scheduling, early multi-agent simulations often relied on rigid, synchronized, turn-based updates with fixed-increment discrete time steps, which introduce artificial synchronization, execution bias, and propagation delays ([]). More importantly, it introduce temporal synchronization errors that fail to capture human behavioral dynamics ([[kosterFastEmbeddedLanguage2024|Koster2024]]). As a result, the state-of-the-art frameworks increasingly deploy event-driven queues and continuous-time loops to capture more realistic social interactions ([[fabriDisentanglingHumanAIHybrids2023|Fabri2023]], [[williamsEventTriggeredFrameworkTrustMediated2025|Williams2025]]).

<!--- Game-Theoretic Protocols -->

On another step, the public game-theoretic protocols matter: introducing autonomous agents (AAs) into human populations can facilitate or inhibit cooperation depending on the social dilemma structure. Cooperative AAs have limited impact in prisoner's dilemma games but facilitate cooperation in stag hunt games, while defective AAs paradoxically promote complete dominance of cooperation in snowdrift games [[guoFacilitatingCooperationHumanagent2023|Guo2023]].
The dynamics effects depend not only on the games' inherent nature (that is, if its whether a coordination, co-existence or C-dominance game), but on the games' configurations. In a mixed spatial prisoner's dilemma environment using reinforcement learning–based machine strategies, it was shown that in low-temptation settings, machines strengthen cooperative stability, whereas in high-temptation environments, cooperation relies more on human strategies ([[quanHumanMachineCooperation2026|Quan2026]]).

Additionally, the interaction temporal framing, that is, the horizon framing substantially alter artificial agent influence. The fact that dilemmas are framed as repeated or one-shot has a major impact on the cooperative dynamics not only under human societies ([[terruchaArtCompensationHow2024|Terrucha2024]], [[akataPlayingRepeatedGames2025|Akata2025]]), but more importantly under hybrid societies ([[barreda-tarrazonaExploitingMachineHuman2026|Barreda-Tarrazona2026]]). As an example, while the likelihood of cooperation does not depend on whether the counterpart is human or artificial in the one-shot Prisoner's Dilemma  games, the same is not true for repeated Prisoner's Dilemma, where cooperation is less likely when participants play with an artificial agent than when they play with other humans ([[barreda-tarrazonaExploitingMachineHuman2026|Barreda-Tarrazona2026]]).

<!--- Matching Mechanisms -->

On a last step, we analyze the matching mechanisms, that is, who interacts with who. Note a major difference between the matching mechanisms and the social structure: while the network says which pairs can meet, the matching rule says which pairs do actually meet. 

Firstly, in multi-populational settings, different sub-populations may have different preferences towards whom they interact with. In large-scale simulations, researchers demonstrated that algorithmic partner choice fundamentally reshapes social dynamics, driving transitions between assortative pairing, human displacement, and cooperative stabilization ([[jiaAsymmetricInteractionPreference2025|Jia2025]]). Here enter the concepts of homophily and heterophily, that is, how likely are individuals to interact with those of the same or other kind, respectively.  For instance, when agents evaluate candidate partners under explicit identity disclosure, humans exhibit an initial aversion toward AI, yet learn to prefer hyper-prosocial AI partners over human alternatives as repeated interactions unfold ([[jiangHumansLearnPrefer2025|Jiang2025]]). This translates in 


<!--- Institutions -->

Lastly, we explore institutions as formalized exogenous rule systems and enforcement protocols that constrain how humans and artificial agents interact. Rather than operating as passive backgrounds, institutional frameworks actively act on the structure of the fitness landscape, dictating whether cooperation elevates or collapses under hybrid systems ([[bartelheimerConceptualizingHybridIntelligent2025|Bartelheimer2025]]).
Researchers have been 



<!--- ===== Agent Design ===== -->

Agent design comes as a very complex contingency in the AI impact on humans populations, as it integrates an elaborate set of dimensions, from its core components, like memory, embodiment and identity, to its more superficial set of social skills, like communication, affection, perception, or problem-solving ([[oecdIntroducingOECDAI2025|OECD2025]]). The whole architecture of agents, will dictate how AAs behave in the world, shaping the cooperative dynamics of societies. 

While hybrid populations have been widely studied at scale, as previously discussed, cognition is typically abstracted to a fixed policy. On the other hand, cognition in hybrid settings has been richly studied, but either at dyadic or small-scale groups, mostly in real scenarios. 
At a dyadic-scale, researchers have been focused on understanding coordination dynamics ([[zhaoRoleAdaptationCollective2025|Zhao2025]],[[carrollUtilityLearningHumans2019|Carroll2019]]]), communication ([[pataranutapornInfluencingHumanAI2023|Pataranutaporn2023]], [[zhangInvestigatingAITeammate2023|Zhang2023]], [[crandallCooperatingMachines2018|Crandall2018]]), perception ([[ishowo-olokoBehaviouralEvidenceTransparency2019|Ishowo-oloko2019]], [[karpusAlgorithmExploitationHumans2021|Karpus2021]]) and trust ([[gliksonHumanTrustArtificial2020|Glikson2020]]). 
At small-scale groups, researchers have been paying more attention to collective ([[guptaFosteringCollectiveIntelligence2025|Gupta2025]]) and shared cognitions ([[aggarwalSelfbeliefsTransactiveMemory2025|Aggarwal2025]], [[schelbleLetsThinkTogether2022|Schelble2022]]), trust ([[oneillHumanAutonomyTeaming2022|Oneill2022]], [[georgantaWouldYouTrust2024|Georganta2024]]), and team composition and performance ([[mcneeseWhoWhatMy2021|Mcneese2021]]).

Additionally, some frameworks have been proposed aiming to explore the bridging mechanisms that connect dyads to small groups, by treating trust, memory and cognition as a multi-level mechanism rather than properties of a single interaction scale ([[ulfertShapingMultidisciplinaryUnderstanding2024|Ulfert2024]]). This comes as extremely relevant attending to the fact that AI exposure affects shared cognition beyond the immediate human-AI interaction, hence implying major effects on larger scale scenarios ([[riedlCognitiveSpilloverHuman2026|Riedl2026]]). 

Under the domain of agent design, research has been spreading in different dimensions.

The first dimension is adaptability, or whether the agent's actions are dependent on its recipient behavior or not, meaning it adapts to the environment. When there's no adaptability, we fall on the sub-space of unconditional bots, that take one same action regardless of their peers responses. Studies on the effects of unconditional versus the conditional action have shown that Samaritan-AI agents (that help everyone unconditionally) promote higher cooperation than Discriminatory AI that only helps those considered worthy/cooperative, especially in slow-moving societies where change based on payoff difference is moderate (small intensities of selection) ([[bookerDiscriminatorySamaritanWhich2023|Booker2023]], [[sharmaSmallBotsBig2023|Sharma2023]], [[zimmaroEmergenceCooperationOneshot2024|Zimmaro2024]], [[shiradoNetworkEngineeringUsing2020|Shirado2020]]).
 
Pro-social agents balancing their own payoffs with opponents' foster the highest cooperation, while extreme altruism or pure individualism hinders it ([[guoEngineeringOptimalCooperation2024|Guo2024]]). 




Finally we consider the reasoning mechanism. Here we specifically discuss the architecture of the agents' [[research/notes/cognition/Cognitive Profile|cognitive profile]], i.e., how the agent's reasoning repertoire is organized. 


While efforts are being made to develop a major understanding of the AI cognitive impact in hybrid populations, human cognition have been widely studied in large-scales simulations. Namely, researchers have shown how different reasoning profiles can drastically change the cooperative dynamics. 


Although imitation (social learning) traditionally presents the most rational answer ([[kendalSocialLearningStrategies2018|Kendal2018]]), it is not the most frequent heuristic used by humans, as individuals often resort to different reasoning mechanisms. 

Despite the usage of these different reasoning types is highly contingent on dynamical and populational structure, their unique nature can have major implications in the cooperative dynamics population-wise. 

For instance, conformity-driven individuals can change the equilibria of the game dynamics in well-mixed populations ([[mollemanEffectsConformismCultural2013|MollemanE2013]]), while enhancing network reciprocity in social dilemmas ([[szolnokiConformityEnhancesNetwork2015|Szolnoki2015]]), namely on spatial public goods game ([[quanRationalConformityBehavior2022|Quan2022]]). While these findings are solid, there are caveats: while the most favorable outcomes emerge if the masses conform, forcing leaders to confirm can significantly worsen the overall cooperative performance ([[szolnokiLeadersShouldNot2016|Szolnoki2016]]).

Aspiration-driven individuals can also have great impacts on the game equilibria: independently on the population structure, in non-dyadic games, aspiration favors different strategies than imitation does ([[duAspirationDynamicsMultiplayer2014|Du2014]]). However, mixing aspiration with imitation can promote cooperation in well-mixed populations, but not in structured populations ([[wangEvolutionaryGameDynamics2019|Wang2019]]).


Moving to more deliberative reasoning mechanisms, counterfactual thinking has too a great impact on social dynamics: while a small fraction of counterfactuals may promote high standards of cooperation ([[pereiraCounterfactualThinkingCooperation2019|Pereira2019]]), this effect has a maximum threshold, from which cooperation starts fail ([[fernandesCounterfactualThinkingStochastic2024|Fernandes2024]]). Additionally, these effects are highly contingent of the nature of the game being played.

<mark style="background:#ff4d4f">add theory of mind here</mark>


<!--- Cognitive Evolution -->

Lastly, we have cognitive evolution. Because time is the unconditional factor, the way that the population cognition evolves naturally have a major impact on the cooperative dynamics. 
In large-scale simulations of hybrid societies, cognitive evolution has advanced beyond rigid payoff matrices toward dynamic generative architectures, active belief updating, and hierarchical social learning. Current research models the mind as an evolving, adaptive engine whose internal representations, cognitive biases, and learning horizons continuously coevolve with cultural and institutional norms. These extra-ordinary flexibility leads to major impacts on the overall cooperation dynamics. 
This effect has been seen in humans, where researchers proposed that cooperation and cognition can coevolve, suggesting that enhanced cognition could have transformed the nature of cooperative dilemmas faced by early humans, thereby explaining the maintenance of cooperation between unrelated partners ([[dossantosCoevolutionCooperationCognition2018|Santos2018]]).
Another example is, when investigating adaptive time dynamics in learning, researchers found that individuals relied more on (conformist) social learning after spatial compared with temporal changes ([[deffnerDynamicSocialLearning2020|Deffner2020]]).


The effects of time are similarly visible in hybrid societies. For instance, researchers have proposed LLM-based agent simulation framework that can bring cognitive realism to this question: agents with varying moral dispositions perceive, remember, reason, and decide in a simulated prehistoric hunter-gatherer society ([[zihengWhyAreWe2025|Ziheng2025]])



we find that cooperation and mutual help are the central driver of evolutionary survival, with universal and reciprocal morality exhibiting the most stable outcomes across conditions while selfishness is strongly disfavored.

we further identify cognition as a central mediator -- most clearly through a cost of moral judgment that shifts the winning moral type across settings, with a self-purging effect among selfish agents as an additional cognitive pattern



strong consensus may be insufficient to guarantee social stability, that the cognitive coherence of belief-systems is vital in determining their ability to spread, and that coherent belief-systems may pose a serious problem for resolving social polarization, due to their ability to prevent consensus even under high levels of social exposure ([[rodriguezCollectiveDynamicsBelief2016|Rodriguez2016]])


<!--- In fact, some findings suggest that introducing autonomous agents (AAs) into human populations can either facilitate or inhibit cooperative action depending on the social dilemma structure. For instance, while AI agents have limited impact in the prisoner's dilemma, it enables cooperation in coordination games, such as the stag hunt, and, paradoxically, promotes complete dominance of cooperation in co-existence games, such as the snowdrift game. 

In another design, it is shown that, in optional prisoner’s dilemma game, AAs operating under unconditionally cooperative bots induce the emergence of cooperation, in both well-mixed populations and a regular lattice under weak imitation scenarios. However, under different circumstances, such as strong imitation, the results vary significantly. These findings emphasize the significance of bot design in promoting cooperation and offer useful insights for encouraging cooperation in real-world scenarios . -->


<!--- [[hanSocialPhysicsAge2026|Han2026]] for the gap -->


<mark style="background:#ff4d4f">add CULTURE here</mark>

## What none of this addresses is...

The biggest gap in the field of AI cognition in hybrid populations is the near-total absence of works that examine how AI cognitive capabilities alter cooperative dynamics. Evolutionary game models overwhelmingly use fixed-behavior agents as proxies for AI, explicitly abstracting away cognitive complexity. 

Not only that, but most works consider an AI just as another evolutionary individual that evolves over time, rather than assuming a different species, with distinct motivations, different cognitive profile, unique attributes and, most importantly, that does not reproduce nor imitate for fitness. This overwhelmingly simplifies the real asymmetry between AI and humans, thus providing possibly inaccurate results.


TODO: Guo2023
Although interesting, these insights are highly limited. The authors only consider the simplest social dilemmas, by the dynamics design. AI-AI interactions are not considered

it remains uncertain how they would perform in more complex
scenarios, such as stochastic games and sequential social dilemma games


#### Limitations that we will not address

While these theoretical findings may provide powerful insights, they are bounded to mathematical models in controlled environments that are yet to be empirically validated. While most behavioral studies bridge these models to reality, most experiments assume human-AI pairs, omitting the group (and large group) processes that generate emergent norm expectations [[mutznerBoundedNormativeEquivalence2026|Mutzner2026]].