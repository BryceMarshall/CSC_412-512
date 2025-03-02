## Accessibility 

Understanding how users interact with digital interfaces requires a comprehensive approach that considers the diverse ways individuals perceive, process, and physically engage with information. Mental models, which shape user expectations and behaviors, vary significantly based on cognitive abilities, sensory perception, and motor skills. To design truly inclusive and accessible interfaces, [user models](INSERT LINK) must account for these differences. 

[Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718) grouped such user models into three distinct categories:
1. Perceptual impairments (e.g., vision loss, color blindness).
2. Cognitive processes (e.g., right vs left language lateralization, decision-making speed, memory constraints).
3. Motor impairments (e.g., tremours, involuntary movement)

---
Examples of design to support accessibility:
- [[Apple’s design documentation for Right to Left (RTL) languages]]
- [[Universal Design Principles in Graphical User Interface Understanding Visual Ergonomics for the Left-Handed Users in the Right-Handed World.]]

--- 
### Perceptual Impairments
-> note from lindsay: I have more to add here
#### Mental model of blind users to assist designers in system development

- Understanding the mental model of blind users has been challenging.
- Existing mental models for the blind are configured by Kurniawan and Sutcliffe. In the study by Kurniawan et al, blind people have 3 strategies in dealing with a new environment.

- **Structural mental model**: one or two-dimensional array of icons of applications
- **Functional mental model**: created when each application in computers were associated with application (e.g. CTRL + M + W = Microsoft Words).
- **Hybrid mental model**: Combination of above two models 
![[Pasted image 20250301193640.png | center |500]]

- For the blind people there are 3 stages in the mental model of system interaction

- **Exploration**: explore desktop, explore application, discover new features…
- **Task-action**: plan interaction, execute, change strategy…
- **Configuration**: configure/use



--- 
### Cognitive Processes

This tab summarizes 3 papers related to accessibility.

- Mental model of User Interface of Blind People
- Right to Left language User Interface
- Handedness and GUI Mental Model

**Note**

I want to look into the Right to Left language user’s mental model instead of interaction design in AR/VR.

- Saei, S. N. S. M., Sulaiman, S., & Hasbullah, H. (2010). Mental model of blind users to assist designers in system development. 2010 International Symposium on Information Technology, 1, 1–5. [https://doi.org/10.1109/ITSIM.2010.5561350](https://doi.org/10.1109/ITSIM.2010.5561350)
- Jin, Y., Ma, M., & Zhu, Y. (2022). A comparison of natural user interface and graphical user interface for narrative in HMD-based augmented reality. Multimedia Tools and Applications, 81(4), 5795–5826. [https://doi.org/10.1007/s11042-021-11723-0](https://doi.org/10.1007/s11042-021-11723-0)
- Apple’s developer design guide documentation. Right to Left languages. [https://developer.apple.com/design/human-interface-guidelines/right-to-left](https://developer.apple.com/design/human-interface-guidelines/right-to-left)
- Basak, A., Roy, S. T., & Chakrabarti, A. (2019). Universal Design Principles in Graphical User Interface: Understanding Visual Ergonomics for the Left-Handed User s in the Right-Handed World. In Research into Design for a Connected World (Vol. 135, pp. 793–806). Springer. [https://doi.org/10.1007/978-981-13-5977-4_67](https://doi.org/10.1007/978-981-13-5977-4_67)


--- 

### Motor Impairments

Users with motor impairments develop different expectations and strategies for interacting with digital interfaces compared to users without impairments. Their mental model of interaction is shaped by their physical limitations—they anticipate difficulty with precise cursor movements, the need for alternative navigation methods, or slower response times. If an interface does not accommodate these expectations, such as requiring double-clicking or precise dragging, it disrupts their workflow, making the system feel unintuitive and frustrating. 

![image](https://github.com/user-attachments/assets/2e087d6c-c8dc-4af5-934d-6ab3dbda23ad)
Above: Mouse movement trajectory for a user with cerebral palsy, from ([Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718)) 

([Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718)) discusses how motor impairments affect users' ability to interact with digital interfaces and how [simulation-based modeling](LINK TO MENTAL MODEL STUDIES) can help designers anticipate and address these challenges, outlined below.

- Difficulty with precise cursor movements (e.g., due to tremors, muscle weakness, or limited dexterity)
  - Solution: Increase button sizes and clickable areas to reduce the need for precision.
- Accidental clicks and unintended actions (common in conditions like Parkinson’s disease)
  - Solution: Implement customizable click delay settings to filter out unintended rapid clicks.
- Struggles with double-clicking or dragging elements (common for users with motor impairments)
  - Solution: Provide single-click alternatives and allow keyboard navigation for selection and movement.
- Prolonged reaction times and difficulty with timed tasks (e.g., users with cerebral palsy or multiple sclerosis)
  - Solution: Offer adjustable time limits or allow users to disable time-based interactions.
- Inability to use a traditional mouse or touchscreen
  - Solution: Support alternative input methods such as voice commands, eye-tracking, or adaptive switches.
- Fatigue from prolonged interaction or repetitive motions
  - Solution: Implement keyboard shortcuts, predictive text, and reduced motion options to minimize effort.
 
This research underscores the need for a proactive approach to accessibility, where user models are used not just to identify barriers, but to inform design choices that empower all users, regardless of physical ability.

---

### Adaptive Security

When user interfaces (UIs) are not designed with accessibility in mind, they can create serious security vulnerabilities for individuals with disabilities. These issues arise because security features—such as password entry, authentication systems, and privacy settings—are often designed for users with full motor, cognitive, and sensory abilities, ignoring the needs of those with impairments. Both ([Sulong & Raja Yusof (2024)](https://doi.org/10.1007/s10209-023-01035-5)) and ([Biswas *et al* (2012)](https://doi.org/10.1080/10447318.2011.565718)) addressed these shortcomings, particularily for those with visual impairments. 

- Users with visual impairments rely on screen readers, voice commands, or magnification tools to navigate interfaces. If security features like CAPTCHAs, password entry fields, or MFA notifications are not compatible with assistive technologies, they become barriers rather than protections.
  - Example: A user who is blind and depends on screen readers may struggle with image-based authentication or inaccessible CAPTCHA challenges, forcing them to seek assistance and exposing private credentials.
  - Solution: Security measures should align with perceptual user models by incorporating audio-based CAPTCHAs, voice-activated authentication, and screen reader-friendly verification prompts.
-  Users with cognitive disabilities (e.g., dyslexia, ADHD, memory impairments) may struggle with complex passwords, time-sensitive logins, or multi-step verification processes. Security measures that require quick responses, pattern recognition, or precise recall may not align with their mental model.
  - Example: A user with a memory impairment may struggle to recall strong passwords or security questions, leading to frequent lockouts or unsafe behaviors like writing down passwords.
  - Solution: Security features should be cognitively accessible, allowing for password managers, biometric authentication (fingerprint/face ID), and customizable security settings that reduce cognitive strain.
- Users with motor impairments (e.g., Parkinson’s, cerebral palsy, arthritis) may struggle with precise cursor movements, fast typing, or completing time-sensitive authentication steps. Security interfaces that assume rapid and precise input create major usability barriers.
  - Example: A user with tremors may struggle to enter a password without typos or complete a two-factor authentication (2FA) code within a short time frame, leading to account lockouts.
  - Solution: Security models should support alternative input methods, such as adaptive keyboards, voice-based authentication, and longer timeframes for entering verification codes.

For more information on mental models and the UI of cyber security, see [Security](INSERT LINK).
