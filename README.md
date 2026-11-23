# Lesson Desk Skill

Prepare English, Chinese language arts, and chemistry lessons in Hermes Agent or another compatible Agent Skills client. Generate editable PowerPoint slides and a courseware package you can import into [Lesson Desk](https://github.com/zazedwhwhy/lesson-desk).

[Download v0.5.0](https://github.com/zazedwhwhy/lesson-desk-skill/releases/download/v0.5.0/lesson-desk-export-v0.5.0.zip) · [Release notes](https://github.com/zazedwhwhy/lesson-desk-skill/releases/tag/v0.5.0) · [SHA-256 checksum](dist/SHA256SUMS.txt)

## Use with Hermes Agent

1. Extract the ZIP and place the entire `lesson-desk-export` directory in the active Hermes profile's skills folder. The default is `~/.hermes/skills/`.
2. Run `/reload-skills`, then invoke `/lesson-desk-export` with your reading passage or exam paper. Include the relevant answer key for question-by-question review.
3. Open Lesson Desk and choose **Import Courseware Package** from the project library. Select the generated `.lesson.zip` to review and edit it. Importing and editing require no Lesson Desk API key.

Hermes needs a connected model, Node.js 22 or later, and access to the files in its execution environment. Chemistry formula previews in PowerPoint also require `@napi-rs/canvas@1.1.0` in the script's working directory.

> /lesson-desk-export Make a vocabulary notebook and sentence analysis for this English reading. For questions 21–24, explain which lines support or rule out each option. Deliver an editable PowerPoint and a Lesson Desk courseware package.

## Subject coverage

| Subject | Teaching materials |
| --- | --- |
| English | Question-by-question explanations, Chinese translations, sentence analysis, passage structure, vocabulary notebooks, writing transfer, and independent practice. Targeted reviews cover answer-choice evidence, gap-fill cohesion, cloze clues, writing prompts, and story continuation. |
| Chinese language arts | Question-by-question explanations, text structure, close reading, Classical Chinese translation and annotation, writing guidance, and practice. |
| Chemistry | Question-by-question explanations, concept summaries, problem-solving methods, experiment analysis, and practice. |

All three subjects support exam organization, scanned-page transcription, and review reports. Chemistry can retain candidate figures cropped from the source paper. English supports evidence-based corrections with an undo record. For preparation-only work, request the courseware package and review checklist without a PowerPoint file.

Question reviews check the reference answer against its cited source. If you ask the model to solve questions without an answer key, the proposed solutions stay in a review draft until a teacher confirms them. PowerPoint export uses the passages, questions, and modules you select.

## Source and license

The packaged Node.js builder is maintained with Lesson Desk. See the [TypeScript source](https://github.com/zazedwhwhy/lesson-desk/tree/61279437d2500d0edbd7e4c2a853c98d7fdc5806/skills/lesson-desk-export/tool) and [packaging script](https://github.com/zazedwhwhy/lesson-desk/blob/61279437d2500d0edbd7e4c2a853c98d7fdc5806/scripts/package-lesson-skill.mjs). The Skill uses the [MIT License](LICENSE). Third-party notices are included in `skills/lesson-desk-export/licenses/`.
