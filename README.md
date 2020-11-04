# gpt2_film

This GPT2-film model generates film script text.  
When you enter text for the beginning of the film script, the model gives you the rest of the film script as long as you want.

## How to use

This API has 2 routing address

**# POST parameter**

***/long***  
text : begining of the text you want to generate  
number_samples : the number of sentence that will be generated  
length : the length of each sentence  

***/short***  
text : begining of the text you want to generate  
number_samples : the number of word that will be generated  

**# With CLI** :  

curl --location --request POST 'https://main-gpt2-film-gmlee329.endpoint.ainize.ai/gpt2-story/long' --form 'text=once upon a time' --form 'num_samples=5' --form 'length=10'
  
curl --location --request POST 'https://main-gpt2-film-gmlee329.endpoint.ainize.ai/gpt2-story/short' --form 'text=once upon a time' --form 'num_samples=5'

**# With swagger** : 

You can test this API with swagger.yaml on [swagger editor](https://editor.swagger.io/)
