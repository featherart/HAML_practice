Example app to teach students Haml and Haml coffee

notes: 

- you can only do for loops in jst templates, so don't even *think* about using an each block

- the only reason this direct ajax call works is that the OMDB api accepts jsonp! to work with an api that doesn't accept jsonp you have to either use a callback or do the call in your controller:

def api
  url = url of api you're calling
  data = open(url)

  render :json => data
end

then call your own method, passing in any variables by the query string.



