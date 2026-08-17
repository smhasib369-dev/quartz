---
publish: true
created: 2026-08-17T00:39:28.278+06:00
modified: 2026-08-17T18:59:30.942+06:00
---

## 1.Task Analysis

Task Analysis (TA) is a systematic method used to study, understand, and document how users complete tasks to achieve specific goals.

It is widely applied in Human-Computer Interaction (HCI), usability research, and system design to enhance user experiences.

### Importance Of Task Analysis in HCI

- _Breaking Down Tasks_ – Decomposing tasks into smaller, manageable steps.
- _Examining User Actions_ – Analyzing the sequence, dependencies, and complexity of actions.
- _Identifying Bottlenecks_ – Finding inefficiencies, errors, and user frustrations.
- _Improving System Design_ – Making interactions smoother and more intuitive.
- _Understanding User Goals_ – Identifying what users want to achieve.

## Models of Task Analysis in HCI

- Hierarchical Task Analysis (HTA)
- Cognitive Task Analysis (CTA)
- GOMS and KLM Model

### Hierarchical Task Analysis (HTA)

HTA হলো বড় একটা task-কে ছোট ছোট subtask-এ ভাগ করে tree-এর মতো দেখানো।

👉 **Main Task → Subtask → আরও ছোট Subtask**

HTA সাধারণত tree-like structure-এ দেখানো হয়, যাতে task-এর dependency এবং workflow সহজে বোঝা যায়।

Example:

```
Goal: Online Flight Booking

Book Flight
│
├── Search Flight
│   ├── Enter From
│   ├── Enter To
│   └── Select Date
│
├── Select Flight
│   └── Choose Flight
│
├── Passenger Information
│   ├── Name
│   └── Passport
│
└── Payment
    ├── Card Information
    └── Confirm Payment
```

### Cognitive Task Analysis — CTA

Cognitive Task Analysis হলো user কোনো কাজ করার সময় তার মাথার ভিতরে কী ধরনের mental process চলছে, সেটা বিশ্লেষণ করা।

**Cognitive Task Analysis (CTA)
includes —**

🧠 _Perception_
User environment থেকে information কীভাবে নেয়।

💡 _Decision Making_
Information দেখে কীভাবে সিদ্ধান্ত নেয়।

🔄 _Problem Solving_
Problem হলে কীভাবে সমাধান করে।

📚 _Memory & Learning_
আগের knowledge কীভাবে মনে করে এবং ব্যবহার করে।

#### Expert-Based Knowledge in CTA

Experts develop intuitive skills through experience, but these skills can be hard to document. CTA helps:

- _Extract expert knowledge_ – Understanding strategies used by skilled individuals.
- _Make implicit knowledge explicit_ – Capturing mental models experts use.
- _Design better training programs_ – Teaching novices the best cognitive strategies.

#### Why use CTA? (Advantages)

- _✔ Improves_ training by transferring expert knowledge to novices.
- _✔ Enhances_ user-centered design by aligning interfaces with cognitive workflows.
- _✔ Identifies_ bottlenecks in decision-making to improve efficiency.

### GOMS

- GOMS =
  - G = Goals
  - O = Operators
  - M = Methods
  - S = Selection Rules

এটা HCI-তে user কীভাবে কোনো task সম্পন্ন করে তা analyze করার একটি model।

এটি task-এর efficiency এবং completion time estimate করতেও সাহায্য করে।

In Details —

_Goals_: User কী achieve করতে চায়।
**Example:** Send an Email

_Operators:_ User-এর basic actions।
**Example:** Click, Type, Move mouse, Press Enter

_Methods_: Goal অর্জন করার জন্য operators-এর sequence।
**Example:** যেমন Gmail-এ email পাঠানো:
Move → Click Compose → Type Email → Type Subject → Type Message → Click Send

_Selection Rules_: একই goal করার একাধিক method থাকলে কোনটা ব্যবহার করবে সেটা decide করা।
**Example:** User চাইলে Send button click করতে পারে অথবা Ctrl + Enter ব্যবহার করতে পারে।

#### KLM — Keystroke-Level Model

KLM হলো GOMS-এর একটি variant।
এটা দিয়ে user কোনো task করতে আনুমানিক কত সময় লাগবে সেটা estimate করা যায়।

Mouse movement ≈ 1.1 sec
Click ≈ 0.2 sec

Typing-এর সময় আলাদাভাবে ধরা হয়
যদি typing = 10 sec
এবং mouse clicks = 3 sec

তাহলে মোট estimated time:
10 + 3 = 13 seconds

