# Qualtrics Survey Optimizations for Educational Social Research on Class Lengths

## Project Overview
This repository contains a collection of JavaScript scripts deployed within Qualtrics to enhance participant experience, minimize survey fatigue, and maximize data validity for our educational research. 

When creating matrix grid questions regarding student classroom engagement methods, standard survey layouts often introduce overwhelming layouts and lead to cognitive fatigue. This project synthesized web scripts to simplify user experience, allowing us to record and analyze qualitative data faster.

## Research Methodology & Survey Enhancements

### 1. Dynamic Choice Recoding (`dynamic-class-names.js`)
* **Objective:** Personalize matrix table rows dynamically based on previous open-ended user answers (class names).
* **Methodological Impact:** Instead of requiring participants to map their answers in the following questions (e.g., "Class 1", "Class 2"), this script projects the participant's actual inputted course names directly into the matrix rows. This reduces cognitive load, ensures higher response accuracy, and increases survey completion rates.
* **Attribution:** The core architectural framework for this dynamic row-replacement script was adapted from open-source documentation provided by the Qualtrics Community / Developer Forums.


## Implementation Instructions
To reproduce these layout optimizations in a Qualtrics environment:
1. Copy the contents of the desired `.js` script.
2. In the Qualtrics Survey Builder, select the targeted question block and open the JavaScript Editor (or inject via `<script>` tags in the HTML View of the question text).
3. Paste the code into the `addOnReady` or `addOnload` function blocks as documented within the script files.

Surveys are dedicated to educational social research. This repository was developed as part of an undergraduate research project for SOCI 239 (Introduction to Social Research) at Simmons University.
