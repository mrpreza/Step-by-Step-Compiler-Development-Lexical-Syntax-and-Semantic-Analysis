# Step-by-Step-Compiler-Development-Lexical-Syntax-and-Semantic-Analysis
A multi-phase Java-based compiler project implementing lexical analysis, syntax analysis, and code generation using JFlex and custom parsing techniques. Includes test cases and sample outputs for validation.





## 📖 Project Overview
The project is divided into several phases:

1. **Phase 1 – Lexical Analysis**  
   - Implemented using **JFlex**.  
   - Converts raw source code into a stream of tokens.  
   - Handles identifiers, keywords, operators, and literals.  

2. **Phase 2 – Syntax Analysis (Parsing)**  
   - Builds a **parser** to validate token streams against the grammar.  
   - Detects syntax errors and generates structured parse trees.  

3. **Phase 3 – Semantic Analysis & Code Generation**  
   - Performs semantic checks.  
   - Translates validated code into intermediate/output representation.  

---

## 🛠️ Technologies Used
- **Java** (main implementation language)  
- **JFlex** (lexical analyzer generator)  
- **Custom parser & utility classes**  
- Standard Java I/O for test files and outputs  

---

## 📂 Repository Structure
```

.
├── src/                  # Source code
│   ├── phaze_one.java    # Lexical analyzer
│   ├── Utility.java      # Helper functions
│   ├── Yytoken.java      # Token structure
│   ├── Project.flex      # JFlex lexer specification
│   └── recov.txt
├── test.txt              # Sample input program
├── output_testFile.txt   # Sample output from lexer
├── output.good           # Expected output
├── compiler.iml          # IntelliJ project configuration
├── phase2/               # Syntax analysis phase
├── phase3/               # Semantic analysis & code generation phase
└── docs/                 # Reports, notes, and additional files

````

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/your-username/compiler-project.git
cd compiler-project
````

### 2. Build the project

Compile the Java sources:

```bash
javac src/*.java
```

### 3. Run the compiler

Execute the main entry point (adjust classpath if needed):

```bash
java src/phaze_one test.txt
```

---

## ✅ Example

Input (`test.txt`):

```text
int a = 5 + 3;
```

Output (`output_testFile.txt`):

```text
[INT] [IDENTIFIER:a] [ASSIGN] [NUMBER:5] [PLUS] [NUMBER:3] [SEMICOLON]
```

---

## 📌 Future Improvements

* Extend grammar support.
* Implement full semantic checking.
* Add intermediate code optimization.
* Build a backend code generator for assembly output.

---

## 🤝 Contributors
*  Reza Paktinat
*  Seyed Mohammad Ebrahim Mosavi


---

## 📜 License

This project is provided for educational purposes.
Feel free to fork and experiment with the implementation.

```