#### GOMS কেন important?

- UI-এর unnecessary steps কমাতে
- System implement করার আগেই efficiency predict করতে
- Repetitive কাজ identify করে automation করতে

### Dialog Notations and Design

#### Dialogue কী?

HCI-তে Dialogue হলো user এবং computer-এর মধ্যে interaction-এর sequence।

`User কিছু করে` → `Computer response দেয়` → `User আবার action নেয়` → `Computer response দেয়`

এটা অনেকটা একটা play-এর script-এর মতো।

**Dialog Description-এর দুই ধরনের notation:**

_A. Diagrammatic Notations_
চোখে দেখে সহজে বোঝা যায়।
এর মধ্যে আছে:

- State Transition Networks
- Petri Nets
- State Charts
- Flow Charts
- Jackson Structured Diagram

_B. Textual Notations_
Formal analysis-এর জন্য বেশি সুবিধাজনক।

- Grammar
- Production Rules

## Groupware

### Groupware কী?

Groupware হলো এমন software/system যা একাধিক মানুষকে একসাথে cooperative work করতে সাহায্য করে।

Example: WhatsApp, Slack, Zoom, Google Docs, Miro

**Groupware-এর প্রধান functional category দুইটি:**

_**Computer-Mediated Communication — CMC**_
Technology ব্যবহার করে participants-এর মধ্যে communication করানো।

Examples: Email, Bulletin Boards, Instant Messaging, Video Conferencing

WhatsApp → real-time chat
Zoom → video conference
Email → asynchronous communication

_**Meeting & Decision Support Systems**_
এগুলো group-এর discussion, brainstorming এবং decision-making support করে।

Examples:

- _Argumentation Tools:_ Design decision বা argument document করতে সাহায্য করে।
- _Electronic Meeting Rooms:_ Physical meeting-এর discussion support করে।
- _Shared Drawing Surface:_ একাধিক মানুষ একই virtual whiteboard-এ কাজ করতে পারে।

**Groupware-এর Key Considerations**

- _Control & Feedback:_ কে shared document পরিবর্তন করতে পারবে?
- _Concurrency Issues:_ একসাথে অনেক user একই জিনিস edit করলে conflict কীভাবে avoid করব?
- _Communication Integration:_ Messaging + document collaboration একসাথে কীভাবে কাজ করবে?

## Time/Space Matrix

Groupware-কে সময় এবং জায়গার ভিত্তিতে classify করা যায়।

**দুইটি প্রশ্ন:**

_Time:_
**সবাই কি একই সময়ে কাজ করছে?**

- `Same Time` → `Synchronous`
- `Different Time` → `Asynchronous`

_Place:_
**সবাই কি একই জায়গায় আছে?**

- `Same Place` → `Co-located`
- `Different Place` → `Remote`

![[Screenshot_2026-08-17-02-05-21-81_c37d74246d9c81aa0bb824b57eaf7062.jpg]]

## CSCW

`CSCW` = `Computer-Supported Cooperative Work`

এটা এমন একটি interdisciplinary field যেখানে technology ব্যবহার করে group collaboration আরও effective করা হয়।

**Objective**
👉 Digital tools ব্যবহার করে teamwork improve করা।

**Application Areas**

- Business
- Education
- Healthcare
- Remote Work

**Key Technologies**

- Video conferencing
- Shared documents
- Workflow systems
- Virtual workspaces

### CSCW-এর Principles

- _Communication Support_
- Communication সহজ করা।
  - Example: Chat, Email
- _Coordination Support_
- Task, role এবং dependency organize করা।
  - Example: Trello, Asana
- _Collaboration Support_
- একসাথে shared work করা।
  - Example: Google Docs
- _Awareness Support_
- Team-এর অন্যরা কী করছে সেটা বুঝতে সাহায্য করা।
  - Example: Notification, Activity Feed
- _Flexibility & Accessibility_
- Different location/device/time zone থেকে কাজ করার সুবিধা।
- _Shared Workspace_
- একটা common environment যেখানে সবাই shared resource তৈরি/edit/manage করতে পারে।
  - Example:
    - Shared documents
    - Collaborative whiteboards
    - Cloud storage

## Ubiquitous Computing — Ubicomp

### Ubicomp কী?

Ubiquitous Computing হলো এমন computing system যেখানে technology আমাদের everyday environment-এর মধ্যে seamlessly integrated থাকে।

মানে computer শুধু desktop বা mobile-এর মধ্যে সীমাবদ্ধ থাকবে না—আমাদের চারপাশের বিভিন্ন object/environment-এর মধ্যেও computing থাকবে।

