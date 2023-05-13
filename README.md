# Request Header Parser Microservice

This is a Request Header Parser Microservice project built for the FreeCodeCamp curriculum. It extracts information from the request headers and returns JSON containing details about the client's IP address, preferred language, and user agent.

## Project Requirements

To complete the project, the following requirements should be met:

- A GET request to `/api/whoami` should return a JSON response containing the client's IP address, preferred language, and user agent.
- The client's IP address should be extracted from either the `X-Forwarded-For` header or `req.ip`.
- The preferred language should be extracted from the `Accept-Language` header.
- The user agent should be extracted from the `User-Agent` header.

## Usage

- Send a GET request to `/api/whoami` to retrieve the client's information.

## Example Response

```json
{
  "ipaddress": "192.168.0.1",
  "language": "en-US,en;q=0.5",
  "software": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.93 Safari/537.36"
}
