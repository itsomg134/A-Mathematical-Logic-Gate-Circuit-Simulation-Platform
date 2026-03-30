# A Mathematical Logic Gate & Circuit Simulation Platform

![Logic Forge Banner](https://img.shields.io/badge/Logic%20Forge-Circuit%20Simulator-blue?style=for-the-badge&logo=javascript)
![Version](https://img.shields.io/badge/version-1.0.0-green)
![License](https://img.shields.io/badge/license-MIT-orange)

**Logic Forge** is an interactive, browser-based digital logic circuit simulator that allows you to build, simulate, and analyze combinational logic circuits through an intuitive drag-and-drop interface. Design circuits using fundamental logic gates, connect them with wires, toggle inputs, and observe real-time outputs — all without writing a single line of code.


##  Features

- **Drag & Drop Circuit Building** — Simply drag gates from the toolbox onto the canvas
- **6 Core Logic Gates** — AND, OR, NOT, NAND, NOR, XOR
- **Interactive Input Nodes** — Click to toggle between 0 and 1 states
- **Visual Wire Connections** — Connect gate outputs to inputs with intuitive dragging
- **Real-Time Evaluation** — Circuit outputs update automatically as you modify connections
- **Truth Table Display** — Live visualization of all input/output states
- **Half-Adder Demo** — One-click example to demonstrate full adder functionality
- **Clean Visual Design** — Grid-based canvas with color-coded gates and status LEDs
- **No Dependencies** — Pure HTML/CSS/JavaScript, runs entirely in the browser

---

## 🎮 How to Use

### 1. Adding Gates
- Locate the **Logic Gates** panel on the left
- Click and drag any gate (AND, OR, NOT, etc.) onto the grid
- Release to place the gate

### 2. Adding Inputs & Outputs
- Click **"Add Input Toggle"** to create a new input node
- Click **"Add Output Probe"** to create an output display
- Inputs can be toggled by clicking directly on them

### 3. Making Connections
- **From Gate Output → Gate Input:** Click and drag from the small circle on the right side of a gate (output pin) to the small circle on the left side of another gate (input pin)
- **From Input Node → Gate Input:** Input nodes can be connected the same way — drag from the input node to a gate's input pin
- Wires appear automatically, and the circuit evaluates immediately

### 4. Simulating
- Toggle input nodes to see how outputs change
- Use the **"Evaluate Circuit"** button to force a refresh
- The **Truth Panel** shows current values for all inputs and outputs with LED indicators

### 5. Managing Your Circuit
- **Clear Circuit** — Remove all gates, wires, and probes
- **Demo: Half-Adder** — Loads a working half-adder circuit (A ⊕ B = SUM, A ∧ B = CARRY)

---

##  Supported Logic Gates

| Gate  | Symbol | Truth Table (A, B → Output) |
|-------|--------|----------------------------|
| **AND** | ∧ | 00→0, 01→0, 10→0, 11→1 |
| **OR** | ∨ | 00→0, 01→1, 10→1, 11→1 |
| **NOT** | ¬ | 0→1, 1→0 |
| **NAND** | ↑ | 00→1, 01→1, 10→1, 11→0 |
| **NOR** | ↓ | 00→1, 01→0, 10→0, 11→0 |
| **XOR** | ⊕ | 00→0, 01→1, 10→1, 11→0 |

---

##  Technology Stack

- **HTML5 Canvas** — For rendering circuits and handling interactions
- **Vanilla JavaScript** — No frameworks, pure logic evaluation
- **CSS3** — Modern gradients, glass-morphism effects, and responsive layout

---

##  Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)

### Local Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/logic-forge.git
   ```
2. Navigate to the project folder:
   ```bash
   cd logic-forge
   ```
3. Open `index.html` in your browser — no build step or server required!

### Deployment
You can deploy instantly using:
- **GitHub Pages**: Push to a `gh-pages` branch or enable Pages in repo settings
- **Netlify/Vercel**: Drag and drop the folder

---

##  Example: Building a Half-Adder

1. Add two input nodes (A and B)
2. Add an **XOR** gate and an **AND** gate
3. Connect input A to both gates' first inputs
4. Connect input B to both gates' second inputs
5. Add output probes connected to XOR (SUM) and AND (CARRY)
6. Toggle inputs and watch the truth table match binary addition

---

##  Project Structure

```
logic-forge/
├── index.html          # Main application file (HTML/CSS/JS)
├── README.md           # This documentation
└── assets/             # (Optional) Screenshots, icons
```

---

##  Future Enhancements

- [ ] **Save/Load Circuits** — Export/import JSON circuit configurations
- [ ] **Undo/Redo** — Support for design iterations
- [ ] **Custom Gate Creation** — Build and save subcircuits as reusable components
- [ ] **Timing Simulation** — Add gate delays and clock signals
- [ ] **Truth Table Generator** — Auto-generate full truth tables for any circuit
- [ ] **Dark/Light Theme Toggle**
- [ ] **Mobile Touch Support** — Improved drag interactions on tablets

---

##  Contributing

Contributions are welcome! If you'd like to improve Logic Forge:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

Please ensure your code follows the existing style and includes appropriate comments.

---

##  License

Distributed under the MIT License. See `LICENSE` file for more information.

---

##  Acknowledgments

- Inspired by classic digital logic simulators like Logisim and Digital
- Circuit evaluation model based on combinational logic theory
- Icons and visual design influenced by modern educational tools

