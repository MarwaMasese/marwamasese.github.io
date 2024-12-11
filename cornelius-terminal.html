<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cornelius Maroa - AI Research Terminal</title>
    <style>
        :root {
            --bg-color: #0c0c0c;
            --text-color: #00ff00;
            --cursor-color: #00ff00;
            --highlight-color: #00ffff;
            --section-color: #00ff99;
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Courier New', monospace;
        }
        body {
            background-color: var(--bg-color);
            color: var(--text-color);
            line-height: 1.6;
            padding: 20px;
            max-width: 800px;
            margin: 0 auto;
        }
        #terminal {
            background-color: rgba(0,0,0,0.8);
            border: 2px solid #333;
            padding: 20px;
            min-height: 500px;
            overflow-y: auto;
            font-size: 14px;
        }
        #input-line {
            display: flex;
            align-items: center;
        }
        #command-input {
            background: transparent;
            border: none;
            color: var(--text-color);
            font-family: 'Courier New', monospace;
            width: 100%;
            outline: none;
            font-size: 16px;
        }
        .prompt {
            color: #00ff00;
            margin-right: 10px;
        }
        .output {
            margin-bottom: 10px;
            white-space: pre-wrap;
        }
        .error {
            color: red;
        }
        .highlight {
            color: var(--highlight-color);
            font-weight: bold;
        }
        .section-title {
            color: var(--section-color);
            font-weight: bold;
            text-decoration: underline;
            margin-bottom: 10px;
        }
        .command-list {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 10px;
        }
        .command-button {
            background-color: #003300;
            color: #00ff00;
            border: 1px solid #00ff00;
            padding: 5px 10px;
            cursor: pointer;
            transition: all 0.3s ease;
        }
        .command-button:hover {
            background-color: #00ff00;
            color: #0c0c0c;
        }
        .cursor {
            animation: blink 1s infinite;
            display: inline-block;
            margin-left: 2px;
            width: 10px;
            height: 20px;
            background-color: var(--cursor-color);
        }
        @keyframes blink {
            0%, 100% { opacity: 1; }
            50% { opacity: 0; }
        }
    </style>
