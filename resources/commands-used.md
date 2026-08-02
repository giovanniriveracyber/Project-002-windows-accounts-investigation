\# Commands Used

This document explains the purpose of each command used during this investigation.

\---

\#\# Command

\`\`\`cmd  
net user  
\`\`\`

\#\#\# Purpose

List all local user accounts configured on the Windows computer.

\#\#\# Investigation Question

\> What local user accounts exist on this system?

\---

\#\# Command

\`\`\`cmd  
net user giolo  
\`\`\`

\#\#\# Purpose

Display detailed information about the specified local user account.

\#\#\# Investigation Question

\> What information does Windows maintain about this account?

\---

\#\# Command

\`\`\`cmd  
whoami  
\`\`\`

\#\#\# Purpose

Display the identity of the account currently running the Command Prompt session.

\#\#\# Investigation Question

\> Which account is currently running this session?

\---

\#\# Key Takeaway

One of the biggest lessons from this case was that commands should not be memorized by themselves.

Instead, every command should be connected to the investigative question it answers.  
