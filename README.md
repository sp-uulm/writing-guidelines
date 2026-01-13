# Writing Guidelines

This document summarizes general writing guidelines at the
[Institute of Software Engineering and Programming Languages][sp]
at [Ulm University][uulm].
If you have suggestions for improvements, or think something is outdated, please open [a new issue][new-issue].

<p align="center">

   [[General](#general-guidelines)] &emsp;•&emsp; [[Proposal](#proposal-specific-guidelines)] [[Thesis](#thesis-specific-guidelines)] [[Presentation](#presentation-specific-guidelines)]

</p>

All of these guidelines are subject to discussion with your supervisor to be adapted to your specific scenario.

Current list of templates provided by the institute can be found on the [SP GitHub page][sp@github] or the general [template page][fancy-templates@github]

## General Guidelines

These guidelines apply to all types of scientific writing at our institute, like lecture papers, theses (bachelor and master), and the accompanying presentations.

### Formatting and Language

- Stay consistent!\
  No matter whether you use British or American English, or whether you prefer the Oxford comma or not: Just stay consistent throughout your work.
  And, of course, make sure that you not suddenly break context and introduce new things/concepts, etc. &mdash; we can do better than the average LLM.
- Abide by the template-specific formatting guidelines (check out the [SP GitHub page][sp@github] or the general [template page][fancy-templates@github] for available templates).
- Follow the current guidelines on AI usage in scientific writing as provided by your supervisor or institute ([Ulm University AI Guidelines][]).
- Tense-wise we follow this convention: present tense is used for everything that relates to your work. 
  For example, instead of "Section 7 will introduce..." or "we will show more of this in..." we write "Section 7 introduces..." and "we show more of this in...". Past tense may be used for existing works and processes that happened before your thesis while future tense should be reserved for future work  (i.e., things that happen after your thesis).
- Use a spell or grammar checker (e.g., [Grammarly](https://www.grammarly.com/), [LanguageTool](https://languagetool.org/), or the built-in checkers of your text editor). A couple of typos are acceptable, but too many distract from the content and look unprofessional.
- Do not use `\\` for creating paragraphs, just use empty lines for creating a new paragraph. The template will take care of the correct visual layout.
- Whenever you come up with a descriptive and fitting section title,
  try to avoid leading "The"/"A"/"On" etc. (we may use these for example headings). Generally, "Characteristics of the Penguin Species" reads much better than "The Characteristics of the Penguin Species" (especially when most of the other sections would also start with "The")
- Present your ideas in easy to follow, complete sentences.\
  Bullet-points are fine for summaries, just like this document, but they make your work harder to follow and look "cheap"/incomplete. If you have difficulties formulating complete sentences, check out resources like a [Phrase Book](https://phrasebankresearch.net/wp-content/uploads/2019/10/Academic-Phrasebank-Sample-PDF-2018.pdf).
- [Know your dashes!](https://www.merriam-webster.com/grammar/em-dash-en-dash-how-to-use)\
  In LaTeX, we use `-` (-) for hyphens, `--` (&ndash;) for en-dashes (like numeric ranges `pages 12--23`), and `---` for em-dashes &mdash; like this.

### Citations

- Do not "just" cite a paper from, e.g., [arXiv][] without quality control like peer review.[^1]
- Whenever possible, try to use the bibliography entries provided by [dblp.org][] and ensure that a [DOI][] is available for the respective entry (ask your supervisor whether a procured bibliography for important references is already available).
- When citing, make sure that references contain not just author, title, and year, but also the venue (e.g., the conference like ICSE, MSR, ASE, or a journal like TSE, TOSEM, or JSS).
- Prefer full publications over vision, tool-demo, or (especially) poster publications.
- We don't want to have citations at the start of a line.\
  In LaTeX, you can use `~` to prevent a line break between two words (a non-breaking space). For example, instead of writing `cute \cite{Sihler2025,Sihler2026}`, write `cute~\cite{Sihler2025,Sihler2026}`.
- We try to avoid cites-as-subjects with numeric citation styles.\
  Instead of writing "As shown by [2]", we prefer "As shown by Sihler et al. [2]". In LaTeX you can use something like `\citeauthor*{Sihler2025}~\cite{Sihler2025}`.
- This includes [presentations](#presentation-specific-guidelines). Here an on-slide citation should read, e.g. "Sihler et al. (ICSE, 2025): On the Cuteness of Penguins".
- Use a proper system to format citations (like [BibLaTeX](https://ctan.org/pkg/biblatex), templates should already include this).

### Follow Best-Practices

I mean, this sounds obvious, but still, there are countless existing best practices for writing scientific texts but also for conducting evaluations, and more. The following is just an incomplete list and you should definitely ask your supervisor for further guidance.

- Empirical (Software) Evaluations:\
  [SIGSOFT Empirical Standards](https://www2.sigsoft.org/EmpiricalStandards/), [SIGPLAN Checklist](https://raw.githubusercontent.com/SIGPLAN/empirical-evaluation/master/checklist/checklist.pdf)
- Picking the best/correct visualization for your data:\
  <https://www.data-to-viz.com/>

## Proposal-Specific Guidelines

Please be aware, that these guidelines hold _additionally_ of the [General Guidelines](#general-guidelines).

- Include rough estimates of your work.\
  Of course you cannot know exactly how long something will take, but roughly calculating the time against the available time (e.g., roughly 45 days for a bachelor's thesis) helps to judge the feasibility of your planned work.[^2]
- Ideally plan multiple iterations of your work to conduct intermediate evaluations and implement feedback from earlier iterations.
- Plan an additional buffer for writing your thesis before the submission date (at least 2 weeks buffer)

## Thesis-Specific Guidelines

Please be aware, that these guidelines hold _additionally_ of the [General Guidelines](#general-guidelines).

### Thesis-Specific Content Guidelines

- Include a proper abstract summarizing your work.\
  Style-wise we recommend you follow a [structured abstract](https://web.archive.org/web/20250807230549/https://procomm.ieee.org/transactions-of-professional-communication/for-prospective-authors/guidelines-to-follow/preparing-structured-abstracts/) approach.
- We do not write click-bait articles.\
  Start with the most important information and the results. List the details afterward. Ideally, your work follows a "pyramid shape" in which you progressively go into more and more detail for the specific aspects of your work.
- The "pyramid" metaphor also holds for the thesis at large. The abstract and the introduction should cover/summarize all parts of the thesis at a high abstraction level. Each individual chapter then goes into the details of that chapter's topic.
- Consequently, already answer your research questions/list your contributions in the introduction.\
  You can also hint at them in the abstract, but your introduction should communicate to the reader what your research questions are and how you answered them (i.e., what your contributions are).
- For bigger segments like chapters and sections, include [topic-sentences](https://web.archive.org/web/20250913173407/https://academic-englishuk.com/topic-sentences/).\
  These summarize the content of the respective segment and help the reader to quickly grasp the content (e.g., when skimming through the document).
- Know your limits, know your threats.\
  Threats to validity are an important part of scientific work. Make sure to discuss the limitations of your work and how they might threaten the validity of your results (e.g. [Types of Validity](https://web.archive.org/web/20250620015439/https://tagvault.org/blog/types-of-validity/), also consider [Lago et al., ESEM '24](https://doi.org/10.1145/3674805.3686691)).

### Submitting your Thesis

- Include the signed declaration of authenticity\
  (The thesis template provides a module for this). The thesis submission is only valid if a signed declaration of authenticity is included in the submitted thesis.
- Persist your final state in an easily accessible way.\
  We encourage you to (at least at Ulm University) upload the compiled version of your final and submitted thesis to your thesis repository as well.
  Please use the format `<Surname><Firstname>-<Type>.pdf` for the file name, where `<Type>` is either `BachelorThesis` or `MasterThesis` (e.g., `SihlerFlorian-MasterThesis.pdf`).
- Alongside your thesis you usually have to submit a reproducibility package. Please check out the respective guidelines ([Ulm University Rep-Package Guidelines][]).
- Read the [University FAQ Page](https://www.uni-ulm.de/studium/pruefungsverwaltung/pruefungen-und-module-faq/) for up-to-date information on submission guidelines.

## Presentation-Specific Guidelines

Please be aware, that these guidelines hold _additionally_ of the [General Guidelines](#general-guidelines).

- Provide citations _on_ the slides.\
  These allow to quickly search for the reference during the presentation.
  The citation should (at least) contain the title, year, first-author and venue (e.g., "Sihler et al. (ICSE, 2025): On the Cuteness of Penguins").

[^1]: If you are unsure about the quality of a reference, please discuss this with your supervisor. In general, if there exists a peer-reviewed version of a work, prefer citing that version.
[^2]: Consider a classical benchmark evaluation. If you do not at least estimate the maximum runtime you may be stumped by an evaluation that was deemed sufficient but requires multiple weeks or months of computation. Something like 10k files, with a timeout of 5 minutes each results in (without parallelization) over 34 days of computation time - just for a _single_ run. And benchmarks should always be run multiple times to account for variance.

[arXiv]: https://arxiv.org/
[DOI]: https://www.doi.org/
[dblp.org]: https://dblp.org/
[new-issue]: https://github.com/sp-uulm/general-writing-guidelines/issues/new
[uulm]: https://www.uni-ulm.de/
[sp]: https://www.uni-ulm.de/in/sp/
[sp@github]: https://github.com/sp-uulm/
[fancy-templates@github]: https://github.com/Fancy-Templates
[Ulm University AI Guidelines]: https://github.com/Fancy-Templates/latex-thesis/blob/main/ai-rules-uulm.md
[Ulm University Rep-Package Guidelines]: https://github.com/Fancy-Templates/latex-thesis/blob/main/rep-package-guidelines.md
