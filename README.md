# Churn-Analysis-And-Prediction
### What is customer churn?
Customer churn, also known as customer attrition, is when a customer essentially stops being a customer ie, they choose to stop using your products or services. The customer churn rate is the rate at which your customers stop doing business with you. Every company experiences churn, the key is to understand why your customers are churning and decrease the churn rate.


In this repository, we have performed the end to end Exploratory Data Analysis, and idenfitied the characteristics of the customers that are more likely to churn, and I have used them wisely to create a model, and lately, have deployed the model.

### For EDA, please refer to : Churn Analysis EDA.ipynb
### For Model Building, please refer to: Churn Analysis Model.ipynb
### For Model Deployment, please refer to app.py


### 🔵 Creating the flask API

```
app = Flask("__name__")
```

The loadPage method calls our home.html.
```
@app.route("/")
def loadPage():
	return render_template('home.html', query="")
```

The predict method is our POST method, which is basically called when we pass all the inputs from our front end and click SUBMIT.
```
@app.route("/", methods=['POST'])
def predict():
```
  
The run() method of Flask class runs the application on the local development server.
```
app.run()
```


Yay, our model is ready, let’s test our bot.
The above given Python script is executed from Python shell.

Go to Anaconda Prompt, and run the below query.
```
python app.py
```


Below message in Python shell is seen, which indicates that our App is now hosted at http://127.0.0.1:5000/ or localhost:5000
```
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```


HERE'S HOW OUR FRONTEND LOOKS LIKE:

![Customer Retention](https://user-images.githubusercontent.com/100705267/162373330-e9ae8495-da40-4212-967f-5666f146bd30.png)
