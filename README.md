<h1 align="center">
	<img width="300" src="https://i.ibb.co/yY7tfDg/Logo.jpg" alt="explainX.ai"> 
	<br>
</h1>


explainX.ai helps data scientists understand, explain and validate any machine learning model - in just one line of code.

[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Explain%20any%20black-box%20Machine%20Learning%20model%20in%20just%20one%20line%20of%20code%21&url=https://www.explainx.ai&hashtags=xai,explainable_ai,explainable_machine_learning,trust_in_ai,transparent_ai)

Visit [explainx.ai][https://www.explainx.ai] to learn more.

## Try it out

* [Installing explainX](https://explainx-documentation.netlify.app/)
* [Working Example](https://explainx-documentation.netlify.app/working-example/)
* [explainX Dashboard Features](https://explainx-documentation.netlify.app/analyze-dashboard/t)
[comment]: <> (This is a comment, it will not be included * [Provide Feedback to Improve explainX](https://mindsdb.typeform.com/to/c3CEtj))

Open your Jupyter Notebook and follow this example to get started with explainx in less than five mins.
```bash
!pip install explainx

## Usage

#Import the library
from explainx import *

#Load Dataset
X_data, Y_data = explainx.dataset_boston()

#Pass X_data, Y_data as numpy arrays into your XGBoost Model
model = xgboost.train({"learning_rate": 0.01}, xgboost.DMatrix(X, label=Y_data), 100)

#Pass your X_data, Y_data, y_variable name, model and model name to the explainx function
explainx.ai(X_Data, Y_Data, model, model_name="xgboost")

#Click on the link to access the dashboard
App running on https://127.0.0.1:8050
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)
