# A Machine Learning Approach to Resolving Conflicts in Physical Human-Robot Interaction

## Overview
This GitHub repository contains resources related to the research paper titled "A Machine Learning Approach to Resolving Conflicts in Physical Human-Robot Interaction" authored by Enes Ulas Dincer, Zaid Al-Saadi, Yahya M. Hamad, Yusuf Aydin, Ayse Kucukyilmaz, and Cagatay Basdogan.

### Paper Abstract
As artificial intelligence techniques become more sophisticated, we anticipate that robots collaborating with humans will develop their own intentions, leading to potential conflicts in interaction. This development calls for advanced conflict resolution strategies in physical human-robot interaction (pHRI), a key focus of our research. We use a Machine Learning (ML) classifier to detect conflicts during co-manipulation tasks to adapt the robot's behavior accordingly using an admittance controller. In our approach, we focus on two groups of interactions, namely "harmonious" and "conflicting", corresponding to the cases of the human and the robot working in harmony to transport an object when they aim for the same target and human and robot are in conflict when human changes the manipulation plan such as a change in the direction of movement or parking location of the object, respectively. 

Co-manipulation scenarios were designed to investigate the efficacy of the proposed ML approach, involving 20 participants. Task performance achieved by the ML approach was compared against three alternative approaches: a) a Rule-Based (RB) Approach, where interaction behaviors were rule-derived from statistical distributions of haptic features; b) an unyielding robot that is proactive during harmonious interactions but does not resolve conflicts otherwise, and c) a passive robot which always follows the human partner. This mode of cooperation is known as "hand guidance" in pHRI literature and is frequently used in industrial settings for so-called "teaching" a trajectory to a collaborative robot.

The results show that the proposed ML approach is superior to the others in task performance. However, a detailed questionnaire administered after the experiments, which contains several variables, covering a spectrum of dimensions, to measure the subjective opinion of the participants reveals that the most preferred mode of interaction with the robot is surprisingly passive. This preference indicates a strong inclination towards an interaction mode that gives more control to humans and offers less demanding interaction, even if it is not the most efficient in task performance. Hence, there is a clear trade-off between task performance and the preferred mode of interaction of humans with a robot, and a well-balanced approach is necessary for designing effective pHRI systems in the future.      

### Contents
- **Animations:** This folder contains animations and visual demonstrations of co-manipulation scenarios used in our research. These animations are designed to illustrate the interactions and conflict resolution strategies between a human participant and a robot. The contents are detailed as follows:
  - **Animation of subjects:** This folder contains animations and visual demonstrations of co-manipulation scenarios used in the research to illustrate the interactions and conflict resolution strategies.
    - **Current Object Location:** A black rectangle on the screen represents the current location of the manipulated object.

    - **Robot's Force Vector:** A green arrow points in the direction of the force applied by the robot. The length and direction of the arrow indicate the magnitude and direction of the robot's force vector.

    - **Robot's Intended Goal:** A dashed green rectangle outlines the robot's intended goal location. This serves as a visual reference for where the robot aims to move the object during the interaction.

    - **Human's Force Vector:** A blue arrow represents the force exerted by the human participant. Similar to the robot's force vector, the length and direction of the blue arrow illustrate the magnitude and direction of the human's force vector during the co-manipulation task.

  - **Animations of a testing scenario (Ts-S2):** This animation illustrates sub-tasks 1-4 of a testing scenario (Ts-S2) from Table 4. In the video, we compare four different interaction modes (ML, RB, Unyielding, Passive) using exemplary data from a participant.
    - **Sub-task 1:** Assesses the ability of the RB and ML modes to detect the CP pattern. The animation shows that the ML mode successfully detects the CP pattern, while the RB mode does not.
    - **Sub-task 2:** Compares the magnitude of human force under the Unyielding and ML modes, demonstrating that the Unyielding mode results in higher human force on average.
    - **Sub-task 3:** Examines the human effort under Passive and ML modes, showing that the Passive mode leads to higher effort on average.
    - **Sub-task 4:** Presents representative animations of the manipulated object under all four interaction modes, providing a comprehensive view of how each mode impacts the co-manipulation task.

- **Comparative Evaluation of Machine Learning Models Using Various Cross-Validation Techniques Introduction**: 
  - **Introduction:** This report presents a comprehensive evaluation of three popular machine learning models: Neural Networks, Random Forests, and Support Vector Machines (SVM), across different cross-validation setups. The aim is to identify the model and parameter configuration that yields the highest classification accuracy in our dataset.
  
  - **Methodology:**: We employed three types of cross-validation methods to evaluate the robustness of the models:
    
    - **K-Fold Cross-Validation:** The dataset was divided into (K = 4, 5, 6, 8) subsets. Each subset was used as a training set sequentially, with the remaining subsets forming the test set.
    - **Subject-Wise Cross-Validation:** The dataset was divided into sub-groups of (N = 4, 5, 6) participants. Data from each sub-group was used as a training set sequentially, with the remaining sub-groups forming the test set.
    - **Trial-Wise Cross-Validation:** The dataset was divided into sub-sets of (T = 22, 24, 26) trials. Each sub-set was used as a training set  sequentially, with the remaining trials forming the test set.

- **Questionnaire:** The "Questionnaire" folder contains the detailed questionnaire administered after the experiments, which contains several variables, covering a spectrum of dimensions, to measure the subjective opinion of the participants. These responses provide insights into user preferences and perceptions related to human-robot interaction.

## Usage
Feel free to explore the animations and questionnaires in this repository to gain a better understanding of the research and its findings. If you wish to use or reference the materials in your own work, please make sure to appropriately cite the original paper.

## Citation
If you find this research or its materials useful in your work, please cite the original paper:

[Enes Ulas Dincer, Zaid Al-Saadi, Yahya M. Hamad, Yusuf Aydin, Ayse Kucukyilmaz, and Cagatay Basdogan. 2025. A Machine Learning Approach to Resolving Conflicts in Physical Human-Robot Interaction. J. Hum.-Robot Interact. Just Accepted (January 2025). https://doi.org/10.1145/3706029]

## Contact
For any questions or inquiries related to this research, you can contact the authors:

- Enes Ulas Dincer (edincer22@ku.edu.tr)
- Zaid Al-Saadi (zalsaadi13@ku.edu.tr)
- Yahya M. Hamad (yalqaysi13@ku.edu.tr)
- Yusuf Aydin (aydiny@mef.edu.tr)
- Ayse Kucukyilmaz (Ayse.Kucukyilmaz@nottingham.ac.uk)
- Cagatay Basdogan (cbasdogan@ku.edu.tr)
