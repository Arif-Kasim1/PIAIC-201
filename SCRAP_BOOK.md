recipe_llm = HuggingFaceEndpoint(
    repo_id = "Qwen/QwQ-32B-Preview", #"meta-llama/Llama-3.2-3B-Instruct",
    huggingfacehub_api_token = userdata.get('HUGGINGFACE_API_KEY')
)
