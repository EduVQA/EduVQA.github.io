# 📂 Dataset Annotation Format

The annotation files of **EduAIGVBench** are provided in CSV format.  
Each row corresponds to a single educational AI-generated video together with its associated prompt and human-annotated Mean Opinion Scores (MOS).

## 🔹 CSV Structure

Each row in the CSV file corresponds to a single video sample.  
The columns are organized in the following order:

| Column Index | Content |
|--------------|----------|
| Column 1 | Relative path to the video file |
| Column 2 | Text prompt used for video generation |
| Column 3 | MOS score for Overall Perceptual Quality |
| Column 4 | MOS score for Sentence-Level (Overall) Alignment |
| Column 5 | MOS score for Spatial Quality |
| Column 6 | MOS score for Temporal Quality |
| Column 7 onward | MOS score for Word-Level Alignment |

---

## 🔹 Example

```csv
CogVideo/Geometry/Analyze_compare_create_and_compose_shapes/1.mp4,A boy builds a car out of rectangular and circular blocks,3.6842105263157894,3.9473684210526314,3.5789473684210527,3.8947368421052633,5.0,4.947368421052632,4.105263157894737,4.882352941176471,3.8947368421052633,,,4.578947368421052,,3.8947368421052633,4.647058823529412
CogVideo/Number/Count_to_tell_the_number_of_objects/74.mp4,Four ducks quack and swim in a line down the stream,4.0,3.0526315789473686,4.0,4.315789473684211,1.2105263157894737,4.894736842105263,3.235294117647059,,4.578947368421052,,4.933333333333334,4.222222222222222,3.176470588235294,,4.7368421052631575
```

---

## 🔹 Quality Dimensions

### Overall Perceptual Quality
Reflects a holistic impression integrating spatial and temporal aspects.

### Sentence-Level (Overall) Alignment
Evaluates how well the overall visual semantics correspond to the intended meaning of the prompt.

### Spatial Quality
Evaluates frame-level fidelity through texture clarity, edge sharpness, and artifact absence.

### Temporal Quality
Assesses motion coherence across frames, considering smoothness and temporal stability.

### Word-Level Alignment
Examines whether individual keywords or visual entities specified in the prompt are accurately represented in the video.

---
