AZURE RESOURCE MANAGER
Azure Resource Manager enables you to work with the resources in your solution as a group. You can deploy, update, or delete all the resources for your solution in a single, coordinated operation.

-Consistent Management Layer
Azure Resource Manager provides a consistent management layer to perform tasks through Azure PowerShell, Azure CLI, Azure portal, REST API, and client SDKs.


Terminology
-resource
-resource group
-resource provider
-template
-declarative syntax

-Resource Providers
Before deploying your resources, you should gain an understanding of the available resource providers. Knowing the names of resource providers and resources helps you define resources you want to deploy to Azure. Also, you need to know the valid locations and API versions for each resource type. 
The name of a resource type is in the format: {resource-provider}/{resource-type}. For example, the key vault type is Microsoft.KeyVault/vaults.

-Resource Groups
When creating a resource group, you need to provide a location for that resource group.
The resource group stores metadata about the resources. Therefore, when you specify a location for the resource group, you're specifying where that metadata is stored. For compliance reasons, you may need to ensure that your data is stored in a particular region.

By scoping permissions to a resource group, you can add/remove and modify resources easily without having to recreate assignments and scopes.

Azure Resource Manager Locks
Read-Only
Delete

Move Resources
Just because a service can be moved doesn’t mean there aren’t restrictions. For example, you can move a virtual network, but you must also move its dependent resources, like gateways.

Remove Resource Groups
-Pwhs for delete
Remove-AzResourceGroup -Name "ContosoRG01"


AZURE CLOUD SHELL
Azure Cloud Shell is a command-line environment you can access through your web browser. You can use this environment to manage Azure resources, including VMs, storage, and networking. Just like you do when using the Azure CLI or Azure PowerShell.

--Cloud Shell Tools--
Category	Name
Linux tools	bash
	zsh
	sh
	tmux
	dig
Azure tools	Azure CLI and Azure classic CLI
	AzCopy
	Azure Functions CLI
	Service Fabric CLI
	Batch Shipyard
	blobxfer
Text editors	code (Cloud Shell editor)
	vim
	nano
	emacs
Source control	git
Build tools	make
	maven
	npm
	pip
Containers	Docker Machine
	Kubectl
	Helm
	DC/OS CLI
Databases	MySQL client
	PostgreSql client
	sqlcmd Utility
	mssql-scripter
Other	iPython Client
	Cloud Foundry CLI
	Terraform
	Ansible
	Chef InSpec
	Puppet Bolt
	HashiCorp Packer
	Office 365 CLI


BASH
Bash is a vital tool for managing Linux machines. The name is short for "Bourne Again Shell."
A shell is a program that commands the operating system to perform actions. You can enter commands in a console on your computer and run the commands directly, or you can use scripts to run batches of commands. Shells like PowerShell and Bash give system administrators the power and precision they need for fine-tuned control of the computers they're responsible for.

Bash Fundamentals
Syntax for Bash commands
     command [options] [arguments]
"ls" for list command to display the contents of the current working directory. "ls /etc"

Most Bash commands have options for modifying how they work. Options, also called flags, give a command more specific instructions. As an example, files and directories whose names begin with a period are hidden from the user and aren't displayed by ls. However, you can include the -a (for "all") flag in an ls command and see everything in the target directory:
" ls -a /etc "

-Wildcards
Wildcards are symbols that represent one or more characters in Bash commands. The most frequently used wildcard is the asterisk. It represents zero characters or a sequence of characters. Suppose your current directory contains hundreds of image files, but you only want to see the PNG files; the ones whose file names end with .png. Here's the command to list only those files:
" ls *.png "

Now let's say the current directory also contains JPEG files. Some end in .jpg, while others end in .jpeg. Here's one way to list all the JPEG files:
" ls *.jp*g "

Linux has no formal concept of a file-name extension as other operating systems do. This doesn't mean that PNG files won't have a .png extension. It simply means Linux attaches no special significance to the fact that the file names end with .png.

If you need to use one of the wildcard characters as an ordinary character, you make it literal or "escape it" by prefacing it with a backslash. So, if for some reason you had an asterisk as part of a file name—something you should never do intentionally—you could search for it by using a command such as:
" $ ls *\** "

Bash Commands
	- ls
	- cat
	- sudo
	- cd
	- mkdir
	- rm, rmdir
	- cp
	- ps
	- w
Bash I/O Commands
	- <
	- >
	- >>
	- |
	

POWERSHELL
PowerShell is a command-line shell and a scripting language all in one. It was designed as a task engine that uses cmdlets to wrap tasks that people need to do. In PowerShell, you can run commands on local or remote machines. You can do tasks like managing users and automating workflows.

-Get-Command: The "Get-Command" cmdlet lists all of the available cmdlets on your system. Filter the list to quickly find the command you need.
-Get-Help: Run the "Get-Help" core cmdlet to invoke a built-in help system. You can also run an alias "help" command to invoke "Get-Help" but improve the reading experience by paginating the response.
-Get-Member: When you call a command, the response is an object that contains many properties. Run the "Get-Member" core cmdlet to drill down into that response and learn more about it.


