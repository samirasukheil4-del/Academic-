<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
  <title>Tanzanian Syllabus: Academic Writing Guide & Quiz</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #f0f7f0;
      font-family: 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif;
      line-height: 1.5;
      color: #1a2e1f;
      padding: 2rem 1rem;
    }

    /* main container */
    .container {
      max-width: 1200px;
      margin: 0 auto;
      background: white;
      border-radius: 28px;
      box-shadow: 0 20px 35px -12px rgba(0, 32, 0, 0.2);
      overflow: hidden;
      transition: all 0.2s;
    }

    /* header with Tanzanian touch */
    .header {
      background: linear-gradient(135deg, #1e5a2e, #0b3b1a);
      padding: 2rem 2rem 1.8rem;
      color: white;
      text-align: center;
    }

    .header h1 {
      font-size: 2.2rem;
      letter-spacing: -0.3px;
      margin-bottom: 0.5rem;
      font-weight: 700;
    }

    .header p {
      font-size: 1.1rem;
      opacity: 0.9;
      max-width: 700px;
      margin: 0 auto;
    }

    .flag-strip {
      height: 6px;
      background: linear-gradient(90deg, #1ebd52, #ffcc00, #3399ff, #000000);
      width: 100%;
    }

    /* content sections */
    .content {
      padding: 2rem 2rem 1rem;
    }

    .section {
      margin-bottom: 2.5rem;
      border-left: 5px solid #2b7a3e;
      padding-left: 1.5rem;
      transition: 0.1s;
    }

    .section h2 {
      font-size: 1.8rem;
      margin-bottom: 1rem;
      color: #145c2c;
      display: flex;
      align-items: center;
      gap: 12px;
      flex-wrap: wrap;
    }

    .section h2 i {
      font-size: 1.6rem;
    }

    .section h3 {
      font-size: 1.3rem;
      margin: 1.2rem 0 0.6rem 0;
      color: #1f5434;
    }

    .card-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 1.5rem;
      margin-top: 1rem;
    }

    .def-box, .consider-box, .example-box {
      background: #fefef7;
      border-radius: 24px;
      box-shadow: 0 6px 14px rgba(0, 0, 0, 0.05);
      padding: 1.4rem 1.8rem;
      flex: 1 1 280px;
      border: 1px solid #d9ead3;
    }

    .def-box p, .consider-box p {
      margin-top: 0.5rem;
    }

    .definition-highlight {
      background: #e9f5e9;
      padding: 1rem;
      border-radius: 20px;
      font-size: 1.05rem;
      border-left: 4px solid #2e7d32;
    }

    .list-consider {
      list-style: none;
      padding-left: 0;
    }

    .list-consider li {
      margin-bottom: 0.85rem;
      display: flex;
      gap: 12px;
      align-items: flex-start;
    }

    .list-consider li strong {
      min-width: 100px;
      color: #1c6e3c;
    }

    /* EXAMPLE FORMAT TABLE / CARD */
    .format-card {
      background: #fafbf7;
      border-radius: 24px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      overflow: hidden;
      border: 1px solid #cde2cd;
      margin-top: 0.8rem;
    }

    .format-header {
      background: #2b7a3e;
      color: white;
      padding: 0.9rem 1.5rem;
      font-weight: bold;
      font-size: 1.2rem;
    }

    .format-body {
      padding: 1.2rem 1.8rem;
    }

    .format-body table {
      width: 100%;
      border-collapse: collapse;
    }

    .format-body td, .format-body th {
      padding: 12px 8px;
      vertical-align: top;
      border-bottom: 1px solid #e2f0dc;
    }

    .format-body tr:last-child td {
      border-bottom: none;
    }

    .section-label {
      font-weight: 700;
      width: 120px;
      color: #1c4d2d;
    }

    .italic-note {
      font-style: italic;
      color: #3a5a3a;
      background: #f2f9ec;
      padding: 0.8rem;
      border-radius: 16px;
      margin-top: 1rem;
      font-size: 0.9rem;
    }

    /* QUIZ SECTION */
    .quiz-section {
      background: #fbfef8;
      border-radius: 28px;
      margin: 1.5rem 0 2rem;
      padding: 1.8rem;
      border: 1px solid #c8e0bc;
      box-shadow: 0 6px 12px rgba(0, 0, 0, 0.03);
    }

    .quiz-section h2 {
      border-left: none;
      margin-top: 0;
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .quiz-question {
      background: white;
      border-radius: 20px;
      margin-bottom: 1.4rem;
      padding: 1rem 1.2rem;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.05);
      border: 1px solid #e2efda;
    }

    .question-text {
      font-weight: 700;
      font-size: 1.05rem;
      margin-bottom: 0.6rem;
      color: #0a2f1a;
    }

    .options {
      display: flex;
      flex-wrap: wrap;
      gap: 1rem;
      margin: 0.5rem 0 0.2rem;
    }

    .option {
      display: flex;
      align-items: center;
      gap: 8px;
      background: #f7fcf4;
      padding: 0.3rem 0.9rem;
      border-radius: 40px;
      cursor: pointer;
      transition: 0.1s;
      border: 1px solid #d0e6c4;
    }

    .option:hover {
      background: #e2f0da;
    }

    input[type="radio"] {
      accent-color: #2b7a3e;
      width: 18px;
      height: 18px;
    }

    .quiz-feedback {
      margin-top: 1rem;
      background: #eef3ea;
      border-radius: 32px;
      padding: 1rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }

    .btn {
      background: #2b7a3e;
      border: none;
      color: white;
      font-weight: bold;
      padding: 0.75rem 2rem;
      border-radius: 60px;
      font-size: 1rem;
      cursor: pointer;
      transition: 0.2s;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }

    .btn:hover {
      background: #1e5f30;
      transform: translateY(-1px);
    }

    .reset-btn {
      background: #5a6e5a;
    }
    .reset-btn:hover {
      background: #3c533c;
    }

    .score {
      font-size: 1.2rem;
      font-weight: bold;
      background: white;
      padding: 0.3rem 1rem;
      border-radius: 40px;
      color: #145c2c;
    }

    .explanation {
      margin-top: 12px;
      font-size: 0.9rem;
      color: #3b5c2e;
      background: #f1f8ec;
      padding: 0.5rem 0.8rem;
      border-radius: 14px;
      display: inline-block;
    }

    hr {
      margin: 1rem 0;
      border-color: #cfe2cf;
    }

    footer {
      text-align: center;
      font-size: 0.8rem;
      padding: 1.5rem;
      background: #eef3ea;
      color: #325a2c;
      border-top: 1px solid #cde0c4;
    }

    @media (max-width: 680px) {
      .content {
        padding: 1.2rem;
      }
      .section {
        padding-left: 1rem;
      }
      .options {
        flex-direction: column;
        gap: 0.4rem;
      }
      .format-body td, .format-body th {
        display: block;
        width: 100%;
      }
      .section-label {
        width: auto;
        font-weight: bold;
        margin-top: 10px;
      }
    }
  </style>
</head>
<body>
<div class="container">
  <div class="flag-strip"></div>
  <div class="header">
    <h1>📘 Academic Writing | Tanzania Syllabus</h1>
    <p>Master the principles, structure, and style of university-level academic writing</p>
  </div>

  <div class="content">
    <!-- SECTION 1: DEFINITION -->
    <div class="section">
      <h2>📖 1. Definition of Academic Writing</h2>
      <div class="definition-highlight">
        <p><strong>Academic writing</strong> is a formal, structured, and evidence-based style of writing used in universities and scholarly publications. Its main purpose is to inform, analyze, and argue using logical reasoning, credible sources, and precise language. Unlike casual or creative writing, academic writing follows strict conventions regarding tone, citation, and organization.</p>
        <p style="margin-top: 8px;">📌 In the Tanzanian context, academic writing aligns with the Tanzania Commission for Universities (TCU) standards, emphasizing clarity, objectivity, and respect for intellectual property.</p>
      </div>
      <div class="card-grid">
        <div class="def-box">
          <h3>🎯 Core features</h3>
          <p>✔ Formal tone & vocabulary<br>✔ Evidence & citations (APA, MLA, etc.)<br>✔ Clear thesis statement<br>✔ Logical flow & coherence<br>✔ Impersonal & objective style</p>
        </div>
        <div class="def-box">
          <h3>📚 Common genres</h3>
          <p>• Research papers<br>• Essays (argumentative, expository)<br>• Literature reviews<br>• Dissertations & Theses<br>• Reports & case studies</p>
        </div>
      </div>
    </div>

    <!-- SECTION 2: WHAT TO CONSIDER IN ACADEMIC WRITINGS -->
    <div class="section">
      <h2>⚙️ 2. What to Consider in Academic Writings</h2>
      <div class="card-grid">
        <div class="consider-box" style="flex: 2;">
          <ul class="list-consider">
            <li><strong>📌 Audience & Purpose:</strong> Identify readers (lecturers, researchers) and aim (to argue, explain, or analyze).</li>
            <li><strong>📌 Clarity & Precision:</strong> Avoid vague expressions; define key terms and use discipline-specific vocabulary accurately.</li>
            <li><strong>📌 Structure & Organization:</strong> Follow IMRAD (for sciences) or essay structure (intro, body, conclusion) with logical paragraph transitions.</li>
            <li><strong>📌 Evidence & Referencing:</strong> Use peer-reviewed sources, cite correctly to avoid plagiarism. Common styles: APA 7th, MLA, Chicago.</li>
            <li><strong>📌 Objectivity & Formality:</strong> Avoid emotional language, slang, contractions, and personal anecdotes (unless permitted).</li>
            <li><strong>📌 Academic Integrity:</strong> Paraphrase properly, use quotation marks for direct quotes, and provide full bibliography.</li>
            <li><strong>📌 Language & Grammar:</strong> Correct tense usage, subject-verb agreement, and sophisticated sentence structures.</li>
            <li><strong>📌 Critical Thinking:</strong> Not just describing facts, but evaluating, synthesizing, and presenting original arguments.</li>
          </ul>
        </div>
      </div>
    </div>

    <!-- SECTION 3: EXAMPLE FORMAT OF ACADEMIC WRITING (ESSAY STRUCTURE) -->
    <div class="section">
      <h2>📝 3. Example Format: Standard Academic Essay</h2>
      <div class="format-card">
        <div class="format-header">📄 Structure of an Argumentative Academic Essay</div>
        <div class="format-body">
          <table>
            <tr><td class="section-label">Title Page</td><td>Title, Author's name, Course code, Instructor, Date (if required)</td></tr>
            <tr><td class="section-label">Abstract (optional)</td><td>Concise summary (150-250 words): research problem, methods, key findings, and conclusion.</td></tr>
            <tr><td class="section-label">Introduction</td><td>Hook, background context, problem statement, thesis statement (main argument).</td></tr>
            <tr><td class="section-label">Body Paragraphs</td><td>Each paragraph: topic sentence → evidence (citations) → analysis → linking sentence. Multiple paragraphs to support the thesis.</td></tr>
            <tr><td class="section-label">Counterargument</td><td>Address opposing views and rebut them with evidence (strengthens credibility).</td></tr>
            <tr><td class="section-label">Conclusion</td><td>Restate thesis, summarize main points, suggest implications or future research. No new ideas.</td></tr>
            <tr><td class="section-label">References</td><td>List all cited sources alphabetically (APA format example: Author, A. (Year). Title. Publisher).</td></tr>
          </table>
          <div class="italic-note">
            💡 <strong>Tanzanian note:</strong> Most universities (UDSM, SUA, OUT) prefer APA 7th edition for social sciences, sciences, and education. Always confirm with your department.
          </div>
        </div>
      </div>
      <!-- mini example snippet -->
      <div style="margin-top: 1rem; background:#faf9f0; border-radius: 20px; padding: 1rem; border:1px solid #e2e8cf">
        <strong>✍️ Short excerpt (Academic paragraph example):</strong><br>
        "Climate change poses a direct threat to Tanzania’s agricultural productivity, particularly in semi-arid regions (Mushi & Juma, 2021). According to recent longitudinal studies, maize yields have declined by 18% over the past decade due to erratic rainfall patterns (TCRA, 2022). These findings underscore the urgency for adopting drought-resistant crops and sustainable irrigation methods."
      </div>
    </div>

    <!-- QUIZ SECTION: 10 QUESTIONS -->
    <div class="quiz-section" id="quizContainer">
      <h2>📋 4. Academic Writing Quiz (10 Exam-Style Questions)</h2>
      <p style="margin-bottom: 1.2rem;">Test your understanding of academic writing rules, structure, and conventions. Select the best answer for each question.</p>
      <form id="quizForm">
        <!-- questions injected by JS -->
        <div id="questionsList"></div>
        <div class="quiz-feedback">
          <button type="button" class="btn" id="submitQuiz">✅ Submit Answers</button>
          <button type="button" class="btn reset-btn" id="resetQuiz">⟳ Reset Quiz</button>
          <div id="scoreDisplay" class="score">Score: -- / 10</div>
        </div>
        <div id="globalFeedback" style="margin-top: 16px; font-size:0.9rem;"></div>
      </form>
    </div>
  </div>
  <footer>
    📚 Aligned with Tanzanian Higher Education Syllabus | Academic Integrity & Writing Excellence
  </footer>
</div>

<script>
  // 10 quiz questions (directly mapped to academic writing topics)
  const questionsData = [
    {
      text: "1. Which of the following BEST defines academic writing?",
      options: [
        "Writing that uses personal stories and informal language.",
        "A formal, evidence-based writing style with logical reasoning and citations.",
        "Creative writing focused on emotions and imagination.",
        "A type of journalistic writing for newspapers."
      ],
      correct: 1, // zero-indexed
      explanation: "Academic writing is formal, structured, and relies on evidence & citations."
    },
    {
      text: "2. In academic writing, what is the main purpose of a thesis statement?",
      options: [
        "To present a question without answer.",
        "To provide background information only.",
        "To state the central argument or claim of the paper.",
        "To list all references used in the research."
      ],
      correct: 2,
      explanation: "The thesis statement declares the writer's main argument or position."
    },
    {
      text: "3. Which of the following should be AVOIDED in formal academic writing?",
      options: [
        "Evidence from peer-reviewed journals",
        "Contractions (e.g., don't, it's, can't)",
        "Logical transitions between paragraphs",
        "Objective tone"
      ],
      correct: 1,
      explanation: "Contractions are informal; academic writing uses full forms (do not, it is, cannot)."
    },
    {
      text: "4. What is plagiarism?",
      options: [
        "Using someone else’s work without proper acknowledgment.",
        "Paraphrasing with citation.",
        "Adding too many references.",
        "Using direct quotes within quotation marks."
      ],
      correct: 0,
      explanation: "Plagiarism is presenting others' ideas or words as your own without credit."
    },
    {
      text: "5. Which citation style is commonly used in Tanzanian universities for social sciences?",
      options: [
        "MLA 8th edition",
        "Chicago author-date",
        "APA 7th edition",
        "Harvard referencing"
      ],
      correct: 2,
      explanation: "APA 7th edition is widely adopted by Tanzanian universities (UDSM, SUA, etc.) for social sciences."
    },
    {
      text: "6. Which of the following is a characteristic of academic writing tone?",
      options: [
        "Emotional and sensational language",
        "Use of slang and colloquialisms",
        "Impersonal and objective language",
        "Frequent use of rhetorical questions"
      ],
      correct: 2,
      explanation: "Academic writing is objective, avoids personal bias, and remains formal."
    },
    {
      text: "7. What does IMRAD structure stand for?",
      options: [
        "Introduction, Methods, Results, and Discussion",
        "Index, Main text, References, Appendix, Data",
        "Idea, Methodology, Review, Analysis, Draft",
        "Introduction, Meaning, Research, Abstract, Document"
      ],
      correct: 0,
      explanation: "IMRAD is standard for scientific papers: Introduction, Methods, Results, and Discussion."
    },
    {
      text: "8. Which of the following sentences sounds MOST appropriate for academic writing?",
      options: [
        "The experiment totally failed, and that's pretty bad.",
        "The results indicate a significant deviation from the hypothesized values.",
        "We think the data looks kinda weird.",
        "You can see the table is not matching up."
      ],
      correct: 1,
      explanation: "Academic sentences use precise, formal vocabulary and avoid colloquialisms."
    },
    {
      text: "9. Why is referencing important in academic writing?",
      options: [
        "To increase page length of the essay.",
        "To avoid plagiarism and give credit to original authors.",
        "To make the essay look sophisticated.",
        "To replace the need for original analysis."
      ],
      correct: 1,
      explanation: "Referencing acknowledges sources, supports arguments, and prevents plagiarism."
    },
    {
      text: "10. In an academic essay conclusion, what should you do?",
      options: [
        "Introduce new evidence or fresh argument.",
        "Restate the thesis and summarize main points without introducing new ideas.",
        "Write a personal story about the topic.",
        "Add random quotes from famous people."
      ],
      correct: 1,
      explanation: "Conclusion synthesizes main arguments and restates thesis; no new information."
    }
  ];

  let userAnswers = new Array(questionsData.length).fill(null);
  let quizSubmitted = false;

  function renderQuestions() {
    const container = document.getElementById("questionsList");
    if (!container) return;
    let html = '';
    questionsData.forEach((q, idx) => {
      const selectedVal = userAnswers[idx] !== null ? userAnswers[idx] : '';
      html += `
        <div class="quiz-question" data-qidx="${idx}">
          <div class="question-text">${q.text}</div>
          <div class="options" id="options-${idx}">
      `;
      q.options.forEach((opt, optIdx) => {
        const isChecked = (selectedVal === optIdx.toString());
        html += `
          <label class="option">
            <input type="radio" name="q${idx}" value="${optIdx}" ${isChecked ? 'checked' : ''} data-qidx="${idx}" data-optidx="${optIdx}">
            <span>${String.fromCharCode(65+optIdx)}. ${opt}</span>
          </label>
        `;
      });
      html += `</div><div class="explanation-area" id="exp-${idx}" style="margin-top:8px;"></div></div>`;
    });
    container.innerHTML = html;

    // attach event listeners for radio buttons after render
    for (let i = 0; i < questionsData.length; i++) {
      const radios = document.querySelectorAll(`input[name="q${i}"]`);
      radios.forEach(radio => {
        radio.addEventListener('change', (e) => {
          if (quizSubmitted) {
            // if quiz already submitted, we allow reset but better behavior: show message?
            // we can just allow change, but then need to clear submitted flag? for usability, allow re-submit if change.
            quizSubmitted = false;
            document.getElementById("submitQuiz").innerText = "✅ Submit Answers";
            document.getElementById("globalFeedback").innerHTML = "";
            // update score display to placeholder
            document.getElementById("scoreDisplay").innerHTML = `Score: -- / 10`;
            // clear all explanation boxes
            for(let j=0;j<questionsData.length;j++){
              const expDiv = document.getElementById(`exp-${j}`);
              if(expDiv) expDiv.innerHTML = '';
            }
          }
          const selectedValue = parseInt(e.target.value);
          userAnswers[i] = selectedValue;
        });
      });
    }
  }

  function computeScoreAndShowExplanations() {
    let correctCount = 0;
    for (let i = 0; i < questionsData.length; i++) {
      const userChoice = userAnswers[i];
      const isCorrect = (userChoice === questionsData[i].correct);
      if (isCorrect) correctCount++;
      // show explanation for each question
      const expDiv = document.getElementById(`exp-${i}`);
      if (expDiv) {
        if (userChoice === null) {
          expDiv.innerHTML = `<span class="explanation" style="background:#ffe6e6; color:#9b2c2c;">⚠️ Not answered. Correct answer: ${String.fromCharCode(65+questionsData[i].correct)}. ${questionsData[i].explanation}</span>`;
        } else if (isCorrect) {
          expDiv.innerHTML = `<span class="explanation" style="background:#e0f2df;">✅ Correct! ${questionsData[i].explanation}</span>`;
        } else {
          expDiv.innerHTML = `<span class="explanation" style="background:#ffefef;">❌ Incorrect. Correct answer: ${String.fromCharCode(65+questionsData[i].correct)}. ${questionsData[i].explanation}</span>`;
        }
      }
    }
    return correctCount;
  }

  function updateScoreUI(correctCount) {
    const scoreSpan = document.getElementById("scoreDisplay");
    if (scoreSpan) {
      scoreSpan.innerHTML = `Score: ${correctCount} / ${questionsData.length}`;
    }
    const globalDiv = document.getElementById("globalFeedback");
    if (correctCount === questionsData.length) {
      globalDiv.innerHTML = `<div style="background:#c8e6d9; padding:12px; border-radius:32px;">🎉 Excellent! You've mastered academic writing principles — well done! 🎉</div>`;
    } else if (correctCount >= 7) {
      globalDiv.innerHTML = `<div style="background:#fff3cf; padding:12px; border-radius:32px;">👍 Good effort! Review the areas you missed to strengthen your academic writing skills.</div>`;
    } else {
      globalDiv.innerHTML = `<div style="background:#ffdede; padding:12px; border-radius:32px;">📚 Keep learning! Revisit the 'what to consider' section and try the quiz again.</div>`;
    }
  }

  function submitQuizHandler() {
    // check unanswered
    let allAnswered = true;
    for (let i = 0; i < questionsData.length; i++) {
      if (userAnswers[i] === null) {
        allAnswered = false;
        break;
      }
    }
    if (!allAnswered) {
      // but we still show score, but highlight missing ones
      // we will compute score only for answered? Better compute and show as partial.
      // But to encourage: we'll still grade but display missing as wrong.
    }
    const correctCount = computeScoreAndShowExplanations();
    updateScoreUI(correctCount);
    quizSubmitted = true;
    const submitBtn = document.getElementById("submitQuiz");
    if (submitBtn) submitBtn.innerText = "✅ Submitted";
    // disable further changes? Not necessary but we can keep radois functional but after re-submit it resets flag if user changes, we already handle in change event.
  }

  function resetQuizHandler() {
    userAnswers.fill(null);
    quizSubmitted = false;
    // reset radio selections
    for (let i = 0; i < questionsData.length; i++) {
      const radios = document.querySelectorAll(`input[name="q${i}"]`);
      radios.forEach(radio => radio.checked = false);
      const expDiv = document.getElementById(`exp-${i}`);
      if (expDiv) expDiv.innerHTML = '';
    }
    const scoreSpan = document.getElementById("scoreDisplay");
    if (scoreSpan) scoreSpan.innerHTML = `Score: -- / 10`;
    const globalDiv = document.getElementById("globalFeedback");
    if (globalDiv) globalDiv.innerHTML = '';
    const submitBtn = document.getElementById("submitQuiz");
    if (submitBtn) submitBtn.innerText = "✅ Submit Answers";
  }

  // initial render and attach event handlers
  renderQuestions();

  const submitBtn = document.getElementById("submitQuiz");
  const resetBtn = document.getElementById("resetQuiz");
  if (submitBtn) submitBtn.addEventListener("click", submitQuizHandler);
  if (resetBtn) resetBtn.addEventListener("click", resetQuizHandler);
  
  // manual fix for dynamic radio state if user hasn't answered but later clicks reset, etc.
  window.addEventListener("load", () => {
    // ensure existing user answers mapping sync
    for (let i = 0; i < questionsData.length; i++) {
      const radios = document.querySelectorAll(`input[name="q${i}"]`);
      radios.forEach(radio => {
        radio.addEventListener('change', (e) => {
          if (quizSubmitted) {
            quizSubmitted = false;
            document.getElementById("submitQuiz").innerText = "✅ Submit Answers";
            document.getElementById("globalFeedback").innerHTML = "";
            document.getElementById("scoreDisplay").innerHTML = `Score: -- / 10`;
            for(let j=0;j<questionsData.length;j++){
              const expDiv = document.getElementById(`exp-${j}`);
              if(expDiv) expDiv.innerHTML = '';
            }
          }
          const idx = parseInt(radio.getAttribute('data-qidx') || i);
          const optVal = parseInt(radio.value);
          userAnswers[idx] = optVal;
        });
      });
    }
  });
</script>
</body>
</html>
