Juggler
=======

	The following program takes an input as described for the Juggle Fest problem, uses a greedy implementation to determine the juggler allocation, and outputs a specified solution. 

	A score list is created by taking the dot product of every j juggler and each c circuit within their preference list. Assuming that there are c circuits within each preference list, j*c scores are created. The scores are then sorted. We then walk through the sorted list, assigning the highest scoring juggler to their corresponding circuit. If we encounter a score of a juggler that we've previously assigned, the score is skipped. If we encounter a circuit that has been filled, the score is skipped. 

	Upon completion of traversal of the score list, it's possible that there will remain jugglers who do not have assignments (where their entire preference list of circuits is filled by... more qualified jugglers). A second score list is constructed by taking the dot product of each remaining juggler and each remaining circuit. The list is sorted, and jugglers are assigned following the same rule criteria as indicated above. 

	At this point, all jugglers would have been assigned to the circuits. An output file is formated and delivered.
