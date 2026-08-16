# Governance and QA

## Bedrock Agent Tracing

- response provide details how this reasong processing
- what knowledge base it hit
- bedrock will provide you details of the request and processing what step, what action all

## Foundation Model evaluation

- so many question, to understand how this result comes up
- is the correct answers
- is this correct sense
- as testing you should know the answer then we can evaludate the response
- You can evalue with following
    - Accuracy
    - speed
    - scalbility
    - context retrival
- you can use another model to judge it

## Rouge

- This is another way of evaluation it, text summarization and machine translation
- Rouge-N (N is the number tell that evaluation)
- Rouge-L (uses longest common sub sequence)
- let say certificed AI Practitioner
    - Unigram means three different words
    - bigram mean two word
## BLEU

- This metrics is to compare with human translation with everything to see if this is correct

## BERTScore

- LLM depends on the vector storeage which look closeer matching works to the embadding vectors

## Bedrock Model Evaluation

- text summerirzation Q&A classfictions
- tons of built in task todo this
- Human
- there are evaluating model to use the judge the output
- there are RAG evaluation jobs as well

## Considerration for deployment workflow

- checking response consistancy
- AI Specfic output validations

## Princple of Responsible AI

- you need look fairness of the application, why did its say something
- pravacy and security, you need to make sure its not exposing information
- explaination: you need to look why this explain it
- Governance, how AI following of the governance
- transpartnetly, how AI transparent to the answers

## AWS Tools for Responsible AI

- AWS bedrock model for evauation
- sagemaker clerify, bias detection model evualtion
- sagemake model monitr check the inaccurac y

## Cloudwatch and GenAI

- prompt input and model responses foundation to monitroing it
- foundation model interaction tracing
- business impact metrics
- anomly detection like token brusts
- bedrock model invokation
- cost anomly detections

## Cloudtrail

- any thing interacting with bedrock logged in cloudtrail

## AWS Lakeformation

- this is built top of glue, whatever you can do with glue same you can do with lakeformation
- you can implement column base security this can be achieve it using lakeformation




