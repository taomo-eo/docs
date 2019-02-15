## Governance Mechanism of NEO: An Guide 

### *or: How Consensus Nodes are Voted and Elected*

As NEO plans to [accelerate its decentralization](https://neo.org/blog/details/4125) in 2019 and beyond, more and more community-run Consensus Node candidates will be available for NEO holders to vote for. This write-up is an introduction to the concepts and procedures involved in electing and voting for consensus nodes in the NEO network.

### 1. Overview

Consensus Nodes are the block producers, or 'bookkeepers' in the NEO network. Therefore, the 'governance mechanism' of the network is determined by how the network selects its Consensus Nodes. ***Every NEO you hold is a share of the right to manage the network***, because NEO holders can decide what nodes become Consensus Nodes in these two ways: 

1. Anyone can register to become a candidate for a Consensus Node by paying a system fee of 1000 GAS. 
2. Anyone can vote for any number of candidates. The number of votes they have correspond to the number of NEO they hold in real time. 

The network then calculates and updates the list of Consensus Nodes each time a new block is produced. 

The following sections will explain this process in more detail. 

### 2. How Many Votes Do You Have

Any node that holds NEO can vote for an unlimited number of candidates. The number of votes correspond to the number of NEO held in the account. If an account votes for multiple candidates, votes do not divide among the candidates, rather, each candidate receives votes equal to the real time balance of the voting account. ***If NEO balance changes, the candidates' votes will be updated simultaneously to reflect the change in balance.*** 

For Example, if there are 100 NEO in an account, and the account voted for 3 candidates, each candidate receives 100 votes. If 10 NEO in the account is spent after the vote, the candidates' votes will simultaneously be decreased by 10. 

###3. How Are Consensus Nodes Selected

When the network calculates to determine which candidates are going to be consensus nodes, there are roughly two major steps involved: 

- First, the network calculates ***N***, which is how many Consensus Nodes are going to be chosen. 
- Then all candidates, including nodes that are already consensus nodes are sorted by the number of votes they receive, and the network chooses the top ***N*** candidate nodes as Consensus Nodes. 

***N*** is calculated as follows: 

1. Sort the number of candidates each account voted for by size. e.g. C1, C2, ..., Cn

   > *For example, if an account, x, voted for 3 candidates, then Cx would be 3.*

2. Remove the first 25% and the last 25% of the array. 

3. Calculate the *weighted average*\* of the remaining 50% data, which is then determined as the number of consensus nodes to be selected, N. 

   > *\*: weighted average depends on the NEO held in each account. This means that accounts that hold more NEO contribute proportionally more to the average when calculating the number of consensus nodes to be selected.* 

It is worth noting that this calculation is carried out each time NEO produces a new block. 

#### What This Means For Voters

Given the mechanism described above, there are things to keep in mind for voters when voting for candidate nodes: 

- Each vote includes 2 important decisions: 1) *How many* candidates you are going to vote for; and 2) *Which* candidates you are going to vote for. (elaborate: both are gonna affect the algo, be weary of too many or too few candidates that you vote for)
- The balance of your voting account *after* voting matters. 

### Two Approaches To Candidacy: On-chain & Off-chain Governance

Any node that pays the system fee of 1000 GAS can become 'candidate' nodes and are eligible to receive votes from other nodes. But a candidate can only become a Consensus Node by gathering enough votes. Considering that NEO Foundation still holds a significant amount of NEO, partnering with NEO Foundation can be a mean to secure votes. The terms **on-chain** and **off-chain** governance describes whether the candidates chooses to partner with NEO Foundation to secure votes from them. 

**On-chain governance** candidates rely entirely on the mechanism of the NEO blockchain. They gather votes independently through their website and campaigns. 

**Off-chain governance** candidates elect to enter a strategic partnership with NEO Foundation. Once they complete a six-month test-running period, their candidate node registered on the blockchain receive votes from NEO Foundation. 



on-chain governance

off-china governance



### Vote Calculation 



NEO is 



#### Election

On-chain governance means that the election process relies entirely on the mechanism of the NEO blockchain. Potential candidates spend 1000 gas to register on the blockchain as a candidate, and become consensus nodes once they have gathered sufficient votes from NEO holders. 

Off-Chain Governance candidates go through the same process as their On-chain counterpart, but they also partner with NEO Foundation 'outside the blockchain' to gain votes from the foundation in addition to other NEO holders. 

#### Voting

Anyone holding NEO can vote for candidate nodes. Votes from NEO nodes are calculated every time a block is produced. Two values are calculated from votes: a) how many candidate nodes are chosen as consensus nodes. b) How many votes each candidate has received. 

There are two approaches to be elected as a consensus node: Off-chain Governance and On-chain Governance. 

Candidate nodes are then sorted by the number of votes they receive. 



## For Candidates

xxxxx

### Ways to become a Candidate Node



### You are a Candidate Node, now what? 

(gather support, support page)(refer to 'how votes are calculated')



## For Voters

### How Many Votes Do You Have 

Any node that holds NEO can vote for an unlimited number of candidates. The number of votes corresponds to the number of NEO held in the account. If NEO balance changes, the candidate's votes will be updated simultaneously to reflect the change in balance.  

For Example, if there are 100 NEO in an account, and the account voted for 3 candidates, each candidate receives 100 votes. If 10 NEO in the account is spent after the vote, the candidates' votes will simultaneously be decreased by 10. 

### How to Cast Your Vote



### How Are Votes Calculated

