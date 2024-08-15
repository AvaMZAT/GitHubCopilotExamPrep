#flashcards/GitHubCopilot/Features

What does the **“block suggestions matching public code”** feature do?
?
Prevent potential risks of using public code that might have legal or licensing implications in suggestions of GitHubCopilot.

How is the **“block suggestions matching public code feature”** enabled for GitHub Copilot Individual Users?
?
Go to Github Settings (Profile Picture) => click on the left sidebar “Copilot” => under “Suggestions matching public code” set to block => click save

How is the **“block suggestions matching public code feature”** enabled for GitHub Copilot Organisations?
?
Go to profile => select “Your organizations” => choose the relevant organization => Settings => “Copilot” => “Code, planning and automation“ section => under “Policies” select “Suggestions matching public code”

What  does the **“Exclude specified files from Copilot“** feature do?
?
Configure content exclusions on repository or organization level. Also for VSCode there is the option to use a .copilotignore file.

How do you configure the  **“Exclude specified files from Copilot“** feature on repository-level?
?
Go to repository settings => “Code  & automation” => “Copilot”. Enter the repository paths into “Paths to exclude in this repository” - Textbox. Format is YAML. ie: *- “PATH/TO&DIRECTORY/OR/FILE*

How do you configure the **“Exclude specified files from Copilot“** feature on organization level?
?
go to your profile => “Your organizations” => “Settings” => “Copilot”. In the “Repositories and paths to exclude” textbox enter the repositories and paths to exclude. Format is YAML.
``` example

octo-repo: 
- "/src/secrets.json"
- "/src/some-dir/kernel.rs"
https://github.com/test/repo.git:
- "/src/bin"
```
<!--SR:!2024-08-08,1,230-->


How do you use a .copilotignore file for the **“Exclude specified files from Copilot“** feature?
?
like the .gitignore file place a .copilotignore file and add definitions of to exclude directory and files like in .gitignore. Example:
``` plaintext
# Ignore all environment files
**/.env

# Ignore all files in the scripts directory
/scirpts/**
```

What does the feature **“Organization-wide policy management”** mean?
?
As an org owner on GitHub you can manage various apsects of GitHub Copilot

How do I set policies for the feature **“Organization-wide policy management”**?
?
go to your profile => “Your organizations” => “Settings” => “Code, planning, and automation” => “Copilot” => “Policies”. There you can enable and disable features like:
- Copilot Chat in IDE
- Copilot Chat in GitHub Mobile
- Copilot in the CLI
- sugesstions matching public code <!--SR:!2024-08-08,1,230-->

How do I Grant and manage access for the feature **“Organization-wide policy management”**?
?
**Option 1 Grant Access:** in the “Copilot” settings go to “Access” select “Enable For: all members of the organization” and confirm seat purchase. also possible: “Enable For: Selected members” here assign individually or in bulk via CSV upload
**Option 2 Manage Requests:** Approve or deny access requests in the “Requests from members” section of the “Access” settings

What do the “Audit Logs for Github Copilot” include?
?
Audit logs cover events for the last 180 days. Detailed entries for following events: Seat assignments, Policy updates, Content exklusions and more

How do you access the “Audit Logs for GitHub Copilot”?
?
Go to your profile => “Your organizzations” => “Settings” => on the sidebar under “Archives” => “Logs” => “Audit log”

How do you search in the Audit Log Events?
?
Within the logs you can search by several qualifiers: By Action, By Operation Type, By Repository, By User.

What are Copilot chat skills?
?
Skills are abilities to assist developers in their coding tasks. Core skills are
- Answering Coding Questions
- Writing Code
- Fixing and Improving Code
- Explaining Code
- Generating Tests
- Setting up projects

What are Key features of **”Pull request summeries”**?
?
- Automatic summerization
- Summary Components: Prose Overview, Bulleted lists
- enhanced review efficiency by helping in focusing on critical parts of the code

How does the **”Pull request summaries”** work?
?
**Option 1 Pipeline process:** When a summary is manually requested
**Option 2 Automated:** When creating a pull request, when editing a pull request description or by adding a comment to a pull request

What are limitations of **“Pull request summaries”**?
?
- supports only english currently
- handling very large pull requests
- review the summaries for accuracy and completeness (ethical AI use!)
- Consider it as a supplemental tool as reviewers should add context

What is **“Copilot knowledge base”** aka **Docsets**?
?
Knowledge base adds contextual assistance to the AI’s abilities by using the organizations internal documentation. It is an enterprise feature <!--SR:!2024-08-08,1,230-->

How do you create and manage a **“Copilot knowledge base”**?
?
You do have to have administrative rights within your Organization
Creation: go to your profile => organization settings => Copilot settings => configure knowledge bases.
Configuring: Name your knowledge base and provide a description (optional). Now select the repositories you want to include and apply the selection

How is “Copilot knowledge base” used?
?
**Option 1 Contextual Assistance:** based on your prompt Copilot recognizes to use a knowledge base
**Option 2 Specific mention:** example prompt: @copilot, using the ‘sample 1’ knowledge base, can you explain ...

What are best practices using “Copilot knowledge base”?
?
- Regular Updates
- Feedback Loop (use the feedback option in Copilot)

What does “Zero data retention for code snippets and usage telemetry” mean?
?
**For Code snippets and prompts:** Real-time processing of snippets and prompts which are not stored one a suggestion is returned it is discarded immediately
**Data collection settings:** Users and organizations can control  if prompts and snippets are used for product improvement in the Copilot settings

What telemetry data is collected and used by GitHub for Copilot?
?
- **User engagement data:** metrics include suggestions accepted or dismissed, error rates and feature usage statistics. Does only include specific code content unless enabled in settings
- **Pseudonymous identifiers:** telemetry data is submitted without directly linking personal data

Which security tools can be integrated in Copilot?
?
**Microsoft Copilot for Security:** SecOps AI assistant helps by including potential security threats and providing detailed prompts and suggestions for mitigating this risks
**GitHub Advanced Security(GHAS):** help developers to identify and fi security issues Includes automatic detection and provide coding suggestions
**Audits Logs and Telemetry:** Provide UI based and REST API for organizations to monitor and report Copilot activities to maintain compliance and security standards.


