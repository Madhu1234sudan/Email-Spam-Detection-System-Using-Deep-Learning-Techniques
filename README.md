# Email Spam Detection System Using Deep Learning Techniques

This project implements an email spam detection system using machine learning techniques, including Naive Bayes and Active Learning with Random Forest. The system processes a dataset of emails, classifies them as spam or ham, and evaluates the performance of the models.

## Project Structure

## Features

- **Dataset Preprocessing**: Text data is vectorized using TF-IDF, and labels are mapped to binary values (`spam` = 1, `ham` = 0).
- **Naive Bayes Classifier**: A baseline model for spam detection.
- **Active Learning**: Implements manual uncertainty sampling with a Random Forest classifier to iteratively improve the model using a small labeled dataset.
- **Performance Evaluation**: Metrics such as accuracy, precision, and recall are calculated for both models.
- **Visualization**: A learning curve is plotted to show the improvement in accuracy during active learning.

## Usage

1. **Dataset**: Ensure the `spam.csv` file is in the project directory. The dataset should have two columns: `text` (email content) and `label` (`spam` or `ham`).

2. **Run the Notebook**: Open `active_learning.ipynb` in Jupyter Notebook or Visual Studio Code and execute the cells step by step.

3. **Results**:
   - Model performance metrics are saved in `model_performance.csv`.
   - The active learning curve is saved as `active_learning_curve.png`.

## Dependencies

Install the required Python libraries using:

```bash
pip install pandas numpy scikit-learn matplotlib
```
