# ffuf

> A fast web fuzzer written in Go.
> The `FUZZ` keyword is used as a placeholder. `ffuf` will try to hit the URL by replacing the word `FUZZ` with every word in the wordlist.
> More information: <https://github.com/ffuf/ffuf#usage>.

- Enumerate directories using colored output and a wordlist specifying a target uRL:

`ffuf -c -w {{path/to/wordlist.txt}} -u {{https://example.com/FUZZ}}`

- Enumerate webservers of subdomains by changing the position of the keyword:

`ffuf -w {{path/to/subdomains.txt}} -u {{https://FUZZ.example.com}}`

- Fuzz with specified threads (default: 40) and proxying the traffic and save output to a file:

`ffuf -o -w {{path/to/wordlist.txt}} -u {{https://example.com/FUZZ}} -t {{500}} -x {{http://127.0.0.1:8080}}`

- Fuzz a specific Header ("Name: Value") and match HTTP status codes:

`ffuf -w {{path/to/wordlist.txt}} -u {{https://example.com}} -H "{{Host: FUZZ}}" -mc {{200}}`

- Fuzz with specified HTTP method and data, while filtering out specific status codes and response size:

`ffuf -w {{path/to/postdata.txt}} -X {{POST}} -d "{{username=admin\&password=FUZZ}}" -u {{https://example.com/login.php}} -fc {{302,401-499}} -fs {{1234}}`

- Fuzz multiple positions with multiple wordlists using different modes and auto calibration to reduce false positives:

`ffuf -w {{path/to/keys:KEY}} -w {{path/to/values:VALUE}} -mode {{pitchfork|clusterbomb}} -u {{https://example.com/id?KEY=VALUE}} -ac`

- Proxy requests through a HTTP MITM proxy (such as Burp Suite or `mitmproxy`):

`ffuf -w {{path/to/wordlist}} -x {{http://127.0.0.1:8080}} -u {{https://example.com/FUZZ}}`
