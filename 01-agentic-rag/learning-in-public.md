🚀 Module 1 of LLM Zoomcamp by @DataTalksClub — done!

I just wrapped up Module 1: Agentic RAG, and it really demystified the "magic" behind RAG and agents for me. We built the whole thing from scratch in plain Python — no heavy framework hiding the moving parts, so I could actually see how each piece fits.

What I learned to do:
✅ Build a RAG pipeline from scratch: search → build context → prompt → generate
✅ Index and search documents with minsearch (text vs keyword fields, boosting, filtering)
✅ Chunk long documents with a sliding window for sharper, more relevant retrieval
✅ Turn the pipeline into an agent with function calling — hand the LLM a search tool and let it decide when and what to search

The part that clicked for me 💡: chunking isn't just a buzzword. When I measured it, going from whole pages to overlapping chunks cut my prompt from ~8,200 input tokens down to ~2,600 for the exact same question — roughly 3× less context, so cheaper and more precise, with no loss in answer quality.

And the jump to "agentic" is smaller than I expected: it's the same search function, except now the model holds the tool and keeps looping until it's satisfied. In my run the agent chose to search 3 times with different keywords on its own — versus plain RAG's single fixed query. Watching it do that made the whole concept concrete.

Bonus: I ran it with Claude instead of OpenAI just by swapping the client and the usage fields — a nice reminder that these patterns are provider-agnostic.

📓 My full solution (an annotated notebook, step by step): https://github.com/hiagofng/llm-zoomcamp-2026

Huge thanks to Alexey Grigorev for making this knowledge free and this hands-on.

You can sign up here 👉 https://github.com/DataTalksClub/llm-zoomcamp/

#LLM #RAG #AIEngineering #LLMZoomcamp #LearningInPublic
