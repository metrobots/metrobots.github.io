<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Driver Benchmarking</title>

  <link rel="apple-touch-icon" sizes="180x180" href="https://metrobots.github.io/assets/favicon/apple-touch-icon.png">
  <link rel="icon" type="image/png" sizes="32x32" href="https://metrobots.github.io/assets/favicon/favicon-32x32.png">
  <link rel="icon" type="image/png" sizes="16x16" href="https://metrobots.github.io/assets/favicon/favicon-16x16.png">
  <link rel="manifest" href="https://metrobots.github.io/assets/favicon/site.webmanifest">
  <link rel="mask-icon" href="https://metrobots.github.io/assets/favicon/safari-pinned-tab.svg" color="#5bbad5">
  <meta name="msapplication-TileColor" content="#333333">
  <meta name="theme-color" content="#ffffff">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
    }

    body {
      background-color: #f9f9f9;
    }

    .header {
      background: #0f1955;
      padding: 1rem;
      color: white;
    }

    .header-content {
      max-width: 960px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 1.5rem;
      font-weight: bold;
      cursor: pointer;
    }

    .back-button {
      color: white;
      text-decoration: none;
      padding: 0.5rem 1rem;
      border-radius: 3px;
      background: rgba(255, 255, 255, 0.1);
      display: none;
    }

    .container {
      max-width: 960px;
      margin: 2rem auto;
      padding: 0 1rem;
    }

    .tests-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
      gap: 1rem;
    }

    .test-card {
      background: white;
      border-radius: 4px;
      padding: 2rem;
      text-align: center;
      cursor: pointer;
      box-shadow: 0 1px 3px rgba(0, 0, 0, 0.12);
      transition: box-shadow 0.2s;
    }

    .test-card:hover {
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.15);
    }

    .test-icon {
      width: 48px;
      height: 48px;
      margin: 0 auto 1rem;
    }

    .test-title {
      font-size: 1.25rem;
      margin-bottom: 0.5rem;
      color: #333;
    }

    .test-description {
      color: #666;
      font-size: 0.9rem;
    }

    .test-stats {
      margin-top: 1rem;
      padding-top: 1rem;
      border-top: 1px solid #eee;
      font-size: 0.9rem;
      color: #666;
    }

    .game-container {
      display: none;
      width: 100%;
      height: 400px;
      background: white;
      margin-top: 2rem;
      position: relative;
      cursor: pointer;
    }

    .reaction-screen {
      width: 100%;
      height: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
      color: white;
      font-size: 1.5rem;
      transition: background-color 0.1s;
    }

    .waiting {
      background-color: #2b87d1;
    }

    .ready {
      background-color: #ce1f1f;
    }

    .go {
      background-color: #3fca5f;
    }

    .result {
      background-color: white;
      color: #333;
    }

    .target {
      position: absolute;
      width: 25px;
      height: 25px;
      background: #2b87d1;
      border-radius: 50%;
      transform: translate(-50%, -50%);
      cursor: pointer;
    }

    .sequence-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 10px;
      max-width: 400px;
      margin: 2rem auto;
    }

    .sequence-square {
      aspect-ratio: 1;
      background: #e0e0e0;
      border-radius: 4px;
      cursor: pointer;
      transition: background-color 0.2s;
      border: 2px solid #0f1955;
    }

    .sequence-square.active {
      background: #2b87d1;
    }

    .sequence-info {
      text-align: center;
      margin-bottom: 1rem;
      color: #333;
    }

    .attempts-exceeded {
      display: flex;
      height: 100%;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      text-align: center;
      padding: 2rem;
    }

    .best-score {
      font-size: 2rem;
      margin: 1rem 0;
      color: #2b87d1;
    }

    .modal-backdrop {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0, 0, 0, 0.5);
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 1000;
    }

    .modal {
      background: white;
      border-radius: 8px;
      padding: 2rem;
      max-width: 90%;
      width: 400px; 
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
      animation: modalSlideIn 0.3s ease-out;
    }

    @keyframes modalSlideIn {
      from {
        transform: translateY(-20px);
        opacity: 0;
      }

      to {
        transform: translateY(0);
        opacity: 1;
      }
    }

    .modal-title {
      font-size: 1.5rem;
      font-weight: bold;
      margin-bottom: 1rem;
      color: #2b87d1;
    }

    .modal-content {
      margin-bottom: 1.5rem;
      line-height: 1.5;
      color: #444;
    }

    .modal-buttons {
      display: flex;
      justify-content: flex-end;
      gap: 1rem;
    }

    .modal-button {
      padding: 0.5rem 1rem;
      border-radius: 4px;
      border: none;
      cursor: pointer;
      font-size: 0.9rem;
      transition: all 0.2s;
    }

    .modal-button.primary {
      background: #0f1955;
      color: white;
    }

    .modal-button.primary:hover {
      background: #355C8D;
    }

    .modal-button.secondary {
      background: #e0e0e0;
      color: #333;
    }

    .modal-button.secondary:hover {
      background: #d0d0d0;
    }

    .export-form {
      margin: 1rem 0;
    }

    .form-group {
      margin-bottom: 1rem;
    }

    .form-label {
      display: block;
      margin-bottom: 0.5rem;
      color: #444;
      font-weight: 500;
    }

    .form-input {
      width: 100%;
      padding: 0.5rem;
      border: 1px solid #ddd;
      border-radius: 4px;
      font-size: 0.9rem;
    }

    .form-select {
      width: 100%;
      padding: 0.5rem;
      border: 1px solid #ddd;
      border-radius: 4px;
      font-size: 0.9rem;
      background: white;
    }

    .export-button {
      color: white;
      text-decoration: none;
      padding: 0.5rem 1rem;
      border-radius: 3px;
      background: rgba(255, 255, 255, 0.1);
      cursor: pointer;
      margin-left: 1rem;
    }
  </style>
