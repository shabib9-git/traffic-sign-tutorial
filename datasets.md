[Home](index.md) | [Classical](classical.md) | [Deep Learning](deep-learning.md) | [Datasets & Eval](datasets.md) | [Success/Failure](successes-failures.md) | [Challenges](challenges.md) | [Future](future.md) | [Bibliography](bibliography.md)


# Datasets & Evaluation Metrics

## Common datasets
- **GTSRB** — German Traffic Sign Recognition Benchmark (classification).
- **BelgiumTSC** — Belgium Traffic Sign Classification.
- **TT100K** — Large-scale traffic sign detection in the wild.
- (Optionally mention Mapillary Traffic Sign Dataset.)

![GTSRB Samples](assets/images/gtsrb-samples.jpg)

<hr>

<p><strong>Interactive Quiz:</strong> These signs come from which benchmark dataset?</p>
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


## Metrics
- **Accuracy** (classification), **Precision/Recall/F1**.
- **mAP** (mean Average Precision) for detection.

![Dataset Table](assets/images/datasets-table.png)  


**TODOs**
- Add a small table image or screenshot of sample classes.
- Audio note explaining metrics briefly.

<audio controls src="assets/audio/datasets.mp3">Your browser does not support audio.</audio>
