![title](cover.png)
Prompted from Dall-E 2: A cat studying a magic book about spelling in a dark classroom, digital art

# Prompt Handbook: Rules of Thumb 👍 for Writing Good Magical Prompts

Yao Fu. University of Edinburgh. yao.fu@ed.ac.uk

Some good enough rules when writing prompts. Let us explore the emergent abilities of large language models together!

Contributions and suggestions wellcome!! Add your experiences when writing prompts so we can be better witcher/ magician/ sorcerer/ alchemist, or scientist. 

Disclaimer: 
* Suggestions below are from a variety of sources (papers, blogs, talks, discussions, .etc), which makes many of them hard to cite and credit precisely. I am still trying to find out the best way to credit everyone contributed, so definitely tell me if you feel your contributions is listed below but not credited properly. 
* Althought the purpose of this project is to list reliable rules when writing prompts, prompting can be unstable in many cases. So please do raise an issue if you find a rule is not a good one to follow. 

# The Prompt Handbook

## Choosing a Language Model 

* Use the largest model you have access to. Conclusions made on small models may not stand for large models. 
* GPT3 text-davinci-002 and code-davinci-002 are probably the best publically available models. 
* Upon registration, OpenAI gives $18 credits. As a reference, CoT prompting a 200-sized dev set cost about $3
* code-davinci-002 is currently free but requires application
* code-davinci-002 is better at structured inputs and complex reasoning; text-davinci-002 is better at natural inputs and intuitive reasoning. 

## Prompting 
* Use the right number of examples. 1 example may be too few. 20 examples may be to many. 
* For text-davinci-002, use natural language, use your human intuition to judge if one sentence is more natural than another. The more natural the language, the better  
* For code-davinci-002, you can mix natural language with pseudo code. 
* Use chain-of-thoughts prompts. 
   * Be specific when writing chain of thoughts. 
   * Be detailed when writing chain of thoughts, do not jump between steps, do not take shortcuts 
   * Choose complex chain of thoughts, not simple chains, as your prompt

## Chain of Thought

## Explanation

## Recall Internal Knowledge

## Decomposition
* If a question is too complicated, split it into multiple simpler subquestions, then ask the subquestions one-by-one
* You may want to google a question instead of prompting 
  * Google is better for obtaining knowledge, LMs are better for reasoning with given knowledge

## Decoding 
* sample multiple reasoning chains then majority voting
improves multi-step reasoning. 

## Generalization Performance v.s. Fine-tuning
* Currently (2022.10) there is little study comparing prompting v.s. fine-tuning in a fair setting. Many existing work compares prompting large models v.s. fine-tuning small models 
* When the test set is in-distribution, the impression is that fine-tuning is better. Yet for out-of-distribution setting, prompting seems to be more robust.

# References

## General 
* [GPT-3 Hunt](https://www.buildgpt3.com)
* [GPT-3 Demo](https://gpt3demo.com)

## Chain of Thoughts Series
TBC

## General Prompting 
TBC

## Training, Tuning, Scaling
TBC

## Planning the Generation
TBC

## Retrieval and Knowledge
TBC

## Generalization 
TBC

## Calibration
TBC

## Theory and Analytics 