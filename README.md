## Inspiration
Imagine: A major earthquake hits. Thousands call 911 simultaneously. In the call center, a handful of operators face an impossible task. Every line is ringing. Every second counts. There aren't enough people to answer every call.
This isn't just hypothetical. It's a real risk in today's emergency services. A startling **82% of emergency call centers are understaffed**, pushed to their limits by non-stop demands. During crises, when seconds mean lives, staffing shortages threaten our ability to mitigate emergencies.

## What it does
DispatchAI reimagines emergency response with an empathetic AI-powered system. It leverages advanced technologies to enhance the 911 call experience, providing intelligent, emotion-aware assistance to both callers and dispatchers. 

Emergency calls are aggregated onto a single platform, and filtered based on severity. Critical details such as location, time of emergency, and caller's emotions are collected from the live call. These details are leveraged to recommend actions, such as dispatching an ambulance to a scene. 

Our **human-in-the-loop-system** enforces control of human operators is always put at the forefront. Dispatchers make the final say on all recommended actions, ensuring that no AI system stands alone.

## How we built it
We developed a comprehensive systems architecture design to visualize the communication flow across different softwares.

![Architecture](https://i.imgur.com/FnXl7c2.png)

We developed DispatchAI using a comprehensive tech stack:

### Frontend:
- Next.js with React for a responsive and dynamic user interface
- TailwindCSS and Shadcn for efficient, customizable styling
- Framer Motion for smooth animations
- Leaflet for interactive maps

### Backend:
- Python for server-side logic
- Twilio for handling calls
- Hume and Hume's EVI for emotion detection and understanding
- Retell for implementing a voice agent
- Google Maps geocoding API and Street View for location services
- Custom-finetuned Mistral model using our proprietary 911 call dataset
- Intel Dev Cloud for model fine-tuning and improved inference

## Challenges we ran into
- Curated a diverse 911 call dataset
- Integrating multiple APIs and services seamlessly
- Fine-tuning the Mistral model to understand and respond appropriately to emergency situations
- Balancing empathy and efficiency in AI responses

## Accomplishments that we're proud of
- Successfully fine-tuned Mistral model for emergency response scenarios
- Developed a custom 911 call dataset for training
- Integrated emotion detection to provide more empathetic responses

## Intel Dev Cloud Hackathon Submission

### Use of Intel Hardware
We fully utilized the Intel Tiber Developer Cloud for our project development and demonstration:
- Leveraged IDC Jupyter Notebooks throughout the development process
- Conducted a live demonstration to the judges directly on the Intel Developer Cloud platform

### Intel AI Tools/Libraries
We extensively integrated Intel's AI tools, particularly IPEX, to optimize our project:
- Utilized Intel® Extension for PyTorch (IPEX) for model optimization
- Achieved a remarkable reduction in inference time from 2 minutes 53 seconds to less than 10 seconds
- This represents a 80% decrease in processing time, showcasing the power of Intel's AI tools

### Innovation
Our project breaks new ground in emergency response technology:
- Developed the first empathetic, AI-powered dispatcher agent
- Designed to support first responders during resource-constrained situations
- Introduces a novel approach to handling emergency calls with AI assistance

### Technical Complexity
- Implemented a fine-tuned Mistral LLM for specialized emergency response with Intel Dev Cloud
- Created a complex backend system integrating Twilio, Hume, Retell, and OpenAI
- Developed real-time call processing capabilities
- Built an interactive operator dashboard for data summarization and oversight

### Design and User Experience
Our design focuses on operational efficiency and user-friendliness:
- Crafted a clean, intuitive UI tailored for experienced operators
- Prioritized comprehensive data visibility for quick decision-making
- Enabled immediate response capabilities for critical situations
- Interactive Operator Map

### Impact
DispatchAI addresses a critical need in emergency services:
- Targets the 82% of understaffed call centers
- Aims to reduce wait times in critical situations (e.g., Oakland's 1+ minute 911 wait times)
- Potential to save lives by ensuring every emergency call is answered promptly

### Bonus Points
- Open-sourced our fine-tuned LLM on HuggingFace with a complete model card
  (https://huggingface.co/spikecodes/ai-911-operator)
  - And published the training dataset: https://huggingface.co/datasets/spikecodes/911-call-transcripts
- Submitted to the Powered By Intel LLM leaderboard (https://huggingface.co/spaces/open-llm-leaderboard/open_llm_leaderboard)
- Promoted the project on Twitter (X) using #HackwithIntel
  (https://x.com/spikecodes/status/1804826856354725941)

## What we learned
- How to integrate multiple technologies to create a cohesive, functional system
- The potential of AI to augment and improve critical public services

## What's next for Dispatch AI
- Expand the training dataset with more diverse emergency scenarios
- Collaborate with local emergency services for real-world testing and feedback
- Explore future integration
