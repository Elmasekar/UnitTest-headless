# How to run browser in headless mode in UnitTest on [LambdaTest](https://www.lambdatest.com/?utm_source=github&utm_medium=repo&utm_campaign=UnitTest-headless)

If you want to run a browser in headless mode for an automation test in UnitTest on Lambdatest, you can use the following steps. You can refer to sample test repo [here](https://github.com/LambdaTest/Python-UnitTest-Selenium).

# Steps:

You can run a test in headless mode by providing it as a capability in test file. The capabilities would look something like this:

```python
desired_caps = {
            'LT:Options': {
                "build": "Python Demo",  # Change your build name here
                "name": "Python Demo Test",  # Change your test name here
                "platformName": "Windows 11",
                "selenium_version": "4.0.0",
                "headless": True    
            },
            "browserName": "Chrome",
            "browserVersion": "98.0",
        }

```

## Run your test

```bash
python lambdatest.py
```

# Links:

[LambdaTest Community](http://community.lambdatest.com/)

