#phd 

## What the field has established

In the past few years, the understanding of the cooperation impact of AI Cognition in hybrid societies of humans and autonomous agents (AAs) has seen a significant progress, despite studies at large-scale still being on its embryonic stage. Only in the past few years researchers have started to contribute to the literature, that has now span the fields of evolutionary game theory, organizational theory and behavioral experiments. 

The current state of the art suggests that artificial agents can significantly impact the cooperative dynamics of human societies, even when employing fixed behaviors ([[bookerDiscriminatorySamaritanWhich2023|Booker2023]], [[sharmaSmallBotsBig2023|Sharma2023]], [[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[terruchaArtCompensationHow2024|Terrucha2024]], [[quanHumanMachineCooperation2026|Quan2026]]). However, the direction and magnitude of these effects are highly contingent on all the default dimensions of large-scale simulations: population structure, dynamics structure, agent design, and the cognitive evolution over time. We will now be looking at each of these dimensions in particular.

<!--- ===== Population Structure===== -->

Starting with the foundation, the population structure is the backbone of large-scale simulations, as it describes the basis of the social environment on which agents can act, at different level. Specifically, we'll look into the social structure, that defines who can interact with who, the individuals' intrinsic nature, which specifies who is the agent, and the population composition, which is specific to what is the overall population composition.

<!--- Social Structure -->

On a first level, the social structure of a population has major impacts on its overall cooperation dynamics. Whether modelled as unstructured well-mixed systems, rigid networks, or even an hybrid intermediate configurations between the two systems, topology fundamentally changes how cooperative behaviors emerge, stabilize, or decay ([[randStaticNetworkStructure2014|Rand2014]], [[allenEvolutionaryDynamicsAny2017|Allen2017]]). Researchers have shown that this result remains unaltered even when considering hybrid societies of human and agents: networked populations maintain enhanced cooperation irrespective of imitation strength, while well-mixed populations require weak imitation for agents to be effective ([[guoEngineeringOptimalCooperation2024|Guo2024]]).

<!---  Intrinsic Nature -->

On a second level, the intrinsic nature of each individual, that is, whether it is a human or an artificial agent, heavily impacts cooperation. Direct empirical and theoretical comparisons show that interacting with a human elicits different communicative patterns, emotional evaluations, and relational expectations than interacting with an artificial intelligence system ([[guzmanOntologicalBoundariesHumans2020|Guzman2020]], [[mouMediaInequalityComparing2017|Mou2017]]). This effect operates partly through belief: what others think an agent is matters independently of how it behaves. In a repeated prisoner's dilemma where participants were given true or false information about their partner's nature, bots were better than humans at inducing cooperation, but lost this advantage once disclosed as bots, and participants did not recover from their bias against bots over time ([[ishowo-olokoBehaviouralEvidenceTransparency2019|Ishowo-Oloko2019]]). Conversely, when identity is hidden, humans misattribute bot behavior to humans and vice versa, even when the bots are more prosocial and linguistically distinguishable ([[jiangHumansLearnPrefer2025|Jiang2025]]). 
The effect of disclosure is not uniform, however. In network experiments, bots improved human coordination and cooperation even when participants knew they were interacting with bots ([[shiradoLocallyNoisyAutonomous2017|Shirado2017]], [[shiradoNetworkEngineeringUsing2020|Shirado2020]]). Evolutionary models also show that identifiability matters: when human-like agents can tell whether a co-player is human or artificial, cooperation is enhanced when they disregard the AI's performance ([[zimmaroEmergenceCooperationOneshot2024|Zimmaro2024]]). This reveals the impact that each individual's intrinsic nature, and its visibility to others, has in hybrid societies.

<!--- Population Composition -->

Lastly, we must also consider the population composition, in specific, the sub-population proportionality. The relative proportions, and relative scales of interacting sub-populations directly govern the survival, spread, and phase transitions of cooperation ([[huangEffectHeterogeneousSubpopulations2015|Huang2015]]). The same is true for hybrid societies, where researchers suggest that the proportion of AAs to humans in a hybrid society play a critical role on cooperation. For instance, while increasing the number of agents can foster cooperation, beyond a certain threshold for instance a significant increase in the number of agents can lead to a cooperation collapse ([[guoFacilitatingCooperationHumanagent2023|Guo2023]], [[fuOptimalIntegrationIntelligent2026|Fu2026]]).

<!--- ===== Dynamics Structure ===== -->

The dynamics structure, although arguably yet another part of the population structure, is rich enough to be a core component of large-scale simulations in its own right. It defines the temporal scheduling, which defines when individuals can interact; the public game-theoretic interaction protocols, which demonstrate the rules of how the interactions unfold; and the matching mechanisms, which determine who interacts with whom, among humans and artificial agents alike. Recent literature has shown that cooperation rates are highly sensitive to these operational rules, hence determining whether prosocial behaviors spread or collapse ([], []).

<!--- Temporal Scheduling -->

Starting with temporal scheduling, early multi-agent simulations often relied on rigid, synchronized, turn-based updates with fixed-increment discrete time steps, which introduce artificial synchronization, execution bias, and propagation delays ([]). More importantly, it introduce temporal synchronization errors that fail to capture human behavioral dynamics ([[kosterFastEmbeddedLanguage2024|Koster2024]]). As a result, the state-of-the-art frameworks increasingly deploy event-driven queues and continuous-time loops to capture more realistic social interactions ([[fabriDisentanglingHumanAIHybrids2023|Fabri2023]], [[williamsEventTriggeredFrameworkTrustMediated2025|Williams2025]]).

<!--- Game-Theoretic Protocols -->

On another step, the public game-theoretic protocols matter: introducing autonomous agents (AAs) into human populations can facilitate or inhibit cooperation depending on the social dilemma structure. Cooperative AAs have limited impact in prisoner's dilemma games but facilitate cooperation in stag hunt games, while defective AAs paradoxically promote complete dominance of cooperation in snowdrift games ([[guoFacilitatingCooperationHumanagent2023|Guo2023]]).
The dynamics effects depend not only on the games' inherent nature (that is, if its whether a coordination, co-existence or C-dominance game), but on the games' configurations. In a mixed spatial prisoner's dilemma environment using reinforcement learning–based machine strategies, it was shown that in low-temptation settings, machines strengthen cooperative stability, whereas in high-temptation environments, cooperation relies more on human strategies ([[quanHumanMachineCooperation2026|Quan2026]]).

Additionally, the interaction temporal framing, that is, the horizon framing substantially alter artificial agent influence. The fact that dilemmas are framed as repeated or one-shot has a major impact on the cooperative dynamics not only under human societies ([[terruchaArtCompensationHow2024|Terrucha2024]], [[akataPlayingRepeatedGames2025|Akata2025]]), but more importantly under hybrid societies ([[barreda-tarrazonaExploitingMachineHuman2026|Barreda-Tarrazona2026]]). As an example, while the likelihood of cooperation does not depend on whether the counterpart is human or artificial in the one-shot Prisoner's Dilemma  games, the same is not true for repeated Prisoner's Dilemma, where cooperation is less likely when participants play with an artificial agent than when they play with other humans ([[barreda-tarrazonaExploitingMachineHuman2026|Barreda-Tarrazona2026]]).

<!--- Matching Mechanisms -->

On a last step, we analyze the matching mechanisms, that is, who interacts with whom. 
We first reinforce that matching should be distinguished from the social structure: while the network determines which pairs can meet, the matching rule determines which pairs actually do. In hybrid human-AI societies, matching mechanisms govern partner formation, task allocation, and coalition structuring between humans and artificial agents. Rather than assuming static random mixing, recent advances formalize matching as an endogenous process. This view builds on evolutionary models in which cooperation prevails when individuals can adjust their social ties (Santos2006), and on network experiments in which people sever links with defectors and form new ones with cooperators (Rand2011). We organize this literature around three mechanisms: strategic partner selection, capability complementarity, and network assortment.

Strategic partner selection is a deliberate decision that establishes matching based on what individuals know about their partners, specifically on how one expects them to behave. In collective-risk dilemmas involving humans and artificial agents, participants follow outcome-based rules: those whose group failed prefer teams without defectors, whereas those whose group succeeded become more lenient (Santos2020). Humans' preferences among reinforcement-learning partners also track the agents' perceived warmth and competence, beyond their objective performance (McKee2024). 

Partner choice also interacts with the identity effects discussed above. In a communication-based partner-selection game, disclosed LLM bots were initially selected less often, but gradually outcompeted human candidates as selectors learned how each partner type behaved ([[jiangHumansLearnPrefer2025|Jiang2025]]). Additionally, matching can also be delegated to AI. A deep reinforcement learning social planner that recommends which ties to form or break fostered cooperation in human groups, not by isolating defectors but by embedding them in small cooperative neighborhoods (McKee2023). Autonomous agents that engineer network connections likewise increased cooperation (Shirado2020).

Capability complementarity is a process of matching based on individuals complementarity, where individuals' different skills make the pair more productive than either would be alone. While empirical meta-analyses indicate that combining human and machine capabilities does not automatically guarantee synergy ([[vaccaroWhenCombinationsHumans2024|Vaccaro2024]]), newer frameworks characterize the conditions under which human-AI teams outperform both humans and AI alone ([[gonzalezScienceHumanAI2026|Gonzalez2026]]). In assignment problems, confidence-based deferral systems let the algorithm make part of the matching decisions and route the rest to humans ([[arnaiz-rodriguezHumanAIComplementarityMatching2025|Arnaiz-Rodriguez2025]]). Complementarity also operates at the level of team composition: replacing some group members with artificial agents can enhance cooperation in collective-risk dilemmas, but only under specific conditions ([[terruchaArtCompensationHow2024|Terrucha2024]]).

Lastly, researchers have seen the impact of matching in the cooperative dynamics based on network assortment, i. e., a pattern that establishes matching between individuals based on how physically or socially closed they are. This is the case of homophilic or heterophilic matching, that show how likely are individuals to interact with those of the same or other kind, respectively. 

In spatial hybrid games, when agents evaluate candidate partners under explicit identity disclosure, humans exhibit an initial homophilic behavior, presenting aversion toward AI, yet learn to prefer hyper-prosocial AI partners over human alternatives as repeated interactions unfold ([[jiangHumansLearnPrefer2025|Jiang2025]]). 
Structural role asymmetries, such as distinguishing between offer proposers and responders, also fundamentally alter strategic selection and the evolutionary stability of fairness in hybrid populations ([[cimpeanuPromotingFairProposers2021|Cimpeanu2021]]). In fact, evolutionary game-theoretic models show that unconditional generosity can fail in asymmetric environments, whereas conditional enforcement mechanisms systematically stabilize equitable norms ([[songEvolutionFairnessHybrid2026|Song2026]]). 
Finally, we mention that topological hub placement magnifies influence: inserting autonomous agents into high-degree nodes steers hybrid equilibria, whereas uncoordinated delegation risks sociotechnical lock-in ([[guoFacilitatingCooperationHumanagent2023|Guo2023]]). 



In large-scale simulations, researchers demonstrated that algorithmic partner choice fundamentally reshapes social dynamics, driving transitions between assortative pairing, human displacement, and cooperative stabilization ([[jiaAsymmetricInteractionPreference2025|Jia2025]]). 


<!--- Institutions -->

Lastly, we explore institutions as formalized exogenous rule systems and enforcement protocols that constrain how humans and artificial agents interact. Rather than operating as passive backgrounds, institutional frameworks actively act on the structure of the fitness landscape, dictating whether cooperation elevates or collapses under hybrid systems ([[bartelheimerConceptualizingHybridIntelligent2025|Bartelheimer2025]]). Researchers have been formalizing this view in evolutionary game theory. Pre-funded sanctioning institutions can outcompete peer punishment ([[sigmundSocialLearningPromotes2010|Sigmund2010]]), and switching adaptively from rewards to penalties minimizes the advantage of defectors ([[chenFirstCarrotThen2015|Chen2015]]), although maximizing cooperation need does not maximize social welfare ([[hanEvolutionaryMechanismsThat2024|Han2024]]). Despite these results being focused on a human-centered environment, recent work extends these models to hybrid populations. AI agents that help only cooperators, or that reduce disagreement over reputations, can sustain human cooperation ([[zimmaroEmergenceCooperationOneshot2024|Zimmaro2024]]). By contrast, rules imposed on the agents themselves, such as requiring them to always cooperate, fail to raise human cooperation ([[hintzePromotingCooperationPublic2026|Hintze2026]]). Yet most studies treat AI as a fixed-strategy participant under static, human-designed rules, and how institutions co-evolve with the humans and AI agents they govern remains open ([[hanSocialPhysicsAge2026|Han2026]]).

<!--- ===== Agent Design ===== -->

Agent design comes as a very complex contingency in the AI impact on humans populations, as it integrates an elaborate set of dimensions, from its core components, like memory, embodiment and identity, to its more superficial set of social skills, like communication, affection, perception, or problem-solving ([[oecdIntroducingOECDAI2025|OECD2025]]). The whole architecture of agents, will dictate how AAs behave in the world, shaping the cooperative dynamics of societies. 

While hybrid populations have been widely studied at scale, as previously discussed, cognition is typically abstracted to a fixed policy. On the other hand, cognition in hybrid settings has been richly studied, but either at dyadic or small-scale groups, mostly in real scenarios. 
At a dyadic-scale, researchers have been focused on understanding coordination dynamics ([[zhaoRoleAdaptationCollective2025|Zhao2025]],[[carrollUtilityLearningHumans2019|Carroll2019]]]), communication ([[pataranutapornInfluencingHumanAI2023|Pataranutaporn2023]], [[zhangInvestigatingAITeammate2023|Zhang2023]], [[crandallCooperatingMachines2018|Crandall2018]]), perception ([[ishowo-olokoBehaviouralEvidenceTransparency2019|Ishowo-oloko2019]], [[karpusAlgorithmExploitationHumans2021|Karpus2021]]) and trust ([[gliksonHumanTrustArtificial2020|Glikson2020]]). 
At small-scale groups, researchers have been paying more attention to collective ([[guptaFosteringCollectiveIntelligence2025|Gupta2025]]) and shared cognitions ([[aggarwalSelfbeliefsTransactiveMemory2025|Aggarwal2025]], [[schelbleLetsThinkTogether2022|Schelble2022]]), trust ([[oneillHumanAutonomyTeaming2022|Oneill2022]], [[georgantaWouldYouTrust2024|Georganta2024]]), and team composition and performance ([[mcneeseWhoWhatMy2021|Mcneese2021]]).

