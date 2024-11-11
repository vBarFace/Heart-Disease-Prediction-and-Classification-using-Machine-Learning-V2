# Heart Disease Prediction and Classification using Machine Learning

**Foundations of Artificial Intelligence**  
**Prof: Petia Georgieva(petia@ua.pt) & Eugénio Rocha(eugenio@ua.pt)**  
**Academic Year: 2021/22**

### Contributors
- **André Reis Fernandes**  
  - **Number**: 97977  
  - **Program**: Computational Engineering, Physics Department  
  - **Email**: [andre.fernandes16@ua.pt](mailto:andre.fernandes16@ua.pt)  
  - **Work Rate**: 50%

- **Gonçalo Jorge Loureiro de Freitas**  
  - **Number**: 98012  
  - **Program**: Computational Engineering, Physics Department  
  - **Email**: [goncalojfreitas@ua.pt](mailto:goncalojfreitas@ua.pt)  
  - **Work Rate**: 50%

---

## Abstract
This project aims to predict and classify heart disease using machine learning. We implemented various machine learning algorithms in both Python and RapidMiner software to assess predictive performance and determine the best model for heart disease classification based on a given dataset.

## Keywords
- Machine Learning
- Artificial Intelligence
- Hidden Markov Models (HMM)
- Bayesian Networks
- Kalman Filter
- Performance Metrics
- ROC and AUC
- Cost/Loss Functions

---

## Approach

To classify and predict heart disease, we utilized the following models:

1. **Logistic Regression** (Python)
2. **Support Vector Machine** (Python)
3. **Gaussian Naive Bayes** (Python)
4. **Decision Tree** (Python)
5. **K-Nearest Neighbor** (Python)
6. **Neural Networks** (RapidMiner)
7. **Hidden Markov Models (HMM)** (Python)
8. **Bayesian Networks** (Python)

### Hidden Markov Model (HMM)
HMMs are sequence models used to compute a sequence of outputs based on a sequence of inputs. In this project, we modelled HMM with two hidden states: **disease** and **no disease**. Observations were based on a sequence of 3 features: sex, ca, and thal, which were chosen for their predictive power. With 24 possible sequences, we calculated transition and emission probabilities to study the sequences leading to heart disease or the absence of it. 

The HMM analysis allowed us to predict disease probability based on specific sequences of features, revealing, for instance, that men are generally at higher risk, and certain combinations of ca and thal values influence the likelihood of heart disease.

### Bayesian Networks
Bayesian networks provide a probabilistic graphical model structure using directed acyclic graphs (DAGs) to show dependencies among variables. For this project:
- **First Implementation**: Used sex, ca, and thal as nodes, with edges connecting each feature to the condition. Performance metrics were derived to measure model accuracy.
- **Second Implementation**: Excluded certain features to study simplified networks, using user-defined inputs to determine disease probability and observe the deletion of branches in the network based on conditional dependencies.

While Bayesian Networks offer interpretability, their performance in this context was less robust, suggesting that other models may be more effective for this dataset.

### Kalman Filter (Conceptual Application)
Although not implemented in this project, the Kalman Filter could theoretically be used to predict changes in diagnostic status based on sequential feature observations, providing an iterative method to refine disease predictions over time.

---

## Acknowledgments

Special thanks to **Prof. Petia Georgieva** and **Prof. Eugénio Rocha** for guidance and support in the Foundations of Artificial Intelligence course.
