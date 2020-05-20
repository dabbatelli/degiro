# Unofficial DeGIRO Python API
Very basic **unofficial** Python API for [DeGiro](https://www.degiro.nl). This API is only able to get details about your portfolio. It cannot be used for automatic trading. For a way more extensive Node.js API have a look at [pladarias](https://github.com/pladaria/degiro) work.

:warning: DeGiro could change their API at any moment, if something is not working, please open an issue.

## Example usage
```python
from degiro import degiro

dg = degiro()
dg.login('myuser','mypass') # User and pass optional. Will ask if None
dg.getConfig()
dg.getData
dg.data # Lots of data, unorganised
orders = dg.getOrders # Returns a DataFrame
transactions = dg.getTransactions # Returns a DataFrame
```
