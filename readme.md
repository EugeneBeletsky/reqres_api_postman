
### Install dependencies
To install dependencies:

```bash
npm i
```

### Run Collection Locally
To run all tests locally use:

```bash
newman run postman_collection.json -e qa_env.json
```

### Launch with npx for Allure report
To launch tests use:

```bash
npx newman run postman_collection.json -e qa_env.json -r allure --reporter-allure-output=./allure-results
```

### Generate Allure report

```bash
allure generate ./allure-results --output ./allure-report --clean
```

### Open report
```bash
allure open ./allure-report
```



### Run tests with scripts from package.json
```bash
npm run test:api
npm run report:allureLocal
```