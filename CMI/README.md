# CMI Plugin Documentation

## Will update personal CMI documentation here

Notes:
- I was looking at perms and saw admins have access to cmi.interactivesign.*
- the regex is wrong on default. config.yml > InteractiveSigns >   SignRegex: (\[ic:([a-zA-Z0-9-]+)\]) # was missing dash after 9
  * < ^ this is new updated line in case goes bad again, it was able to find the ic name i was using ^>