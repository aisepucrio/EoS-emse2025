# Reading between the Smells: Investigating Developer Responses to Code Smells

This repository contains supplementary results and the data used in the study "Reading between the Smells: Investigating Developer Responses to Code Smells". The study investigates how code smells affect developers' cognitive load, program comprehension, and reading behaviors using eye-tracking technology.

The accepted paper can be accessed here.

## Overview

This study examines the cognitive and perceptual responses of developers to code snippets containing three types of code smells: Long Method, Feature Envy, and Data Class. Code smells are design flaws that degrade software quality and increase the cognitive effort required to comprehend and modify code.

To explore these impacts, we conducted an experiment using the Tobii TX300 eye tracker to measure developers' visual engagement. Metrics such as fixation count (FC) and average fixation duration (AFD) were used to evaluate cognitive load, while qualitative feedback was gathered through developer questionnaires.

The study involved 27 participants, who analyzed 13 Java code snippets selected from the MLCQ dataset. These snippets were manually reviewed and labeled by 26 professional developers from the software industry. Participants identified the presence, type, and severity of code smells, as well as their perceived comprehension difficulty for each snippet.

This repository provides access to the data collected, the analysis scripts, and the code snippets used in the study. The findings aim to inform refactoring strategies, improve developer training, and enhance tools for program comprehension.

## Repository Structure

The repository consists of the following files and directories:

- `data/`: Contains the CSV files with the data used for the analysis.
  - `all_exp_fixations_original2.csv`: Original fixation data.
  - `answers_experiments.tsv`: Developers' answers during the experiment.
  - `code_smell_comprehension_data_rq1.xlsx`: Contains data and analyses directly supporting Research Question 1. Includes both raw data and processed tables used in the study, with each sheet contributing to the analysis of how code smells affect developers' perception of comprehension difficulty.
    - Key Tables:
        - Levels_of_Understanding (Table 1 in the paper): Categorizes participants' comprehension levels, providing a framework for analysis.
        - Difficulty_Categories (Table 2 in the paper): Lists categories of difficulties perceived by developers, such as Logical Complexity and Confusing Names.
        - Code_Smell_Distribution_by_Category_Paper (Table 3 in the paper): Relates difficulty categories to the presence of code smells, highlighting their specific impacts.
        - Smell_Count_By_Level (Table 4 in the paper): Links comprehension levels with the identification of code smells, detailing the frequency of recognized and unrecognized smells.
    - Supplementary Tables:
        - Code_Smell_Distribution_by_Category_v1 and Code_Smell_Distribution_by_Category_v2: Exploratory versions of the distribution of difficulties by categories and code smells.
        - General_Table: Consolidates qualitative and quantitative data, serving as a basis for cross-analyses.
        - General_Table_Translated: Adjusted version of General_Table, translated and prepared for presentation.
        - General_Table_Structured: Refined structure of the general table, facilitating programmatic analyses.
    - Reference Tables for Analysis:
        - the other sheets presented, such as Total_Compre_Yes, Analysis_Total_Compre_Yes, Total_Compre_No and similar ones, represent intermediate data used for building the final tables. These sheets contain segmentations of responses by comprehension levels (e.g., Total Comprehension, No Comprehension) and associated qualitative analyses. Although not directly presented in the paper, they document the analytical process and are available for future exploration.
  
- `notebooks/`: Contains the Jupyter Notebooks for data analysis.
  - `fixation_analisysRQ2.ipynb`: Cognitive effort analysis (RQ2).
  - `fixation_analisysRQ3.ipynb`: Reading behavior analysis (RQ3).
  
- `supplementary/`: Contains additional resources.
  - `data_dictionary.pdf`: Details on the collected data fields.
  - `code_snippets.xlsx`: Description of the 13 analyzed code snippets.
  - `survey.pdf`: The survey used for participant responses.

## Required Skills

The reviewer should have a basic understanding of Java programming to review and understand the code snippets. Familiarity with common Java coding patterns and practices will be beneficial for interpreting the code snippets and identifying the presence of code smells.

## Required Resources

The artifacts can be reviewed and executed on any standard computer system. There are no specific hardware requirements. The artifacts are compatible with any operating system. No additional software packages or specific devices are required.

## Data Provenance

The dataset was sourced from the "MLCQ" dataset, which provides 4,770 manually reviewed code samples from 792 open-source projects. These samples were labeled by 26 professional developers, who provided detailed severity classifications for various code smells. This rigorous manual review process enhances the dataset's reliability and relevance.

## Ethical and Legal Statements

The study was approved by the research ethics committee (CAAE number omitted for anonymity). All participants signed a Free and Informed Consent Form (TCLE), ensuring their data remained anonymous and protected.

## License

This repository is licensed under the GNU License. Please see the LICENSE file for more details.
