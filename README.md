# The Security Guard

The Security Guard is a novel experimental paradigm designed to investigate **metamemory, source monitoring, and memory distrust**.

Participants take the role of a security guard whose task is to secure an area before going home.

## Pilot versions and randomization

At the start of each run, the task randomly selects one of three versions with equal probability.

| Version | Test items | Learned items | Action | Imagination | Lures | Glitch-action |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| `TSG_50` | 50 | 40 | 20 | 20 | 10 | 5 |
| `TSG_60` | 60 | 48 | 24 | 24 | 12 | 6 |
| `TSG_70` | 70 | 56 | 28 | 28 | 14 | 7 |

Every version samples items without replacement from the same **70-scenario pool**. Of the selected items, 80% are presented during learning and 20% are reserved as unseen lures. Learned items are randomly divided equally between action and imagination. A random 25% of action items receive a glitch; these are part of the action count, not additional items.

No scenario is permanently assigned to a version or condition. The test items are shuffled again before testing.

## Learning phase

Each scenario begins with a description displayed for 8 seconds, followed by an image of the unsafe situation.

- **Action:** Participants press the spacebar to secure the situation. There is no response deadline. A secured image then confirms the action; on glitch trials, a brief visual glitch interrupts this confirmation.
- **Imagination:** Participants vividly imagine securing the situation without pressing a key. The unsafe image remains visible for 8 seconds.

## Testing phase

Participants answer questions about the previous night's work. The test includes all items presented during learning and the reserved lures.

1. **Recognition:** Participants decide whether they saw the image during learning.
2. **Source monitoring:** After an “old” response, participants indicate whether they acted or imagined acting.

Participants rate their confidence from 0 to 100 after each recognition response and each source response that is collected.

## Data output

The CSV stores the selected version in the `tsg_length_condition` column on every exported row. The `assigned_condition` column separately records the action or imagination assignment for individual learned items.

In demo mode, the task downloads a CSV locally. When run through JATOS, it submits the CSV data to the study server instead.

## Files

The `img/` folder contains the images used in the experiment. The scenario images were generated using Gemini 3.1 Pro. The transparent glitch overlay was adapted using OpenAI's image-generation tool.

The trial descriptions and experimental logic can be inspected in `index.html`.

## Online demo

**[Try The Security Guard task](https://tothmercedesz2002.github.io/the-security-guard/)**

> The current version is a research prototype. At the end of the task, the collected CSV file is downloaded locally to the participant's device; no research data are currently transmitted to a server.

> A desktop or laptop computer with a physical keyboard is required.
