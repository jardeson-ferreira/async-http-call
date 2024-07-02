# Example of Non-blocking HTTP Call in Django

This is a simple example of an asynchronous function in Django that makes a non-blocking HTTP call using the `httpx` library. This approach allows the code to continue executing other tasks while waiting for the HTTP call response.

## Prerequisites

Make sure you have Python and Django installed in your development environment.

## Installation

1. Clone this repository to your local machine.

2. Navigate to the project directory.

## Usage

1. Run the Django development server.

2. Open your browser and go to `http://localhost:8000`.

3. You will see the message "Non-blocking HTTP request!" in the browser.

## Code Explanation

The code consists of two main functions:

- The `http_call_async` function is an asynchronous function that makes a non-blocking HTTP call. It iterates from 1 to 5, waiting 1 second in each iteration and displaying the corresponding number. Then, it makes an asynchronous GET request to the URL "https://httpbin.org/" using the `httpx` library's HTTP client.

- The `async_view` function is a Django asynchronous view that initiates the asynchronous HTTP call in the background and returns an immediate HTTP response.

## Contribution

Contributions are welcome! If you have suggestions, improvements, or corrections, feel free to open an issue or submit a pull request.

## Developers

| [<img src="https://avatars.githubusercontent.com/jardeson-ferreira" width=115><br><sub>Jardeson Ferreira</sub>](https://github.com/jardeson-ferreira) |
| :----------------------------------------------------------: |