</head>
<body>
    <div id="terminal">
        <div id="output"></div>
        <div id="command-list" class="command-list"></div>
        <div id="input-line">
            <span class="prompt">visitor@cornelius-research:~$</span>
            <input type="text" id="command-input" autocomplete="off">
            <span class="cursor"></span>
        </div>
    </div>

    <script>
        const output = document.getElementById('output');
        const commandInput = document.getElementById('command-input');
        const commandList = document.getElementById('command-list');
        const cursor = document.querySelector('.cursor');

        // Commands and their handlers
        const commands = {
            help: () => `Available commands:
    • about     : Personal introduction
    • research  : Detailed research experience
    • publications : Research publications
    • skills    : Technical expertise
    • contact   : Contact information
    • clear     : Clear terminal screen`,

            about: () => `
\x1b[1;36m[PERSONAL PROFILE]\x1b[0m
\x1b[1;33mCORNELIUS MAROA\x1b[0m
marwamasese@gmail.com | linkedin.com/in/marwamasese

\x1b[1;36m[RESEARCH INTERESTS]\x1b[0m
Artificial Intelligence | Multi-Agent Systems | Neural-Symbolic Reasoning | Multimodal Learning | Embodied AI

\x1b[1;36m[EDUCATION]\x1b[0m
Bachelor of Science in Software Engineering
KCA University, Nairobi | GPA: 3.5
Thesis: "Emergent Behaviors in Multi-Agent Reinforcement Learning Systems"
• Investigated the emergence of cooperative strategies in multi-agent environments using novel reward shaping
• Implemented custom MARL environment using PyTorch, achieving 47% improvement in agent coordination`,

            research: () => `
\x1b[1;36m[RESEARCH EXPERIENCE]\x1b[0m

\x1b[1;33mResearch Lead & Co-founder, Intelliverse AI\x1b[0m
\x1b[3m(Jan 2022 - Present)\x1b[0m
• Pioneering research in multi-agent systems for distributed problem-solving, resulting in 2 technical reports
• Developed novel architecture combining transformer-based reasoning with symbolic knowledge representation
• Led team of 10 researchers in implementing scalable multi-agent training framework on Bittensor network (Distributed Training)
• The research resulted in 3x improvement in agent cooperation metrics compared to baseline approaches

\x1b[1;33mAI Research Engineer, Once Inc - Shamba Records\x1b[0m
\x1b[3m(2020 - 2021)\x1b[0m
• Designed and implemented vision-language model for crop disease detection achieving 92% accuracy
• Developed causal inference framework for agricultural yield prediction, reducing error by 35%
• Published technical whitepaper on scalable AI systems for agricultural intelligence
• Created novel data augmentation techniques for limited agricultural visual data

\x1b[1;36m[SELECTED RESEARCH PROJECTS]\x1b[0m
\x1b[1;33mMulti-Agent Reasoning Framework (2023)\x1b[0m
• Developed novel architecture for emergent reasoning in distributed agent networks
• Implemented a hybrid approach combining transformer attention and symbolic reasoning

\x1b[1;33mCross-Modal Knowledge Integration System (2022)\x1b[0m
• Built system for integrating visual, textual, and structured knowledge
• Implemented novel attention mechanism for cross-modal alignment

\x1b[1;33mRafiki: Advanced Mental Health AI System\x1b[0m
• Developed novel approach to emotional intelligence in conversational AI
• Technologies: LLaMA, RAG, Custom emotional embeddings`,

            publications: () => `
\x1b[1;36m[CONFERENCES & SEMINARS]\x1b[0m
• Applied Machine Learning Days (AMLD) Africa - USIU Africa
  - Featured Speaker: "How AI and Virtual Reality Can Help Revolutionize Cultural Heritage in Africa"
• Deep Learning Indaba - Senegal
  - Invited Speaker: "Neural-Symbolic Integration in Agricultural AI Systems"

\x1b[1;36m[PUBLICATIONS & TECHNICAL WRITING]\x1b[0m
1. "Emergent Reasoning in Distributed Agent Networks" (Technical Report, 2023)
2. "Cross-Modal Knowledge Integration for Agricultural Intelligence" (Whitepaper, 2022)
3. "Scaling Multi-Agent Training on Decentralized Networks" (Technical Report, 2023)`,

            skills: () => `
\x1b[1;36m[TECHNICAL EXPERTISE]\x1b[0m
• Deep Learning Frameworks: PyTorch, JAX, TensorFlow (Advanced)
• AI/ML: Transformers, MARL, Neural-Symbolic Systems, Causal Inference
• Research Tools: Weights & Biases, Ray, Docker, Kubernetes
• Languages: Python, C++, Julia
• Infrastructure: Distributed Systems, Cloud (GCP, Azure)`,

            contact: () => `
\x1b[1;36m[CONTACT INFORMATION]\x1b[0m
📧 Email: \x1b[1;33mmarwamasese@gmail.com\x1b[0m
🔗 LinkedIn: \x1b[1;33mlinkedin.com/in/marwamasese\x1b[0m

\x1b[1;36m[REFEREES]\x1b[0m
1. Dr. Wanyoike John Ngaii
   • Email: jwanyoike@kcau.ac.ke
   • Affiliation: Faculty of Computing, KCA University

2. Mohammed Dhraief
   • Email: mohamed.ali.dhraief@ibm.com
   • Affiliation: PRESIDENT AMLD AFRICA`,

            clear: () => {
                output.innerHTML = '';
                return '';
            }
        };

        function processCommand(command) {
            command = command.trim().toLowerCase();
            
            if (commands[command]) {
                return commands[command]();
            } else {
                return `\x1b[1;31mUnknown command. Type 'help' for available commands.\x1b[0m`;
            }
        }

        function addOutput(text) {
            const outputDiv = document.createElement('div');
            outputDiv.classList.add('output');
            outputDiv.innerHTML = text.replace(/\x1b\[([0-9;]+)m/g, (match, p1) => {
                const styles = p1.split(';');
                let className = '';
                
                if (styles.includes('1')) className += ' highlight';
                if (styles.includes('3')) className += ' italic';
                if (styles.includes('31')) className += ' error';
                if (styles.includes('33')) className += ' section-title';
                if (styles.includes('36')) className += ' section-title';
                
                return `<span class="${className.trim()}">`;
            }).replace(/\x1b\[0m/g, '</span>');
            
            output.appendChild(outputDiv);
            output.scrollTop = output.scrollHeight;
        }

        function createCommandButtons() {
            commandList.innerHTML = '';
            Object.keys(commands).forEach(cmd => {
                if (cmd !== 'clear') {
                    const button = document.createElement('button');
                    button.textContent = cmd;
                    button.classList.add('command-button');
                    button.addEventListener('click', () => {
                        addOutput(`<span class="prompt">visitor@cornelius-research:~$</span> ${cmd}`);
                        addOutput(processCommand(cmd));
                        commandInput.focus();
                    });
                    commandList.appendChild(button);
                }
            });
        }

        function initTerminal() {
            addOutput(`
\x1b[1;36mWelcome to Cornelius Maroa's Research Terminal\x1b[0m
Type a command or click a button to explore`);
            createCommandButtons();
        }

        commandInput.addEventListener('keypress', (e) => {
            if (e.key === 'Enter') {
                const command = commandInput.value;
                addOutput(`<span class="prompt">visitor@cornelius-research:~$</span> ${command}`);
                addOutput(processCommand(command));
                commandInput.value = '';
            }
        });

        initTerminal();

        document.addEventListener('click', () => {
            commandInput.focus();
        });
    </script>
</body>
</html>