Additionally, some frameworks have been proposed aiming to explore the bridging mechanisms that connect dyads to small groups, by treating trust, memory and cognition as a multi-level mechanism rather than properties of a single interaction scale ([[ulfertShapingMultidisciplinaryUnderstanding2024|Ulfert2024]]). This comes as extremely relevant attending to the fact that AI exposure affects shared cognition beyond the immediate human-AI interaction, hence implying major effects on larger scale scenarios ([[riedlCognitiveSpilloverHuman2026|Riedl2026]]). 

Under the domain of agent design, research has been spreading in different dimensions.

The first dimension is adaptability, or whether the agent's actions are dependent on its recipient behavior or not, meaning it adapts to the environment. When there's no adaptability, we fall on the sub-space of unconditional bots, that take one same action regardless of their peers responses. Studies on the effects of unconditional versus the conditional action have shown that Samaritan-AI agents (that help everyone unconditionally) promote higher cooperation than Discriminatory AI that only helps those considered worthy/cooperative, especially in slow-moving societies where change based on payoff difference is moderate (small intensities of selection) ([[bookerDiscriminatorySamaritanWhich2023|Booker2023]], [[sharmaSmallBotsBig2023|Sharma2023]], [[zimmaroEmergenceCooperationOneshot2024|Zimmaro2024]], [[shiradoNetworkEngineeringUsing2020|Shirado2020]]).
 
