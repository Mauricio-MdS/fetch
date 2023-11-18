# Fetch

Fetch prints the content found at a URL.

These are exercises 1.7, 1.8 and 1.9 from the book The Go Programming Language by Brian W. Kernighan and Alan Donovan.

## How to Run

To run the Fetch program, use the following command:

```bash
go run fetch.go [url]
```

## Example Usage

```bash
go run fetch.go https://go.dev/
```

## Tasks

[x] The function call io.Copy(dst, src) reads from src and writes to dst. Use it instead of ioutil.ReadAll to copy the response body to os.Stdout without requiring a buffer large enough to hold the entire stream. Be sure to check the error result of io.Copy.

[ ] Modify fetch to add the prefix http:// to each argument URL if it is missing. You might want to use strings.HasPrefix.

[ ] Modify fetch to also print the HTTP status code, found in resp.Status.
