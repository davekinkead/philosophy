---
bibtex: @InCollection{sep-social-choice,
  author       =  {List, Christian},
  title        =  {Social Choice Theory},
  booktitle    =  {The Stanford Encyclopedia of Philosophy},
  editor       =  {Edward N. Zalta},
  howpublished =  {\url{http://plato.stanford.edu/archives/win2013/entries/social-choice/}},
  year         =  {2013},
  edition      =  {Winter 2013},
}
---

# Social Choice Theory

> Condorcet anticipated a key theme of modern social choice theory: majority rule is at once a plausible method of collective decision making and yet subject to some surprising problems. Resolving or bypassing these problems remains one of social choice theory's core concerns. 

Epistemic justifications of democracy 

> Condorcet assumed that each individual is better than random at making a correct judgment (the competence assumption) and that different individuals' judgments are stochastically independent, given the state of the world (the independence assumption). 

> Formally, let V1, V2, …, Vn (capital letters) denote the random variables generating the specific individual votes v1, v2, …, vn (small letters), and let V = f(V1, V2, …, Vn) denote the resulting random variable representing the social decision v = f(v1, v2, …, vn) under a given aggregation rule f, such as majority rule.  [X denoting the state of the world (1 or 0)]

> Condorcet's assumptions can be stated as follows:

> Competence: For each individual i ∈ N and each state of the world x ∈ {−1,1}, Pr(Vi = x | X = x) = p > 1/2, where p is the same acrosndividuals and states.

> Independence: The votes of different individuals V1, V2, …, Vn are independent of each other, conditional on each value x ∈ {−1,1} of X.

> Theorem (Condorcet's jury theorem): For each state of the world x ∈ {−1,1}, the probability of a correct majority decision, Pr(V = x | X = x), is greater than each individual's probability of a correct vote, Pr(Vi = x | X = x), and converges to 1, as the number of individuals n increases.[1]


Challenging CJT Assumptions

> Although an average (not necessarily equal) individual competence above 1/2 may be sufficient for Condorcet's conclusion (e.g., Grofman, Owen, and Feld 1983; Boland 1989; Kanazawa 1998)

> The theorem's conclusion can also be undermined in less extreme cases (Berend and Paroush 1998), for instance when each individual's reliability, though above 1/2, is an exponentially decreasing function approaching 1/2 with increasing jury size (List 2003a).

> Although Condorcet's conclusion is robust to the presence of some interdependencies between individual votes, the structure of these interdependencies matters (e.g., Boland 1989; Ladha 1992; Estlund 1994; Dietrich and List 2004; Berend and Sapir 2007; Dietrich and Spiekermann 2013). If all individuals' votes are perfectly correlated with one another or mimic a small number of opinion leaders, the collective judgment is no more reliable than the judgment among a small number of independent individuals.

> Dietrich (2008) has argued that Condorcet's two assumptions are never simultaneously justified, in the sense that, even when they are both true, one cannot obtain evidence to support both at once.

> game-theoretic work challenges an implicit assumption of the jury theorem, namely that voters will always reveal their judgments truthfully...a voter expects a higher chance of bringing about a correct collective judgment by voting against his or her own private judgment than in line with it (Austin-Smith and Banks 1996; Feddersen and Pesendorfer 1998).

A utilitarian argument for majority rule

> Suppose each voter gets some utility from the collective decision, which depends on whether the decision matches his or her vote (preference): specifically, each voter gets a utility of 1 from a match between his or her vote and the collective outcome and a utility of 0 from a mismatch.[3] The Rae-Taylor theorem then states that if each individual has an equal prior probability of preferring each of the two alternatives, majority rule maximizes each individual's expected utility (see, e.g., Mueller 2003).

On prefeence cycling:

> How frequent are intransitive majority preferences? It can be shown that the proportion of preference profiles (among all possible ones) that lead to cyclical majority preferences increases with the number of individuals (n) and the number of alternatives (|X|). If all possible preference profiles are equally likely to occur (the so-called ‘impartial culture’ scenario), majority cycles should therefore be probable in large electorates (Gehrlein 1983).

Arrow's Theorem & The 5 assumptions that no (ordinal) preference aggregation rule can satisfy:

> Universal domain: The domain of F is the set of all logically possible profiles of complete and transitive individual preference orderings.

> Ordering: For any profile <R1, R2, …, Rn> in the domain of F, the social preference relation R is complete and transitive.

> Weak Pareto principle: For any profile <R1, R2, …, Rn> in the domain of F, if for all i ∈ N xPiy, then xPy.

> Independence of irrelevant alternatives: For any two profiles <R1, R2, …, Rn> and <R*1, R*2, …, R*n> in the domain of F and any x, y ∈ X, if for all i ∈ N Ri's ranking between x and y coincides with R*i's ranking between x and y, then xRy if and only if xR*y.

> Non-dictatorship: There does not exist an individual i ∈ N such that, for all <R1, R2, …, Rn> in the domain of F and all x, y ∈ X, xPiy implies xPy.

> Theorem (Arrow 1951/1963): If |X| > 2, there exists no preference aggregation rule satisfying universal domain, ordering, the weak Pareto principle, independence of irrelevant alternatives, and non-dictatorship.

Universal Domain

> It has been suggested, for example, that group deliberation can induce single-peaked preferences, by leading participants to focus on a shared cognitive or ideological dimension (Miller 1992; Knight and Johnson 1994; Dryzek and List 2003). Experimental evidence from deliberative opinion polls is consistent with this hypothesis (List, Luskin, Fishkin, and McLean 2013), though further empirical work is needed.

Welfare Aggregation

> In voting contexts, this assumption may be plausible, but in welfare-evaluation contexts—when a social planner seeks to rank different social alternatives in an order of social welfare—the use of richer information may be justified. Sen (1970b) generalized Arrow's model to incorporate such richer information.

The Doctrinal Paradox

> Kornhauser and Sager (1986) described the following problem. (A structurally similar problem was discovered by Vacca 1921 and, as Elster 2013 points out, by Poisson 1837.) A three-judge court has to make judgments on the following propositions:

> p: The defendant was contractually obliged not to do action X.  
> q: The defendant did action X.  
> r: The defendant is liable for breach of contract.  

                p    q      r
    Judge 1   True  True  True
    Judge 2   False True  False
    Judge 3   True  False False
    Majority  True  True  False

> Although each individual judge respects the relevant legal doctrine, there is a majority for p, a majority for q, and yet a majority against r—in breach of legal doctrine.

This leads to logical inconsistences when p & q -> r

