# 📂 Local Doc Q&A Starter Kit

**Goal:** Ask questions about your own documents securely, without sending data to the cloud.

## What you need
- Open WebUI or Flowise installed locally
- A folder of PDFs (health records, manuals, research papers)
- LlamaIndex or Chroma DB for embeddings

## Steps
1. **Set up document ingestion**
   ```yaml
   tools:
     - name: "local_docs"
       type: "llama_index"
       config:
         path: "./docs"
   ```

2. **Import a Starter Prompt**

   ```
   You are my Local Doc Q&A Agent.
   - Answer questions ONLY from my uploaded documents.
   - If the answer isn’t in the docs, say: "I don’t see that here."
   - Always provide the source (file name + page).
   ```

3. **Run your first query**
   Upload a PDF (like a medical lab report).  
   Ask: *"What was my cholesterol level on my last test?"*

## Next Step
Add more docs and build a personal knowledge hub.
