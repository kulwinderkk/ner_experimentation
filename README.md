## Analyzed various approaches to NER
Experimented with below -
- OpenAI Direct Call Oneshot Prompting (gpt-3.5-turbo and gpt-4)
- Using OpenAI through LlamaIndex Oneshot Prompting (gpt-3.5-turbo and gpt-4)
- Spacy
- Hugging Face transformers

## Observations
If there is a change in the text of the prompt O/p changes.
Both Direct Call to OpenAI and LlamaIndex yield more or less the same result. I experimented with a couple of other documents gpt-4 is performing better in those documents.
If the O/p format is changed to List of Tuples (with List of entity and value pairs the LLM gets confused for the O/p format). However it works for the other text data that I experimented with. I'm sure the prompt cam be improved to catch this error.
The output format of Dictionary Object seems to be more robust with LLM.
Pretrained Spacy could be a next best option after LLM.
Hugging Face results are okay not that good.

### Finally implemented NER using LlamaIndex OpenAI with gpt-4-1106-preview as it as good as gpt-4 and slightly cheaper.
Also made a provision of Spacy as some time the ouptut Json or Dictionary is not evaluated properly.
  
