# Python `requests` Module Cheat Sheet

## 1. **Installing the Requests Module**
```sh
pip install requests
```

## 2. **Importing Requests**
```python
import requests
```

## 3. **Making a GET Request**
```python
response = requests.get('https://jsonplaceholder.typicode.com/posts/1')
print(response.status_code)  # HTTP status code
print(response.text)  # Response body as text
print(response.json())  # Parse response as JSON
```

## 4. **Making a POST Request**
```python
url = 'https://jsonplaceholder.typicode.com/posts'
data = {'title': 'foo', 'body': 'bar', 'userId': 1}
response = requests.post(url, json=data)
print(response.json())
```

## 5. **Making a PUT Request**
```python
url = 'https://jsonplaceholder.typicode.com/posts/1'
data = {'title': 'updated title', 'body': 'new content', 'userId': 1}
response = requests.put(url, json=data)
print(response.json())
```

## 6. **Making a DELETE Request**
```python
response = requests.delete('https://jsonplaceholder.typicode.com/posts/1')
print(response.status_code)  # 200 if successful
```

## 7. **Passing Query Parameters**
```python
params = {'userId': 1}
response = requests.get('https://jsonplaceholder.typicode.com/posts', params=params)
print(response.json())
```

## 8. **Handling Headers**
```python
headers = {'User-Agent': 'my-app'}
response = requests.get('https://jsonplaceholder.typicode.com/posts', headers=headers)
print(response.json())
```

## 9. **Handling Timeouts**
```python
try:
    response = requests.get('https://jsonplaceholder.typicode.com/posts', timeout=5)
    print(response.json())
except requests.Timeout:
    print("Request timed out")
```

## 10. **Downloading a File**
```python
url = 'https://example.com/sample.pdf'
response = requests.get(url, stream=True)
with open('sample.pdf', 'wb') as file:
    for chunk in response.iter_content(chunk_size=1024):
        file.write(chunk)
```

---
This cheat sheet covers essential Python `requests` module functions. 🚀
