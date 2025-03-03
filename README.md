# test-nest

## A. INIT PROJECT


### Typescript

```bash
    npm init -y
    npm install -D typescript ts-node @type/node
    npx tsc --init
```

### Playwright 

```bash
    npm install -D @playwright/test
    npx playwright install
```

### Cucumber

```bash
    npm install -D @cucumber/cucumber
```

### Setup tsconfig.json

```json
    {
        "compilerOptions": {
            "target": "ESNext",
            "module": "CommonJS",
            "outDir": "dist",
            "rootDir": "./",
            "strict": true
        }
    }
```


### Structure

```
    test-nest/
    ├── features/
    │   ├── signup.feature
    │   └── ekyc-fraud-detection.feature
    ├── steps/
    │   ├── signup.steps.ts
    │   └── ekyc-fraud-detection.steps.ts
    ├── utils/
    │   ├── locatorManager.ts
    │   ├── testDataGenerator.ts
    │   ├── aiStepDefinitionGenerator.ts
    │   └── aiVisualBugDetector.ts
    ├── ai/
    │   ├── apiClient.ts
    │   └── ekycService.ts
    ├── mocks/
    │   └── mockServer.ts
    ├── ci-cd/
    │   └── ci-cd-test-runner.ts
    ├── locators/
    │   └── signup-locators.json
    ├── package.json
    └── tsconfig.json
```