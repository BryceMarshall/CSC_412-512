## Accessibility 

Understanding how users interact with digital interfaces requires a comprehensive approach that considers the diverse ways individuals perceive, process, and physically engage with information. Mental models, which shape user expectations and behaviors, vary significantly based on cognitive abilities, sensory perception, and motor skills. To design truly inclusive and accessible interfaces, [[User Models]] must account for these differences. 

[Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718) grouped such user models into three distinct categories:
1. Cognitive processes (e.g., handedness, language lateralization).
2. Perceptual impairments (e.g., vision loss, color blindness).
3. Motor impairments (e.g., tremours, involuntary movement)

---
### Cognitive processes

Examples of design to support accessibility:
- [[Apple’s design documentation for Right to Left (RTL) languages]]
- [[Visual Ergonomics for Left-Handed Users]]

--- 
### Perceptual Impairments

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

Above: Norman’s action cycle model, which guided [Sulong & Raja Yusof (2024)](https://doi.org/10.1007/s10209-023-01035-5) in their development of a mental model for blind users. Norman's action cycle is often used to inform the [[design of user interfaces|Applications of Mental Models to Design]]

#### Design solutions for perceptual impairments

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


--- 

### Motor Impairments

Users with motor impairments develop different expectations and strategies for interacting with digital interfaces compared to users without impairments. Their mental model of interaction is shaped by their physical limitations—they anticipate difficulty with precise cursor movements, the need for alternative navigation methods, or slower response times. If an interface does not accommodate these expectations, such as requiring double-clicking or precise dragging, it disrupts their workflow, making the system feel unintuitive and frustrating. 

![image](https://github.com/user-attachments/assets/2e087d6c-c8dc-4af5-934d-6ab3dbda23ad)

Above: Mouse movement trajectory for a user with cerebral palsy, from ([Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718)) 

[Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718) also discusses how motor impairments affect users' ability to interact with digital interfaces and how designers can anticipate and address these challenges, outlined below.

#### Design solutions for motor impairments

| **Problem**                                         | **Solution(s)** |
|------------------------------------------------------|-----------------|
| **Cognitive Load Management** – Users may feel overwhelmed by too much information at once. | Use progressive disclosure, breaking information into smaller steps to reduce cognitive strain. |
| **Parallel Processing and Multitasking** – Users struggle with managing multiple tasks in information-heavy systems. | Design clear visual hierarchies, ensuring primary actions are distinguishable from secondary ones. |
| **Response Time and Interaction Efficiency** – Users take longer to process and act on information. | Minimize clicks and navigation depth; ensure frequently used features are **easily accessible**. |
| **Navigation and Mental Workload** – Users may have difficulty building a mental model of where to find information. | Maintain predictable navigation structures, use breadcrumbs and clear labeling to improve discoverability. |
| **Error Reduction and Recovery** – Users may make mistakes and struggle to correct them efficiently. | Implement undo options, clear feedback messages, and flexible navigation paths to support error recovery. |


This research underscores the need for a proactive approach to accessibility, where user models are used not just to identify barriers, but to inform design choices that empower all users, regardless of physical ability.

---

### Adaptive Security

When user interfaces (UIs) are not designed with accessibility in mind, they can create serious security vulnerabilities for individuals with disabilities. These issues arise because security features—such as password entry, authentication systems, and privacy settings—are often designed for users with full motor, cognitive, and sensory abilities, ignoring the needs of those with impairments. Both [Sulong & Raja Yusof (2024)](https://doi.org/10.1007/s10209-023-01035-5) and [Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718) addressed these shortcomings, particularily for those with visual impairments. 

#### Design solutions for adaptive security

| **Problem** | **Example** | **Solution** |
|------------|------------|-------------|
| **Users with visual impairments rely on screen readers, voice commands, or magnification tools, but many security features (CAPTCHAs, password fields, MFA notifications) are not compatible with assistive technologies.** | A user who is blind and depends on screen readers may struggle with image-based authentication or inaccessible CAPTCHA challenges, forcing them to seek assistance and exposing private credentials. | Implement audio-based CAPTCHAs, voice-activated authentication, and screen reader-friendly verification prompts. |
| **Users with cognitive disabilities (e.g., dyslexia, ADHD, memory impairments) may struggle with complex passwords, time-sensitive logins, or multi-step verification processes. Security measures that require quick responses, pattern recognition, or precise recall may not align with their mental model.** | A user with a memory impairment may struggle to recall strong passwords or security questions, leading to frequent lockouts or unsafe behaviors like writing down passwords. | Provide password managers, biometric authentication (fingerprint/face ID), and customizable security settings that reduce cognitive strain. |
| **Users with motor impairments (e.g., Parkinson’s, cerebral palsy, arthritis) may struggle with precise cursor movements, fast typing, or completing time-sensitive authentication steps. Security interfaces that assume rapid and precise input create major usability barriers.** | A user with tremors may struggle to enter a password without typos or complete a two-factor authentication (2FA) code within a short time frame, leading to account lockouts. | Support alternative input methods, such as adaptive keyboards, voice-based authentication, and longer timeframes for entering verification codes. |

For more information on mental models and the UI of cyber security, see [[Security]].
