1.	Terraform Runtime :
a.	Download Terraform runtime from Terraform site
 https://releases.hashicorp.com/terraform/
b.	Extract executable and place it under folder ex: C:/Program Files/Terraform
c.	Add executable file path to "PATH" environment variables, so that we can use it from terminal

2.	Terraform Provider
a.	Download Terraform Provider for Cloud2 
 https://artifactory.danskenet.net/artifactory/db-generic-cld2/terraform-provider/latest/terraform-provider-cloud2_Windows-x86_64.zip. 
b.	Place the provider under Your OS Terraform implied local mirror directory, For Windows it is %appdata%/HashiCorp/Terraform/plugins/tfregistry.danskenet.net/cloud2/cloud2/{version}/windows_amd64
cd C:\Users\bc2855\AppData\Roaming    
 
md  HashiCorp\Terraform\plugins\tfregistry.danskenet.net\cloud2\cloud2\{Version}\windows_amd64
      3. Code editor:
               a.Inastll VS Code
               b.Install HashiCorp Terraform - Visual Studio Marketplace plugin to your VS Code. Adds syntax highlighting and other editing features 
      4. Set Credentials (at global)
              a. Set environment variable CLOUD2_API_USER & CLOUD2_API_PASSWORD with your userid and password.
                  If you do not want to set credentials at global and just want to set credentials for that session follow below mentioned RunTimeSetup - SetCredentials procedure. 
      5. Access
               a. User needs to be SPI admin to run Terraform
RunTimeSetup
1.	Set Credentials
a.	Set environment variables from PowerShell using commands $Env:CLOUD2_API_USER="bxxxxx" & $Env:CLOUD2_API_PASSWORD="MySuperSecurePassword"
