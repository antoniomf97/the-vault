#phd 
# Research Questions

This thesis addresses the two parts of the gap identified previously on the state of the art. It investigates how the cognitive profiles of artificial agents, from fixed policies to heuristic and deliberative mechanisms, affect the evolution of cooperation in hybrid human-AI societies, first with all profiles held fixed, then letting those of humans evolve, and finally letting those of artificial agents change as well. Each step corresponds to one research question.

**RQ1:** Compared with a human-only population, how do the cognitive profiles of artificial agents (fixed, heuristic or deliberative) affect the emergence, stability and evolution of cooperation among humans, and how do the population structure (share of agents) and the dynamics (game protocols, assortment between kinds) change the direction and magnitude of these effects?

_Expected contribution:_ a model of hybrid populations in which artificial agents carry fixed, heuristic or deliberative profiles within a single framework, and a map of the conditions under which each profile raises, lowers or leaves unchanged cooperation among humans.

**RQ2:** When the humans' cognitive profiles evolves over time, which profiles spread among humans under each kind of artificial agent, and do the answers to RQ1 still hold?

_Expected contribution:_ a model in which the humans' profiles evolve, showing which profiles spread under each kind of artificial agent and whether conclusions obtained with a fixed human update rule survive.

**RQ3 (extension):**  When the artificial agents' cognitive profiles are also revised over time, which combinations of human and artificial profiles persist, and do the answers to RQ2 still hold?

_Expected contribution:_ if time allows, a first co-evolutionary model, identifying which combinations of human and artificial profiles persist.

Together, these contributions are expected to show which cognitive profiles of artificial agents support or undermine cooperation among humans, under which conditions, and whether that answer survives once humans adapt to them. This gives those who design, deploy and regulate artificial agents a basis for anticipating their effects on human societies.

# Model

Having established the research questions, we now move on to designing the model on which our results will be built on. Within evolutionary game theory, we model a hybrid population of humans and artificial agents who interact in cooperation games. Every individual carries a cognitive profile, that is, a rule for choosing an action and for revising that choice. The profile of the artificial agents is set by design and is the quantity we compare, while a human-only population serves as the baseline. The three research questions use the same model and relax one assumption at a time. In RQ1 all profiles are held fixed, in RQ2 those of humans evolve, and in RQ3 those of artificial agents are revised as well. We explicitly specify the model along the four dimensions used in the review, population structure, dynamics structure, agent design and cognitive evolution, stating for each what is varied and what is held fixed, the latter being the limitations of this work.

## Population structure

As expected, we will be considering a hybrid population, implying we have two distinct sub-populations or humans and AI agents. As for taxonomy distinction, throughout this work we may address to them as biological and artificial agents.

Regarding the network, we will be adopting a well-mixed approach, meaning each individual will be able to interact with another. In another words, this is the limit where a network is fully connected.

Regarding identity, we must strictly differentiate biological from artificial agents. This separation will be distinct on RQ1/2 and RQ3
1. **Nature:** the agents kind (biological or artificial) is fixed and immutable
2. **Visibility:** each individuals' kind is visible to all; we can assume both AI and humans know the nature of their opponents (But this can be a good direction of future research)
3. **Knowledge:** AI has global knowledge; humans have local knowledge;
4. **Action:** fixed and heuristic reasonings 
5. **Bias:** AI is more heterophilic while humans can vary between homophilic to well mixed
6. **Left out:** we assume agents don't care about reputation, affection, roles, etc


#### Complex environments

when considering cognitive complexity, one ought to explore complex environments as well, so the effects of such rich cognitive processes become visible and identifiable. In hybrid human-AI populations, specifically, we must consider the complex populational structure, rather than assuming the typical homogenous well-mixed populations, highly considered in evolutionary game theory. While some works have been done now assuming heterogeneity ([[vasconcelosClimatePoliciesWealth2014|Vasconcelos2014]], [[kimuraCoevolutionaryNetworksHomophily2008|Kimura2008]][[vasconcelosClimatePoliciesWealth2014|]]), they only consider a factor of homophily, while heterophily (very relevant in current AI companions for instance) remains highly unexplored.

Theory of mind is about simulating others reasoning. Its effects are seen better under complex environments or complex dynamics.

To provide a more complex dynamics, we can assume AI play one game while humans play another (asymmetric protocols). This, however, may introduce an extra variable, thus increasing the complexity of the simulations (?). But if we dont have this how can we model Theory of mind?

## Agent Design


 The field convention is that speed, memory and reasoning cost are the same, regardless of the nature.
   RQ1/2: for higher reasoning, like ToM or CT, memory and reasoning cost are mandatory to be discussed. They are different depending on human/AI AND they can be explicit on the payoff matrix.


Cogntive profile:

RQ1/2: we will assume AI cognitive profile will be fixed, while human cognitive profile will be fixed (RQ1) or variable (RQ2).
AI cognitive profile will be:
1. fixed (always cooperate/always defect)
2. heuristic (immitation)
3. deliberative (ToM and/or CT)

Human cognitive profile will be:
1. empirically provided (stochastic, 50% conformism, 40% heuristic, 10% deliberative) 
2. starts with empirically defined and evolves.
	1. when interact with human imitates, when interact with AI there's a change of changing the profile (we must check papers that support how human reasoning evolve with exposure to AI vs to human)

RQ3: AI cognitive profile will be variable
1. AI interacting with AI will imitate (?) while interacting with human may evolve profile (or its profile may converge towards human profile (?))
	1. we must investigate how could AI reasoning evolve
	2. should AI evolution be conditioned?
	3. AI can evolve with "global" information, while humans only with "local"!

2. RQ1/2: humans can imitate AI while AI doesn't imitate humans
   RQ3: AI will be able to imitate humans as well

3. The field convention is that speed, memory and reasoning cost are the same, regardless of the nature.
   RQ1/2: for higher reasoning, like ToM or CT, memory and reasoning cost are mandatory to be discussed. They are different depending on human/AI AND they can be explicit on the payoff matrix.


#### Human cognitive profiling

As for the human part, a cognitive profiling is highly unexplored. Agents proxies of humans are mostly considered to have a single fixed learning rule, playing a single game, while in reality humans encompass different ones depending on the social situation, environment, and other factors . Moreover, socials situations can be very distinct hence it becomes important to consider different games that represent different situations. However, the oversimplicity that moved us away from realistic proxying can be dethroned when considering a more variable social richness (considering multiple games) and a cognitive profile empirically grounded.

<!---
#### Cultural context

There is a big asymmetry between humans and AI: humans acquiring culture locally from neighbours, AI globally from a training corpus.

Evolução condicionada ou nao?

1. should AI maintain their culture or learn from others?
2. AI

## Taxonomy 

Although the different frameworks offer a wide range of interpretations of how to describe autonomous agent, a more high-level model could be helpful to generalize any conclusions from this work (<mark style="background:#ff4d4f">review this sentence</mark>).

In specific, we propose an framework inspired on the social intelligence of AI ([[oecdIntroducingOECDAI2025|OECD2025]]). This framework conceptually organizes AI agents, separating its social skill dimensions, such as communication, affective, perception and problem-solving skills, from its core components, such as memory, embodiment and identity.

However, some adjustments have to be taken. For instance, embodiment does not have a representation in the formalism of social simulations populational-wise (although we may suggest an open door in this direction as a future direction), meaning for now we can move without it. Consequently, affective skills, namely the expression of emotional states, cannot be represented in its physical dimension, but this is a limitation we are willing to take for now.--->