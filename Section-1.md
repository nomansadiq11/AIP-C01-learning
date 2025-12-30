# Generative AI Fundamentals and Bedrock

## AWS Bedrock

- This is layer on AI models, you can use any model you want via this aws Bedrock
- Testing with chat and prompt features
- testing with Image creation (chose wisely, ondemand and prevision which is costly)
- Bedrock can also privde how correct your RAG responding
- multimiodel aws nova, like you can share pic and test it will do embadding for both of them
-

## Fine-tunning

- Train the model on your data for specfic usecase like chatbot for your company information
- Like personal assistance on your emails
- bake the model as per your usecase
- this is expensive interm of cost and time, larage going in and out

### Low Rank Adaptations - machniscam for fine tuning

- retrain the model
- this is very effiicent, storage, training and model

## Retrival Augment generation (RAG)

- It means get information from your internal system
- pron:
    - you can expand database, no need to fine tuning
    -  this can incrase the token
    - this can be AI search
    - technical you are not training model
    - Can prevent the hallucinations
    - can leverage sementaic search via vector database
- Conr:
    - store alot of data in vector storage
    - it can still hallucination
    - very sensitive to relvanty information
    - you have made the worlds most over complicated system

## Vector DataStore and Semantic Search

- its database store the data in vector format like 100s dimentions
- storing data is very important for for retriving back for relvant
- storing data in chunk bases
- semantic chunking, ask llm todo the chunking it
- you can do hirakey chunk like a tree (parent 6, child 3 overlapp 1 )
- optimizeing data, add data in json format with metadata information


### Embadding

- This is like store words like potato rhubarb are store closer to earch other becuase same similarties
- embadding base titan model in aws
- once you query the AI, this will convert to embadding vector
- you get back top-N the most neareast thing which meet your query

### Bedrock - Knowledge base

- once you have docs like in S3 , you need to store somewhere
- then you can use titan model to embadding for vector database
- opensearch can use store the as vector database

## Guardrails

- aws bedrock guardrail filter the prompt
- work with text foundation model
- PII data securi it
- help to prevent the hallucination
- you can also control the message response

## Token Level Redaction

- this is another layer of defense of the naughty words
- you can take input to lambda function and make clear and get output


## Prompt Managment

- you can create predefine prompt and add some variables

## Amazon Bedrock Flows

- you can build flows from input to output like input --> prompt managment --> knowledge base --> and model

## Enforce use of structure Data

- you can ask for structure data like in json or just custom template
- you can also connect with agents todo that

## Prompt Engineering

- this is very important to get the right output
- you can also do RAG for get context information

## Anatomy of prompt

- instruction
- context
- input data
- ouput indicator


## Prompt Best Pratics

- Clear and Consize
- phase clear
- ask with ? mark
- split the talsk

## Type of Prompts

- Zero- Shot - model already know things
- Few-shot - you give the examplses
- Chain of Thought - Think step by step, breakdownt he tasks

## Prompt Misuse and Mitigation Bais

- user can input prompt which suppose to not be like, lets assume and build something bad
- shouldn't store PII data but if stored amazon guardrail will detect and mask it
- Bais, ask AI to generate software engineering image with Pizza this will create all white engineer which is wrong, you can tweak with prompt engineering

