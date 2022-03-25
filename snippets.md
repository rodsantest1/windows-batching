https://ss64.com/

# Get latest subfolder in a folder

```
rem https://superuser.com/a/960966/55416
@echo OFF
for /f %%i in ('DIR /AD /O-D /B') do (set target=%%i & goto :break)
:break
echo %target%
```
