# PrimaryTokenTheft
Main code taken from [@kondecuotas](https://twitter.com/kondencuotas) [blog](https://ired.team/).

Steal a primary token and spawn cmd.exe using the stolen token.

Dug into the minimum privileges needed for OpenProcess(), OpenProcessToken() and DuplicateTokenEx(). Added the ability to pass a PID by command-line argument.

# Credit 
https://ired.team/offensive-security/privilege-escalation/t1134-access-token-manipulation

Figured out minimum privileges to call DuplicateTokenEx() with for CreateProcessWithTokenW to work here: https://stackoverflow.com/questions/5447418/why-is-createprocesswithtokenw-failing-with-error-access-denied (MSDN docs are wrong)
