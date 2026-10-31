#phd

## Social dilemmas

The simplest model of cooperation is a symmetric game in which each of two players either cooperates (C) or defects (D). Mutual cooperation yields the reward $R$ to both players and mutual defection the punishment $P$, while a cooperator facing a defector receives the sucker's payoff $S$ and the defector the temptation $T$. The game is a social dilemma when mutual cooperation is better than mutual defection ($R>P$) but each player has an incentive to defect: greed, when exploiting a cooperator pays more than cooperating with it ($T>R$), or fear, when being exploited pays less than defecting ($P>S$) (Macy2002). Which incentives are present defines the three games in Table 1. It is common to fix $R=1$ and $P=0$, so that each game is a region of the plane spanned by $T$ and $S$ (Santos2006b).

**Table 1.** The three social dilemmas used in this thesis.

| Game | Payoff order | Incentive to defect | Best reply to C / to D | Infinite well-mixed population |
| --- | --- | --- | --- | --- |
| Prisoner's dilemma (PD) | $T>R>P>S$ | greed and fear | D / D | defection dominates |
| Stag hunt (SH) | $R>T>P>S$ | fear | C / D | all cooperate or all defect, depending on the initial share of cooperators (bistability) |
| Snowdrift game (SG) | $T>R>S>P$ | greed | D / C | cooperators and defectors coexist |

The three games differ in how the best reply depends on the partner. For a player who maximizes its own payoff, defection is the best reply in the PD whatever the partner does, whereas in the SH the best reply is to match the partner's action, and in the SG to do the opposite. Anticipating a partner's action can therefore change the best action in the SH and the SG, but not in the PD, which is why the PD serves as a control in this thesis. Individuals may also weigh their partner's payoff against their own ([[guoEngineeringOptimalCooperation2024|Guo2024]]). Humans are assumed to give it no weight, and only then is the PD a control: at intermediate weights, the best reply in the PD depends on the partner's action. Repeated, group and fairness games appear in the State of the Art, such as the public goods game, in which contributions to a common pool are multiplied and shared; the collective-risk dilemma, in which a group must reach a contribution target to avoid a probable collective loss; and the ultimatum game, in which a responder accepts or rejects a proposer's split of a sum, but this thesis uses one-shot pairwise games.

## Evolutionary game theory

Evolutionary game theory asks which strategies spread in a population when more successful strategies become more common, through reproduction in biology or imitation in social settings (MaynardSmith1973). In an infinite well-mixed population this process is described by the replicator dynamics, under which the share of a strategy grows when its payoff exceeds the population average (Taylor1978), and which lead to the outcomes in Table 1.

In finite populations, strategy changes are noisy and the process becomes stochastic. Under the pairwise comparison rule, an individual $A$ picks a random role model $B$ and adopts its strategy with probability

$$p_{A\leftarrow B}=\frac{1}{1+e^{-\beta(\pi_B-\pi_A)}},$$

where $\pi_A$ and $\pi_B$ are their payoffs (Szabo1998, Traulsen2006). The intensity of selection $\beta\geq 0$, also called imitation strength, sets how closely imitation follows payoffs: under weak selection ($\beta\to 0$) imitation is almost random, and under strong selection ($\beta\to\infty$) individuals copy only role models that earn more. With a small probability $\mu$, an individual instead adopts a random strategy, which represents exploration or error.

The number of individuals using each strategy then changes as a Markov chain. Without exploration, the population ends up in a state where everyone uses the same strategy, and the probability that a strategy introduced by a single individual takes over, its fixation probability, measures whether selection favors it (Nowak2004). With exploration, the population never settles, and the stationary distribution gives the long-run share of time spent in each state, and hence the average level of cooperation. When exploration is rare, this distribution can be computed from the transitions between homogeneous states alone (Fudenberg2006). These quantities are computed exactly when the number of states allows it, as in populations that mix update rules ([[fernandesCounterfactualThinkingStochastic2024|Fernandes2024]]), and estimated by simulation otherwise.

