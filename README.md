# <div align="center">Snify</div>
<div align="center">
</div>
<p>

Snify is a Python based tool designed to scan Android applications (APK files) for security vulnerabilities. It specifically targets the OWASP Top 10 mobile vulnerabilities, providing an easy and efficient way for developers, penetration testers, and security researchers to assess the security posture of Android apps.

![Model](https://github.com/ValdyFox/Snify/blob/main/Screenshot%202025-02-07%20103324.png)





## Features

Snify is a Python-based tool that performs various operations on APK files. Its main features include:

- **APK Analysis** -> Scans Android application package (APK) files for security vulnerabilities.
- **OWASP Coverage** -> Covers OWASP Top 10 vulnerabilities to ensure a comprehensive security assessment.
- **Advanced Detection** -> Utilizes custom python code for APK file analysis and vulnerability detection.
- **Sensitive Information Extraction** -> Identifies potential security risks by extracting sensitive information from APK files, such as insecure authentication/authorization keys and insecure request protocols.
- **In-depth Analysis** -> Detects insecure data storage practices, including data related to the SD card, and highlights the use of insecure request protocols in the code.
- **Intent Filter Exploits** -> Pinpoint vulnerabilities by analyzing intent filters extracted from AndroidManifest.xml.
- **Local File Vulnerability Detection** -> Safeguard your app by identifying potential mishandlings related to local file operations
- **Report Generation** -> Generates detailed and easy-to-understand reports for each scanned APK, providing actionable insights for developers.
- **CI/CD Integration** -> Designed for easy integration into CI/CD pipelines, enabling automated security testing in development workflows.
- **User-Friendly Interface** -> Color-coded terminal outputs make it easy to distinguish between different types of findings.

## Installation

To use Snify, make sure you have Python 3.10 (recommended) or higher installed, along with Java or OpenJDK. Once those are set up, you can install Snify by running the following command:
### For Linux
```
git clone https://github.com/d78ui98/Snify.git
cd /Snify
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python Snify.py --help
```
### For Windows
```
git clone https://github.com/d78ui98/Snify.git
cd \Snify
python3 -m venv venv
.\venv\Scripts\activate
pip install -r .\requirements.txt
python Snify.py --help
```

## Usage

To simply scan an APK, use the below command. Mention the apk file with `-apk` argument. 
Once the scan is complete, a detailed report will be displayed in the console.

```
python3 Snify.py -apk file.apk
```

If you've already extracted the source code and want to provide its path for a faster scan you can use the below command.
Mention the source code of the android application with `-source` parameter.
 
```
python3 Snify.py -apk file.apk -source <source-code-path>
```
To generate detailed PDF and HTML reports after the scan you can pass `-report` argument as mentioned below.
```
python3 Snify.py -apk file.apk -report
```


For those interested in contributing code, please follow the standard GitHub process.
We'll review your contributions as quickly as possible :)

