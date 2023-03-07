# API-Compliance-Checker
API Security Compliance Checker

The API Security Compliance Checker is a tool for checking the security compliance of an API endpoint based on industry standards such as ISO 27001, PCI-DSS, and HIPAA. This tool can be run on a local machine or integrated into a CI/CD pipeline.

The tool uses the OpenSCAP compliance-checking library to evaluate the security configuration of the API endpoint and determine if it is compliant with the specified standard. If non-compliance issues are found, the tool can attempt to remediate the issues automatically if the user chooses to enable this feature.
Installation

    Install OpenSCAP on your local machine or CI/CD pipeline.
    Clone the repository to your local machine or pull it into your CI/CD pipeline.
    Ensure that Python 3 is installed on your local machine or CI/CD pipeline.
    Install the required Python libraries by running pip install -r requirements.txt.

Usage

To use the API Security Compliance Checker, follow these steps:

    Run the api_compliance_checker.sh script.
    Enter the API endpoint and associated security configuration file path when prompted.
    Select the desired compliance check(s) to perform from the menu.
    If non-compliance issues are found, choose to enable automated remediation if desired.
    Review the compliance check results in the terminal or output file.

Menu Options

The API Security Compliance Checker menu allows you to select which compliance check(s) to perform:

markdown

*****************************************
*         API Compliance Checker         *
*****************************************
* 1. Check compliance against ISO 27001  *
* 2. Check compliance against PCI-DSS    *
* 3. Check compliance against HIPAA      *
* 4. Check compliance in a CI/CD pipeline*
* 5. Exit                                *
*****************************************
Select an option:

    Option 1: Checks compliance against the ISO 27001 standard.
    Option 2: Checks compliance against the PCI-DSS standard.
    Option 3: Checks compliance against the HIPAA standard.
    Option 4: Checks compliance in a CI/CD pipeline against all three standards.
    Option 5: Exits the program.

Output

The API Security Compliance Checker outputs the compliance check results to an XML file for each standard checked. The non-compliance issues are printed to the terminal, and if automated remediation is enabled, the remediation steps taken are also printed.

In a CI/CD pipeline, the tool will exit with a status code of 1 if non-compliance issues are found, allowing the pipeline to fail the build or deployment.
Authors

This project was created by Tadash10.

To install and use the API Security Compliance Checker tool through CLI bash, follow the instructions below:
Installation

    Clone the GitHub repository:

bash

git clone https://github.com/your_username/api-security-compliance-checker.git

    Install OpenSCAP compliance-checking library if it is not already installed:

csharp

sudo apt-get install openscap-utils

    Navigate to the cloned directory:

bash

cd api-security-compliance-checker

Usage

    Execute the script using the command:

bash api_security_compliance_checker.sh

    Follow the prompts to enter the API endpoint and the path to the associated security configuration file.

    The script will check compliance against ISO 27001, PCI-DSS, and HIPAA standards and display the results. If non-compliance issues are found, the script will give the option to attempt automated remediation.

    To run compliance checks in a CI/CD pipeline, use the check_pipeline_compliance() function and pass the relevant standard as an argument.

    To customize the tool for additional compliance standards or add new features, modify the Python script accordingly.

Note: This tool is intended as a starting point for API security compliance checking and should be customized to suit your specific needs and compliance requirements.


