# Example of Asynchronous HTTP Call

This is a simple example of an asynchronous function in Django that performs a non-blocking HTTP call using the `httpx` library. This approach allows the code to continue executing other tasks while waiting for the HTTP call response.

## Prerequisites

Make sure you have Python and Django installed in your development environment.

## Installation

1. Clone this repository to your local machine.

2. Navigate to the project directory.

3. Install the `httpx` library:
    ```bash
    pip install httpx
    ```

## Usage

1. Run the Django development server:
    ```bash
    python manage.py runserver
    ```

2. Open your browser and go to `http://localhost:8000`.

3. You will see the message "Non-blocking HTTP request!" in your browser.

## Code Explanation

The code consists of two main functions:

- The `http_call_async` function is an asynchronous function that performs a non-blocking HTTP call. It iterates from 1 to 5, waiting for 1 second on each iteration and displaying the corresponding number. Then, it makes an asynchronous GET request to the URL "https://httpbin.org/" using the HTTP client from the `httpx` library.

- The `async_view` function is a Django asynchronous view that initiates the asynchronous HTTP call in the background and returns an immediate HTTP response.

## Contribution

Contributions are welcome! If you have suggestions, improvements, or fixes, feel free to open an issue or submit a pull request.
