[Home](index.md) | [Classical](classical.md) | [Deep Learning](deep-learning.md) | [Datasets & Eval](datasets.md) | [Success/Failure](successes-failures.md) | [Challenges](challenges.md) | [Future](future.md) | [Refs](bibliography.md)

# Datasets & Evaluation Metrics

## Common datasets
- **GTSRB** — German Traffic Sign Recognition Benchmark  
  - 43 classes, ~50k images  
  - Standard for classification  
- **BelgiumTSC** — Belgium Traffic Sign Classification  
  - 62 classes, smaller but diverse  
- **TT100K** — Tsinghua–Tencent 100K  
  - 221 classes, 100k+ images  
  - Large-scale detection dataset  
- **MTSD** — Mapillary Traffic Sign Dataset  
  - 300+ classes, multi-country, challenging conditions  

## Examples
![GTSRB Samples](assets/images/gtsrb-samples.jpg)  
*Figure: Examples from the GTSRB dataset.*

![Dataset Table](assets/images/datasets-table.png)  
*Figure: Overview of common traffic sign datasets.*

## Evaluation metrics
- **Accuracy** → for classification  
- **Precision, Recall, F1-score** → measure detection quality  
- **mAP (mean Average Precision)** → key metric for detection  

<audio controls src="assets/audio/datasets.mp3">Your browser does not support audio.</audio>

<hr>

## Interactive Quiz
<p><strong>Quiz:</strong> These signs come from which benchmark dataset?</p>
<img src="assets/images/gtsrb-samples.jpg" alt="Dataset Sample" width="300">

<form id="quizForm2">
  <label><input type="radio" name="q2" value="correct"> GTSRB</label><br>
  <label><input type="radio" name="q2" value="wrong"> COCO</label><br>
  <label><input type="radio" name="q2" value="wrong"> ImageNet</label><br>
</form>

<p id="quizResult2" style="font-weight:bold; margin-top:10px;"></p>

<script>
  const quizForm2 = document.getElementById("quizForm2");
  const quizResult2 = document.getElementById("quizResult2");

  quizForm2.addEventListener("change", function(e) {
    const answer = e.target.value;
    if (answer === "correct") {
      quizResult2.textContent = "✅ Correct! These are samples from the German Traffic Sign Recognition Benchmark (GTSRB).";
      quizResult2.style.color = "green";
    } else {
      quizResult2.textContent = "❌ Not quite. Hint: this dataset has 43 classes and is the standard for traffic signs.";
      quizResult2.style.color = "red";
    }
  });
</script>
