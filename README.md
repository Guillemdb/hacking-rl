# Hacking Reinforcement Learning

[Repository](https://github.com/Guillemdb/hacking-rl)


[EuroPython Slides with notes](https://docs.google.com/presentation/d/1aquFoqMz8gYhua2zr-PCckL2-6-weQFfbZ4fRVywW2Y/edit?usp=sharing)

[PyConEs slides](https://docs.google.com/presentation/d/1rYJPNGRunMP5gNzzIP7P0rSqYTZAbNClfdofDW8I9oQ/edit?usp=sharing)

**The FractalAI repository is now private. If you want me to send you a copy please contact me 
opening  an issue in this repository.**

Creating huge datasets of top performing examples for Reinforcement Learning (RL) has always been tricky, but if we allow
ourselves to cheat a bit it can be done very easily. During this talk, I will present a new family of algorithms that allow to efficiently generate very high quality samples for any known RL environment.

This new generation of planning algorithms achieves a performance which is several orders of magnitude higher
than any other existing alternative, while offering linear time complexity and good scalability.

## The talk
This talk will be a practical example
of how we can use new tools for hacking any reinforcement learning environment, and make it generate superhuman level games.

Hacking RL, as any other hacking process will be divided in four phases:


### 1. Information Gathering

During information gathering, I will briefly explain what are the main ideas behind Reinforcement Learning.
I will also talk about how our theory (FractalAI) came to be, and what are the fundamental concepts behind it.

### 2. Scanning and vulnerability detection

We will find an attack vector against the environment API, and explain how it can be exploited. I will explain
the fundamental concepts needed to build a new generation of exploits, that will allow us to have complete control over the data the environment produces.

### 3.Exploitation & privilege escalation

This is the time to test the new exploits and to show a proof of concept. We will exploit the attack vector to gain access
to the environment. Using only a laptop I will show how it is possible to sample data which surpasses human performance way faster than real time.

### 4. Maintaining access & managing tracks

Once we have gained control of the environment, we will measure how well the exploits work, and how well the techniques presented
can generalize to other types of environments.

## The Q&A

I want the talk to be as simple and fast as possible, with a lot of graphical examples, videos, and a Jupyter notebook.
The Q&A session is the time to apply some social engineering to get me to talk about the details that you find more interesting.
I have prepared additional material covering the most common questions and concerns, but feel free to ask whatever you want, I love challenging questions ;)

Some of the topics covered in the additional material are:

* Reinforcement Learning as a supervised problem
* Improving AlphaZero
* Hacking OpenAI baselines
* How the algorithm works
* An overview of the FractalAI repository
* Improving world models
* Combining FractalAI with neural networks

## References

1. Repository with the code of the Swarm Wave and Fractal Monte Carlo algorithms: [https://github.com/FragileTheory/FractalAI](https://github.com/FragileTheory/FractalAI)
2. [Planning with Pixels in (Almost) Real Time](https://arxiv.org/pdf/1801.03354.pdf)
3. [Blind Search for Atari-Like Online Planning Revisited](https://www.ijcai.org/Proceedings/16/Papers/460.pdf)
4. [Google spreadsheet with all bencharks on Atari](https://docs.google.com/spreadsheets/d/1JcNw2L0YL_I2iGZPJ0bNKJshlTaqMuEl5CP2W5zie6M/edit?usp=sharing)

5. [Code used to run the examples](https://github.com/Guillemdb/FractalAI/tree/learning). (Not merged to the FractalAI repo yet)