# Qualtrics Survey Optimizations for Social Research on Education Class Times

## Project Overview
This repository contains a collection of JavaScript scripts deployed within Qualtrics to enhance the participant experience, minimize survey fatigue, and maximize data validity for longitudinal educational research. 

When deploying complex matrix grids regarding student classroom engagement, standard survey layouts often introduce cognitive clutter. This project utilizes customized web scripts to streamline user interfaces and capture granular qualitative data dynamically.

## Research Methodology & Survey Enhancements

### 1. Dynamic Choice Recoding (`dynamic-class-names.js`)
* **Objective:** Personalize matrix table rows dynamically based on prior open-ended user inputs.
* **Methodological Impact:** Instead of forcing participants to map their answers to abstract placeholders (e.g., "Class 1", "Class 2"), this script injects the participant's actual inputted course names directly into the matrix rows. This reduces cognitive load, prevents alignment errors, and ensures higher contextual accuracy in responses.
* **Attribution:** The core architectural framework for this dynamic row-replacement script was adapted from open-source documentation provided by the Qualtrics Community / Developer Forums.

### 2. Contextual Field Visibility (`conditional-other-toggle.js`)
* **Objective:** Dynamically generate and reveal a text clarification box only when a participant selects the "Other" checkbox within a specific course matrix row.
* **Methodological Impact:** Keeps the survey instrument compact and visually clean. It prevents overwhelming participants with dozens of empty conditional text boxes upfront while still seamlessly gathering qualitative, open-ended explanations on demand.

## Implementation Instructions
To reproduce these layout optimizations in a Qualtrics environment:
1. Copy the contents of the desired `.js` script.
2. In the Qualtrics Survey Builder, select the targeted question block and open the JavaScript Editor (or inject via `<script>` tags in the HTML View of the question text).
3. Paste the code into the `addOnReady` or `addOnload` function blocks as documented within the script files.