Pro-social agents balancing their own payoffs with opponents' foster the highest cooperation, while extreme altruism or pure individualism hinders it ([[guoEngineeringOptimalCooperation2024|Guo2024]]). 


Finally, we reinforce the relevance of the reasoning mechanism in its effects on the cooperative dynamics. In specific, we discuss the architecture of the agents' cognitive profile, i. e., how the agent's reasoning repertoire is organized.

While efforts are being made towards better understanding of some of the AI reasoning mechanisms and its impacts in hybrid populations, the effects of richer reasoning repertoire in cooperation has been widely studied in large-scale simulations. In fact, researchers have shown how different reasoning profiles can drastically change the cooperative dynamics in populations. 

While imitation (social learning) traditionally presents the most rational answer ([[kendalSocialLearningStrategies2018|Kendal2018]]), it is not the most frequent heuristic used by humans, as individuals often resort to different reasoning mechanisms. Despite the usage of these different reasoning types being highly contingent on dynamical and populational structure, their unique nature can have major implications in the cooperative dynamics population-wise. 

For instance, conformity-driven individuals can change the equilibria of the game dynamics in well-mixed populations ([[mollemanEffectsConformismCultural2013|MollemanE2013]]), while enhancing network reciprocity in social dilemmas ([[szolnokiConformityEnhancesNetwork2015|Szolnoki2015]]), namely on spatial public goods game ([[quanRationalConformityBehavior2022|Quan2022]]). While these findings are solid, there are caveats: while the most favorable outcomes emerge if the masses conform, forcing leaders to confirm can significantly worsen the overall cooperative performance ([[szolnokiLeadersShouldNot2016|Szolnoki2016]]).

