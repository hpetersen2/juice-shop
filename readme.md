# OWASP - Juice Shop

# 1. Find score board
call the url: /score-board

# 2. Give the shop zero stars
use burpsuite and call the url: /contact
change the request to rating on zero and press forward in burpsuite

# 3. Find a confidential document from ftp folder
1. go to the about us section. 
2. in the text find you a link for the terms. 
3. the terms are in the ftp folder. 
4. at the url can you go change in other folders.

# 4. DOM XSS
go to the search bar at paste: <iframe src="javascript:alert(`xss`)">

# 5. Missing Encoding
go to the photo wall and search the picture doesn't load. inspect the src url. that you see the # character. the next step is going to: cyberchef on google. search url encoding and encode the # character. next, replace the # with %23. And the picture is there!

# 6. Exposed Metrics
call the url 127.0.0.1:3000/metrics an see the secrets information