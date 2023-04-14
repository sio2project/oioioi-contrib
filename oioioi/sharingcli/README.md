# sharingcli

A module which allows you to add a new problem using a link
from another similar website. Currently it is possible to use with
(after the website admin's approval): [ki.staszic.waw.pl](http://ki.staszic.waw.pl)

Please note that [ki.staszic.waw.pl](http://ki.staszic.waw.pl) is not functioning actively anymore.

## Installation

- Add the module to `oioioi` directory, add `oioioi.sharingcli` to `INSTALLED_APPS`. 
- Add `'oioioi.sharingcli.problem_sources.RemoteSource'` to `PROBLEM_SOURCES`. 
- Add`SHARING_SERVERS` variable to settings. Use the format:
```python
SHARING_SERVERS = (
    ('site_url', 'sharing_url', 'client_id', 'client_secret'),
)```