VoiceLink
Inspiration
We were inspired by the daily challenges faced by individuals with disabilities when interacting with technology and the world around them. Traditional interfaces—keyboards, touchscreens, and complex gestures—are often inaccessible, leaving many people without the ability to fully connect, create, or control their environment. We wanted to bridge that gap.

The inspiration for VoiceLink became even more personal when one of our team members saw the challenges faced by their grandmother, who has ALS. Seeing firsthand how limited accessibility can impact daily life strengthened our resolve to create a tool that could make a real difference.

VoiceLink was born from the belief that technology should empower everyone equally. Our goal was to transform natural voice, subtle gestures, and human intent into action, creating an intuitive, hands-free way for users to interact with digital systems and their surroundings. By prioritizing accessibility from the start, we aimed to design a tool that restores autonomy, fosters independence, and enables meaningful engagement for people who have long been underserved by conventional interfaces.

What it Does
VoiceLink is a web-based assistive communication platform designed to give users full digital agency, regardless of motor or speech limitations. Key features include:

Gesture-Based Interaction: Users can navigate websites, send messages, and engage in live conversations using simple, detectable facial and head gestures captured through their webcam.
AI-Powered Assistance: VoiceLink leverages intelligent agents that can perform tasks on the user’s behalf, from drafting emails and searching online to browsing Amazon products.
Seamless Communication: Users can connect effortlessly with caregivers, family members, or colleagues without requiring specialized or expensive hardware.
In essence, VoiceLink acts as both a personal assistant and digital voice, empowering users to interact with the world around them in a fluid, intuitive way.

How We Built It
VoiceLink is the product of careful integration of front-end development, computer vision, and AI technologies:

Frontend: Built with React, offering a responsive, user-friendly interface that is accessible directly through a web browser.
Gesture Recognition: Utilizes MediaPipe and other computer vision models to detect facial and head gestures in real-time, ensuring reliable control even for subtle movements.
Interaction Layer: Maps gestures to digital actions, enabling smooth communication, web navigation, and task execution.
AI Backend: Gemini Large Language Models generate real-time conversational responses, perform complex tasks, and maintain context-aware dialogue. Fetch.ai ASI1 to talk to specialized agents to send emails, browse Amazon, and search the web.
Speech Output: Text-to-speech functionality provides clear audio feedback, giving users a “voice” to communicate naturally.
Accessibility Focus: Entirely browser-based—no specialized hardware required—making VoiceLink instantly available to anyone with a laptop.
How We Used Fetch.ai
We integrated ASI1 from Fetch.ai to seamlessly interact with specialized agents and extend VoiceLink’s capabilities beyond core communication.

One highlight of this integration is our custom Amazon agent called "Amazon Search Agent", deployed on Agentverse. VoiceLink queries ASI1 to pick and communicate with this agent, enabling users to shop on Amazon hands-free.

The Amazon agent is built using Gemini API for reasoning and connects to an amazon-mcp model for commerce-related tasks. This allows us to offer users a rich shopping experience powered entirely by natural interactions.

Core Features of the Amazon Agent:

Product Search: Find products on Amazon using natural language, with filters like price, brand, and category.
Natural Language Understanding & Recommendation: Interprets conversational requests to provide personalized product recommendations.
Authenticated Purchases: Securely purchase items using shipping and payment details (via API key).
By connecting VoiceLink’s gesture-based interface with Fetch.ai’s agent ecosystem, users can now search, compare, and purchase products on Amazon—without ever touching a keyboard or screen. This demonstrates the power of combining accessibility-first design with intelligent autonomous agents.

How We Used AgentMail
Using AgentMail, VoiceLink enables users to compose and send emails seamlessly. Gestures or voice input allow users to draft messages, select recipients, and send emails without ever touching a keyboard, providing independence and efficiency in digital communication. This allows users who cannot normally type and send emails to utilize our agent to manage their inbox for them through gestures.

Challenges We Ran Into
Building VoiceLink came with a host of technical and design challenges:

Integrating the frontend with multiple backend APIs (Fetch.ai, AgentMail) and ensuring smooth, reliable communication.
Enhancing the word navigator, which initially predicted only one response path. We extended it to continue predicting context-aware options for longer conversations.
Implementing real-time transcription and integrating it with the LLM to enable predictive, context-aware dialogue.
Developing an autocomplete system for the virtual keyboard that intelligently predicts words based on ongoing conversations.
Overcoming these challenges strengthened our skills in system design, real-time computation, and user-centered AI development.

Accomplishments We’re Proud Of
Real Conversations: Created a working prototype that allows users to hold fluid back-and-forth conversations using only subtle gestures.
Low Latency: Achieved real-time gesture detection and AI response generation, providing a natural and seamless experience.
Universal Accessibility: Built a platform that runs entirely in a web browser, eliminating the need for specialized hardware.
Task Automation: Enabled AI-driven actions, giving users the ability to execute complex tasks independently.
What We Learned
VoiceLink taught us that accessibility is not just a feature—it is a philosophy. Designing for inclusivity pushed us to rethink assumptions about user interaction and challenged us to simplify complex systems without compromising capability.

On the technical side, we gained deep experience in integrating AI models with real-time gesture detection, optimizing performance for real-world conditions, and balancing responsiveness with accuracy. Beyond that, we discovered a fundamental truth: when technology is built with accessibility at its core, it benefits everyone—not just users with disabilities. Simplicity, adaptability, and reliability are universally empowering.

What’s Next for VoiceLink
We envision a future where VoiceLink is fully personalized, portable, and seamlessly integrated into daily life:

Customizable Gestures: Users will define gestures tailored to their comfort and abilities.
Expanded AI Ecosystem: Integration with more agents, productivity tools, smart home devices, and communication platforms.
Mobile Support: Portability on smartphones and tablets to extend accessibility wherever users go.
Clinical Partnerships: Collaborating with ALS, rehabilitation, and accessibility-focused clinics to refine and test VoiceLink with real users.
Open-Source Collaboration: Sharing VoiceLink with the developer and accessibility community to scale its impact and foster innovation.
VoiceLink is more than a tool—it’s a step toward a world where technology truly empowers everyone.
