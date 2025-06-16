# M.C.Q.-TEST-SERIES
NEET
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>MCQ Test</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
    }
    .question {
      margin-bottom: 20px;
    }
    .question h3 {
      margin-bottom: 10px;
    }
    button {
      padding: 10px 20px;
      font-size: 16px;
    }
    #result {
      margin-top: 20px;
      font-weight: bold;
      font-size: 18px;
    }
  </style>
</head>
<body>

  <h1>MCQ Test</h1>
  <form id="quizForm">
    
    <div class="question">
      <h3>1. What is the capital of France?</h3>
      <label><input type="radio" name="q1" value="A"> A. Berlin</label><br>
      <label><input type="radio" name="q1" value="B"> B. Madrid</label><br>
      <label><input type="radio" name="q1" value="C"> C. Paris</label><br>
      <label><input type="radio" name="q1" value="D"> D. Rome</label>
    </div>

    <div class="question">
      <h3>2. Which planet is known as the Red Planet?</h3>
      <label><input type="radio" name="q2" value="A"> A. Earth</label><br>
      <label><input type="radio" name="q2" value="B"> B. Venus</label><br>
      <label><input type="radio" name="q2" value="C"> C. Mars</label><br>
      <label><input type="radio" name="q2" value="D"> D. Jupiter</label>
    </div>

    <div class="question">
      <h3>3. Who wrote 'Romeo and Juliet'?</h3>
      <label><input type="radio" name="q3" value="A"> A. Mark Twain</label><br>
      <label><input type="radio" name="q3" value="B"> B. William Shakespeare</label><br>
      <label><input type="radio" name="q3" value="C"> C. Charles Dickens</label><br>
      <label><input type="radio" name="q3" value="D"> D. Jane Austen</label>
    </div>

    <button type="button" onclick="submitQuiz()">Submit</button>
  </form>

  <div id="result"></div>

  <script>
    function submitQuiz() {
      const answers = {
        q1: 'C',
        q2: 'C',
        q3: 'B'
      };
      
      let score = 0;
      let total = Object.keys(answers).length;
      
      for (let q in answers) {
        let selected = document.querySelector(`input[name="${q}"]:checked`);
        if (selected && selected.value === answers[q]) {
          score++;
        }
      }

      document.getElementById('result').innerText =
        `You scored ${score} out of ${total}`;
    }
  </script>

</body>
</html>
