# tempory-file-storage-server

An express server for stubbing out the API needs of the new front-end-powered creator system.

# Installation

`npm install`

# Running

`node index.js`

Will bind to port 3001. You can now hit `http://localhost:3001/` with various requests.

# Routes

## /upload

Hit with a multi-part POST request. Uploaded files will be stored inside the project folder at `store` and can be reached at `http://localhost:3001/store/[filename]` where filename is a sha1 hash generated by the sever. Returns JSON payload with URL.

## /twitter/oembed/?url=[URL]

Converts a twitter tweet URL into a Twitter Card. Returns a JSON payload that includes the HTML.
