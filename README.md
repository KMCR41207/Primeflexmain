# PRIME FLEX 💪
### AI-Powered Personalized Fitness Platform

PRIME FLEX is an intelligent fitness platform designed to make fitness more personalized, accessible, and engaging. It combines AI-powered fitness coaching, personalized workout planning, nutrition guidance, progress tracking, and computer vision-based exercise form analysis into one unified experience.

The platform aims to deliver context-aware fitness recommendations using Retrieval-Augmented Generation (RAG), user-specific information, and machine learning.

## ✨ Key Features

- **🤖 PRIME AI Coach:** An AI-powered fitness assistant for workout, nutrition, recovery, and fitness-related questions.
- **🧠 RAG-Based Knowledge System:** Retrieves relevant fitness knowledge to support more grounded and context-aware AI responses.
- **🏋️ Personalized Workouts:** Workout plans tailored to individual goals, experience levels, and fitness preferences.
- **🥗 Smart Nutrition:** Nutrition guidance, meal planning, and dietary recommendations.
- **📊 Progress Tracking:** Track fitness goals, workout performance, personal records, and progress over time.
- **📸 Exercise Form Detection:** A planned computer vision and machine learning system for analyzing exercise movements, identifying potential form errors, and providing feedback.
- **👤 User Personalization:** Uses user profiles, preferences, and fitness goals to customize the experience.
- **🎯 Gamification:** Achievements, challenges, and progress milestones to encourage consistency.
- **💎 Premium Experience:** Designed to support enhanced features, including unlimited AI conversations for eligible premium users.

## 🧠 AI Architecture

PRIME FLEX combines retrieval-based knowledge access with language model generation to support fitness-focused conversations.

**Proposed RAG workflow:**

1. Receive a user's question.
2. Retrieve relevant information from the fitness knowledge base.
3. Combine retrieved information with the user's available fitness context.
4. Generate a contextual response using a language model.
5. Validate the response and return useful guidance.

### Exercise Form Detection

The planned form analysis pipeline includes:

1. Capture exercise video or camera input.
2. Detect human pose landmarks.
3. Extract joint angles, alignment, range of motion, and movement features.
4. Classify exercise movements and potential form errors.
5. Generate understandable feedback, with confidence checks.

Synthetic pose data may be used to develop and evaluate the classification model. Actual performance will depend on validation against representative real-world data.

## 🛠️ Technology Stack

The final stack may evolve as development progresses.

| Area | Technologies |
|---|---|
| Frontend | React, Vite, TypeScript |
| UI Styling | CSS / Tailwind CSS |
| 3D Experience | Three.js |
| Backend | Node.js, Express |
| Database & Authentication | Supabase |
| AI Integration | Large Language Models (LLMs), RAG |
| Machine Learning | Python, computer vision, pose estimation |
| Data Processing | Python, Pandas |
| Version Control | Git and GitHub |

## 🏗️ Project Architecture

```text
PRIME FLEX
├── Frontend
│   ├── Dashboard
│   ├── Workout Management
│   ├── Nutrition
│   ├── Progress Tracking
│   └── AI Coach Interface
├── Backend
│   ├── Authentication
│   ├── User Profiles
│   ├── Workout and Nutrition APIs
│   └── AI Integration
├── AI Systems
│   ├── RAG Knowledge Pipeline
│   ├── Contextual Response Generation
│   └── Exercise Form Detection
└── Data Layer
    ├── User Data
    ├── Workout History
    ├── Nutrition Records
    └── Fitness Knowledge Base
```

*This diagram represents the intended system architecture; individual components may be at different stages of implementation.*

## 🚀 Getting Started

### Prerequisites

- Node.js and npm
- Git
- Access to the required backend services and API credentials

### Installation

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/prime-flex.git

# Enter the project directory
cd prime-flex

# Install dependencies
npm install

# Start the development server
npm run dev
```

Replace `YOUR_USERNAME` with your GitHub username. These commands assume the repository uses a Vite-based frontend; backend setup may require additional steps depending on the current project structure.

## 🔐 Environment Variables

Store API keys, database credentials, and other secrets in environment variables. Keep private credentials out of source control.

Example `.env.example`:

```env
VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=
BACKEND_PORT=5000
LLM_API_KEY=
```

Use the actual variable names expected by your application. Never expose private service-role keys or secret API credentials in frontend code. Add `.env` to `.gitignore` before committing.

## 🗺️ Roadmap

- [ ] Complete core fitness dashboard
- [ ] Implement personalized workout management
- [ ] Integrate nutrition planning and tracking
- [ ] Develop the RAG-powered PRIME AI Coach
- [ ] Build and evaluate the fitness knowledge base
- [ ] Develop the exercise form detection model
- [ ] Evaluate synthetic training data against real-world samples
- [ ] Integrate 3D visualizations and interactive experiences
- [ ] Add achievements, challenges, and community features
- [ ] Improve security, accessibility, and mobile responsiveness

## 🔬 Research Direction

PRIME FLEX also explores how Retrieval-Augmented Generation, user personalization, and computer vision can work together to improve digital fitness coaching.

Potential research areas include:

- Comparing RAG-based responses with standalone LLM responses.
- Evaluating the effect of user context on recommendation quality.
- Measuring exercise form classification performance.
- Studying the transferability of synthetic pose data to real-world exercise videos.
- Evaluating response quality, reliability, and inference latency.

## 🛡️ Privacy & Safety

- Protect user information and credentials.
- Apply appropriate authentication and database access controls.
- Handle camera input and exercise data responsibly.
- Treat AI-generated fitness advice as informational, not as a substitute for professional medical guidance.
- Avoid presenting uncertain exercise-form predictions as definitive assessments.

## 🤝 Contributing

Contributions, suggestions, bug reports, and feature improvements are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes with clear messages.
4. Open a pull request describing the changes.

## 📄 License

A license has not yet been specified. Add a `LICENSE` file before distributing the project under open-source terms.

---

**PRIME FLEX — Train smarter. Eat better. Progress consistently.** 💪
