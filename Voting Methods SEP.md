Voting Methods in SEP
=====================
Eric Pacuit

The central question addressed is 
  
  Given a group of people faced with some decision, how should a central authority combine the individual opinions so as to best reflect the “will of the group”?

But this presupposes that voting on the issue is the best course of action or even justified.

Condorcet winner - the candidate that beats every other in one-on-one elections

Bordet winner - the candidate with the most margin in one-on-one elections over others

Voters can vote: 

- sincerely - reflecting their actual preferences, or
- strategically - reflecting the expected choice that best leads to their preferred outcome.

##Voting rules


Plurality voting - each voter indicates one preference and the candidate with the most wins.  It severely restricts the information able to be expressed and penalises competition amongst similar candidates. Encourages strategic voting.

Borda Count - each voter provides a linear list of preferences. 0 to n-1 points are awarded for the last to first candidate on each ballot. The candidate with the most points wins.  Penalises incomplete ballot papers.  Insertion of irrelevant candidates can change outcomes, even when ordinal preferences remain the same.

Plurality Runoff - plurality vote with a second ballot for the top two if no candidate gets an absolute majority. Requires voting twice and penalises competition amongst similar candidates. Is also non-monontonic

Hare rule - Ballots are linear orders over the set of candidates. Repeatedly delete the candidate with the fewest first-place votes. Eliminated candidate's votes are then transferred. 
 
Coombs rule - Ballots are linear orders over the set of candidates. Repeated delete the candidate who has most last votes. The last candidate left is the winner.

Negative voting - voters can give one candidate a +1 or -1. Most points wins.  Doesn't require linear preferences but loses information.

Approval voting - votes select a set of candidates they would be happy with. Candidate with the most approvals wins.

Cumulative voting - each voter has a number of points they can distribute amongst candidates as they please. Most votes wins.  Conveys more information but is more complex.

Condorcet Rule:
Each voter submits a linear ordering over all the candidates. If there is a Condorcet winner, then that candidate wins the election. Otherwise, all candidates tie for the win. 

Dodgson's Method:
Each voter submits a linear ordering over all the candidates. For each candidate, determine the fewest number of pairwise swaps needed to make that candidate the Condorcet winner. The candidate(s) with the fewest swaps is(are) declared the winner(s). 

Black's Procedure:
Each voter submits a linear ordering over all the candidates. If there is a Condorcet winner, then that candidate is the winner. Otherwise, let the winners be the Borda Count winners.

Monotonicity - voting is monotonic if gaining more votes does not disadvantage the candidate.

##Paradoxes 

Condorcet's Paradox - even if each individual voting preference order is transitive, the resulting aggregate order may not be.

Borda paradox - if there is a condorcet winner, then they should be the winner. But a borda winner may not be the condorcet winner.

Theorem (Fishburn 1974).
For all m ≥ 3, there is some voting situation with a Condorcet winner such that every weighted scoring rule will have at least m−2 candidates with a greater score than the Condorcet winner. 

Anscombe's paradox (Anscombe 1976), in which:
It is possible for a majority of voters to be on the losing side of a majority of issues. 

##Strategic Voting

Strategic voting can occur when voters express non-sincere preferences in order in increase the likelihood that their sincerely preferred candidate wins.  It can also occur in the ordering of votes and runoffs.

Gibbard-Satterthwaite Theorem: Under natural assumptions, there is no voting method that guarantees that voters will choose their ballots sincerely

##Assessment

Voting can be judged by standards of procedures or standards of truth tracking.  Procedural standards assess the fairness of voting amongst equals and its normative axioms include:

- Anonymity
- Neutrality
- Universal Domain
- Unanimity
- Positive Responsiveness (candidates win if they receive extra votes after a tie)

Rather than concern with the 'right way', epistemic standards of voting are concerned with the 'right answers'.

Epistemic justifications typically require:

- an independent account of the truth that voting can be mapped to
- a cognitive account of voting
- an account of adaptive decision making in light of other beliefs

Condorcet Jury Theorem.
Suppose that Independence and Voter Competence are both satisfied. Then, as the group size increases, the probability that the majority chooses the correct option increases and converges to certainty. 

Notice that CJT explicitly rejects updating of beliefs.

Regenwetter et al. 2006 - many of the usual voting methods that are considered irreconcilable (e.g., plurality, Borda count and methods that choose the Condorcet winner) are, in fact, in perfect agreement.


Bibtex

  @InCollection{sep-voting-methods,
    author       =  {Pacuit, Eric},
    title        =  {Voting Methods},
    booktitle    =  {The Stanford Encyclopedia of Philosophy},
    editor       =  {Edward N. Zalta},
    howpublished =  {\url{http://plato.stanford.edu/archives/win2011/entries/voting-methods/}},
    year         =  {2011},
    edition      =  {Winter 2011},
  }