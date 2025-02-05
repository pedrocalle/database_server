# DatabaseServer

## CODE PRESENT IN THE BOOK ELIXIR IN ACTION BY SASA JURIC

This module implements a simple concurrent database server in Elixir using processes. It handles asynchronous query execution and returns results to the caller.

## USAGE

# Start the server
server = DatabaseServer.start()

# Run an asynchronous query
DatabaseServer.run_async(server, "SELECT * FROM users")

# Get the result (with a timeout of 5 seconds)
result = DatabaseServer.get_result()

# Output the result
IO.inspect(result)