Two further choices shape the dynamics. The first is when individuals revise: all at once (synchronous updating) or one at a time (asynchronous updating), as in the Moran process (Nowak2004). In structured populations this choice can decide whether cooperation survives (Huberman1993), and so can the order of events within asynchronous updating. On graphs, cooperation can be favored when a random individual dies and is replaced by the offspring of a neighbor chosen according to payoff (death-birth), but not when an individual is first chosen according to payoff to reproduce and its offspring replaces a random neighbor (birth-death) (Ohtsuki2006). In well-mixed populations these choices matter less (Roca2009), although the outcome still depends on how many interactions take place between revisions (Roca2006).

The second choice is with whom individuals interact. In a well-mixed population every pair is equally likely to meet, whereas on a network individuals meet only their neighbors and the outcome depends on the network's structure ([[allenEvolutionaryDynamicsAny2017|Allen2017]]). Between these extremes, assortment is the excess probability of meeting one's own type, and it favors cooperation when it brings cooperators together (Eshel1982). In a hybrid population, assortment can also be by kind: homophilic when individuals meet their own kind more often than chance would predict, and heterophilic when they meet the other kind more often.

The mechanisms through which cooperation can evolve fall into five classes: kin selection, direct reciprocity, indirect reciprocity, network reciprocity and group selection (Nowak2006). A well-mixed population playing one-shot games without reputations has none of them, so selection favors defection in the PD. This is the human-only baseline against which the effect of artificial agents is measured.

## Cognitive profiles

Most evolutionary models describe an individual only by its strategy, the action it takes, and let all individuals revise it with the same update rule, usually payoff-based imitation. This thesis also describes each individual by its cognitive profile, the rule by which it chooses an action and revises that choice. The two levels are kept apart: under a given profile actions change all the time, whereas profiles change only through cognitive evolution, in which profiles rather than actions are copied or selected (Cardillo2010, Bear2016).

We speak of cognitive profiles rather than cognitive architectures, a term that in artificial intelligence denotes complete models of the mind (Kotseruba2020), most of which a population model does not represent. Many frameworks have been proposed to describe artificial agents ([[allmendingerMultiagentAI2026|Allmendinger2026]]), emphasizing aspects as different as the interface between agent and environment ([[stahleDesignSpaceIntelligent2025|Stahle2025]]), communication ([[borghoffHumanartificialInteractionAge2025|Borghoff2025]]) and machine behavior ([[rahwanMachineBehaviour2019|Rahwan2019]]). We adopt the social interaction scale of the OECD AI Capability Indicators ([[oecdIntroducingOECDAI2025|OECD2025]]), which separates an agent's core components (embodiment, social memory and identity) from its social skills (communication, affective skills, social perception and social problem solving), and orders its decision process by sophistication, from pre-set responses, through learning from past interactions, to inferring others' intent and weighing alternative courses of action. Our model represents the decision process and identity, and leaves out embodiment, social memory, affect and communication.

To place a rule on this scale, we ask what information it uses (Table 2), in line with the view of a heuristic as a strategy that ignores part of the available information (Gigerenzer2011). Fixed policies use no information beyond, at most, the partner's observable action, and are never revised; unconditional ones are what evolutionary models call zealots (Masuda2012). Heuristic update rules revise the action from outcomes, observed in others or experienced by the individual itself, without a model of the game or of the partner. Model-free reinforcement learning, which revises the action from the individual's own past payoffs, also belongs to this level ([[guoEngineeringOptimalCooperation2024|Guo2024]], [[quanHumanMachineCooperation2026|Quan2026]]). Deliberative mechanisms use a model of the game, of the partner, or of both. They are usually costlier to apply, and whether deliberation spreads depends on whether its benefit outweighs its cost (Bear2016). The scale therefore classifies decision processes, not technologies: the same agent based on a large language model can be fixed, heuristic or deliberative, depending on what it uses to decide and whether it revises its behavior.

**Table 2.** The cognitive profiles considered in this thesis.

| Level | Rule | Information used | How the action is chosen or revised |
| --- | --- | --- | --- |
| Fixed | Unconditional policy | none | always the same action, e.g. always cooperate |
| Heuristic | Payoff-based imitation | others' actions and payoffs | copies a role model by the pairwise comparison rule |
| Heuristic | Conformity | others' actions | adopts the most common action among those observed ([[szolnokiConformityEnhancesNetwork2015\|Szolnoki2015]]) |
| Heuristic | Aspiration | own payoff | keeps its action if the payoff meets an aspiration level, and switches otherwise ([[duAspirationDynamicsMultiplayer2014\|Du2014]]) |
| Deliberative | Counterfactual thinking | own payoff, the partners' actions and the game | tends to switch if the other action would have earned more against the same partners ([[pereiraCounterfactualThinkingCooperation2019\|Pereira2019]], [[coutoIntrospectionDynamicsSimple2022\|Couto2022]]) |
| Deliberative | Theory of mind | the game and a model of the partner | best-replies to its partner's predicted action, modeling the partner as a reasoner of lower depth (Camerer2004, [[yoshidaGameTheoryMind2008\|Yoshida2008]]) |

