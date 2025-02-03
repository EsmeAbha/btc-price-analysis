# Bitcoin Price Prediction using Deep Learning

This project demonstrates how to predict Bitcoin's high price using a deep learning model. The dataset includes historical BTC data, such as Open, High, Low, Close, Adjusted Close, and Volume. The model is built using TensorFlow and Keras, with a focus on predicting the 'High' price based on the features extracted from the dataset.

## Steps Involved:
1. **Dataset Loading**: The dataset containing Bitcoin price data is loaded from a CSV file.
2. **Data Preprocessing**: 
    - The 'Date' column is split into separate Year, Month, and Day columns.
    - Features such as Year, Month, Day, Open, Low, Close, Adj Close, and Volume are selected to train the model.
3. **Data Splitting**: The dataset is divided into training and testing sets (80% for training and 20% for testing).
4. **Feature Scaling**: MinMaxScaler is used to normalize the features.
5. **Model Construction**: A deep learning model with multiple Dense layers and ReLU activation is built.
6. **Model Training**: The model is trained with early stopping to avoid overfitting. The model trains for up to 100 epochs.
7. **Model Evaluation**: The model's performance is evaluated on both the training and testing sets, and the loss values are printed to assess its accuracy.

## Requirements:
- Python 3.x
- Pandas
- NumPy
- Scikit-learn
- TensorFlow (Keras)

## Setup Instructions:
1. Clone the repository:
    ```bash
    git clone <repository_url>
    cd <repository_name>
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Ensure that the `BTC-USD.csv` file is available at the specified path (`/content/drive/MyDrive/bitcoin/BTC-USD.csv`).

4. Run the Python script:
    ```bash
    python btc_price_prediction.py
    ```

## Output:
- The model's training and testing loss values will be printed to the console, indicating the model's performance.
- The script also saves the training and validation datasets to CSV files (`training_data.csv` and `validation_data.csv`).

## License:
This project is licensed under the MIT License - see the LICENSE file for details.

## Author:
[Your Name]
