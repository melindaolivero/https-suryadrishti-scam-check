# System Architecture

## High-Level Flow

User Input (Voice/Text)
        ↓
Frontend (Lovable UI)
        ↓
Input Processing Layer
        ↓
Claude API (LLM)
        ↓
Structured Scam Analysis Response
        ↓
UI Rendering (Risk + Explanation)

---

## Components

### 1. Frontend
- Built using Lovable AI UI builder
- Handles:
  - text input
  - voice input (browser speech-to-text)
  - results display

### 2. AI Layer
- Claude API (Anthropic)
- Performs:
  - scam detection reasoning
  - explanation generation
  - recommendation output

### 3. Voice Layer
- Browser Web Speech API
- Converts speech → text before sending to AI

---

## Data Flow

1. User speaks or types message
2. Input is captured in UI
3. Text is sent to Claude API
4. Claude returns structured JSON-like response
5. UI renders results in categorized sections

---

## Design Principles
- Explainability over automation
- Safety over complexity
- Accessibility over density
- Trust over speed

---

## Future Enhancements
- Real-time call monitoring
- Deepfake detection integration
- Family alert system
- Scam pattern database
