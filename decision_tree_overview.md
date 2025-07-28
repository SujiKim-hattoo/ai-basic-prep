## 1. What is a Decision Tree (DT) 결정트리란 무엇인가?

A  **non-parametric supervised learning method 비모수 지도 학습 알고리즘**.
-> A method for both classification and regression analysis

* **Goal:** simple data features --predict--> the value of a trget variable (e.g., determining if an animal in a photo is a cat or not).
* **Structure:** Hierarchical, tree-like structure similar to a flowchart, consisting of:

  * **Root Node:** Starting point of the decision process
  * **Internal Nodes:** Decision points within the tree
  * **Leaf Nodes:** Represent all possible outcomes
  * **Branches:** Connections between nodes, representing decisions or conditions
* **Depth:** Tree depth ∝ complexity of the model
* **Principle:** Uses a "divide and conquer" approach from top-down

## 2. Traits of Decision Trees 결정트리의 특성

### 2.1 Pros 장점

* **Simplicity & Interpretability:** Its intuitive, flowchart-like structure makes the decision-making process easy to understand and explain.
* **Data Flexibility:** It effectively handles both numerical and categorical data, requiring minimal preparation like scaling or normalization.
* **Non-parametric Nature:** Making no strong assumptions about data distribution, it can capture complex, non-linear relationships.

### 2.2 Cons 단점

* **Overfitting:** They tend to create overly complex trees that fit training data too closely, leading to poor generalization on unseen data.
* **High Variance:** Highly sensitive to minor data changes, a small alteration can significantly change the tree structure and impact predictions.
* **Poor Extrapolation:** Not well-suited for predictions beyond training data range; their step-wise nature hinders effective extrapolation to new values.

## 3. Summary 한줄요약

* Decision Trees are *intuitive and interpretable* methods suitable for various tasks, though they require careful handling to avoid issues like *overfitting and instability*.
---

## Reference 참고 자료

* IBM [Decision Trees](https://www.ibm.com/think/topics/decision-trees)
* scikit-learn [Decision Tree](https://scikit-learn.org/stable/modules/tree.html)
* Wikipedia [Decision Tree](https://en.wikipedia.org/wiki/Decision_tree)
