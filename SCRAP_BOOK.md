recipe_llm = HuggingFaceEndpoint(
    repo_id = "Qwen/QwQ-32B-Preview", #"meta-llama/Llama-3.2-3B-Instruct",
    huggingfacehub_api_token = userdata.get('HUGGINGFACE_API_KEY')
)
 
embeddings = GoogleGenerativeAIEmbeddings(model="models/embedding-001",
                          google_api_key=userdata.get("GOOGLE_API_KEY"))
                          
llm = ChatGoogleGenerativeAI(model="gemini-1.5-flash", temperature=0.3)

 self.llm = ChatGoogleGenerativeAI(model="gemini-pro", temperature=0, convert_system_message_to_human=True)
 #"gemini-2.0-flash-exp"
  
 import nest_asyncio
 
 nest_asyncio.apply() #to solve asyncio problem in Crewai Flow
 



 