</head>

<body>
  <header class="header">
    <div class="header-content">
      <div class="logo" onclick="showHome()">Driver Benchmarking</div>
      <div>
        <a href="#" class="back-button" onclick="showHome()">← Tests</a>
        <span class="export-button" onclick="showExportModal()">Export Scores</span>
      </div>
    </div>
  </header>

  <div class="container">
    <div class="tests-grid" id="testsGrid"></div>
    <div id="gameContainer" class="game-container"></div>
  </div>

  <script>
    const USER_KEY = 'hb_user_id';
    const SCORES_KEY = 'hb_scores';
    const ATTEMPTS_KEY = 'hb_attempts';
    let gameState = {
      currentTest: null,
      reactionState: 'waiting',
      reactionTimeout: null,
      reactionStartTime: null,
      aimTargets: 0,
      aimStartTime: null,
      sequence: [],
      userSequence: [],
      sequenceLevel: 3,
      showingSequence: false
    };

    function initializeUser() {
      if (!localStorage.getItem(USER_KEY)) {
        localStorage.setItem(USER_KEY, crypto.randomUUID());
      }
      if (!localStorage.getItem(SCORES_KEY)) {
        localStorage.setItem(SCORES_KEY, JSON.stringify({
          reaction: [],
          aim: [],
          sequence: []
        }));
      }
      if (!localStorage.getItem(ATTEMPTS_KEY)) {
        localStorage.setItem(ATTEMPTS_KEY, JSON.stringify({
          reaction: 0,
          aim: 0,
          sequence: 0
        }));
      }
    }

    function getAttempts(test) {
      const attempts = JSON.parse(localStorage.getItem(ATTEMPTS_KEY));
      return attempts[test];
    }

    function incrementAttempts(test) {
      const attempts = JSON.parse(localStorage.getItem(ATTEMPTS_KEY));
      attempts[test]++;
      localStorage.setItem(ATTEMPTS_KEY, JSON.stringify(attempts));
    }

    function saveScore(test, score) {
      const scores = JSON.parse(localStorage.getItem(SCORES_KEY));
      scores[test].push(score);
      localStorage.setItem(SCORES_KEY, JSON.stringify(scores));
    }

    function getBestScore(test) {
      const scores = JSON.parse(localStorage.getItem(SCORES_KEY));
      if (scores[test].length === 0) return null;
      if (test === 'reaction' || test === 'aim') {
        return Math.min(...scores[test]);
      }
      return Math.max(...scores[test]);
    }

    function showAttemptExceeded(test) {
      const bestScore = getBestScore(test);
      const container = document.getElementById('gameContainer');
      let scoreDisplay = '';
      if (bestScore !== null) {
        switch (test) {
          case 'reaction':
            scoreDisplay = `${bestScore}ms`;
            break;
          case 'aim':
            scoreDisplay = `${bestScore.toFixed(2)}s`;
            break;
          case 'sequence':
            scoreDisplay = `Level ${bestScore}`;
            break;
        }
      }
      container.innerHTML = `
                <div class="attempts-exceeded">
                    <h2>Maximum attempts reached</h2>
                    ${bestScore !== null ? `
                        <p>Your best score:</p>
                        <div class="best-score">${scoreDisplay}</div>
                    ` : ''}
                    <p>Each test can only be taken twice per user</p>
                </div>
            `;
    }

    function updateTestsGrid() {
      const testsGrid = document.getElementById('testsGrid');
      testsGrid.innerHTML = `
                <div class="test-card" onclick="startReactionTest()">
                    <svg class="test-icon" viewBox="0 0 24 24" fill="none" stroke="#0f1955" stroke-width="2">
                        <circle cx="12" cy="12" r="10"/>
                        <polyline points="12 6 12 12 16 14"/>
                    </svg>
                    <h2 class="test-title">Reaction Time</h2>
                    <p class="test-description">Test your reaction speed</p>
                    <div class="test-stats">
                        Attempts: ${getAttempts('reaction')}/2
                        ${getBestScore('reaction') ? `<br>Best: ${getBestScore('reaction')}ms` : ''}
                    </div>
                </div>

                <div class="test-card" onclick="startAimTest()">
                    <svg class="test-icon" viewBox="0 0 24 24" fill="none" stroke="#0f1955" stroke-width="2">
                        <circle cx="12" cy="12" r="10"/>
                        <circle cx="12" cy="12" r="3"/>
                    </svg>
                    <h2 class="test-title">Aim Trainer</h2>
                    <p class="test-description">Test your aim accuracy</p>
                    <div class="test-stats">
                        Attempts: ${getAttempts('aim')}/2
                        ${getBestScore('aim') ? `<br>Best: ${getBestScore('aim').toFixed(2)}s` : ''}
                    </div>
                </div>

                <div class="test-card" onclick="startSequenceTest()">
                    <svg class="test-icon" viewBox="0 0 24 24" fill="none" stroke="#0f1955" stroke-width="2">
                        <path d="M12 3v18M3 12h18"/>
                    </svg>
                    <h2 class="test-title">Sequence Memory</h2>
                    <p class="test-description">Test your memory</p>
                    <div class="test-stats">
                        Attempts: ${getAttempts('sequence')}/2
                        ${getBestScore('sequence') ? `<br>Best: Level ${getBestScore('sequence')}` : ''}
                    </div>
                </div>
            `;
    }

    function showHome() {
      document.getElementById('testsGrid').style.display = 'grid';
      document.getElementById('gameContainer').style.display = 'none';
      document.querySelector('.back-button').style.display = 'none';
      gameState.currentTest = null;
      updateTestsGrid();
    }

    function showGame() {
      document.getElementById('testsGrid').style.display = 'none';
      document.getElementById('gameContainer').style.display = 'block';
      document.querySelector('.back-button').style.display = 'block';
    }

    function startReactionTest() {
      if (getAttempts('reaction') >= 2) {
        showGame();
        showAttemptExceeded('reaction');
        return;
      }
      incrementAttempts('reaction');
      showGame();
      gameState.currentTest = 'reaction';
      const container = document.getElementById('gameContainer');
      container.innerHTML = `
                <div class="reaction-screen waiting">
                    Click to start
                </div>
            `;
      container.onclick = handleReactionClick;
    }

    function handleReactionClick() {
      const screen = document.querySelector('.reaction-screen');
      if (gameState.reactionState === 'waiting') {
        gameState.reactionState = 'ready';
        screen.className = 'reaction-screen ready';
        screen.textContent = 'Wait for green...';
        const delay = 2000 + Math.random() * 5000;
        gameState.reactionTimeout = setTimeout(() => {
          gameState.reactionState = 'go';
          gameState.reactionStartTime = Date.now();
          screen.className = 'reaction-screen go';
          screen.textContent = 'Click!';
        }, delay);
      } else if (gameState.reactionState === 'ready') {
        clearTimeout(gameState.reactionTimeout);
        gameState.reactionState = 'waiting';
        screen.className = 'reaction-screen result';
        screen.innerHTML = `
                    <div>Too soon!</div>
                    <div style="font-size: 1rem; margin-top: 1rem;">Click to try again</div>
                `;
      } else if (gameState.reactionState === 'go') {
        const reactionTime = Date.now() - gameState.reactionStartTime;
        saveScore('reaction', reactionTime);
        gameState.reactionState = 'waiting';
        screen.className = 'reaction-screen result';
        screen.innerHTML = `
                    <div>${reactionTime}ms</div>
                    <div style="font-size: 1rem; margin-top: 1rem;">Click to try again</div>
                `;
        showHome();
      }
    }

    function startAimTest() {
      if (getAttempts('aim') >= 2) {
        showGame();
        showAttemptExceeded('aim');
        return;
      }
      incrementAttempts('aim');
      showGame();
      gameState.currentTest = 'aim';
      gameState.aimTargets = 0;
      gameState.aimStartTime = Date.now();
      const container = document.getElementById('gameContainer');
      container.innerHTML = `
                <div style="position: absolute; top: 1rem; left: 1rem;">
                    Targets: <span id="targetCount">0</span>/30
                </div>
            `;
      spawnTarget();
    }

    function spawnTarget() {
      const container = document.getElementById('gameContainer');
      const target = document.createElement('div');
      target.className = 'target';
      const x = Math.random() * (container.offsetWidth - 50) + 25;
      const y = Math.random() * (container.offsetHeight - 50) + 25;
      target.style.left = x + 'px';
      target.style.top = y + 'px';
      target.onclick = () => {
        gameState.aimTargets++;
        document.getElementById('targetCount').textContent = gameState.aimTargets;
        if (gameState.aimTargets < 30) {
          target.remove();
          spawnTarget();
        } else {
          const timeTaken = (Date.now() - gameState.aimStartTime) / 1000;
          saveScore('aim', timeTaken);
          container.innerHTML = `
                        <div style="display: flex; height: 100%; align-items: center; justify-content: center; flex-direction: column;">
                            <div style="font-size: 1.5rem; margin-bottom: 1rem;">Complete!</div>
                            <div style="font-size: 1.25rem; margin-bottom: 1rem;">Time: ${timeTaken.toFixed(2)}s</div>
                            <button onclick="showHome()" style="padding: 0.5rem 1rem; background: #2b87d1; color: white; border: none; border-radius: 4px; cursor: pointer;">
                                Continue
                            </button>
                        </div>
                    `;
        }
      };
      container.appendChild(target);
    }

    function startSequenceTest() {
      if (getAttempts('sequence') >= 2) {
        showGame();
        showAttemptExceeded('sequence');
        return;
      }
      incrementAttempts('sequence');
      showGame();
      gameState.currentTest = 'sequence';
      gameState.sequence = [];
      gameState.userSequence = [];
      gameState.sequenceLevel = 3;
      const container = document.getElementById('gameContainer');
      container.innerHTML = `
                <div class="sequence-info">
                    Level: <span id="levelCount">1</span>
                </div>
                <div class="sequence-grid">
                    ${Array(9).fill(null).map((_, i) => `
                        <div class="sequence-square" data-index="${i}" onclick="handleSequenceClick(${i})"></div>
                    `).join('')}
                </div>
            `;
      startNewSequence();
    }

    function startNewSequence() {
      gameState.sequence = [];
      gameState.userSequence = [];
      for (let i = 0; i < gameState.sequenceLevel; i++) {
        gameState.sequence.push(Math.floor(Math.random() * 9));
      }
      showSequence();
    }

    function showSequence() {
      gameState.showingSequence = true;
      const squares = document.querySelectorAll('.sequence-square');
      gameState.sequence.forEach((number, index) => {
        setTimeout(() => {
          squares[number].classList.add('active');
          setTimeout(() => {
            squares[number].classList.remove('active');
            if (index === gameState.sequence.length - 1) {
              gameState.showingSequence = false;
            }
          }, 500);
        }, index * 1000);
      });
    }

    function handleSequenceClick(index) {
      if (gameState.showingSequence) return;
      const squares = document.querySelectorAll('.sequence-square');
      squares[index].classList.add('active');
      setTimeout(() => squares[index].classList.remove('active'), 300);
      gameState.userSequence.push(index);
      if (gameState.userSequence.length === gameState.sequence.length) {
        if (gameState.sequence.every((num, i) => num === gameState.userSequence[i])) {
          gameState.sequenceLevel++;
          document.getElementById('levelCount').textContent = gameState.sequenceLevel - 2;
          setTimeout(startNewSequence, 1000);
        } else {
          saveScore('sequence', gameState.sequenceLevel - 3);
          const container = document.getElementById('gameContainer');
          container.innerHTML = `
                        <div style="display: flex; height: 100%; align-items: center; justify-content: center; flex-direction: column;">
                            <div style="font-size: 1.5rem; margin-bottom: 1rem">Game Over!</div>
                            <div style="font-size: 1.25rem; margin-bottom: 1rem">Final Level: ${gameState.sequenceLevel - 2}</div>
                            <button onclick="showHome()" style="padding: 0.5rem 1rem; background: #2b87d1; color: white; border: none; border-radius: 4px; cursor: pointer;">
                                Continue
                            </button>
                        </div>
                    `;
        }
      }
    }

    
