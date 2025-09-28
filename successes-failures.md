[Home](index.md) | [Classical](classical.md) | [Deep Learning](deep-learning.md) | [Datasets & Eval](datasets.md) | [Success/Failure](successes-failures.md) | [Challenges](challenges.md) | [Future](future.md) | [Bibliography](bibliography.md)

# Successes and Failures

## Where it works well
Traffic sign recognition systems achieve very high accuracy in controlled conditions.  
In good lighting, with clear and visible signs, most modern models perform extremely well.  

![Success Detection](assets/images/success-detection.png)  
*Figure: Successful detection example.*

## Common failure cases
However, there are still important failure cases.  
Small or distant signs can be hard to detect. Signs may also be missed when they are partially blocked, poorly lit, or damaged by fading and graffiti.  
These weaknesses highlight the gap between benchmark performance and real-world deployment, and show why continued research is needed.  

![Failure Detection](assets/images/failure-detection.png)  
*Figure: Example of a missed sign.*

<audio controls src="assets/audio/success-failure.mp3">Your browser does not support audio.</audio>

<hr>

## Interactive Quiz
<p><strong>Quiz:</strong> Why might this traffic sign have been missed by the detector?</p>
<img src="assets/images/quiz-stop.jpg" alt="Blurred STOP Sign" width="300">

<form id="quizForm">
  <label><input type="radio" name="q4" value="correct"> Occlusion or poor visibility</label><br>
  <label><input type="radio" name="q4" value="partial"> Model not trained on this class</label><br>
  <label><input type="radio" name="q4" value="both"> Both could be possible</label><br>
</form>

<p id="quizResult" style="font-weight:bold; margin-top:10px;"></p>

<script>
  const quizForm = document.getElementById("quizForm");
  const quizResult = document.getElementById("quizResult");

  quizForm.addEventListener("change", function(e) {
    const answer = e.target.value;
    if (answer === "correct") {
      quizResult.textContent = "✅ Correct! Blur and poor visibility are common reasons detectors fail.";
      quizResult.style.color = "green";
    } else if (answer === "both") {
      quizResult.textContent = "⚠️ Close — poor visibility is the main issue here, but dataset coverage can also matter.";
      quizResult.style.color = "orange";
    } else {
      quizResult.textContent = "❌ Not quite. This example mainly shows blur and visibility issues.";
      quizResult.style.color = "red";
    }
  });
</script>
