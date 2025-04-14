### Run Collection Locally
To run all tests locally use:

```bash
newman run postman_collection.json -e qa_env.json
```


### Run Collection Locally with HTML report
To run all tests locally with HTML report use:

```bash
newman run postman_collection.json -e qa_env.json -r html --reporter-html-export report.html
```