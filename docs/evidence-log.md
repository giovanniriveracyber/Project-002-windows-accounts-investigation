\# CF-0002 Evidence Log

\#\# Case Information

Case ID: CF-0002

Case Title: Windows Accounts Investigation

Investigator: Giovanni Rivera

Status: Closed

\---

\# Evidence Item 001

Evidence Name

Windows Local User Accounts

File

01-net-user-output.png

Source

Command Prompt

Command

net user

Purpose

Identify every local account configured on the Windows computer.

Observation

Windows returned a list of local accounts including built-in accounts and user-created accounts.

Importance

This establishes the baseline of accounts that exist before investigating privileges or suspicious activity.

\---

\# Evidence Item 002

Evidence Name

Detailed User Account Information

File

02-net-user-giolo.png

Source

Command Prompt

Command

net user giolo

Purpose

Collect detailed information about the current Windows account.

Observation

Windows displayed account status, password information, local group memberships, last logon information, and additional account details.

Importance

This information helps determine whether an account is active and what groups it belongs to.

\---

\# Evidence Item 003

Evidence Name

Current Logged-in User

File

03-whoami-output.png

Source

Command Prompt

Command

whoami

Purpose

Verify which account is currently running the Command Prompt session.

Observation

Windows confirmed that the current session was running under the "giolo" account.

Importance

This validates the identity of the user performing the investigation.

\---

\# Evidence Summary

Three separate commands were used during this investigation.

Each command answered a different investigative question.

When combined, they provided a more complete understanding of the current Windows user environment than any single command alone.

\---

\# Evidence Handling

Original screenshots remain stored inside the private case folder.

Before public publication, screenshots will be reviewed and sanitized to remove or obscure identifying information if necessary.  
