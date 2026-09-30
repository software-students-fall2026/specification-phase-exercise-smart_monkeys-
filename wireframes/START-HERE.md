# Abel's wireframes — start here

This is the wireframe draft for the graph and chart part of The Slide Machine. The idea is to let an instructor generate a graph during a lecture, check it, add it to a slide, and fix it later. Students can view the saved graph or chart in the lecture materials.

[Figma file — The Slide Machine / Abel Wireframes](https://www.figma.com/design/wSWJrmAMIJM4rebIHOglQ4)

The file is in **Abel Ma's team**. It includes the screens and the handoff notes. These are static wireframes: the buttons show the intended actions, but the prototype connections still need to be added.

## What to look at first

There are 32 frames, but a lot of them are different states of the same screen. They are not 32 separate features. Start with these paths:

- **Generate a graph:** I01 → I02 → I03 → I04. The instructor asks for a graph, waits for it, checks the preview, and adds it to the slide.
- **Edit a saved graph:** I04 → I05 → I06 → I08. The instructor changes the equation or settings, previews the change, and saves it.
- **Edit a chart:** C01 → C02 → C03 → C04 → C05. This includes reviewing the generated chart, adding it, changing its data, and saving the corrected version.
- **Review as a student:** S01 → S02 → S03. The student sees the original graph, notices that a correction is available, and opens the corrected graph. S08 and S09 show the matching chart views.

I09 and C06 cover editing a new item before it has been added. I10 shows selecting a graph. The other frames cover input errors, failed requests, failed saves, missing graphs, and corrections that are not available yet. S07 shows the student-facing presentation during class.

## How the file is organized

The Figma pages separate the starting notes, instructor graphs, instructor charts, student views, and error states. Each screen has an ID, a short explanation, and the intended button destinations. The longer notes on the left explain what each state is for and how it fits into the flow. The imported frames include editable text and vector shapes. The text outside the application border is there to help us discuss the wireframe; it is not part of the product UI.

The local package includes:

- `svg/`: vector versions of all 32 frames, for importing or adjusting.
- `png/`: full-size previews for quick review and the repository README.
- `overview.png`: a quick look at four main screens.
- `README-wireframes.md`: the full screen list, user-story mapping, flow notes, and images.

## Notes for Matt

The main thing to keep consistent when connecting the prototype is the difference between a new preview and an existing saved graph. A new graph goes through **Add to slide**. Editing a graph that is already on the slide goes through **Save**. Preview should not update what students see, and Cancel should leave the saved content alone.

For the main demo, I would start with graph generation, then edit y = x² to y = x² + 2, and finally show the saved correction in the student view. The chart path is a second example: Week 2 changes from 58% to 64%, and the chart changes from Bar to Line. The saved student chart needs to keep both changes.

The error frames can be connected as alternate paths. A failed save keeps the draft so the instructor can retry. A failed load still lets a student read the lecture text. For retrying a corrected graph, we should request that correction again rather than silently showing the old version as if it were the correction.

Matt is handling the clickable prototype and its public, no-login link. This file provides the wireframes and connection notes for that step.

## Things we still need to agree on

1. **The exact layout and navigation.** I used the screenshots and prototype video shared in the chat. I have not checked Matt's original Figma file or confirmed the exact navigation in the live app yet, so those details still need to be lined up.
2. **How correction messages work.** Rwan's diagram includes both “correction available” and “no correction available” branches. The screens cover both, but we still need to decide how a graph gets marked as needing a correction and how students learn about an update. These screens do not add a separate student feedback system.
3. **Agreement between the screens and diagrams.** The allowance limit comes from the assignment requirements. Field validation and failed-save states fill in the recovery behavior. We should check that the final stories and activity diagrams agree with these choices.
4. **Which chart types we are showing.** The draft includes Bar and Line. The example uses ordered weeks, so a line chart makes sense. We should not automatically use a line for categories that have no order.

## What this draft is based on

I used Rwan's activity diagrams for instructor stories 1 and 7 and student stories 8 and 9, Matt's prototype video and error screenshot from the group chat, and the eight SVG references Rayyan emailed on September 27. Rayyan's files helped with graph selection, editing fields, chart data, and the student views.

This package expands those references into a more complete set of screens and states. Rayyan's reference designs are still his work. Abel's part is the wireframe expansion, the missing states, and the handoff notes, with the team checking the final choices together.
