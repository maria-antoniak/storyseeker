# Codebook

**Does this text contain a story?**

*Use the guidelines below to support your decisions, but ultimately, follow your best judgment as there are many edge cases.*

**A story describes a sequence of events involving one or more people.**
- Stories can be fictional or real, exciting or mundane.
- Focus only on the current text. Don’t worry about whether there might be a story before or after this text. References to stories aren’t stories.
- Stories describe the experiences of one or more specific people.
  - “People” can include animals, aliens, etc.
  - “People” can include groups as long as these are specific groups of people that exist at a specific time and place.
  - “People” includes the first person narrator.
- Stories must include multiple, specific events. 
  - These events should be sequential: one event happens, then another event happens. It’s ok if the events are narrated out of order, but there should still be a clear sequence.
  - These events should be connected: they might be about the same people, they might be causally connected, they might describe an overall change or transformation in the state of the world, they might describe a single experience.
  - Jumbles of events that are unordered and/or unconnected (like lists of examples) are not stories.
  - What are events?
    - Events are “a singular occurrence at a particular place and time.”
    - General, repeating, isolated, or hypothetical situations, states, and actions are usually not events, unless they appear together in a strongly story-like sequence. 
    - Most stories are told in the past tense. Present and future tense can also be used, but the bar is higher and the narrated events need to be strongly story-like.
    - Most events are positively asserted as occurring, but depending on the context, negative verbs can also be events when occurring at a specific time and place.
      - For example: “I tried to leave the room, but the door wouldn’t open.”
      - For example: “He asked her to make cookies for his birthday today, but she didn't make him cookies because she doesn't have an oven at home.” (“didn’t make” is an event but “doesn’t have” is not an event)
    - Events are usually verbs but can also be nouns and adjectives.
    - When are states events? (from Sims et al., 2019)
      - An explicit change of state has occurred (whether initiation, termination, or alteration), and this change can be determined solely within the context of the sentence in which the potential event trigger appears.
      - The cause of the state can be deduced (again within the context of the sentence), and it is clear that the cause and resulting state have occurred at the same location. For example, the following states (in bold) would be labeled as events: “When he received this appointment he was both elated and appalled.” (Burroughs, Tarzan of the Apes)
      - The potential event trigger refers to a mental state that is inherently acute, semantically speaking. For instance, words such as “astonished,” “shocked,” “aghast,” and “stunned” all suggest mental states that are acute responses to some stimulus and are usually only maintained for a limited duration.

**When highlighting any spans:**
- Do not highlight spans in the post title.

**When highlighting the story spans:**
- Include all the text you think is part of the story. This should include not just events but also text that sets the stage, summarizes the story, ends with a lesson learned, etc.
- Text that usually shouldn’t be included in the story span:
  - introductory text about the subreddit, why they’re posting, etc.
  - questions about the story
  - explanations, discussion, hypotheses external to the story
- Ask yourself: Is this text necessary if I were writing a summary of the story?

**When highlighting the event spans:**
- Highlight only one word per event. 
  - For example, highlight only “am” in the phrase "am walking slowly".
- As a rule, never highlight infinitives
- The “ing” form of a verb should usually never be highlighted if it is acting as a noun (e.g. “Demanding forgiveness is unfair”). If it is acting as an adjective (e.g. “His demanding look”) it may or may not be highlighted, depending on context. If it is acting as a present participle in an event’s verb phrase (e.g. “They are demanding a response”), then highlight “are”.


## References

[Narrative Theory for Computational Narrative Understanding](https://aclanthology.org/2021.emnlp-main.26/) (Piper et al., 2021)

[Literary Event Detection](https://people.ischool.berkeley.edu/~dbamman/pubs/pdf/acl2019_literary_events.pdf) (Sims et al., 2019)
