# ansi-pull
testing ansible-pull

Patching at Scale

It has been noted by many parties that ansible doesn’t operate well at scale due to the limits of open ssh sessions from the ansible workstation. The solution to ansible’s scale limitations  is to use ansible’s pull mode with ansible-pull. 

Architecture: 

A github repository that contains the ansible playbook. Presently this would be a simple task to run yum update, but we could add tasks as needed for emergent conditions. 

A way to trigger this job. This could be accomplished in a number of ways. The least effort may be to use ansible in push mode to invoke the ansible-pull command.
