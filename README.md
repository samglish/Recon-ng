# Recon-ng
### Recognition tool
```bash

    _/_/_/    _/_/_/_/    _/_/_/    _/_/_/    _/      _/            _/      _/    _/_/_/
   _/    _/  _/        _/        _/      _/  _/_/    _/            _/_/    _/  _/       
  _/_/_/    _/_/_/    _/        _/      _/  _/  _/  _/  _/_/_/_/  _/  _/  _/  _/  _/_/_/
 _/    _/  _/        _/        _/      _/  _/    _/_/            _/    _/_/  _/      _/ 
_/    _/  _/_/_/_/    _/_/_/    _/_/_/    _/      _/            _/      _/    _/_/_/    


                                          /\
                                         / \\ /\
    Sponsored by...               /\  /\/  \\V  \/\
                                 / \\/ // \\\\\ \\ \/\
                                // // BLACK HILLS \/ \\
                               www.blackhillsinfosec.com

                  ____   ____   ____   ____ _____ _  ____   ____  ____
                 |____] | ___/ |____| |       |   | |____  |____ |
                 |      |   \_ |    | |____   |   |  ____| |____ |____
                                   www.practisec.com

                      [recon-ng v5.1.1, Tim Tomes (@lanmaster53)]                       

[*] No modules enabled/installed.

[recon-ng][default] > 
```
to use it you must add a workspace.
* facebook
```bash
[recon-ng][default] > workspaces create facebook
```
Add Domains
```bash
[recon-ng][facebook] > db insert domains
```
```
domain (TEXT): facebook.com
```
[*] 1 rows affected.
* samglishinc
```bash
[recon-ng][default] > workspaces create samglishinc
```
Add Domains
```bash
[recon-ng][samglishinc] > db insert domains
```
```
domain (TEXT): samglishinc.000webhostapp.com
```
[*] 1 rows affected.

we added two workspaces, to view the list of workspaces
```bash
[recon-ng][samglishinc.000webhostapp.com] > workspaces list
```
OUTPUT
```
  +-----------------------------------------------------+
  |           Workspaces          |       Modified      |
  +-----------------------------------------------------+
  | default                       | 2024-08-31 07:54:20 |
  | facebook                      | 2024-08-31 07:59:33 |
  | samglishinc                   | 2024-08-31 07:59:56 |
  +-----------------------------------------------------+

```
let's check the domains
```bash
[recon-ng][facebook.com] > show domains
```
```
  +------------------------------------------------------+
  | rowid |     domain    |     notes     |    module    |
  +------------------------------------------------------+
  | 1     | facebook.com  | scan facebook | user_defined |
  +------------------------------------------------------+

[*] 1 rows returned
```
```bash
[recon-ng][facebook.com] > Workspaces load netcraft
``` 
```bash
[recon-ng][facebook.com] > run
``` 


