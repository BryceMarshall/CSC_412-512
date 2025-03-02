Mental Model studies in HCI

- Student interactions with ATMS: Students asked questions about the functions of an ATM revealed the mental model they held for the functionality and design of the machine and what information is stored on an access card (Collins and Genter, 1987)

Mental Model studies in Software

- Users’ understanding of browsers:  Showed that users do not have an accurate understanding of how the “back” and “forward” buttons of browsers work because they did not have a correct mental model for how search histories are saved and updated when back and forward are clicked (Cockburn and Jones, 1996)

Mental Model studies in Interface Design

- [[Mental Model Measurement Methods|Measuring]] student mental models: Conducted an experiment utilizing a questionnaire designed to measure the “degree of formed mental model” which pertains to logical thinking and organization. This approach provided insights into the potential effectiveness of mental model measurement methods and understanding ussr cognition related to interface design ([Mori and Yamaoka, 2014](https://personales.upv.es/thinkmind/dl/conferences/achi/achi_2014/achi_2014_3_40_20183.pdf)).

Mental Model studies on System Descriptions 

- [[Mental Model Measurement Methods|Measuring]] how initial system descriptions influence mental models and [[Accessibility|user responses]]: Manipulated the participants’ mental models by providing them with either accurate or misleading information about a system’s automated driving functionality before they interacted with it. It was concluded that initial system descriptions significantly influence mental models and user interactions. Findings highlight the importance of accurate and complete instructions when designing systems ([Blömacher et al, 2019](https://www.sciencedirect.com/science/article/abs/pii/S1369847819302086)).

![[mental-model-study.jpg | center | 500]]

**Sulong, S., & Raja Yusof, R. J. (2024). Developing a blind user mental model (BlUMM) for web browsing.** **_Universal Access in the Information Society, 23_****(1343–1367).** [https://doi.org/10.1007/s10209-023-01035-5](https://doi.org/10.1007/s10209-023-01035-5).

- blind users often face barriers to usability that result in frustration and exclusion. The study aims to address this by identifying challenges blind users face, analyzing their web-browsing strategies, and developing a structured mental model based on usability principles, the GOMS (Goals, Operators, Methods, and Selection Rules) model, and Norman’s action cycle model.
- The research involved six blind participants using the JAWS screen reader to browse websites. Their actions, challenges, and feedback were recorded and analyzed to construct a 14-element mental model that describes the steps blind users take when interacting with a website. This model was then mapped into four stages of user action: Planning, Selection, Execution, and Evaluation.
- Mental Model (main)
- It defines a mental model as the way blind users conceptualize and navigate websites, based on prior experience, expectations, and learned strategies.

The BlUMM framework consists of 14 key elements, such as:

- Setting goals
- Exploring a website
- Applying existing knowledge
- Discovering new features
- Selecting and executing tasks
- Perceiving and interpreting feedback
- Adapting strategies when needed

- User Models
- identifying different browsing strategies blind users adopt. Key factors affecting user models:

- Prior experience with technology (eg., Windows navigation habits)
- Screen reader proficiency (eg., JAWS navigation skills)
- Problem-solving strategies when encountering accessibility barriers (eg., using landmarks, search functions, or seeking help from sighted users)

- Some blind users use analogical reasoning, assuming that website navigation should work like their operating system (like expecting the "Search" function to behave like a file search on a computer).
- User Interface
- UI issues identified:

- Complex layouts with multiple sections (e.g., headers, footers, pop-ups)
- Unclear navigation paths (e.g., unlabeled buttons or ambiguous links)
- Inaccessible dynamic content (e.g., auto-playing videos, flash content)
- Inconsistent keyboard navigation

- Solutions proposed:

- Landmarks: Allow blind users to quickly navigate structured sections of a website.
- Consistent heading structures: Help users skim through content.
- Well-labeled elements: Ensure that buttons, forms, and links are properly tagged for screen readers.

- Design

Nielsen’s usability principles:

1. Learnability – Clear structure and easy navigation (e.g., well-organized headings).
2. Efficiency – Quick access to content (e.g., keyboard shortcuts, search functions).
3. Memorability – Users should easily recall how to navigate a website (e.g., consistent layout).
4. Error Reduction – Users should be able to recover if they get lost (e.g., clear backtracking options).
5. User Satisfaction – Websites should be pleasant and stress-free to use.

- Accessibility

Major accessibility barriers identified:

- Lack of alternative text for images and buttons
- Unstructured navigation (e.g., missing heading levels)
- Forms and pop-ups that are not screen-reader friendly
- Inconsistent keyboard support

Proposed accessibility improvements:

- Using semantic HTML to improve screen reader compatibility.
- Providing alternative navigation methods, such as skip links and keyboard shortcuts.
- Ensuring compatibility with assistive technologies, like screen readers.
- Security

Security briefly discussed wrt to social media usage by blind users.

Key concerns:

- Password entry challenges: Blind users often struggle with password masking (i.e., hidden characters).
- Privacy risks: Users may unknowingly share private information due to unclear UI feedback.

Suggested solutions:

- Providing password visibility options (e.g., "Show Password" toggle).
- Clearer voice feedback for sensitive actions (e.g., confirmation before submitting personal data).
- Evaluation of mental models

- Future work


[[CAULDRON]]

  

**Yusoff, N. M., & Salim, S. S. (2020). Shared mental model processing in visualization technologies: A review of fundamental concepts and a guide to future research in human-computer interaction. In D. Harris & W.-C. Li (Eds.),** **_Engineering psychology and cognitive ergonomics: Mental workload, human physiology, and human energy_** **(pp. 238-257). Springer.** [https://doi.org/10.1007/978-3-030-49044-7](https://doi.org/10.1007/978-3-030-49044-7).

explores the Shared Mental Model (SMM) in the context of visualization technologies and its implications for Human-Computer Interaction (HCI). SMM is a cognitive framework that enables teams to have a common understanding of tasks, interactions, and expectations. The paper reviews theoretical concepts, properties, evaluation methods, and applications of SMM in visualization.

- Mental Model (main)
- According to the paper, four types of SMMs exist with respect to the workplace: 

1. Task-Specific Knowledge

- Focuses on how to perform a specific task efficiently.
- Example: Air traffic controllers share knowledge of communication protocols.

1. Task-Related Knowledge

- Involves general knowledge about task-related processes, rather than specific tasks.
- Example: Engineers working on different projects share general troubleshooting strategies.

1. Knowledge of Teammates

- Understanding the preferences, strengths, and tendencies of teammates.

1. Attitudes and Beliefs

- Shared beliefs, attitudes, and cognitive frameworks influence decision-making.

- User Models

- discusses how SMM contributes to user models, particularly in collaborative environments.

- User Interface

- “enhance user interfaces by making cognitive processes explicit.”

- Design
- Design considerations for SMM-friendly visualization systems:

- Consistency: Ensure that the visual design aligns with users’ expectations.
- Interactivity: Support real-time updates, feedback, and modifications.
- Scalability: Adapt interfaces to different user needs and environments.

- CoVis: Collaborative visualization 
- Collaborative Visualization Systems to be effective, the UI must support real-time collaboration and shared cognitive representation. This means that the system should allow multiple users to interact with the data simultaneously, while also providing mechanisms to manage interactions efficiently.
- Floor control: mechanism that manages user access and input permissions in collaborative environments.
- Types of Floor Control in CoVis

- Free-Floor Model _(Peer Collaboration)_

- Any user can interact with and modify the visualization at any time.
- Best for brainstorming sessions or informal collaboration.

- Moderator-Controlled Model _(Hierarchical Collaboration)_

- One user (the moderator) controls access, deciding who can interact with the system at any given time.
- Ideal for team presentations, structured discussions, or teaching scenarios.

- Token-Based Model _(Turn-Based Collaboration)_

- Users take turns interacting with the system using a "token".
- Reduces overlapping actions and ensures equal participation.

- Shared Control Model _(Distributed Collaboration)_

- Control is distributed dynamically based on roles or expertise.
- Example: In a medical imaging system, radiologists control image analysis while doctors control diagnosis discussions.

- Evaluation of mental models
- outlines various methods for evaluating SMM, including:

- Elicitation techniques: Concept maps, similarity ratings, and card sorting.
- Structural representation methods: Multidimensional scaling, pathfinder analysis.
- Cognitive Task Analysis (CTA): Evaluates how users process and represent knowledge.

- Future work
- Shared visualization in big data and analytics

Application in Construction and Geospatial Domains:

- Construction Management: Shared visual tools are essential for managing wide, complex construction sites, where diverse teams need to overcome differences in visual languages, design, and perception.
- GeoVisual Analytics: Collaborative visualization supports the analysis of complex geographical information, aiding in precise spatial decision-making and facilitating both time-critical and long-term analysis.

Innovative Collaborative Systems:

- Mixed-Initiative Systems (e.g., MIVAS): These systems incorporate key components such as data wrangling, alternative discovery, parametric interaction, history tracking, and adaptive collaboration. They enhance team performance and reduce task failure by supporting both human and autonomous decision-making processes.
- Interactive Decision-Making: By combining visualization with data mining techniques, shared visual analytics can effectively communicate uncertainty and support interactive decision-making.

  

**Biswas, P., Robinson, P., & Langdon, P. (2012). Designing inclusive interfaces through user modeling and simulation.** **_International Journal of Human-Computer Interaction, 28_****(1), 1–33.** [**https://doi.org/10.1080/10447318.2011.565718**](https://doi.org/10.1080/10447318.2011.565718) 

 This paper focuses on improving accessibility and inclusivity in interface design through user modeling and simulation. It argues that current design practices often isolate elderly and disabled users, treating them as having “special needs” rather than incorporating accessibility from the outset.

To address this, the paper introduces a simulation-based approach to help designers understand and predict the interaction challenges faced by users with different abilities. The simulation system models:

1. Perceptual impairments (e.g., vision loss, color blindness).
2. Cognitive processes (e.g., how users navigate interfaces).
3. Motor impairments (e.g., difficulty using a mouse or touch interface).

The system evaluates interfaces by simulating interaction patterns for diverse users and can predict task completion times based on user characteristics. It reduces the need for extensive user trials and allows designers to test different design alternatives efficiently.

- Mental Model (main)

- User Models

The paper classifies user models based on:

- Cognitive abilities (e.g., decision-making speed, memory constraints).
- Motor skills (e.g., hand strength, pointer control).
- Visual perception (e.g., color blindness, focus areas).

Three main types of user models used in the simulator:

1. Perceptual Model – Simulates how users see and process visual information.
2. Cognitive Model – Represents decision-making strategies and attention allocation.
3. Motor Behavior Model – Predicts cursor movement and interaction challenges

- User Interface

- Highlights UI challenges for users with disabilities, including

1. Poor text readability
2. Navigation difficulties (complex menus, lack of shortcuts)
3. Inefficient cursor movement

- Design

The authors emphasize the importance of "designing for all" rather than retrofitting accessibility later.

The simulator supports adaptive UI design:

- Customizable text sizes and color contrast for visually impaired users.
- Predictive UI adaptation based on user skill levels.
- Different interaction models for users with motor impairments.

- Accessibility

- Security

  

usability security issues are discussed.

- Password entry for visually/motor-impaired users (e.g., difficulty with masked passwords).
- Confusing authentication methods (e.g., CAPTCHAs that are not screen-reader friendly).
- Accidental actions due to interface misalignment (e.g., misclicks by users with tremors).
- Evaluation of mental models

The paper proposes a systematic method for evaluating mental models:

1. Simulation-based analysis – Predicts how different user groups interact with interfaces.
2. Comparative studies – Validates predictions against real-world user testing.
3. Statistical validation – Uses task completion times and error rates to measure model accuracy.

- Future work
  

  

**Spero, E., & Biddle, R. (2020). Out of sight, out of mind: UI design and the inhibition of mental models of security.** **_New Security Paradigms Workshop 2020 (NSPW ’20)_****, October 26–29, 2020, Online, USA. ACM.** [**https://doi.org/10.1145/3442167.3442174**](https://doi.org/10.1145/3442167.3442174)**.**