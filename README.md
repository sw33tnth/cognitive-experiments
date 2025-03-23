# Cognitive Experiments: Go/No-Go and SART

This repository contains a web-based cognitive experiment implemented using jsPsych, consisting of two tasks: a Go/No-Go task and a Sustained Attention to Response Task (SART). The experiment measures inhibitory control and sustained attention, respectively, and is deployed on GitHub Pages for online access.

## Experiment Overview

- **Purpose**: To measure inhibitory control (Go/No-Go) and sustained attention (SART) using a mobile-friendly web-based interface.
- **Deployment**: The experiment is hosted at [https://sw33tnth.github.io/cognitive-experiments/](https://sw33tnth.github.io/cognitive-experiments/).
- **Files**:
  - `index.html` (or `sart.html`): Main experiment file containing the Go/No-Go and SART tasks.
  - `jspsych/`: Directory containing jsPsych library files (`jspsych.js`, plugins, and `jspsych.css`).

## Task Details

### Go/No-Go Task
- **Purpose**: Measures inhibitory control by requiring participants to respond to "go" stimuli (green circles) and withhold responses to "no-go" stimuli (red circles).
- **Design**:
  - **Stimuli**: Green circles (go) and red circles (no-go).
  - **Frequency**: 120 trials (96 go, 24 no-go; 20% no-go frequency).
  - **Timing**:
    - Fixation: 1000 ms.
    - Stimulus: 1000 ms.
    - Inter-trial interval (ITI): Random, 200–500 ms.
    - Total trial duration: 2200–2500 ms.
  - **Response**: Button press ("Respond") for go trials, withhold for no-go trials.
- **Data Collected**:
  - Accuracy: Percentage of correct responses.
  - Reaction Time (RT): Mean RT for correct go responses (ms).

### SART (Sustained Attention to Response Task)
- **Purpose**: Measures sustained attention and inhibitory control by requiring participants to respond to "go" stimuli (numbers 1, 2, 4–9) and withhold responses to "no-go" stimuli (number 3).
- **Design**:
  - **Stimuli**: Numbers 1–9, with 3 as the no-go stimulus.
  - **Frequency**: 120 trials (96 go, 24 no-go; 20% no-go frequency).
  - **Timing**:
    - Fixation: 500 ms.
    - Stimulus: 500 ms.
    - Inter-trial interval (ITI): Random, 200–500 ms.
    - Total trial duration: 1200–1500 ms.
  - **Response**: Button press ("Respond") for go trials, withhold for no-go trials.
- **Data Collected**:
  - Accuracy: Percentage of correct responses.
  - Reaction Time (RT): Mean RT for correct go responses (ms).

## Validity and Reliability
- **Go/No-Go**:
  - **Validity**: 20% no-go frequency aligns with norms (20–25%; Wessel, 2017). Timing (2200–2500 ms total) is within norms (1500–2500 ms). Random ITI prevents rhythmic responding (Dang et al., 2018).
  - **Reliability**: 120 trials ensure sufficient data (minimum 100 trials; Wessel, 2017). Randomized trial order reduces order effects.
- **SART**:
  - **Validity**: 20% no-go frequency aligns with norms (10–20%; Robertson et al., 1997). Timing (1200–1500 ms total) is within norms (1000–2000 ms) and typical for SART (Cheyne et al., 2009). Random ITI enhances validity.
  - **Reliability**: 120 trials exceed the minimum for reliable measurement (Robertson et al., 1997). Randomized trial order and strict no-go frequency control ensure consistency.
- **Overall**: Built with jsPsych for accurate timing and data collection (de Leeuw, 2015). Mobile-friendly design ensures accessibility.

## Data Collection
- **Participant ID**: A unique 5-digit random ID is generated for each participant.
- **Data Submission**: Results (Participant ID, accuracy, and RT for both tasks) are submitted to a Google Form for analysis.

## How to Run the Experiment
1. Access the experiment online at [https://sw33tnth.github.io/cognitive-experiments/](https://sw33tnth.github.io/cognitive-experiments/).
2. Alternatively, clone this repository and open `index.html` (or `sart.html`) in a web browser to run locally.
3. Follow the on-screen instructions to complete the Go/No-Go and SART tasks.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Built using [jsPsych](https://www.jspsych.org/), a JavaScript library for creating behavioral experiments.
- Deployed on GitHub Pages for online access.
