Blind users often apply existing mental models based on past experiences with structured systems, however, when a website's layout does not align with these expectations — such as inclusion dynamic content loading, unlabeled elements, or inconsistent navigation structures — users experience disorientation and frustration. [Sulong & Raja Yusof (2024)](https://doi.org/10.1007/s10209-023-01035-5) explored how blind users compensate for these challenges by switching strategies, relying on search functions, heading navigation, or assistance from sighted users when necessary. They found serveral differences in the mental models of sighted and blind users, outlined below:

| **Aspect** | **Standard Mental Model (Sighted Users)** | **Blind User Mental Model (BlUMM)** |
|------------|--------------------------------|-------------------------------------|
| **Navigation Approach** | Sighted users visually scan pages, jumping between sections using spatial awareness. | Blind users navigate linearly using screen readers and keyboard commands. |
| **Information Processing** | Users rely on gestalt perception (color, shape, and position) to quickly interpret content. | Users depend on semantic HTML, headings, and ARIA attributes to understand page structure. |
| **Interaction with Dynamic Content** | Recognize dropdowns, pop-ups, and live updates visually. | Rely on audio feedback and focus changes to detect content updates; inaccessible dynamic content causes disorientation. |
| **Search Strategies** | Locate key sections visually and interact using mouse, touch, or trackpad | Use search functionality, heading navigation, and landmarks to efficiently skip unnecessary content. |
| **Error Recovery and Feedback Perception** | Instantly notice visual error messages (e.g., red text for invalid input). | Must receive explicit audio feedback errors must be programmatically linked to form fields for detection. |
| **Cognitive Load and Memory Use** | Can retain layout information visually and revisit elements easily. | Must memorize page structure, keyboard shortcuts, and navigation paths, increasing cognitive load. |

![image](https://github.com/user-attachments/assets/28b94dff-dbcc-4d58-a688-59a073f19d21)

Above: Norman’s action cycle model, which guided [Sulong & Raja Yusof (2024)](https://doi.org/10.1007/s10209-023-01035-5) in their development of a mental model for blind users. Norman's action cycle is often used to inform the [[Applications of Mental Models to Design|design of user interfaces]]

## Design solutions for perceptual impairments

| **Problem** | **Design Solution** | **Implementation Strategy** |
|------------|---------------------|----------------------------|
| **Linear Navigation with Screen Readers** | Ensure clear semantic structure | Use proper HTML5 elements (headings, lists, landmarks) instead of visual-only layouts. |
| **Difficulty with Dynamic Content** | Provide audio feedback and focus changes | Use ARIA live regions to announce updates and ensure focus shifts to new content dynamically. |
| **Challenges in Finding Key Information** | Enable efficient keyboard navigation | Implement skip links, logical tab order, and shortcut keys for quick access to main content. |
| **Unlabeled Buttons and Links** | Ensure all interactive elements are properly labeled | Use alt text, ARIA labels, and descriptive link text instead of "Click Here" or unlabeled buttons. |
| **Form Accessibility Issues** | Associate form inputs with labels and provide error feedback | Use label elements, fieldset/legend for groups, and ARIA alerts for form validation messages. |
| **Inaccessible Captchas** | Provide alternative authentication methods | Use audio CAPTCHAs, biometric authentication, or logic-based verification instead of image-based CAPTCHAs. |
| **Overloaded Cognitive Load from Memorization** | Maintain consistent layouts across pages | Avoid unnecessary UI changes and ensure predictable navigation patterns. |
| **Difficulty Understanding Visual Charts and Graphs** | Provide text descriptions and alternative formats | Offer data tables, textual summaries, and sonification (audio representation of data |

## Mental model of blind users to assist designers in system development

[Siti Nur Syazana Mat Saei, Suziah Sulaiman et al (2010)](https://doi.org/10.1109/ITSIM.2010.5561350) summarizes existing mental model of the blind population and advance the existing model.
- Measuring mental model can be found at [[Mental Model Measurement Methods]]
- Understanding the mental model of blind users has been challenging.
- Existing mental models for the blind are configured by Kurniawan and Sutcliffe. In the study by Kurniawan et al, blind people have 3 strategies in dealing with a new environment.
	- Structural mental model: one or two-dimensional array of icons of applications
	- Functional mental model: created when each application in computers were associated with application (e.g. CTRL + M + W = Microsoft Words).
	- Hybrid mental model: Combination of above two models.

  
![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdQ-jWkwE8JMBmbhb0Mx1E6Y-eYaUWPUGI6QSb28AetmttRcHWwQp2zObp0GlJ1jOlIklrfWJZhj4qD6oRS92k-UCsWFJOZq4wX1zIR8WozrtQdFYqGKZJ3K-1vK9WEZiBv4-0d?key=InPcM8oBWM0qEjlRW5SFMn1x)

- For the blind people there are 3 stages in the mental model of system interaction
	- Exploration: explore desktop, explore application, discover new features…
	- Task-action: plan interaction, execute, change strategy…
	- Configuration: configure/use
