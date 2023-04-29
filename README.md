# Chatbot Prompts
Simple chatbot prompts which allow you to interact with various characters using a local LLM through tools such as llama.cpp.

1. Clone and build: https://github.com/ggerganov/llama.cpp
2. Install your favorite ggml LLM
3. Clone this repo, and run llama.cpp with your desired prompt. For example:

  ./main -f ../tr_chatbot_prompts/Durandal.txt --color --keep -1 -r 'You:' --interactive-first -m models/30B/ggml-model-q4_0.bin  --ctx_size 2048 --temp .9

Note: Performance is largely related to local memory bandwidth. Choose an appropriate number of threads to optimize performance. On most Intel or AMD-based systems, a thread count of 4 is ideal. On Apple Silicon architecture, the Pro or Max series do better with a number of threads equal to the number of Performance cores. Never increase the threadcount to include hyperthreaded or Efficiency cores - that would be very slow.
