# Managing Data for Generative AI

## Structure Data

- GenAI use json format to input the data
- raw text lose structure, GenAi like structure data
- raw text can convert in html format
- divider stirg can be used for better chunking

## Bedrock Data Automation

- you can extract any data
- if you have unstructre data you can use data automation then convert in vector database.
- you can analyse videos, scens and text
- you can find also adds in videos
- there is standard output for this but you can do custom output
- you can also use PDF, JSON data
- image processing: JPEG and PNG, this can turn to json model
- video processing IAB take video and extract inforation
- audio processing: who saying what and transcribe and the output will be in JSON
- there are blueprint exists in ouput

## Satemaker Data Wrangler

- its for data pipelines
- import data like ETL
- visualize the data
- it can transofmr the data or you can integrate your own transofmr model
- quick model, to train your model with your data
- data wranger is just generate code which will transform your data

## AWS Glue

- Glue is kind of database top of your S3 unstructure data
- crawler will scan the data and get the metadata
- partition the data in glue
- create workflow in glue studio
- there are data quality rules you can define and check the quality of the data

## Amazon Transscribe

- automatically convert speech to text
- it uses deeplearning automaticcally speech to text
- it will delete PII information
- you can also access multi language
- we can improve the accurachy for use custom acronoms
- toxicity also detect in this service

## Amazon Comprehand

- NLP, this is uses for name entity recognization
- it useful for NLP
- it will do sentimal analysis of the application
- there is HIPPA compalice amazon compprehand also avaiablle

## OpenSearch

- search in documents like in json
- very good in scalble
- it built top of lucin
- we can also build dashboard for as well in open search
- you can store documents data
- you can provide what type of the data is coming
- indices are, you can search in the document
- every document lives in shared, and each shared live somewhere in nodes
- amazone manged opensearch you can use resouces base policy as well
- there are storage type as well, like hot, warm,ultrawarm, cold,
- automate index managment
- send notificate once policy execuated successfully
- there are 3 master node, 1 will decide which one is the primary nodes
- also you need to choose the right shared
- you also need 3 data nodes
- optimization, there are un balanced shared optimization
- too many shared will be problem again
- opensearch as vector store
- opensearch vector engines (FAISS, nearest neighbour, ANN)
- compression: store in binary values which save more but slower, there are also (FP 16, vectors compression)
- for simentic search you need to careful with sharing
- neural plugin, you can connect with with vector data store.

## Amazon S3 Vector

- you can store your data in s3 as vector database
- you one model for one store
- you need to enable the embaddign before store
- you can define the index
- if you have frequently calling to S3 search then you can use open search
- look for best pratices, insert and deltes in large batch size (use concurrent request for smaller batches )

## Amazon RDS

- RDS is relatinal databasem managment
- you can multiaz
- you can scale
- storage is backed by EBS
- we cannot ssh into rds
- you can also have vector storage

## Amazo Aurora

- its like connect with mysql
- its special, it will provide 6 copies for write
- self healing is part of this database
- you can also have vector storage

## DynamoDB

- this is nosql database, like documentDB
- no query joins
- each item only 400kB