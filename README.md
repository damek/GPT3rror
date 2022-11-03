# GPT3rror
Have GPT3 interpret your errors in jupyter notebook. 

See the [demo notebook](https://github.com/damek/GPT3rror/blob/master/GPT3rror_test.ipynb)

# Requirements

You must have an openai API key.

# Usage

Add the following code to any cell of your jupyter notebook and run that cell. 

```
import GPT3rror

# load the openai api key from openapi_key.txt
with open("openapi_key.txt", "r") as f:
    openai_api_key = f.read()

GPT3rror.raise_error(openai_api_key=openai_api_key, openai_model="text-davinci-002")
```

Now all your cells will send their errors to GPT3.

See the notebook for a quick demo.

