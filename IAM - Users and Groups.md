# Permissions
 Users and groups can be assigned JSON docs called policies.
 - These policies define permissions of the users

# Policies
## Policies inheritance
![[Pasted image 20251223211322.png]]
## Policies Structure
![[Pasted image 20251223212129.png]]
- Consists of
	- **Version**: policy language version, always include "2012-10-17"
	- **id**: an identifier for the policy (optional)
	- **Statement**: one or more individual statements
- Statements consist of
	- **Sid**: and identifier for the statement (optional)
	- **Effect**: whether the statement allows or denies access (Allow, Deny)
	- **Principal**: account/user/role to wich this poliy applied to
	- **Action**: list of actions this policy allows or denies
	- **Resource**: list of resources to wich the actions applied to
	- **Condition**: conditions for when this policy is in effect (optional)
## Password Policy
- Strong passwords = higher security for your account
- In AWS, you can setup a password policy.

# Access AWS
Three options:
- AWS Management Console WEB
- AWS Command Line Interface (CLI): with access keys
- AWS Software Developer Kit (SDK)
## Access Keys
![[Pasted image 20251223214518.png]]
## CLI
Tool that enavles you to interact with AWS services using commands in your command-line shell
- Direct access to the public APIs of AWS services
- You can develop scripts to manage your resources
- Its open source
- ![[Pasted image 20251223214657.png]]
## SDK
Software Development Kit (AWS SDK)
Language.specific APIs (set of libraries)
Enables you to access and manage AWS services programmatically
Embedded within your application
Supports
- SDKs (JavaScript, Python, PHP, .NET, Ruby, Java, Go, Node.js, C++)
- Mobile SDKs (Android, iOS)
- IoT Device SDKs (Embedded C, Arduino)
- Example AWS CLI is built on AWS SDK for Python