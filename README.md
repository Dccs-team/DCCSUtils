
# DCCSUtils - Request Utility Library

Developer: Md Saimun
Team: DCCS

The `DCCSUtils` class provides a set of utility methods for making HTTP requests, handling responses, and performing common HTTP operations.

## Installation

You can install dccs_utils using pip:

```
pip install dccs_utils
```

## Methods

### gpt(url, **kwargs)
Sends a GET request to the specified URL and returns the response.

### Example usage:
```python
response = DCCSUtils.gpt("https://example.com")
content = response.content
```
### pst(url, data=None, json=None, **kwargs)
Sends a POST request to the specified URL with optional data and JSON payload, and returns the response.

### Example usage:

```python
payload = {"key": "value"}
response = DCCSUtils.pst("https://example.com/api", json=payload)
status_code = response.status_code
```
### rnd_choice(sequence)
Returns a random element from the given sequence.

### Example usage:

```python
options = ["apple", "banana", "orange"]
random_option = DCCSUtils.rnd_choice(options)
print(random_option)
```
### 
### rnd_range(start, stop=None, step=1)
Returns a random integer within the specified range.

### Example usage:

```python
random_number = DCCSUtils.rnd_range(1, 10)
print(random_number)
```
### slp(seconds)
Suspends the execution for the specified number of seconds.

### Example usage:

```python
print("Start")
DCCSUtils.slp(2)
print("End")
```
### jld(string, **kwargs)
Parses a JSON string and returns the parsed object.

### Example usage:

```python
json_string = '{"key": "value"}'
parsed_json = DCCSUtils.jld(json_string)
print(parsed_json["key"])
```
### tpe(max_workers=None)
Returns a ThreadPoolExecutor object with the specified maximum number of workers.

### Example usage:

```python
executor = DCCSUtils.tpe(max_workers=5)
# Submit tasks to the executor
executor.submit(my_task_function)
```
### exe(command)
Executes the specified command in the system shell.

### Example usage:

```python
DCCSUtils.exe("ls -l")
```
### 
### dl_file(url, file_path)
Downloads a file from the specified URL and saves it to the specified file path.

### Example usage:

```python
DCCSUtils.dl_file("https://example.com/image.jpg", "path/to/save/image.jpg")
```
### fnd_links(url)
Retrieves all the links from the HTML content of the specified URL and returns them as a list.

### Example usage:

```python
links = DCCSUtils.fnd_links("https://example.com")
for link in links:
    print(link) 
```
### get_ip()
Retrieves the public IP address of the machine.

### Example usage:

```python
ip_address = DCCSUtils.get_ip()
print(ip_address)
```
### get_random_element(sequence)
Returns a random element from the given sequence.

### Example usage:

```python
options = ["apple", "banana", "orange"]
random_option = DCCSUtils.get_random_element(options)
print(random_option)
```
### get_content(response)
Returns the content of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
content = DCCSUtils.get_content(response)
print(content)
```
### get_headers(response)
Returns the headers of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
headers = DCCSUtils.get_headers(response)
print(headers)
```
### get_status_code(response)
Returns the status code of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
status_code = DCCSUtils.get_status_code(response)
print(status_code)
```
### get_cookies(response)
Returns the cookies of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
cookies = DCCSUtils.get_cookies(response)
print(cookies)
```
### set_timeout(timeout)
Sets the timeout value for requests.

### Example usage:

```python
DCCSUtils.set_timeout(10)
response = DCCSUtils.gpt("https://example.com")
```
### set_proxy(proxy)
Sets the proxy for requests.

### Example usage:

```python
proxy = {"http": "http://proxy.example.com", "https": "https://proxy.example.com"}
DCCSUtils.set_proxy(proxy)
response = DCCSUtils.gpt("https://example.com")
```
### set_headers(headers)
Sets the headers for requests.

### Example usage:

```python
headers = {"User-Agent": "Mozilla/5.0"}
DCCSUtils.set_headers(headers)
response = DCCSUtils.gpt("https://example.com")
```
### get_title(url)
Retrieves the title of the HTML page from the specified URL.

### Example usage:

```python
title = DCCSUtils.get_title("https://example.com")
print(title)
```
### download(url, file_path)
Downloads a file from the specified URL and saves it to the specified file path.

### Example usage:

```python
DCCSUtils.download("https://example.com/image.jpg", "path/to/save/image.jpg")
```
### find_links(url)
Retrieves all the links from the HTML content of the specified URL and returns them as a list.

### Example usage:

```python
links = DCCSUtils.find_links("https://example.com")
for link in links:
    print(link)
```
### get_ip_address()
Retrieves the public IP address of the machine.

### Example usage:

```python
ip_address = DCCSUtils.get_ip_address()
print(ip_address)
```
### get_response_content(response)
Returns the content of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
content = DCCSUtils.get_response_content(response)
print(content)
```
### get_response_headers(response)
Returns the headers of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
headers = DCCSUtils.get_response_headers(response)
print(headers)
```
### get_response_status_code(response)
Returns the status code of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
status_code = DCCSUtils.get_response_status_code(response)
print(status_code)
```
### get_response_cookies(response)
Returns the cookies of the response.

### Example usage:

```python
response = DCCSUtils.gpt("https://example.com")
cookies = DCCSUtils.get_response_cookies(response)
print(cookies)
```
### set_request_timeout(timeout)
Sets the timeout value for a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
DCCSUtils.set_request_timeout(request, 10)
```
### set_request_proxy(proxy)
Sets the proxy for a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
proxy = {"http": "http://proxy.example.com", "https": "https://proxy.example.com"}
DCCSUtils.set_request_proxy(request, proxy)
```
### set_request_headers(headers)
Sets the headers for a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
headers = {"User-Agent": "Mozilla/5.0"}
DCCSUtils.set_request_headers(request, headers)
```
### get_request_url(request)
Returns the URL of a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
url = DCCSUtils.get_request_url(request)
print(url)
```
### get_request_method(request)
Returns the HTTP method of a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
method = DCCSUtils.get_request_method(request)
print(method)
```
### get_request_headers(request)
Returns the headers of a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
headers = DCCSUtils.get_request_headers(request)
print(headers)
```
### get_request_body(request)
Returns the body of a request.

### Example usage:

```python
request = DCCSUtils.Request("POST", "https://example.com", data={"key": "value"})
body = DCCSUtils.get_request_body(request)
print(body)
```
### get_request_text(request)
Returns the text content of a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
text = DCCSUtils.get_request_text(request)
print(text)
```
### get_request_status_code(request)
Returns the status code of a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
status_code = DCCSUtils.get_request_status_code(request)
print(status_code)
```
### get_request_cookies(request)
Returns the cookies of a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
cookies = DCCSUtils.get_request_cookies(request)
print(cookies)
```
### get_request_content(request)
Returns the content of a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
content = DCCSUtils.get_request_content(request)
print(content)
```
### set_request_timeout(request, timeout)
Sets the timeout value for a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
DCCSUtils.set_request_timeout(request, 10)
```
### set_request_proxy(request, proxies)
Sets the proxy for a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
proxies = {"http": "http://proxy.example.com", "https": "https://proxy.example.com"}
DCCSUtils.set_request_proxy(request, proxies)
```
### set_request_headers(request, headers)
Sets the headers for a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
headers = {"User-Agent": "Mozilla/5.0"}
DCCSUtils.set_request_headers(request, headers)
```
### set_request_body(request, data)
Sets the body of a request.

### Example usage:

```python
request = DCCSUtils.Request("POST", "https://example.com")
data = {"key": "value"}
DCCSUtils.set_request_body(request, data)
```
### set_request_files(request, files)
Sets the files for a request.

### Example usage:

```python
request = DCCSUtils.Request("POST", "https://example.com")
files = {"file": open("path/to/file.txt", "rb")}
DCCSUtils.set_request_files(request, files)
```
### set_request_auth(request, auth)
Sets the authentication for a request.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
auth = ("username", "password")
DCCSUtils.set_request_auth(request, auth)
```
### execute_request(request)
Executes a request and returns the response.

### Example usage:

```python
request = DCCSUtils.Request("GET", "https://example.com")
response = DCCSUtils.execute_request(request)
content = DCCSUtils.get_response_content(response)
print(content)
```
### execute_async_requests(requests, max_workers=None)
Executes multiple requests asynchronously using a ThreadPoolExecutor and returns the list of responses.

### Example usage:

```python
request1 = DCCSUtils.Request("GET", "https://example.com/api1")
request2 = DCCSUtils.Request("GET", "https://example.com/api2")
requests = [request1, request2]
responses = DCCSUtils.execute_async_requests(requests, max_workers=5)
for response in responses:
    content = DCCSUtils.get_response_content(response)
    print(content)
```

#### Please note that the `DCCSUtils` module and its methods mentioned above are fictional and provided as an example for demonstration purposes. You'll need to implement the actual module and its methods in your code according to your requirements.