Aspiration-driven individuals can also have great impacts on the game equilibria: independently on the population structure, in non-dyadic games, aspiration favors different strategies than imitation does ([[duAspirationDynamicsMultiplayer2014|Du2014]]). However, mixing aspiration with imitation can promote cooperation in well-mixed populations, but not in structured populations ([[wangEvolutionaryGameDynamics2019|Wang2019]]).

In a more deliberative side, counterfactual thinking has too a great impact on social dynamics: while a small fraction of counterfactuals may promote high standards of cooperation in coordination games ([[pereiraCounterfactualThinkingCooperation2019|Pereira2019]]), this effect has a maximum threshold, from which cooperation starts to collapse ([[fernandesCounterfactualThinkingStochastic2024|Fernandes2024]]). Additionally, these effects are highly contingent of the nature of the game being played.

Finally, the impact of theory of mind (ToM) in cooperation has also seen an expanding literature. In fact, researchers have been exploring the effects of ToM in cooperative dynamics, particularly in sequential games. 


We show it is possible to deduce whether players make inferences about each other and quantify their sophistication on the basis of choices in sequential games ([[yoshidaGameTheoryMind2008|Yoshida2008]]).

<mark style="background:#ff4d4f">add theory of mind here</mark>

<!--- ===== Cognitive Evolution ===== -->

