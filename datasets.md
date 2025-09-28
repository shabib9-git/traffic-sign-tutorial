[Home](index.md) | [Classical](classical.md) | [Deep Learning](deep-learning.md) | [Datasets & Eval](datasets.md) | [Success/Failure](successes-failures.md) | [Challenges](challenges.md) | [Future](future.md) | [Bibliography](bibliography.md)

# Datasets & Evaluation Metrics

To train and evaluate traffic sign recognition systems, researchers rely on several benchmark datasets. Below are some of the most widely used:

**Common datasets**  
- **GTSRB** — German Traffic Sign Recognition Benchmark. The most widely used classification dataset (43 classes, ~50,000 images).  
- **BelgiumTSC** — Belgium Traffic Sign Classification. Includes 62 classes, smaller but diverse.  
- **TT100K** — A large-scale detection dataset with 221 classes and 100,000+ images, collected from Chinese road scenes.  
- **Mapillary Traffic Sign Dataset (MTSD)** — More recent, very large dataset with over 300 classes and varied conditions from multiple countries.  

## Example Dataset Images
![GTSRB Samples](assets/images/gtsrb-samples.jpg)  
*Figure: Examples from the GTSRB dataset.*

![Dataset Table](assets/images/datasets-table.png)  
*Figure: Overview of common traffic sign datasets.*

## Evaluation Metrics
Models are typically evaluated using metrics such as:  
- **Accuracy** for classification tasks  
- **Precision, Recall, and F1 score**  
- **mAP (mean Average Precision)** for detection tasks  

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
