Documentation on Adding an Agent in Agent Pool
---------------------------------------------------------------------------------

1)	Login to the Azure Devops Portal and navigate to “Project Settings”, under Pipelines click on Agent Pools 
2)	Click on “Add Pool” select “Pool Type” as self-Hosted agents give the name of Agent Pool select the checkbox “Grant access permissions to all pipelines” 
3)	Click on newly added “Agent Pool” and click on “New Agent”
4)	Download the agent into the VM(Virtual Machine)
5)	Create anew folder “agent” in C folder and extract the downloaded zip folder into the C:/agent folder
6)	Open Command Prompt as administrator and give cd c:/agent
7)	PAT(Personal Access Token): Click on User settings icon on the top right of the Azure Portal page. Click on New Token, Given Name of the Token and in Work Items select “Read write and Manage”, Click on “show all scopes” in Agent Pools select “Read and manage” and click on create. The PAT is generated copy it and store
8)	In the Command Prompt give .\config.cmd
9)	Enter the service URL (the organization link) for e.g: https://dev.azure.com/vnaganikhila
10)	Press Enter for PAT authentication type
11)	Enter the PAT Token
12)	Enter the already created agent pool name
13)	Enter the machine name or press enter for default
14)	Press Enter for Work Folder
15)	Press Y to run agent as service/ N for interactive session
    Difference between service/interactive sessions:
    Service: No need to give external commands to make agent online
    Interactive: external command .\run.cmd is required to make agent online
16)	For service session, User authentication is required (press enter)
17)	To prevent service starting immediately after configuration is finished: Press N
18)	Service Agent is added successfully
