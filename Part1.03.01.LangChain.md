## Langchain / Invoke, Stream / content / 

Lanchain connects between GPT and the user by creating chains.
Load documents - QA system - document needs to be read.
Python code can be very long, but Langchain Framework can do this with 2 lines.

Langchain - DB - Embedding - file loader

LangServe - Hosting deployment

Temperature : How much creativity you want

llm = ChatOpenAI(
      temperature=0.1,
      model_name = "gpt-4.1-nano",
      )

question = "What is the population of Edinburgh?"
print(f"[Answer]: {llm.invoke(question)}")

response = llm.invoke(question)
response.content
response.response_metadata


