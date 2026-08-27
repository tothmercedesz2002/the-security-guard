# The Security Guard

The Security Guard is a novel experimental paradigm designed to investigate **metamemory, source monitoring, and memory distrust**.

Participants take the role of a security guard whose task is to secure an area before going home.

## Learning phase

Participants are presented with **40 potentially unsafe scenarios**, such as a kettle that has been left plugged in.

- In the **action condition** (20 scenarios), participants press the spacebar to secure the object.
- In **5 action trials** (25% of the action trials), a brief visual glitch disrupts the confirmation that the object has been secured.
- In the **imagination condition** (20 scenarios), participants do not press a key but vividly imagine securing the object.

## Testing phase

Participants attend a follow-up meeting with their supervisor and answer questions about the previous night's work.

The test contains all **40 previously presented items** and **10 novel lure items**. For each item, participants answer:

1. **Recognition question:** Did you see this object? (Yes/No)
2. **Source-monitoring question:** If so, did you act on it or imagine acting on it?

After each response, participants rate their **confidence** on a scale from 0 to 100.

## Randomization

The task contains **50 scenarios** in total. For each participant, stimuli are randomly assigned while maintaining the following fixed allocation:

- 40 learning items and 10 lure items
- 20 action items and 20 imagination items
- 5 glitch trials and 15 non-glitch trials among the action items

## Files

The `img/` folder contains the images used in the experiment. The scenario images were generated using Gemini 3.1 Pro. The transparent glitch overlay was adapted using OpenAI's image-generation tool.

The trial descriptions and experimental logic can be inspected in `index.html`.

## Online demo

**[Try The Security Guard task](https://tothmercedesz2002.github.io/the-security-guard/)**

> The current version is a research prototype. At the end of the task, the collected CSV file is downloaded locally to the participant's device; no research data are currently transmitted to a server.

> A desktop or laptop computer with a physical keyboard is required.
