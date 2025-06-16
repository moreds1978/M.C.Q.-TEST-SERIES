<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MCQ Test Paper</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 800px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        h1 {
            text-align: center;
            color: #333;
        }
        .question {
            margin-bottom: 20px;
        }
        .question h3 {
            margin-bottom: 10px;
            color: #2c3e50;
        }
        .options label {
            display: block;
            margin: 5px 0;
            padding: 10px;
            background: #ecf0f1;
            border-radius: 5px;
            cursor: pointer;
        }
        .options input {
            margin-right: 10px;
        }
        #submit-btn {
            display: block;
            margin: 20px auto;
            padding: 10px 20px;
            background: #3498db;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        #submit-btn:hover {
            background: #2980b9;
        }
        #result {
            text-align: center;
            font-size: 18px;
            margin-top: 20px;
            display: none;
        }
        #timer {
            text-align: center;
            font-size: 20px;
            color: #e74c3c;
            margin-bottom: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>MCQ Test Paper</h1>
        <div id="timer">Time Left: 10:00</div>
        <form id="quiz-form">
            <!-- Question 1 -->
            <div class="question">
                <h3>1. What is the capital of France?</h3>
                <div class="options">
                    <label><input type="radio" name="q1" value="a"> a) Paris</label>
                    <label><input type="radio" name="q1" value="b"> b) London</label>
                    <label><input type="radio" name="q1" value="c"> c) Berlin</label>
                    <label><input type="radio" name="q1" value="d"> d) Madrid</label>
                </div>
            </div>
            <!-- Question 2 -->
            <div class="question">
                <h3>2. Which planet is known as the Red Planet?</h3>
                <div class="options">
                    <label><input type="radio" name="q2" value="a"> a) Jupiter</label>
                    <label><input type="radio" name="q2" value="b"> b) Mars</label>
                    <label><input type="radio" name="q2" value="c"> c) Venus</label>
                    <label><input type="radio" name="q2" value="d"> d) Mercury</label>
                </div>
            </div>
            <!-- Question 3 -->
            <div class="question">
                <h3>3. What is 2 + 2?</h3>
                <div class="options">
                    <label><input type="radio" name="q3" value="a"> a) 3</label>
                    <label><input type="radio" name="q3" value="b"> b) 4</label>
                    <label><input type="radio" name="q3" value="c"> c) 5</label>
                    <label><input type="radio" name="q3" value="d"> d) 6</label>
                </div>
            </div>
            <button type="button" id="submit-btn">Submit Test</button>
        </form>
        <div id="result"></div>
    </div>
   </script>
</body>
</html>
