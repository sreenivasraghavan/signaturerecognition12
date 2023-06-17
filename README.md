# signaturerecognition12
signature
from autots import AutoTS
model = AutoTS(forecast_length=4, frequency='infer', ensemble='simple')
model = model.fit(data, date_col='period_end', value_col='followers_gained', id_col=None)
prediction = model.predict()
forecast = prediction.forecast
print(forecast)
data set https://www.kaggle.com