## Hybrid populations

A hybrid population is one in which humans and artificial agents interact in the same games ([[hanSocialPhysicsAge2026|Han2026]]). The term has also been used for populations that mix update rules without artificial agents ([[fernandesCounterfactualThinkingStochastic2024|Fernandes2024]]), but here it always refers to these two kinds of individual. An individual's kind is distinct from its strategy and its profile: it does not change, and it may or may not be visible to others. The two kinds play the same games but may differ in their profiles, in whether and when they revise, and in whom they learn from. They may also differ in the information they revise from. A human revises from its own experience, which we call local information, whereas an AI system trained on the interactions of many users, as a language model is, can revise from the experience of all agents of its kind, which we call global information ([[pedreschiHumanAICoevolution2025|Pedreschi2025]]). If individuals learn only from their own kind, the kinds evolve as two coupled populations; if they also learn from the other kind, as one population with two types. The State of the Art reviews how existing models separate the two kinds, and the Framework states the differences assumed here.

> [!TODO]- To add to Zotero (delete this list once done)
> Labels are placeholders in the style of the State of the Art. "Santos2006b" is not the State of the Art's Santos2006. Bear2016 and Cardillo2010 are cited as in the State of the Art (no source note yet). "Checked" says what was actually read; anything marked *listing only* has its title and venue confirmed, but the claim it supports is from memory, so read it before the draft goes out.
>
> | Label | Reference | Checked |
> | --- | --- | --- |
> | Macy2002 | Macy, M. W., & Flache, A. (2002). Learning dynamics in social dilemmas. *PNAS*, 99(suppl. 3), 7229–7236. doi:10.1073/pnas.092080099 | *listing only*: greed and fear definitions |
> | Santos2006b | Santos, F. C., Pacheco, J. M., & Lenaerts, T. (2006). Evolutionary dynamics of social dilemmas in structured heterogeneous populations. *PNAS*, 103(9), 3490–3494. doi:10.1073/pnas.0508201103 | text: R = 1, P = 0, the T–S plane and its game regions |
> | MaynardSmith1973 | Maynard Smith, J., & Price, G. R. (1973). The logic of animal conflict. *Nature*, 246, 15–18. doi:10.1038/246015a0 | *listing only* |
> | Taylor1978 | Taylor, P. D., & Jonker, L. B. (1978). Evolutionary stable strategies and game dynamics. *Mathematical Biosciences*, 40(1–2), 145–156. doi:10.1016/0025-5564(78)90077-9 | title only; one catalogue gives a different volume, so check volume and pages |
> | Szabo1998 | Szabó, G., & Tőke, C. (1998). Evolutionary prisoner's dilemma game on a square lattice. *Physical Review E*, 58(1), 69–73. doi:10.1103/PhysRevE.58.69 | text: the adoption rule with noise K (β = 1/K) |
> | Traulsen2006 | Traulsen, A., Nowak, M. A., & Pacheco, J. M. (2006). Stochastic dynamics of invasion and fixation. *Physical Review E*, 74(1), 011909. doi:10.1103/PhysRevE.74.011909 | abstract: pairwise comparison, Fermi function, intensity of selection |
> | Nowak2004 | Nowak, M. A., Sasaki, A., Taylor, C., & Fudenberg, D. (2004). Emergence of cooperation and evolutionary stability in finite populations. *Nature*, 428, 646–650. doi:10.1038/nature02414 | 9 Oct reading table |
> | Fudenberg2006 | Fudenberg, D., & Imhof, L. A. (2006). Imitation processes with small mutations. *Journal of Economic Theory*, 131(1), 251–262 | abstract: rare mutations, time spent in homogeneous states |
> | Huberman1993 | Huberman, B. A., & Glance, N. S. (1993). Evolutionary games and computer simulations. *PNAS*, 90(16), 7716–7718. doi:10.1073/pnas.90.16.7716 | 9 Oct: abstract |
> | Ohtsuki2006 | Ohtsuki, H., Hauert, C., Lieberman, E., & Nowak, M. A. (2006). A simple rule for the evolution of cooperation on graphs and social networks. *Nature*, 441, 502–505. doi:10.1038/nature04605 | 9 Oct: main text |
> | Roca2006 | Roca, C. P., Cuesta, J. A., & Sánchez, A. (2006). Time scales in evolutionary dynamics. *Physical Review Letters*, 97, 158701. doi:10.1103/PhysRevLett.97.158701 | 9 Oct: abstract and model |
> | Roca2009 | Roca, C. P., Cuesta, J. A., & Sánchez, A. (2009). Evolutionary game theory: Temporal and spatial effects beyond replicator dynamics. *Physics of Life Reviews*, 6(4), 208–249. doi:10.1016/j.plrev.2009.08.001 | 9 Oct: arXiv text (update rules on complete networks); 31 Oct: citation details from the UC3M repository |
> | Nowak2006 | Nowak, M. A. (2006). Five rules for the evolution of cooperation. *Science*, 314(5805), 1560–1563. doi:10.1126/science.1133755 | *listing only* |
> | Eshel1982 | Eshel, I., & Cavalli-Sforza, L. L. (1982). Assortment of encounters and evolution of cooperativeness. *PNAS*, 79(4), 1331–1335. doi:10.1073/pnas.79.4.1331 | *listing only* |
> | Kotseruba2020 | Kotseruba, I., & Tsotsos, J. K. (2020). 40 years of cognitive architectures: core cognitive abilities and practical applications. *Artificial Intelligence Review*, 53(1), 17–94. doi:10.1007/s10462-018-9646-y | arXiv abstract (84 architectures; the abilities listed in the text). Check volume and pages |
> | Gigerenzer2011 | Gigerenzer, G., & Gaissmaier, W. (2011). Heuristic decision making. *Annual Review of Psychology*, 62, 451–482. doi:10.1146/annurev-psych-120709-145346 | *listing only*: the definition was matched by an exact-phrase search |
> | Masuda2012 | Masuda, N. (2012). Evolution of cooperation driven by zealots. *Scientific Reports*, 2, 646. doi:10.1038/srep00646 | 9 Oct: abstract and model |
> | Camerer2004 | Camerer, C. F., Ho, T.-H., & Chong, J.-K. (2004). A cognitive hierarchy model of games. *Quarterly Journal of Economics*, 119(3), 861–898. doi:10.1162/0033553041502225 | *listing only* |

