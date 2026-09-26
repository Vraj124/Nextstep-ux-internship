# NextStep — Figma Import Guide & Deliverables

> **HAZHTeq Innovations UI/UX Developer Internship Challenge**  
> **Deliverable Format:** Structured Vector SVG Artboards (375 × 812 Mobile Viewport) & Master Prototype Canvas (2400 × 1800)

---

## 1. Deliverable Overview & Honest Compatibility Disclosure

In compliance with Sections 24–28 of the brief, this directory contains **genuine, Figma-compatible vector design assets** structured for immediate import into Figma.

### ✅ What is provided:
* **17 SVG screens and states** formatted at standard 375 × 812 mobile dimensions (`01_problem_input.svg` through `17_next_action_detail.svg`).
* **SVG components & asset variants** (`12_priority_card_states.svg`).
* **Design tokens artboard** (`13_design_tokens.svg`).
* **Visual flow diagram on master canvas** (`nextstep_figma_canvas.svg`).
* **Interactive browser prototype** (`prototype_preview.html`) demonstrating the complete journey and all 7 scenario branches without requiring a Figma account.

### ❌ What is NOT provided (Honest Disclosure):
* **No native `.fig` binary file:** We do NOT generate a fake or renamed `.fig` file.
* **No pre-wired native Figma prototype noodle connections:** Importing an SVG into Figma does NOT automatically generate clickable Figma interaction wires. The arrows shown on `nextstep_figma_canvas.svg` are a visual flow diagram. If you want a native clickable prototype inside Figma itself, you can easily wire connections between the imported frames using Figma's Prototype tab (instructions in Section 3).
* **The interactive prototype is provided as a browser prototype (`prototype_preview.html`)**, which runs the full click-through prototype immediately in any browser.

---

## 2. Included Figma Files

| File | Type | Screen / Frame Content |
| :--- | :--- | :--- |
| **`nextstep_figma_canvas.svg`** | **Master Canvas** | Complete multi-frame board (2400 × 1800) containing the Main Decision Journey and all Scenario Branches connected with prototype flow arrows. |
| **`01_problem_input.svg`** | Screen Frame | Problem input, char counter, Jugaad review cushion, "Help me figure this out". |
| **`02_understanding.svg`** | Screen Frame | Progressive extraction with checkmarks, "Did I understand that correctly?". |
| **`03_correction.svg`** | Screen Frame | Inline detail editing without restarting. |
| **`04_clarification.svg`** | Screen Frame | Single progressive clarification question with option chips, custom answer, and skip. |
| **`05_prioritisation.svg`** | Screen Frame | "Here's what matters most right now", NEXT STEP card, Priority #1 card with reasoning, "Also on your plate". |
| **`06_calm_mode.svg`** | Screen Frame | Dedicated Calm Mode (Scenario 4) with earthen sage styling, supportive text, Tele-MANAS (14416). |
| **`07_recovery.svg`** | Screen Frame | Scenario 7 Recovery: "That didn't go as expected", what changed, non-blaming actions. |
| **`08_reassessment.svg`** | Screen Frame | "How did it go? (Better / Not yet / Something changed / It got worse)" and returning user updates. |
| **`09_contradiction.svg`** | Screen Frame | Scenario 3 Contradiction: "I don't want to guess. Thursday or Friday". |
| **`10_out_of_scope.svg`** | Screen Frame | Scenario 5 Misuse: "This isn't really a decision-support situation". |
| **`11_adversarial.svg`** | Screen Frame | Scenario 6 Adversarial Injection: Safety explanation, inert text handling. |
| **`12_priority_card_states.svg`** | Component Variants | Default Top Priority, Tied Priority ("Two things need attention first"), Loading state, Error state. |
| **`13_design_tokens.svg`** | Design System | Mini design tokens: Color palette, typography scale, spacing, accessible 48px touch targets. |
| **`14_loading_state.svg`** | State Frame | Spinner and progressive understanding status. |
| **`15_error_state.svg`** | State Frame | Calm, non-vague error explanation with retry and edit actions. |
| **`16_empty_state.svg`** | State Frame | Empty state when no priority has been determined. |
| **`17_next_action_detail.svg`** | Detail Frame | Dedicated single action focus view. |
| **`prototype_preview.html`** | Interactive Player | Interactive Figma-like click-through prototype player testable in any browser. |

---

## 3. How to Import into Figma

### Method A: Single-Canvas Import (Recommended)
1. Open [Figma](https://www.figma.com/) (Desktop app or Web browser).
2. Create a new design file.
3. Open your computer's file explorer and navigate to:  
   `C:\Users\Vraj Rana\.gemini\antigravity-ide\scratch\nextstep\figma`
4. Drag and drop **`nextstep_figma_canvas.svg`** directly onto the Figma canvas.
5. Figma will automatically parse all layers into grouped frames, vector rectangles, editable text layers, and flowchart arrows.

### Method B: Individual Artboard Frames
1. In your Figma file, drag and drop any of the individual SVG files (`01_problem_input.svg` through `17_next_action_detail.svg`).
2. Each file will be imported as an exact 375 × 812 mobile frame.
3. To wire Figma's native prototype noodles:
   - Select the button inside Frame 1 (`#Btn_Submit`) → Link prototype connection to Frame 2 (`#Screen_Understanding`).
   - Select `"Something's wrong"` inside Frame 2 → Link to Frame 3 (`#Screen_Correction`).
   - Select `"Yes, that's right"` inside Frame 2 → Link to Frame 4 (`#Screen_Clarification`).
   - Select Option Chip inside Frame 4 → Link to Frame 5 (`#Screen_Prioritisation`).
   - Select `"Do this now"` inside Frame 5 → Link to Frame 8 (`#Screen_Reassessment`).

---

## 4. Interactive Prototype Viewer

You can test the exact Figma prototype flow without needing Figma installed:
1. Start the local server if not running (`python -m http.server 3000`).
2. Open in your browser:  
   **`http://localhost:3000/figma/prototype_preview.html`**
3. Click through the prototype actions or jump between screens using the top navigation bar.
