# Making Google command line script using python
To make a request to the Web search API, we have to import the modules that we
need.

urllib2
Loads the URL response

urllib
To make use of urlencode

json
Google returns JSON

To make it a bit interactive, we will ask the user for an input and save the
result to a variable that we name "query".
query = raw_input("What do you want to search for ? >> ")

Create the response object by loading the the URL response, including the query
we asked for above. 
response = urllib2.urlopen (url + query ).read()

# Process the JSON string.
data = json.loads (response)

