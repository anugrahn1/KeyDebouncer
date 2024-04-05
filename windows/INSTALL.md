First clone the repo:

`git clone https://github.com/mackncheesiest/KeyDebouncer`

If you do not have the `chocolatey` package manager installed, open an elevated `cmd` prompt.

Run:

`@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "[System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"`

Then in the same `cmd` prompt, run:

`choco install make`

If you do not have `g++` installed, you will need to do that as well.


Go to the location where you cloned the repo and in the `windows` folder, you will see a `Makefile`.

Run `make`, and you will see a new `exe`. Run the exe in the background, and the program will work!
