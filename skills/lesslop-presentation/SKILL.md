---
name: lesslop-presentation
description: "Create presentations for requests such as 'make a presentation' or 'prepare slides': gather inputs, build HTML slides, choose a visual style, refine design and copy, and deliver a finished PPTX. Activate automatically when the user asks to create a presentation; do not activate for simply discussing presentations or creating skills."
---

# Create a Presentation

Create the presentation using five required skills: `frontend-slides`, `ui-ux-pro-max`, `impeccable`, `humanizer`, and `pptx`. The primary deliverable is a finished `.pptx` file. Also preserve the HTML presentation as source.

## Before starting: four inputs

First review the original request, attached materials, and known context. Before developing the structure, copy, or design, ask only for missing items from these four:

1. **What is the presentation about?** For example: “How to customize Codex.”
2. **Who is the audience?** For example: “People who are starting to learn Codex.”
3. **What source material should the presentation use?** For example: marketing copy, notes, a document, a spreadsheet, or links. The user may say there are no prepared materials and ask you to develop the content.
4. **What visual references should guide the style?** Request three or four references: images, links, or example presentations.

Ask all missing questions in one message. You may use an available question tool for text answers, but request file or image attachments in an ordinary message. If all four inputs are known, begin immediately. Do not repeat questions the user has already answered.

Wait for answers to missing inputs. “No materials,” “no references,” or “choose for me” are sufficient answers: develop the content or choose a visual direction yourself. If fewer than four references are provided, use what is available; do not demand more merely to reach a count.

These four inputs replace the standard Frontend Slides intake questionnaire. Do not add mandatory questions about slide count, content density, or presentation format. Use parameters the user provides and make reasonable choices for everything else based on the topic and audience. Ask further questions only to resolve a substantial contradiction or unavailable essential material.

## Five skills and the workflow

Read each skill's current `SKILL.md` before applying it. Find them by name in the available skill catalog; common installation locations are `~/.codex/skills/` and `~/.agents/skills/`. Follow their working instructions while respecting the order, intake process, and PPTX delivery requirement here. Merely mentioning a skill does not count as applying it. If a required skill is missing, identify it and do not claim to have completed the full workflow.

1. **Frontend Slides — structure and slide assembly.** After receiving the inputs, identify the main message, organize the sequence, and build the HTML presentation. Use a fixed 16:9 canvas according to the skill's instructions unless the user specifies another format. Determine slide count from the content and audience. Do not invent facts or figures; distinguish supplied information from assumptions.
2. **UI UX Pro Max — typography, colors, and shapes.** Before assembling the full deck, choose a coherent system: a font pairing, type hierarchy, palette, shapes, and graphic elements. Use the skill's search tools to inform these choices. Check support for the presentation's language, including Cyrillic when relevant, and font availability in both HTML and PowerPoint. Apply the system across every slide.
3. **Impeccable — art direction and design refinement.** Define a visual concept based on the topic and references, then review the completed slides for composition, hierarchy, rhythm, spacing, contrast, and readability. Fix generic solutions, arbitrary decoration, and inconsistencies. Keep a consistent character while varying compositions.
4. **Humanizer — copy editing.** Edit titles, body copy, captions, and speaker notes when present. Remove formulaic AI language, bureaucratic phrasing, empty promises, and artificial conclusions. Preserve meaning, facts, terminology, and the author's voice. After editing, check line breaks and text placement.
5. **Pptx — finished PowerPoint.** Read this skill's instructions during planning so the design can be reproduced in PPTX. Create a genuine `.pptx` from the final HTML slides, preserving content, order, proportions, and the visual system. Make text, basic shapes, tables, and supported charts editable using native PowerPoint elements; complex visual effects may use images. Do not replace the entire presentation with screenshots unless the user explicitly requests it. Adapt browser animations to a static state without losing meaning.

Art direction and copy editing may begin before assembly and be repeated on completed slides. If the user has already defined a style or provided sufficient references, follow them without requiring a choice between three new directions. When no direction exists, use visual previews according to Frontend Slides.

## Validation and delivery

- Check the narrative sequence, material coverage, factual accuracy, and absence of fabricated sources.
- Check the HTML and the final PPTX separately for clipped text, overlaps, line breaks, fonts, contrast, margins, and consistent styling.
- Complete the mandatory file validation and visual inspection of every slide according to `pptx`. Fix problems and inspect changed slides again. Checking HTML does not replace checking PowerPoint.
- Deliver the finished `.pptx` link first, followed by the HTML source link. Briefly state the slide count and any remaining material limitations. Do not claim that export or validation succeeded if it was not completed.
