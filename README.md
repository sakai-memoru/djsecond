# Django Second

## Overview
- Create site and apps on Django at Second time

## History

- created date : 2018/06/02

## Environment

- below:

``` powershell
PS G:\> python --version
Python 3.6.5
PS G:\> virtualenv --version
16.0.0

```
- Using virtualenvwrapper

## Installation
- virtual environment

``` powershell
PS G:\> dir Env: | out-string -stream | select-string "WORKON"

WORKON_HOME                    G:\env\py

PS G:\> mkvirtualenv djsecond
PS G:\> cd $Env:WORKON_HOME
PS G:\env\py> .\djfirst\Scripts\activate

```

- python package installation
```
PS G:\> dir Env: | out-string -stream | select-string "PROJECT_HOME"

PROJECT_HOME                    G:\workspace\py

(djsecond) PS G:\> cd $Env:PROJECT_HOME
(djsecond) PS G:\workspace\py> cd .\pjsecond

(djsecond) PS G:\workspace\py\djsecond> pip install -r requirements.txt
```
## Execution

```
(djfirst) PS G:\workplace\py\djsecond> ls


(djfirst) PS G:\workplace\py\djfirst> python manage.py runserver
Performing system checks...

System check identified no issues (0 silenced).

You have 14 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.
June 02, 2018 - 08:22:02
Django version 2.0.5, using settings 'djfirst.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.
```

- access http://127.0.0.1:8000/

// --- end of file

