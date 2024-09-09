---

# Improved Neural Network-based Modeling for Wind Speed Prediction in the Indian Ocean Region

### Project Description
This project involves predicting wind speeds over a large region, specifically in the Indian Ocean, using advanced neural network models. The project explores the use of Convolutional Long-Short Term Memory (ConvLSTM) and Artificial Neural Networks (ANN) for accurate short-term wind speed prediction. These predictions are crucial for industries such as shipping, offshore oil exploration, and disaster management, where timely wind forecasts can help in mitigating the effects of tropical cyclones and other severe weather events.

### Objectives
- Predict wind speed across multiple longitudes and latitudes in the Indian Ocean.
- Implement neural network models, specifically ConvLSTM and ANN, to predict wind speed.
- Compare the models' performance using metrics such as Mean Squared Error (MSE) and Mean Absolute Error (MAE).

### Key Features
- **ConvLSTM Model**: Used for spatial and temporal wind speed prediction. Takes a 3D input for forecasting future wind speeds based on past data.
- **ANN Model**: A simpler, efficient model for time-series prediction, offering fast results with fewer computational resources.
- **Data Collection**: Wind speed data has been collected from Earth Nullschool, derived from the Global Forecast System (GFS), and focuses on 40,000 locations in the Indian Ocean.
- **Use Case**: Tested on Cyclone Chapala (2015) to assess its potential in predicting extreme weather events.

### Models
- **ConvLSTM**: Processes input data as sequential images, making predictions in a frame-by-frame manner. Suitable for capturing both spatial and temporal dependencies in data.
- **ANN**: Uses 8 consecutive time slots of wind speed values to predict the next time slot for a given latitude and longitude.

### Results
- **Accuracy**: The ANN model provided the most accurate results for short-term (6-hour) wind speed prediction, while ConvLSTM models showed potential for longer time frames (12 and 24 hours).
- **Use in Cyclone Prediction**: The models successfully predicted key aspects of Cyclone Chapala’s formation and movement.

### Installation and Usage

#### Requirements
- Python 3.x
- TensorFlow
- NumPy
- Pandas
- Matplotlib
- Keras

#### Installation
1. Clone this repository:
   ```
   git clone https://github.com/your-username/wind-speed-prediction.git
   ```
2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

#### Usage
1. Prepare your dataset by scraping data from the Earth Nullschool website.
2. Train the model using the provided ConvLSTM and ANN scripts:
   ```
   python train_model.py --model [ConvLSTM/ANN]
   ```
3. Test the model on specific time frames and visualize the results:
   ```
   python test_model.py --test-data ./data/test_data.csv
   ```

### Authors
- **Deeptimaan Banerjee** (19BLC1162)
- **Prakhar Narain Srivastava** (19BLC1019)
- **Tarunveer Singh Sidhu** (19BLC1186)

### License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---
