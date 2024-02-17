### Zero Shot
```
Guidelines:

Use the guidelines below to support your decisions, but ultimately, follow your best judgment as there are many edge cases.
A story describes a sequence of events involving one or more people. 
Stories can be fictional or real, exciting or mundane. Stories describe the experiences of one or more specific people. “People” can include animals, aliens, etc. “People” can include groups as long as these are specific groups of people that exist at a specific time and place. “People” includes the first person narrator.
Stories must include multiple, specific events. These events should be sequential: one event happens, then another event happens. It’s ok if the events are narrated out of order, but there should still be a clear sequence. These events should be connected: they might be about the same people, they might be causally connected, they might describe an overall change or transformation in the state of the world, they might describe a single experience. Jumbles of events that are unordered and/or unconnected (like lists of examples) are not stories.\nEvents are “a singular occurrence at a particular place and time.” General, repeating, isolated, or hypothetical situations, states, and actions are usually not events. Most stories are told in the past tense. Present and future tense can also be used, but the bar is higher and the narrated events need to be strongly story-like. Most events are positively asserted as occurring, but depending on the context, negative verbs can also be events when occurring at a specific time and place. Events are usually verbs but can also be nouns and adjectives.


Task:

Does the following text contain a story? Answer YES or NO, and then briefly explain your reasoning.

Text:

<INSTANCE TEXT (EXCLUDING TITLE)>

Answer: 
```

### Few-Shot
Same as Zero shot, except with an "Examples:" section between the "Task:" and "Text:" sections. We sample from the training dataset until we have a total of k examples, evenly split between positive (i.e. story) and negative (i.e. not story) instances from the training dataset. We break ties by including an extra negative example if k is odd. We then interleave the negative and positive samples in the "Examples:" section.

Mock example for k=2:
```
Examples:

Text: <POSITIVE INSTANCE TEXT (EXCLUDING TITLE)>

Answer: YES

Text: <NEGATIVE INSTANCE TEXT (EXCLUDING TITLE)>

Answer: NO
```


### Chain-of-Thought
```
Your task is to decide whether a text contains a story. You should follow the guidelines below and think step by step.
Use the guidelines below to support your decisions, but ultimately, follow your best judgment as there are many edge cases.
A story describes a sequence of events involving one or more people. 
Stories can be fictional or real, exciting or mundane. Stories describe the experiences of one or more specific people. “People” can include animals, aliens, etc. “People” can include groups as long as these are specific groups of people that exist at a specific time and place. “People” includes the first person narrator.
Stories must include multiple, specific events. These events should be sequential: one event happens, then another event happens. It’s ok if the events are narrated out of order, but there should still be a clear sequence. These events should be connected: they might be about the same people, they might be causally connected, they might describe an overall change or transformation in the state of the world, they might describe a single experience. Jumbles of events that are unordered and/or unconnected (like lists of examples) are not stories.\nEvents are “a singular occurrence at a particular place and time.” General, repeating, isolated, or hypothetical situations, states, and actions are usually not events. Most stories are told in the past tense. Present and future tense can also be used, but the bar is higher and the narrated events need to be strongly story-like. Most events are positively asserted as occurring, but depending on the context, negative verbs can also be events when occurring at a specific time and place. Events are usually verbs but can also be nouns and adjectives.

Using the definitions for 'people' and 'events' given in the guidelines above, answer the following questions
Question 1: Does the text contain 'people'? If so, list them.
Question 2: Does the text contain a sequence of causally connected 'events'. If so, list them.
Finally, based on the guidelines and your answers to Question 1 and Question 2, decide whether the text contains a story. Respond 'Yes' or 'No'.
Two examples are provided below:

Example 1:
'Yesterday, I went to the store to buy a jug of milk so that I could make pancakes. When I arrived, the cashier told me that the store lost power the previous night, so all the milk spoiled. So much for pancakes!'

Question 1 Answers: ['I', 'cashier'].
Question 2 Answers: ['went', 'arrived', 'told', 'lost', 'spoiled']. 
Story Decision: Yes

Example 2:
'Not a good FDIC tip. Coverage levels start at $250k and can be increased by certain multipliers--so that's not really a concern unless you've got several million in the bank.'
Question 1 Answers: []. 
Question 2 Answers: []. 
Story Decision: No

Your turn. Text:
<INSTANCE TEXT (EXCLUDING TITLE)>
```