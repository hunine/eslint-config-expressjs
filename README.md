# Eslint config for ExpressJs
This package extends Airbnb's base JS .eslintrc (without React plugins) as an extensible shared config.
## Installation
```bash
npm install --save-dev @h2q318/eslint-config-expressjs
```

## Usage
- First of all, you need to install **Airbnb-base**:
```bash
npm install --save-dev eslint-config-airbnb-base
```
- Create eslint config file (.eslintrc)
- Because this package base on **Airbnb-base**, so you need to extend **Airbnb-base** first and then extend this package:
```json
    "extends": [
        "airbnb-base",
        "@h2q318/eslint-config-expressjs"
    ]
```
- To check eslint, you need to add line in your package.json:
```json
  "scripts": {
    "lint": "eslint --ext .js ."
  }
```
- If you want to add more script to auto fix. You need to add ``` --fix ``` flag like this:
```json
  "scripts": {
    "lint": "eslint --ext .js .",
    "lint:fix": "eslint --fix --ext .js ."
  }
```