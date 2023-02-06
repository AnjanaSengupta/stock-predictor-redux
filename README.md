# stock-predictor-redux

To run the app locally - 

uvicorn main:app --reload --workers 1 --host 0.0.0.0 --port 8000

To test the endpoint, use curl to test the endpoint, use the Public IPv4 address for the instance, and run the following:

curl \
--header "Content-Type: application/json" \
--request POST \
--data '{"ticker":"MSFT", "days":7}' \
http://[YOUR PUBLIC IPv4]:8000/predict
