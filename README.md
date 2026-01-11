# StudyPal
Public showcase and documentation for StudyPal, an AI-powered study assistant.

StudyPal is an AI-powered study assistant designed to help students learn more effectively using active recall, smart notes, and adaptive quizzes.

This public repository serves as a project overview and showcase.  
The core implementation and internal logic are maintained in a private repository.

What StudyPal Does?
- Generates **AI-powered recall cards** from study material
- Creates **structured smart notes** for quick understanding
- Builds **custom quizzes** to test knowledge retention
- Time Based Session for the **last minute revision**
- Validates and processes large text inputs efficiently


🛠️ Technical Evolution & Features (Date: 2025-01-07)

📄 Advanced OCR & Document Processing
Mistral OCR Integration: Incorporated the cutting-edge Mistral OCR API (mistral-ocr-latest) to handle document ingestion.
Universal Reading: Capable of extracting text not just from standard PDFs, but also from scanned documents and images.
High Fidelity: Ensures complex diagrams and textbook pages are accurately converted into text for the AI to analyze.

🧠 Next-Gen AI Architecture
OpenRouter Migration: Transitioned backend infrastructure from Google Gemini to OpenRouter, utilizing the efficient xiaomi/mimo-v2-flash model.
Reasoning Capabilities: Enabled advanced reasoning parameters for deeper logic in card generation.
Context-Aware Tutor:
The "Explain" feature now injects the original source text (from the PDF) into the prompt.
Result: Explanations are grounded in the specific study material, not generic knowledge.
Professor Persona: Tuned the system prompt to act as an encouraging, expert academic tutor.

✨ UX & Interface Polishing
Seamless Workflow:
Background Processing: Extracted text is now handled silently in the background (extractedText state), keeping the UI clean and clutter-free.
Drag & Drop: Fixed browser events to allow smooth PDF drag-and-drop functionality.
Instant Preview: Added one-click PDF preview opening in a new tab.
Rich Visuals:
Smart Formatting: Explanations automatically format key terms with yellow highlights and bold text for better readability.
Local Persistence: Implemented localStorage strategies to save "Understood" and "Review" progress across browser refreshes.


Implementation of SmartNotes (10 Jan 26)
Did the smart ui/ux design for the smart note and also made change in the api with the rate limiting, decling lag issue and better prompt so there wont be more overwhelming for the student to use it. And also made review card with optimal ui/ux in recall cards section. Also I designed the new logo and chnaged it, that matches the theme quite well. 