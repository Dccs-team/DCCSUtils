# DCCSUtils - Request Utility Library

Developer: Md Saimun
Team: DCCS

The `DCCSUtils` class provides a set of utility methods for making HTTP requests, handling responses, and performing common HTTP operations.

## Methods

### gpt(url, **kwargs)
Sends a GET request to the specified URL and returns the response.

### pst(url, data=None, json=None, **kwargs)
Sends a POST request to the specified URL with optional data and JSON payload, and returns the response.

### rnd_choice(sequence)
Returns a random element from the given sequence.

### rnd_range(start, stop=None, step=1)
Returns a random integer within the specified range.

### slp(seconds)
Suspends the execution for the specified number of seconds.

### jld(string, **kwargs)
Parses a JSON string and returns the parsed object.

### tpe(max_workers=None)
Returns a ThreadPoolExecutor object with the specified maximum number of workers.

### exe(command)
Executes the specified command in the system shell.

### dl_file(url, file_path)
Downloads a file from the specified URL and saves it to the specified file path.

### fnd_links(url)
Retrieves all the links from the HTML content of the specified URL and returns them as a list.

### get_ip()
Retrieves the public IP address of the machine.

### get_random_element(sequence)
Returns a random element from the given sequence.

### get_content(response)
Returns the content of the response.

### get_headers(response)
Returns the headers of the response.

### get_status_code(response)
Returns the status code of the response.

### get_cookies(response)
Returns the cookies of the response.

### set_timeout(timeout)
Sets the timeout value for requests.

### set_proxy(proxy)
Sets the proxy for requests.

### set_headers(headers)
Sets the headers for requests.

### get_title(url)
Retrieves the title of the HTML page from the specified URL.

### download(url, file_path)
Downloads a file from the specified URL and saves it to the specified file path.

### find_links(url)
Retrieves all the links from the HTML content of the specified URL and returns them as a list.

### get_ip_address()
Retrieves the public IP address of the machine.

### get_response_content(response)
Returns the content of the response.

### get_response_headers(response)
Returns the headers of the response.

### get_response_status_code(response)
Returns the status code of the response.

### get_response_cookies(response)
Returns the cookies of the response.

### set_request_timeout(timeout)
Sets the timeout value for a request.

### set_request_proxy(proxy)
Sets the proxy for a request.

### set_request_headers(headers)
Sets the headers for a request.

### get_request_url(request)
Returns the URL of a request.

### get_request_method(request)
Returns the HTTP method of a request.

### get_request_headers(request)
Returns the headers of a request.

### get_request_body(request)
Returns the body of a request.

### get_request_text(request)
Returns the text content of a request.

### get_request_status_code(request)
Returns the status code of a request.

### get_request_cookies(request)
Returns the cookies of a request.

### get_request_content(request)
Returns the content of a request.

### set_request_timeout(request, timeout)
Sets the timeout value for a request.

### set_request_proxy(request, proxies)
Sets the proxy for a request.

### set_request_headers(request, headers)
Sets the headers for a request.

### set_request_body(request, data)
Sets the body of a request.

### set_request_files(request, files)
Sets the files for a request.

### set_request_session(request, session)
Sets the session for a request.

### set_request_hooks(request, hooks)
Sets the hooks for a request.

### set_request_params_encoding(request, encoding)
Sets the encoding for a request's parameters.

### set_request_allow_redirects(request, allow_redirects)
Sets the allow_redirects flag for a request.

### set_request_prepared(request, prepared_request)
Sets the prepared request for a request.

### set_request_history(request, history)
Sets the history for a request.

### set_request_original_request(request, original_request)
Sets the original request for a request.

### set_request_is_redirect(request, is_redirect)
Sets the is_redirect flag for a request.

### set_request_is_permanent_redirect(request, is_permanent_redirect)
Sets the is_permanent_redirect flag for a request.

### send_request(request)
Sends a request.

