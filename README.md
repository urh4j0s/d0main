# d0main
Domain checker for Hungarian (*.hu) TLD domains

This is a domain checker application that by default
1. Checks all .hu domains of exactly 3 characters
2. Recognizes all that are not registered by Hungarian authorities
3. And lists them into a generated *txt* file

Based on registration rules, this goes through 46656 potential domains and within ~90 minutes it returns all findings based on the default search criteria
NOTE: you may use _tqdm_ to showcase a progress bar for the ease of use [command in powershell: pip install tqdm]

In this application, you will request information about 10 domains each second, you can speed this up by raising **MAX_WORKERS** or **RATE_LIMIT** in the config file
NOTE: this might reach the treshold of allowed requests per second by the Hungarian game registrar (might be different in other countries)
