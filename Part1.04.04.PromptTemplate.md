LCEL pipeline - chain = prompt | model | output_parser

### PromptTemplate

template: template str {}
input variables:

template: "{country} capital city"
prompt = prompt_template.format(country="Korea")
prompt = prompt_template.format(country="US")

prompt = PromptTemplate.from_template("Tell me about this {topic}")
model = ChatOpenAI()
chain = prompt | model | OutputParser


