# Mtcars Flask API

This project deploys a linear regression model trained on the `mtcars` dataset to predict miles per gallon (MPG) based on other car features.

The model is served using a Flask API, containerized with Docker, and deployed on Google Cloud Run.

---

## How to Use

Make a `POST` request to the `/predict` endpoint with the appropriate JSON input.

### Example `curl` Command:
```bash
curl -X POST https://mtcars-flask-api-711427313394.us-central1.run.app/predict \
  -H "Content-Type: application/json" \
  -d '{"cyl":6,"disp":160,"hp":110,"drat":3.9,"wt":2.62,"qsec":16.46,"vs":0,"am":1,"gear":4,"carb":4}'