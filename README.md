# Specification Phase Exercise

A little exercise to get started with the specification phase of the software development lifecycle. In this exercise, your team specifies a set of improvements and new features for [The Slide Machine](https://theslidemachine.com) — see the [instructions](instructions.md) for detail, and the [background](background.md) for an introduction to the software product you are tasked with extending.

## Team members

See instructions. Delete this line and replace with a list of the names of your team members, including links to each one's GitHub profile.

## Review of the Current Application

See instructions. Delete this line and replace with your team's findings from using the live app at https://theslidemachine.com — at least 10 specific observations, each labeled as a strength, a weakness, or a gap, and drawn from more than one team member's use of the app.

## Prior Art & Originality

See instructions. Delete this line and replace with a short statement of what your team checked (the project's Future Work and Open Questions, its roadmap, and its open issues and pull requests) and which parts of your proposal are original — new work not already specified, scheduled, or proposed by someone else.

## Stakeholders

See instructions. Delete this line and replace with the name(s) of the stakeholder(s) you interviewed and lists showing their goals/needs, and problems/frustrations. Note which type of user each stakeholder represents. You may use pseudonyms or partial names to maintain their privacy, but you must privately share their full names and contact information as part of your submission of this exercise

## Product Vision Statement

See instructions. Delete this line and place your Product Vision Statement here — one sentence describing the improvements and new features your team is proposing for The Slide Machine.

## User Requirements

See instructions. Delete this line and place a list of your User Stories here, grouped by type of user. These should describe functionality that is new or changed, not functionality the app already has.

## Activity Diagrams

See instructions. Delete this line and place images of your UML Activity diagrams here, each with the text of the user story it illustrates.

## Wireframes

These wireframes show how instructors generate, check, and edit graphs and charts during a lecture, and how students view the saved versions in shared materials. There are 32 frames covering the main flow and its different states, including validation errors, failed requests, failed saves, and unavailable corrections.

- [Open the editable Figma file](https://www.figma.com/design/wSWJrmAMIJM4rebIHOglQ4?node-id=2-2)
- [Start here: scope, main paths, and notes for Matt](wireframes/START-HERE.md)
- [See all 32 screens with explanations and button paths](wireframes/README-wireframes.md)
- [Jump to individual screens in Figma](wireframes/FIGMA-LINKS.md)

![Overview of graph preview, graph editing, chart editing, and the student view](wireframes/overview.png)

| Group | Screens | What they cover |
|---|---|---|
| Instructor graphs | I01–I10 | Requesting a graph, checking the preview, adding it, selecting it, and editing the saved version |
| Instructor charts | C01–C08 | Reviewing a chart, editing its data and labels, previewing changes, and handling invalid values or a failed save |
| Student views | S01–S09 | Viewing saved graphs and charts, opening corrections, and continuing when a visual cannot load |
| Errors and recovery | E01–E05 | Connection problems, an unrecognized equation, unsupported requests, the usage limit, and graph save failures |

For the main graph flow, follow **I01 → I02 → I03 → I04**. To edit it, continue through **I05 → I06 → I08**. The matching student correction flow is **S01 → S02 → S03**. The chart example follows **C01 → C02 → C03 → C04 → C05**, with **S08/S09** showing the original and corrected student views.

A new graph or chart is only added after **Add to slide**. Changes to an existing one stay as a draft until **Save** succeeds. **Cancel** keeps the original. Each screen's notes explain the alternate paths and the related user stories.

These are static wireframes; Matt is handling the clickable prototype. The exact navigation still needs to be checked against the live app and Matt's original file. The team also needs to agree on how correction availability is detected. Those open points are listed in the handoff notes.

Prepared by **Abel Ma**, using Rayyan's eight SVG references, Rwan's activity diagrams, and Matt's shared prototype video and error screenshot. This contribution expands those references into the screen states and handoff notes shown here. The reference designs remain credited to their authors.

The [PNG previews](wireframes/png/) can be viewed directly in the repository. The [SVG files](wireframes/svg/) are included for editing and importing.

## Clickable Prototype

See instructions. Delete this line and place a publicly-accessible link to your clickable prototype here.

## Stakeholder Demo

See instructions. Delete this line and place a link to the deck The Slide Machine generated during your presentation here, after you have presented.

## Exit Ticket

See instructions. Delete this line and place a link to the exit-ticket quiz you generated from your demo deck and distributed to the class, along with a short note on what — if anything — you had to correct in the generated questions before publishing.
