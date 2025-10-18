# 🤖 AI Contract Copilot

> Generate and deploy Algorand smart contracts instantly — just by describing them in plain English.

---

## 🧩 Overview

**AI Contract Copilot** is a web-based assistant that lets anyone create, understand, and deploy **Algorand smart contracts** using natural language prompts.

Instead of writing PyTeal from scratch, users simply describe what they want — for example:  
> “Create a smart contract that locks 5 ALGO and releases it after both parties approve.”

Our system uses **AI (OpenAI API)** to generate valid **PyTeal code**, then automatically deploys it to **Algorand TestNet** using **Algokit**.

### 🚀 Why this matters
- Building on Algorand currently requires technical expertise.  
- This project makes blockchain development accessible to **non-coders**.  
- It shows how **AI + blockchain** together can democratize Web3 creation.

---

## 🧠 Problem Statement

Non-technical users struggle to participate in blockchain development because smart contracts require coding knowledge and setup experience.

**AI Contract Copilot** solves this by:
- Enabling anyone to generate smart contracts from natural language  
- Deploying them automatically on Algorand TestNet  
- Providing a transparent preview of the generated code

---

## 💡 Solution

Our web app integrates **AI code generation** with **Algokit automation**:

1. **User prompt:** “I want a simple escrow contract that sends ALGO to Bob after 3 days.”
2. **AI generation:** Backend calls OpenAI API → returns valid PyTeal snippet.
3. **Preview:** The code appears in the UI for user review.
4. **Deploy:** User clicks “Deploy,” triggering an Algokit script that compiles and deploys the contract to TestNet.
5. **Result:** Contract address + transaction ID displayed to the user.

This bridges human language → smart contract → deployed dApp seamlessly.

---

## ⚙️ Tech Stack

| Layer | Technology | Purpose |
|--------|-------------|----------|
| **Frontend** | React (Vite) | Chat-style interface for prompt + code preview |
| **Backend** | FastAPI (Python) | Handles AI requests + contract deployment |
| **AI API** | OpenAI GPT-4o | Generates and formats PyTeal code |
| **Blockchain SDK** | Algokit, PyTeal, Beaker | Smart contract compilation and deployment |
| **Network** | Algorand TestNet | Live contract testing |
| **Storage** | GitHub (Open Source) | Code hosting + submission repo |

---

## 🧱 Architecture Diagram