// Driver Benchmarking Start Popup

    
    function showWelcomePopup() {
      const modal = document.createElement('div');
      modal.className = 'modal-backdrop';
      modal.innerHTML = `
                <div class="modal">
    <h2 class="modal-title">Welcome to Driver Benchmarking</h2>
    <div class="modal-content">
        <p>Test your skills and prepare for the field with these key driver challenges:</p>
        <br>
        <p>🎯 <strong>Reaction Time:</strong> Measure your ability to quickly respond to field events</p>
        <p>🎮 <strong>Fine Motor Control:</strong> Test your joystick control and accuracy in simulation</p>
        <p>🧠 <strong>Sequence Memory:</strong> Evaluate your ability to remember in dynamic scenarios</p>
        <br>
        <p>You only get two attempts per challenge, so make them count! To submit your scores, use the export button, and email the file to <a href="mailto:team3324metrobots@gmail.com">team3324metrobots@gmail.com!</a></p>
    </div> 
    <div class="modal-buttons">
        <button class="modal-button primary" onclick="closeModal(this)">Let's Begin</button> 
    </div>
</div> 

            `;
      document.body.appendChild(modal);
    }

    function showExportModal() {
      const scores = JSON.parse(localStorage.getItem(SCORES_KEY));
      const modal = document.createElement('div');
      modal.className = 'modal-backdrop';
      modal.innerHTML = `
                <div class="modal">
                    <h2 class="modal-title">Export Your Scores</h2>
                    <div class="modal-content">
                        <form class="export-form" onsubmit="handleExport(event)">
                            <div class="form-group">
                                <label class="form-label" for="playerName">Your Name</label>
                                <input class="form-input" type="text" id="playerName" required>
                            </div>
                            <div class="form-group">
                                <label class="form-label" for="scoreType">Select Score</label>
                                <select class="form-select" id="scoreType" required>
                                    <option value="">Choose a score to export...</option>
                                    ${scores.reaction.length > 0 ? 
                                        `<option value="reaction">Reaction Time: ${Math.min(...scores.reaction)}ms</option>` : ''}
                                    ${scores.aim.length > 0 ? 
                                        `<option value="aim">Aim Trainer: ${Math.min(...scores.aim).toFixed(2)}s</option>` : ''}
                                    ${scores.sequence.length > 0 ? 
                                        `<option value="sequence">Sequence Memory: Level ${Math.max(...scores.sequence)}</option>` : ''}
                                </select>
                            </div>
                            <div class="modal-buttons">
                                <button type="button" class="modal-button secondary" onclick="closeModal(this)">Cancel</button>
                                <button type="submit" class="modal-button primary">Export</button>
                            </div>
                        </form>
                    </div>
                </div>
            `;
      document.body.appendChild(modal);
    }

    function calculateOverallScore(scores) {
      let overallScore = 0;
      let testsCompleted = 0;
      // Reaction Time Score (lower is better)
      // Typical human reaction time ranges from 150ms to 600ms
      // Score from 0-33.33
      if (scores.reaction && scores.reaction.length > 0) {
        const bestReaction = Math.min(...scores.reaction);
        // Convert to 0-33.33 scale (150ms = 33.33, 300ms = 0)
        const reactionScore = Math.max(0, Math.min(33.33, ((600 - bestReaction) / (600 - 150)) * 33.33));
        overallScore += reactionScore;
        testsCompleted++;
      }
      // Aim Test Score (lower is better)
      // Good times range from 10s to 40s for 30 targets
      // Score from 0-33.33
      if (scores.aim && scores.aim.length > 0) {
        const bestAim = Math.min(...scores.aim);
        // Convert to 0-33.33 scale (10s = 33.33, 30s = 0)
        const aimScore = Math.max(0, Math.min(33.33, ((40 - bestAim) / (40 - 10)) * 33.33));
        overallScore += aimScore;
        testsCompleted++;
      }
      // Sequence Memory Score (higher is better)
      // Typical scores range from 1 to 20 levels
      // Score from 0-33.34
      if (scores.sequence && scores.sequence.length > 0) {
        const bestSequence = Math.max(...scores.sequence);
        // Convert to 0-33.34 scale (3 = 0, 20 = 33.34)
        const sequenceScore = Math.max(0, Math.min(33.34, ((bestSequence - 1) / (20 - 1)) * 33.34));
        overallScore += sequenceScore;
        testsCompleted++;
      }
      // If no tests were completed, return 0
      if (testsCompleted === 0) return 0;
      // Normalize score based on number of tests completed
      return Math.round((overallScore / testsCompleted) * 3);
    }

    function handleExport(event) {
      event.preventDefault();
      const name = document.getElementById('playerName').value;
      const scores = JSON.parse(localStorage.getItem(SCORES_KEY));
      const overallScore = calculateOverallScore(scores);
      let scoreText = `Name: ${name}\n\n`;
      scoreText += `Overall Score: ${overallScore}/100\n\n`;
      scoreText += "Individual Scores:\n";
      if (scores.reaction && scores.reaction.length > 0) {
        scoreText += `Reaction time: ${Math.min(...scores.reaction)}ms\n`;
      }
      if (scores.aim && scores.aim.length > 0) {
        scoreText += `Aim trainer: ${Math.min(...scores.aim).toFixed(2)}s\n`;
      }
      if (scores.sequence && scores.sequence.length > 0) {
        scoreText += `Sequence memory: Level ${Math.max(...scores.sequence)}\n`;
      }
      const blob = new Blob([scoreText], {
        type: 'text/plain'
      });
      const url = URL.createObjectURL(blob);
      const a = document.createElement('a');
      a.href = url;
      a.download = `${name}-scores.txt`;
      document.body.appendChild(a);
      a.click();
      document.body.removeChild(a);
      URL.revokeObjectURL(url);
      closeModal(event.target);
    }

    function closeModal(element) {
      const modal = element.closest('.modal-backdrop');
      modal.remove();
    }
    initializeUser();
    showHome();
    showWelcomePopup();
  </script>
</body>

</html>
