# Event ID 4738: A user account was changed

## Description
Event ID 4738: A user account was changed

## Data Dictionary
|Standard Name|Field Name|Type|Description|Sample Value|
|---|---|---|---|---|
|user_attribute_dummy|Dummy|UnicodeString||`-`|
|target_user_name|TargetUserName|UnicodeString|the name of the account that was changed.|`ksmith`|
|target_user_domain|TargetDomainName|UnicodeString|target account's domain or computer name.|`CONTOSO`|
|target_user_sid|TargetSid|SID|SID of account that was changed. Event Viewer automatically tries to resolve SIDs and show the account name. If the SID cannot be resolved, you will see the source data in the event.|`S-1-5-21-3457937927-2839227994-823803824-6609`|
|user_sid|SubjectUserSid|SID|SID of account that requested the "change user account" operation. Event Viewer automatically tries to resolve SIDs and show the account name. If the SID cannot be resolved, you will see the source data in the event.|`S-1-5-21-3457937927-2839227994-823803824-1104`|
|user_name|SubjectUserName|UnicodeString|the name of the account that requested the "change user account" operation.|`dadmin`|
|user_domain|SubjectDomainName|UnicodeString|subject's domain or computer name.|`CONTOSO`|
|user_logon_id|SubjectLogonId|HexInt64|hexadecimal value that can help you correlate this event with recent events that might contain the same Logon ID, for example, "4624: An account was successfully logged on."|`0x30dc2`|
|user_privilege_list|PrivilegeList|UnicodeString|the list of user privileges which were used during the operation, for example, SeBackupPrivilege. This parameter might not be captured in the event, and in that case appears as "-". See full list of user privileges in "Table 8. User Privileges.".|`-`|
|target_user_sam_name|SamAccountName|UnicodeString|logon name for account used to support clients and servers from previous versions of Windows (pre-Windows 2000 logon name). If the value of sAMAccountName attribute of user object was changed, you will see the new value here. For example: ladmin. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|target_user_display|DisplayName|UnicodeString|it is a name, displayed in the address book for a particular account. This is usually the combination of the user's first name, middle initial, and last name. You can change this attribute by using Active Directory Users and Computers, or through a script, for example. If the value of displayName attribute of user object was changed, you will see the new value here. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|target_user_principal_name|UserPrincipalName|UnicodeString|internet-style login name for the account, based on the Internet standard RFC 822. By convention this should map to the account's email name. If the value of userPrincipalName attribute of user object was changed, you will see the new value here. You can change this attribute by using Active Directory Users and Computers, or through a script, for example. For local accounts, this field is not applicable and always has "-" value.|`-`|
|target_user_home_directory|HomeDirectory|UnicodeString|user's home directory. If homeDrive attribute is set and specifies a drive letter, homeDirectory should be a UNC path. The path must be a network UNC of the form \Server\Share\Directory. If the value of homeDirectory attribute of user object was changed, you will see the new value here. You can change this attribute by using Active Directory Users and Computers, or through a script, for example. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|target_user_home_path|HomePath|UnicodeString|specifies the drive letter to which to map the UNC path specified by homeDirectory account's attribute. The drive letter must be specified in the form "DRIVE_LETTER:". For example - "H:". If the value of homeDrive attribute of user object was changed, you will see the new value here. You can change this attribute by using Active Directory Users and Computers, or through a script, for example. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|target_user_script_path|ScriptPath|UnicodeString|specifies the path of the account's logon script. If the value of scriptPath attribute of user object was changed, you will see the new value here. You can change this attribute by using Active Directory Users and Computers, or through a script, for example. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|target_user_profile_path|ProfilePath|UnicodeString|specifies a path to the account's profile. This value can be a null string, a local absolute path, or a UNC path. If the value of profilePath attribute of user object was changed, you will see the new value here. You can change this attribute by using Active Directory Users and Computers, or through a script, for example. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|target_user_workstations|UserWorkstations|UnicodeString|contains the list of NetBIOS or DNS names of the computers from which the user can logon. Each computer name is separated by a comma. The name of a computer is the sAMAccountName property of a computer object. If the value of userWorkstations attribute of user object was changed, you will see the new value here. You can change this attribute by using Active Directory Users and Computers, or through a script, for example. For local accounts, this field is not applicable and always appears as "\."|`-`|
|target_user_password_last_set|PasswordLastSet|UnicodeString|last time the account's password was modified. If the value of pwdLastSet attribute of user object was changed, you will see the new value here. For example: 8/12/2015 11:41:39 AM. This value will be changed, for example, after manual user account password reset. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|target_user_account_expires|AccountExpires|UnicodeString|the date when the account expires. If the value of accountExpires attribute of user object was changed, you will see the new value here. . For example, "9/21/2015 12:00:00 AM". You can change this attribute by using Active Directory Users and Computers, or through a script, for example. For local accounts, this field always has some value-if the account's attribute was not changed it will contain the current value of the attribute.|`-`|
|user_primary_group_id|PrimaryGroupId|UnicodeString|Relative Identifier (RID) of user's object primary group.|`-`|
|target_user_allowed_to_delegate|AllowedToDelegateTo|UnicodeString|the list of SPNs to which this account can present delegated credentials. Can be changed using Active Directory Users and Computers management console in Delegation tab of user account, if at least one SPN is registered for user account. If the SPNs list on Delegation tab of a user account was changed, you will see the new SPNs list in AllowedToDelegateTo field (note that you will see the new list instead of changes) of this event.|`-`|
|target_user_old_uac_value|OldUacValue|UnicodeString|specifies flags that control password, lockout, disable/enable, script, and other behavior for the user account. This parameter contains the previous value of userAccountControl attribute of user object.|`0x15`|
|target_user_new_uac_value|NewUacValue|UnicodeString|specifies flags that control password, lockout, disable/enable, script, and other behavior for the user account. If the value of userAccountControl attribute of user object was changed, you will see the new value here.|`0x211`|
|target_user_account_control|UserAccountControl|UnicodeString|shows the list of changes in userAccountControl attribute. You will see a line of text for each change. See possible values in here: "Table 7. User's or Computer's account UAC flags.". In the "User Account Control field text" column, you can see the text that will be displayed in the User Account Control field in 4738 event.|`%%2050 %%2089`|
|target_user_parameters|UserParameters|UnicodeString|if you change any setting using Active Directory Users and Computers management console in Dial-in tab of user's account properties, then you will see \<value changed, but not displayed> in this field. For local accounts, this field is not applicable and always has "\" value.|`-`|
|target_user_sid_history|SidHistory|UnicodeString|contains previous SIDs used for the object if the object was moved from another domain. Whenever an object is moved from one domain to another, a new SID is created and becomes the objectSID. The previous SID is added to the sIDHistory property. If the value of sIDHistory attribute of user object was changed, you will see the new value here.|`-`|
|target_user_logon_hours|LogonHours|UnicodeString|hours that the account is allowed to logon to the domain. If the value of logonHours attribute of user object was changed, you will see the new value here. You can change this attribute by using Active Directory Users and Computers, or through a script, for example.|`-`|

## References
* [MS Source](https://github.com/MicrosoftDocs/windows-itpro-docs/blob/master/windows/security/threat-protection/auditing/event-4738.md)
* [MS Security Auditing Category - Account Management](https://docs.microsoft.com/en-us/windows/security/threat-protection/auditing/advanced-security-audit-policy-settings#account-management)
* [MS Security Auditing Sub-category - Audit User Account Management](https://github.com/MicrosoftDocs/windows-itpro-docs/tree/master/windows/security/threat-protection/auditing/audit-user-account-management.md)

## Tags
* etw_level_Informational
* etw_task_task_0
* Account Management
* Audit User Account Management