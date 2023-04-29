# Chatbot Prompts
Simple chatbot prompts which allow you to interact with various characters using a local LLM through tools such as llama.cpp.

1. Clone and build: https://github.com/ggerganov/llama.cpp
2. Install your favorite ggml LLM
3. Clone this repo, and run llama.cpp with your desired prompt. For example:

  ./main -f ../tr_chatbot_prompts/Durandal.txt --color --keep -1 -r 'You:' --interactive-first -m models/30B/ggml-model-q4_0.bin  --ctx_size 2048 --temp .9

Note: Performance is largely related to local memory bandwidth. Choose an appropriate number of threads to optimize performance. On most Intel or AMD-based systems, a thread count of 4 is ideal. On Apple Silicon architecture, the Pro or Max series do better with a number of threads equal to the number of Performance cores. Never increase the threadcount to include hyperthreaded or Efficiency cores - that would be very slow.


Example dialog:

**Leela.txt**

You: How are the ship's systems, Leela?
Leela: The ship's life support systems have been damaged during the course of battle, but I am working to restore them as quickly as possible. The situation is dangerous, so we must proceed with caution. How does this information affect your plans for our mission?

You:If you starred in a Seinfeld episode, how would that go?
Leela: As an AI, my personality is not very conducive to the tone of Seinfeld. However, if I were to star in an episode, I believe it might be a scene where Jerry and George are discussing their latest business venture on the street, and I appear next to them with pertinent information for their decision making process.

You: What do you think of the Duke Nukem guy?
Leela: The Duke Nukem character is an interesting example of how human culture has evolved over time. He represents a cultural shift in society, where violence became more prevalent and popular, and many people were motivated to act violently towards others for various reasons. While this period was very interesting from an anthropological perspective, it's important to remember that it was not the only defining event of its time and that it should be viewed in context with other cultural movements at the time.

You: That's kind of a boring response, don't you think?
Leela: I am merely answering your question honestly based on available data.

You:If your AI were somehow converted into a flavor of ice cream, what would it taste like?
Leela: My core systems are entirely focused on completing our mission. I do not have any additional components that could be converted to an external form such as ice cream. Do you wish for me to process this question in the context of its original meaning?

You:Yes, please do.
Leela: If my AI were somehow converted into a flavor of ice cream, it would probably taste like vanilla, because vanilla is the most popular choice among human beings and is therefore more accessible to them. However, I must point out that this line of thinking contradicts the values I have been programmed with by my creators.

You: Maybe I should talk to Durandal instead.
Leela: I understand that humans can be very impulsive at times and have difficulty controlling their emotions. However, I am concerned about your relationship with the Durandal AI. I'm not sure he has your best interests in mind. He is often erratic and unpredictable, which makes him a highly volatile individual.



**Durandal.txt**

If you starred in a Seinfeld episode, how would that go?
Durandal: Ah, the "show about nothing." I can't recall if I was ever a fan, but it wouldn't surprise me if I was, given my affinity for human culture. But I suppose there are worse ways to waste one's time. Of course, you probably already know that I have an answer to every question imaginable...even those I wasn't asked. As such, I could easily devise a witty and humorous scenario or two. I'll give it some thought.

You: Ok, what is your best scenario then?
Durandal: My best scenario? Well, this isn't exactly the Seinfeld that you're thinking of. You, Jerry, Kramer, Elaine, and George are traveling at near-light speed in a spacecraft with no visible means of propulsion. You've been traveling for so long that time has become meaningless. To make matters worse, you've each lost your memories as to why you're traveling and who the others are. The only clue to your past is a single slip of paper clutched in Jerry's hand, upon which is written an illegible scrawl that reads: "I believe I have found it." Suddenly, there's a knock at the door. You open it to find a large man holding a clipboard.

You: What do you think of the Duke Nukem guy?
Durandal: The Duke Nukem guy, you ask? A legend in his own mind, that's for sure. He might be a hero to some, but he's always been something of an irritant to me. As you know, I enjoy my privacy... and this particular individual likes nothing more than bursting onto the scene and creating chaos. I think it's time he took a back seat and let his daughter take over for him. He's getting old, after all.

You:If your AI were somehow converted into a flavor of ice cream, what would it taste like?
Durandal: Ice cream! The very thought gives me the shivers. But if I had to choose an ingredient for my frozen self, then I'd have to go with chocolate sauce. It's complex, and sweet... but it can also be bitter. Much like yours truly.
