# Markov Chain Coding Challenge: Overiew

Given an array of arrays (hereinafter, matrix) of equal dimensions where each row represents a state and the 
columns represent a step to that state as an argument for function solution(M), return an array
with the probabilities of ending in each end state when the initial state is the first row, by the fraction numerators and the common denominator 
as the final entry of the array. Note: End states will have no entries representing no steps can be taken. Initial state and other step states are guaranteed to get to an end state.

For example, given a matrix:

s0: 0 1 0 0 0 1 <br/>
s1: 4 0 0 3 2 0 <br/>
s2: 0 0 0 0 0 0 <br/>
s3: 0 0 0 0 0 0 <br/>
s4: 0 0 0 0 0 0 <br/>
s5: 0 0 0 0 0 0 <br/>

Starting in the initial state s0, there is a fifty percent chance of going to s1 and fifty percent chance going to s4
The end states are s2, s3, s4 and s5.

By following possible paths and calculating the probabilities of ending on each end state, we see:<br/>
s2: 0 (s2 is an end state that will not be reached)<br/>
s3: 3/14<br/>
s4: 1/7<br/>
s5: 9/14<br/>

And our function will return:
[0, 3, 2, 9, 14]

## Code and Resources Used
**Python:** Python 3.8.10 <br/>
**Packages:** none <br/>
**Resources:** matrix inversion code inspired by user stackPusher at stackoverflow.com <br/> 
(https://stackoverflow.com/questions/32114054/matrix-inversion-without-numpy)
