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
