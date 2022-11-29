This package is insipired by the following [blog post](https://testdriven.io/blog/fastapi-streamlit/)

It showcases a backend (Fast API calling a DL model to give a "painting style" to a picture) + a frontend (streamlit app to upload a picture and display the restyled picture as a result) orchestrated on docker-compose

Simply run
```bash
./backend/getmodels.sh # to download models
docker-compose up --build # to launch the app on http://localhost:8501/
```
