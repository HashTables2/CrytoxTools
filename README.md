# CrytoxTools
Tools for analyzing Crytox ransomware shellcode. Recently, Crytox has been using shellcode for encryption. 

# IDA Python 
This script can be used in IDA 7+ to label the hashes with the appropriate API call. It requires the call made by the shellcode to be labled `mw_GetDllFunName_and_call` It has multiple hardcoded API calls from various DLLs loaded into svchost.exe where this shellcode gets injected. 

# Standalone
This script is a standalone python script in case IDA Python is not available. You must change the `key_hashes` to contain the API hashes Crytox uses. It has multiple hardcoded API calls from various DLLs where this shellcode gets injected.