Lastly, we have cognitive evolution. Because time is the unconditional factor, the way that the population cognition evolves naturally have a major impact on the cooperative dynamics. 
In large-scale simulations, cognitive evolution has advanced beyond rigid payoff matrices toward dynamic generative architectures, active belief updating, and hierarchical social learning. Current research models the mind as an evolving, adaptive engine whose internal representations, cognitive biases, and learning horizons continuously coevolve with cultural and institutional norms. These extra-ordinary flexibility leads to major impacts on the overall cooperation dynamics. 
This effect has been seen in humans, where researchers proposed that cooperation and cognition can coevolve, suggesting that enhanced cognition could have transformed the nature of cooperative dilemmas faced by early humans, thereby explaining the maintenance of cooperation between unrelated partners ([[dossantosCoevolutionCooperationCognition2018|Santos2018]]).
Another example is, when investigating adaptive time dynamics in learning, researchers found that individuals relied more on (conformist) social learning after spatial compared with temporal changes ([[deffnerDynamicSocialLearning2020|Deffner2020]]).
The evolution of beliefs

strong consensus may be insufficient to guarantee social stability, that the cognitive coherence of belief-systems is vital in determining their ability to spread, and that coherent belief-systems may pose a serious problem for resolving social polarization, due to their ability to prevent consensus even under high levels of social exposure ([[rodriguezCollectiveDynamicsBelief2016|Rodriguez2016]])



