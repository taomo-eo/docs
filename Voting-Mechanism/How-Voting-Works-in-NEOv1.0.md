## Elections and Voting in NEO

As NEO plans to [accelerate its decentralization](https://neo.org/blog/details/4125) in 2019 and beyond, more and more community-run Consensus Node candidates will be available for NEO holders to vote for. This write-up is an introduction to the concepts and procedures involved in electing and voting for consensus nodes in the NEO network.

### 1. Overview

Consensus Nodes are the block producers, or 'bookkeepers' in the NEO network. Therefore, the management of the network is determined by how the network selects its Consensus Nodes. ***Every NEO you hold is a share of the right to manage the network***, because NEO holders can decide what nodes become Consensus Nodes in these two ways:

1. Anyone can register to become a candidate for a Consensus Node by paying a system fee of 1000 GAS.
2. Anyone can vote for any number of candidates. The number of votes they have correspond to the number of NEO they hold in real time.

The network then calculates and determines which candidate nodes would become consensus nodes each time a new block is produced.

The following sections will explain this process in more detail.

### 2. Concerning Candidates 

A node can register as a consensus node on NEO-GUI by paying a system fee of 1000 GAS. You can look up all current candidate nodes registered on the main-net by going to the [Consensus](https://neo.org/consensus) page on neo.org. Information on each candidate node is provided by their respective maintainers. 

There are two types of candidates depending on how they gather their votes:

**On-chain governance** candidates rely entirely on the mechanism of the NEO blockchain. They gather votes independently through their website and campaigns. 

**Off-chain governance** candidates elect to enter a strategic partnership with NEO Foundation. Once they complete a six-month test-running period, their candidate node registered on the blockchain receive votes from NEO Foundation. 

> *For potential candidates, more information can be found here: [How To Become A NEO Consensus Node](https://neo-ngd.github.io/reference/How-To-Become-NEO-Consensus-Node.html)*

### 2. How Many Votes Do You Have

Any node that holds NEO can vote for an unlimited number of candidates. The number of votes correspond to the number of NEO held in the account. If an account votes for multiple candidates, votes do not divide among the candidates, rather, each candidate receives votes equal to the real time balance of the voting account. ***If NEO balance changes, the candidates' votes will be updated simultaneously to reflect the change in balance.*** 

For Example, if there are 100 NEO in an account, and the account voted for 3 candidates, each candidate receives 100 votes. If 10 NEO in the account is spent after the vote, the candidates' votes will simultaneously be decreased by 10. 

### 3. How Are Consensus Nodes Selected

When the network calculates to determine which candidates are going to be consensus nodes, there are two major steps involved: 

- First, the network calculates ***N***, which is how many Consensus Nodes are going to be elected. 
- Then all candidates, including nodes that are already consensus nodes are sorted by the number of votes they receive, and the network chooses the top ***N*** candidate nodes as Consensus Nodes. 

***N*** is calculated as follows: 

1. Sort the number of candidates each account voted for by size. e.g. C1, C2, ..., Cn

   > *For example, if an account, x, voted for 3 candidates, then Cx would be 3.*

2. Remove the first 25% and the last 25% of the array. 

3. Calculate the *weighted average*\* of the remaining 50% data, which is then determined as the number of consensus nodes to be selected, N. 

   > *\*: weighted average depends on the NEO held in each account. This means that accounts that hold more NEO contribute proportionally more to the average when calculating the number of consensus nodes to be selected.* 

It is worth noting that this calculation is carried out each time NEO produces a new block. 

#### What This Means For Voters

Given the mechanism described above, each vote contains two important decisions: 

1) *How many* candidates you are going to vote for. This influences the number Consensus Nodes that are going to be elected. 

2) *Which* candidates you are going to vote for. This influences the vote tally of the candidate nodes that you are voting for. 

### 4. Where to Vote 

Currently, NEO-GUI is the only client that supports voting. [Here](https://neo-ngd.github.io/reference/How-To-Become-NEO-Consensus-Nodev1.5.html#421-voting-with-neo-gui) is a step-by-step guide on how to vote with NEO-GUI. 

Community clients such as [neon wallet](https://github.com/CityOfZion/neon-wallet/releases) also have plans to implement voting features in the future. 