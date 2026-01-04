#########################################################

GetPIDsByProcessEnglishNameAndOptionallyKill_ReubenPython2and3

Code to find and kill a process given either a numerical PID or an English name (like "python").

Reuben Brewer, Ph.D.

reuben.brewer@gmail.com

www.reubotics.com

Apache 2 License

Software Revision I, 12/27/2025

Verified working on:

Python 3.11/12/13.

Windows 10/11 64-bit

Raspberry Pi Bookworm

###

GetPIDsByProcessEnglishName: Returns [PID_DictWithPIDasKey, PID_DictWithEXEenglishNameAsKey] for an input ProcessName string (in English, like "VLC", "python", or "notepad").

KillProcessByPIDlist: Kills/force-closes processes specified by their PID number.

Can kill programs based on their English name from the command line like this:

python GetPIDsByProcessEnglishNameAndOptionallyKill_ReubenPython2and3.py "EnglishNameOfProgramYouWishToKill" "kill"

###

Note: If you receive the error "Invalid Class" when issuing a TASKLIST command in Windows, then you'll need to reubild/fix WMI per the following steps:

https://learn.microsoft.com/en-us/answers/questions/203461/tasklist-error-in-windows-10-pro

cd \windows\system32\wbem

net stop winmgmt

rename Repository Repository.old

net start winmgmt

If issue persists, then please run:

cd \windows\system32\wbem

for /f %s in ('dir /b *.mof *.mfl') do mofcomp %s##

#########################################################

######################################################### Python module installation instructions, all OS's

GetPIDsByProcessEnglishNameAndOptionallyKill_ReubenPython2and3, ListOfModuleDependencies: ['future.builtins', 'pexpect']

GetPIDsByProcessEnglishNameAndOptionallyKill_ReubenPython2and3, ListOfModuleDependencies_TestProgram: []

GetPIDsByProcessEnglishNameAndOptionallyKill_ReubenPython2and3, ListOfModuleDependencies_NestedLayers: []

GetPIDsByProcessEnglishNameAndOptionallyKill_ReubenPython2and3, ListOfModuleDependencies_All:['future.builtins', 'pexpect']

#########################################################