The effects of time are similarly visible in hybrid societies. For instance, researchers have proposed LLM-based agent simulation framework that can bring cognitive realism to this question: agents with varying moral dispositions perceive, remember, reason, and decide in a simulated prehistoric hunter-gatherer society ([[zihengWhyAreWe2025|Ziheng2025]])



we find that cooperation and mutual help are the central driver of evolutionary survival, with universal and reciprocal morality exhibiting the most stable outcomes across conditions while selfishness is strongly disfavored.

we further identify cognition as a central mediator -- most clearly through a cost of moral judgment that shifts the winning moral type across settings, with a self-purging effect among selfish agents as an additional cognitive pattern



<!--- [[hanSocialPhysicsAge2026|Han2026]] for the gap -->


<mark style="background:#ff4d4f">add CULTURE here</mark>

## What none of this addresses is...

We have explored many different works on a wide set of dimensions under the topic of the cooperative impact of AI Cognition in hybrid societies, coming to a final conclusion that reinforces the initial premise: artificial agents can significantly impact the cooperative dynamics of societies, but this impact is highly contingent on the populational and dynamical structures, on the agent design and on the cognitive evolution. 

However, none of these works specifically explores how AI cognitive profiles and their evolutions affect the emergence and stability of cooperation in large-scale hybrid societies. 

Some works have partially explored the evolution of cognition, but using a very general approach, considering it as an abstract trait rather than distinct reasoning types, and only focused in humans ([[dossantosCoevolutionCooperationCognition2018|dos Santos2018]]), or only focused on the beliefs ([[rodriguezCollectiveDynamicsBelief2016|Rodriguez2016]]). Others have studied asymmetric human-AI interactions in large hybrid populations, but softening human-AI distinction, assuming the most significant difference between agents and humans is the flexibility of decision, while restricting the game-protocol to a Prisoner's Dilemma ([[jiaAsymmetricInteractionPreference2025|Jia2025]]).

Additionally, works on the Samaritan vs discriminatory AI have explored the effects of bots in societies, but restricted to AI fixed designs ([[songEvolutionFairnessHybrid2026|song2026]], [[bookerDiscriminatorySamaritanWhich2023|booker2023]], [[zimmaroEmergenceCooperationOneshot2024|Zimmaro2024]]). Finally, some works have proposed reinforcement learning as the reasoning mechanism of AI, although assuming a fixed cognitive profile ([[quanHumanMachineCooperation2026|Quan2026]]).

<!---
While these theoretical findings may provide powerful insights, they are bounded to mathematical models in controlled environments that are yet to be empirically validated. While most behavioral studies bridge these models to reality, most experiments assume human-AI pairs, omitting the group (and large group) processes that generate emergent norm expectations /[[mutznerBoundedNormativeEquivalence2026|Mutzner2026]](.--->