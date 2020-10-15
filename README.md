# UVMS-USM-Overlay
Overlay project for the UVMS-USM project.

# Build Process  
Patches UVMS-USM generated artifacts with custom code:
1. It downloads the UVMS-USM source code
2. Unpacks it
3. Replaces source files
4. Builds it

# Generated Artifacts
It generates the following artifacts:
* eu.europa.ec.fisheries.uvms:Administration-http-Rest-Service-overlay (instead of eu.europa.ec.fisheries.uvms:Administration-http-Rest-Service that UVMS-USM generates): It is called by UVMS-Frontend project to retrieve users features and context from the security context that EU Login has populuated (instead of decoding the JWT security token that USM has created). 
