# Update-WinHttpProxy
Checks the current configutation of the WINHTTP proxy (netsh winhttp show proxy) and updates it as per provided parameters.
User get-help CheckWinHttpProxy -examples (or -full) to see explaination of parameters.

EXAMPLE

PS C:\> CheckWinHttpProxy -bypassurl "*.microsoft.com"
Add's "*.microsoft.com" to the bypass list if it isn't already present.

EXAMPLE

PS C:\> CheckWinHttpProxy -bypassurl "*.microsoft.com","*.symantec.com"
Add's both "*.microsoft.com" and "*.symantec.com" to the bypass list if the URL's aren't already present.

EXAMPLE

PS C:\> CheckWinHttpProxy -bypassurl "*.microsoft.com" -resetbypass
Empty's the Bypass List, then add's "*.microsoft.com" to the bypass list if it isn't already present.

EXAMPLE

PS C:\> CheckWinHttpProxy -resetbypass
Empty's the Bypass List
