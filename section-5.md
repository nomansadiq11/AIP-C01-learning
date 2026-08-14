# Operational Effeciciency and Optimization

## Token efficiency

- We can have token limit and maybe we can add budgets
- cloudwatch track these tokens (input and output )
- TTFT (Time to first token streaming)
- we can imprve token optimization
    - context window
    - also number of chunks you need to control
    - we can also filter those chunks base on the metadata
- also optimzation on output side
    - respnse size control
    - json output base on specific format
- prompt compression
    - use small model to summarization things
    - use knowledge base instead of research on the content

## Cost effective model sleection

- do you really need big models
- use intelligetn prompt selection
- route different model base on the complexities
- we shoudl also measure the performance of the model output with aws evaluation

## Maxmium resouces utlization

- batch embedding up for vectore stores
- bedrock batch inference
- aws service quotas has a bedrock took we can ask for more capacity need more
- we can also buy prevision throughput
- Tensor parallelism
    - shared LLM weight accross GPUs
    - better memory utlization
- bedrock we can previsoun by token or throughput
- we can also do both
- we can also find model utlization with cloudwatch, we can build dashboard
- aws cost expore we can check who is driving aws cost
- autoscale we can maxmimztion , we can use serverless to use lambda, bedrock

## Intelligent caching system

- semantic caching
    - store result in cache somewhere
    - we can cache meaning of the output of the model
- you need to make sure user gettting correct answers
- prompt caching
    - people asking again again same thing
    - you can have predefine prompts
    - you might need to cache uploaded document
    - cache read write are monitor in cloudwatch
    - prompt cache also in bedrock managment tools
- edge caching
    - we can cache data in cloudfront
    - some response are common we can cache at the edge

## Buillding Responsive AI Systems

- parallel requests for complex work
    - buil multi agent system
- also caching can also help to solve this problem quick
- response streaming
- latency optimzie for Foundational model
- keep your prompt consise
- give only information needed
- the less information i sent the faster the response will be
- limit the response size
- breakup the complex tasks

## Optimizing the Retrieval Performance

- Optimize your indices
- Hybrid search imporve the relevance
- Query pre-processing
    - normalize query to the corpus in the terms of style
    - breakup multip part questions don't try to look two different thng at one
    - filter out irrelavant information

## Optimize for specfic Usecases

- different model have different parameters
- you can use A/B testing
    - bedrock evalution tool
- some common parameters
    - temperature - amount of randomes in the respnse
    - Top_p
    - Top_k

## Optimization foundation model system performance

- API calling profiling
    - people calling same thing again and again
- use structure json input and output
- you should have capturing feedback from user so something you can fix it
- you can model parallalizatio split up the model in multiple instances
- you can choose larger instance but small model
- Ultraserver
    - you gonna use multiple machine and they need to coomunicate with low latancy
- lamdba endpoint lifecycle get pull all model on demand

## exponential backoff

- implement backoff retry if service goes down try in 30 sec then 1 min
- connection pool shouldn't be evry single request if yes then use for muyltipel request if you don't work more then close it
- set timeout for the connections

## Bedrock cross region inference

- Its distribute your workload access regions
- each region have quotas
- if SCP block the region bedrock will not work, you need to make sure SCP allowed all the regions
- you can restrickt for Geography like middleeast
- 