\# Windows Accounts Investigation Report

\---

\#\# Case Information

\*\*Case ID:\*\* CF-0002    
\*\*Title:\*\* Windows Accounts Investigation    
\*\*Investigator:\*\* Giovanni Rivera    
\*\*Status:\*\* Closed    
\*\*Environment:\*\* Windows 11 Home    
\*\*Investigation Type:\*\* Guided Training Exercise

\---

\# Executive Summary

A Windows account investigation was performed to establish a baseline understanding of local user accounts on a Windows 11 Home system.

The investigation identified existing local accounts, examined detailed information about the current user account, and verified which account was actively running the current Command Prompt session.

No suspicious activity was identified during this investigation.

The primary objective was to understand how Windows stores and reports account information while developing an evidence-based investigation methodology.

\---

\# Investigation Objectives

The investigation attempted to answer the following questions:

\- What local user accounts exist?  
\- Which account belongs to the current user?  
\- Which account is currently running Command Prompt?  
\- What information does Windows maintain about a user account?  
\- Why should analysts compare multiple sources of evidence?

\---

\# Tools Used

\- Windows Command Prompt  
\- Windows Snipping Tool

Commands executed:

\`\`\`text  
net user

net user giolo

whoami  
\`\`\`

\---

\# Evidence Summary

Evidence collected included:

\- Local Windows account enumeration  
\- Detailed account information  
\- Current user identification  
\- Local group membership information

Three screenshots were captured and preserved as supporting evidence.

\---

\# Findings

\#\# Finding 1

Windows stores multiple local accounts, including both built-in system accounts and user-created accounts.

\---

\#\# Finding 2

The command:

\`\`\`text  
net user giolo  
\`\`\`

returned detailed information about the current account, including password settings, account status, group memberships, and logon information.

\---

\#\# Finding 3

The command:

\`\`\`text  
whoami  
\`\`\`

confirmed that the current Command Prompt session was running under the \*\*giolo\*\* account.

\---

\#\# Finding 4

Each command answered a different investigative question.

The investigation demonstrated that analysts should combine multiple evidence sources before reaching conclusions.

\---

\# Analyst Assessment

No evidence of unauthorized accounts or suspicious account activity was identified during this investigation.

The observed behavior was consistent with expected Windows account management on a personal Windows 11 system.

\---

\# Lessons Learned

This investigation reinforced several key concepts:

\- Commands should be selected based on investigative questions.  
\- No single command provides all necessary information.  
\- Multiple evidence sources improve confidence in conclusions.  
\- Documentation is as important as technical execution.

\---

\# Limitations

This investigation focused only on local Windows accounts.

The following topics were outside the scope of this case:

\- Active Directory  
\- Domain accounts  
\- Account creation  
\- Privilege escalation  
\- Event log correlation  
\- Remote logons

\---

\# Recommended Next Steps

Continue investigating:

\- Administrator privileges  
\- User groups  
\- Windows permissions  
\- Privilege escalation concepts

\---

\# Final Conclusion

The investigation successfully established a baseline understanding of local Windows accounts and demonstrated how multiple Windows commands can be combined to answer different investigative questions.

No indicators of malicious activity were identified.

\---

\# Guided Investigation Disclosure

This investigation was completed through guided instruction as part of an ongoing cybersecurity training program.

All commands were personally executed by the investigator.

All observations, evidence collection, reasoning exercises, and documentation were personally completed.  
