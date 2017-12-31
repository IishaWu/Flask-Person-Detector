# Flask-Person-Detector
Flask based web application that provides a REST endpoint using OpenCV's Deep Neural Network method for Object Detection

## How to run
`python server.py`

## Endpoint
If this is run locally, the endpoint is: `http://localhost:5000/is_person`.

If a person is detected response: `{"response": "person likely found"}`

Response for everything else: `{"response": "no people found"}`

To use the endpoint, send a `POST` request with a JSON blob that looks like this: `{"image_path": "your-image-url-here"}`.

## Dependencies
Libraries: `flask`, `numpy`, `cv2`, `requests`, `os`

### Notes
Note that there are a number of dependencies. I'm not sure what the best way is to list these, so if you get the app working, then hooray. This is more about having a reference of how to make a OpenCV DNN based REST endpoint using Flask.
