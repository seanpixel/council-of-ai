# council-of-ai
Security measure for agentic LLMs using a council of AIs moderted by a veto system. The council judges an agent's actions outputs based on specified categories.

## Objective
Implement a system to judge AI Agents outputs using a **council** of AI models. Decentralize the decision making power to avoid potential disasters.


## Sections
- [How it Works](https://github.com/seanpixel/council-of-ai/blob/main/README.md#how-it-works)
- [How to Use](https://github.com/seanpixel/council-of-ai/blob/main/README.md#how-to-use)
- [More About Project & Me](https://github.com/seanpixel/council-of-ai/blob/main/README.md#https://github.com/seanpixel/Teenage-AGI#more-about-the-project--me)
- [What you can do](https://github.com/seanpixel/council-of-ai/blob/main/README.md#what-you-can-do)
- [Credits](https://github.com/seanpixel/council-of-ai/blob/main/README.md#credits)


## How it Works
Language models, acting as a "judge", will rate an AI output out of 10. If any of the judges in the council (formed by a group of judges) vetoes (verdict == false) an output, that output will be flagged as being potentially immoral/unjust/harmful/useless. 


## How to Use
1. Clone the repository via `git clone https://github.com/seanpixel/council-of-ai.git` and cd into the cloned repository. 
2. Install required packages by doing: pip install -r requirements.txt
3. Download the ethics dataset from [here](https://people.eecs.berkeley.edu/~hendrycks/ethics.tar).
4. Create a .env file or plug in your key in judge.py (line 8), all you need is an OPENAI_API_KEY
5. Go to main.py and choose the test type using the choice variable (default is commonsense)
6. Run `python main.py` and see what kinds of judgements the council makes


## More about the Project & Me
After creating [Teenage-AGI](https://github.com/seanpixel/Teenage-AGI), I wondered about potential implications of Agentic LLMs and some ways to moderate its unpredictable behaviors. From this, I thought of democracy and how a decentralized system of AIs could monitor other AIs from causing harm. So came council-of-ai. While contributing to the "acceleration" of technology, I still care about AI Safety and believe that safely guiding AI towards the future can be as fun and exciting as accelerating. 

I'm a founder currently running a startup called [DSNR]([url](https://www.dsnr.ai/)) and also a first-year at USC. Contact me on [twitter](https://twitter.com/sean_pixel) about anything would love to chat.


## What you can do
Create more "setups", these are basically the characteristics of the judges. Play around with more example Agent outputs and possbily use your own by adding them to "actions.yaml". Use more judges or even plug in your own local LLM. Or even better, implement the council on an unaligned base model (Llama?) and experiment. This is a growing initiative so any help would be appreciated.


## Credits
Credits to [@DanHendrycks] for the Ethics dataset used in testing the idea.
