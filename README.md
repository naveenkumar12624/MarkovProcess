# Markov Process
# Aim : 

![image](https://user-images.githubusercontent.com/104613195/170176804-7a25305b-c5e3-4b93-8201-8ebbe99765cc.png)

# Software required :  

Python

# Theory:

Markov chains, named after Andrey Markov, a stochastic model that depicts a sequence of possible events where predictions or probabilities for the next state are based solely on its previous event state, not the states before. In simple words, the probability that n+1th steps will be x depends only on the nth steps not the complete sequence of steps that came before n. This property is known as Markov Property or Memorylessness. 

Assumptions for Markov Chain :
1. The statistical system contains a finite number of states.
2. The states are mutually exclusive and collectively exhaustive.
3. The transition probability from one state to another state is constant over time.
# Procedure :

![image](https://user-images.githubusercontent.com/104613195/170175685-c6187523-f268-4a3b-b03d-8bbe62647a57.png)

# Program

```python
import numpy as np
p0 = [0.3,0.2,0.5]
p = [[0,2/3,1/3],[1/2,0,1/2],[1/2,1/2,0]]
n=6
for i in range(1,n+1):
    p0 = np.multiply(p0,p)
    print("The %d -step probability distribution is &"%i)
    print(p0)
```
# Output : 

![Capture46](https://user-images.githubusercontent.com/75234588/170327965-c7202aaf-346d-4890-add7-74a7ce02538a.PNG)

# Results :
Thus the n-step probability distribution matrix using Markov's Process has been found.

