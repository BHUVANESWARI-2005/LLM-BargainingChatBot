# LLM-BargainingChatBot

**About the project:**


This project is a Bargaining Chatbot that simulates price negotiation with a user. It combines basic reinforcement learning logic with a pretrained GPT-2 model to create a natural and interactive chat experience. The chatbot starts with an initial selling price and interacts with the user through a negotiation loop, choosing actions like Accept, Reject, or Counteroffer.

While GPT-2 is used for generating textual responses, the core decision-making logic for bargaining is rule-based and can be enhanced further with more advanced learning techniques.

**Implementation Details**


The chatbot begins with a starting price and a predefined action mapping (Accept, Reject, Counteroffer).

The decision engine chooses actions based on the user's offer:

If the offer is high enough → Accept

If it's close → Counteroffer

Otherwise → Reject

The chatbot's responses are currently simulated based on the selected action.

A pretrained GPT-2 model is loaded to optionally generate natural language responses (can be expanded to fully control the chatbot dialogue).

An exploration rate is included to occasionally introduce random actions for a more realistic and dynamic conversation.


**Required Lbraries :**

```
pip install torch transformers numpy
```