#### Key Concepts

##### Pervasiveness

চারপাশে computing devices থাকবে।
Example: Smartphone, sensor, wearable

##### Embeddedness

Technology background-এ থেকে কাজ করবে।
Example: Smart lighting

##### Context-Awareness

Environment/user behaviour বুঝে system নিজেকে adapt করবে।
Example: Smart notification

##### Seamless Interaction

Natural way-তে interaction।
Example: Voice command, gesture

##### Interconnectivity

Different devices একে অপরের সাথে communicate করবে।
Example: IoT, Cloud, 5G

### Context-Aware Computing

Context-aware system user-এর পরিবেশ, situation এবং behaviour বুঝে response দেয়।

### Wearable Technology

যে technology শরীরে পরা যায়।

Examples:

- ⌚ Smartwatch
- 🥽 AR Glasses
- 🏃 Fitness Band

এগুলো user interaction আরও সহজ ও natural করতে পারে।

### Smart Environment

Technology দিয়ে environment-কে intelligent করা।

Example:

- 🏠 Smart Home
- 💡 Smart Lighting
- 📱 IoT devices
- 🤖 AI-based contextual interaction

### Ubicomp Evaluation-এর Challenge

- Traditional HCI অনেক সময় task-centric হয়।
- কিন্তু Ubicomp-এর activities সবসময় task-centric নয়।
- আর technology নতুন হওয়ায় long-term authentic evaluation করা কঠিন হতে পারে।
- এখানে success-এর metric-ও আলাদা হতে পারে, যেমন: Playfulness, Non-distraction, Efficiency

## Virtual Reality — VR

### VR কী?

VR হলো এমন technology যেখানে user একটি virtual/digital environment-এর মধ্যে থাকার মতো experience পায়।

#### VR Hardware

- VR Headset
- Motion Controller
- Software
- Unity
- Unreal Engine

#### HCI-তে VR-এর Applications

- Education
- Healthcare
- Training Simulation

#### Challenges

- Technical limitations
- Ethical issues
- Social implications
- Future trends

## Augmented Reality — AR

AR real world-এর উপর digital information/elements add করে।

সহজ পার্থক্য:
`VR` → `Virtual world-এর মধ্যে নিয়ে যায়`
`AR` → `Real world-এর উপর digital information যোগ করে`

## VR and AR

### Differences between VR and AR

| বিষয়                 | VR                  | AR                               |
| -------------------- | ------------------- | -------------------------------- |
| পরিবেশ               | সম্পূর্ণ ভার্চুয়াল | বাস্তব পরিবেশের উপর ডিজিটাল তথ্য |
| বাস্তব জগত দেখা যায়? | না                  | হ্যাঁ                            |
| ডিভাইস               | VR Headset          | Smartphone বা AR Glasses         |
| অভিজ্ঞতা             | Immersive           | Interactive Overlay              |
| উদাহরণ               | VR Gaming           | Pokémon GO                       |

### Similarities between VR and AR

- দুটো প্রযুক্তিরই কিছু সাধারণ বৈশিষ্ট্য আছে।
- দুটোই ব্যবহারকারীর সঙ্গে Interactive Experience তৈরি করে।
- দুটোতেই 3D Graphics ব্যবহার করা হয়।
- দুটোই HCI-তে User Experience উন্নত করতে সাহায্য করে।
- শিক্ষা, স্বাস্থ্যসেবা ও প্রশিক্ষণে দুটোরই ব্যবহার রয়েছে।

## Non-Linear Information Structure

Traditional text সাধারণত linear:
`Page 1` → `Page 2` → `Page 3`

কিন্তু Hypertext:
`Information A` → `B` → `C`

অথবা
`A` → `D` → `F`

অর্থাৎ user নিজের প্রয়োজন অনুযায়ী বিভিন্ন information-এ যেতে পারে।
Examples: Wikipedia, E-books

এখানে navigation এবং user experience গুরুত্বপূর্ণ।

### Hypertext

#### Hypertext কী?

Hypertext হলো এমন text যেখানে link ব্যবহার করে এক information থেকে অন্য information-এ যাওয়া যায়।

## Multimedia

Multimedia হলো একাধিক ধরনের media একসাথে ব্যবহার করা।

Multimedia Elements:

- 📝 Text
- 🖼️ Images
- 🎥 Videos
- 🎞️ Animations

এগুলো user engagement বাড়াতে পারে।

Applications:

- E-learning
- Digital Marketing
- Gaming