<!---
Original skeleton and taxonomy paragraph (Toino, 30 Sep), kept for reference. The taxonomy now lives, shortened, in "Cognitive profiles".

## Cooperation Games

## Evolutionary Game Theory

## AI Cognitive Architectures

## Hybrid Human-AI Societies


## Taxonomy

The literature on agent design conceptual description is, however, very fragmented, as a large variety of frameworks have been proposed ([[allmendingerMultiagentAI2026|Allmendinger2026]]). Researchers have suggested different frameworks, each emphasizing different aspects of the human-AI collaboration space. 
While some concentrate on specific dimensions, such as agent-environment interface ([[stahleDesignSpaceIntelligent2025|Stahle2025]]), cognitive commitments ([Cila2022]), communication spaces ([[borghoffHumanartificialInteractionAge2025|Borghoff2025]]), or using bidirectional interaction (Human-AI and AI-human) as meta-dimensions ([[dellermannFutureHumanAICollaboration2019|Dellermann2019]]), others rather focus on more high-level concept models, either with focus on AI design as parallelization to humans ([[holterDeconstructingHumanAICollaboration2024a|Holter2024]], [[tremblaySharedMindsCognitive2026|Tremblay2026]]), as machine-architectural centric ([[aboualiAgenticAIComprehensive2025|Ali2025]]), with focus on biology, specifically in ethology ([[rahwanMachineBehaviour2019|Rahwan2019]]), or even reinforcing the need for a multi-disciplinary approach ([[dafoeOpenProblemsCooperative2020|Dafoe2020]]).
--->
