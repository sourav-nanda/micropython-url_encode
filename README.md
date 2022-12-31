

# micropython-url_encode
This is a micropython library aimed at encoding and decoding URLs. 


# Usage


```python
from Url_encode import url_encode

some_api='https://wpmsg.com/?text='
string_to_be_url_encoded='This is a message'

url=url_encode()

encoded_string=url.encode('string_to_be_url_encoded')
url_to_be_decoded=some_api+encoded_string

decoded_url=url.decode(url_to_be_decoded)

print('\nThe encoded string is:',encoded_string)
print('URL:',some_api+encoded_string)
print('\nThe decoded URL is:',decoded_url)

OUTPUT


The encoded string is: string%5fto%5fbe%5furl%5fencoded
URL: https://wpmsg.com/?text=string%5fto%5fbe%5furl%5fencoded
The decoded URL is: https://wpmsg.com/?text=string_to_be_url_encoded
```

