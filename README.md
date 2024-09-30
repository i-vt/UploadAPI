# UploadAPI
Simple SpringBoot API with following functions:
- upload files with a UUID to validate the upload
- one UUID = one 10MB upload.
- UUIDs get "used" after one upload, rejecting further uploads

## Setup
1. Verify dependencies are met (Java, Gradle, & etc.)
2. Download the boilerplate code setup from [here](https://github.com/i-vt/SpringBootTemplate/)
3. Copy-paste this repo files on top of the boilerplate files (replacing them if needed)
4. Change default H2 password (optional disable H2 public page)
5. Test it
6. (Optional) ChatGPT whatever tf broke in the process

## Testing
Upon bootup (bootRun) UUID's are supplied in the running terminal:
```
Initialized tokens: 
UUID: 82b5ee60-c6dd-4f82-a102-c9a2ba357129
UUID: f94867fd-bc11-465e-ae8e-d46f410af79a
UUID: 6a19b543-6c64-40b1-af1a-196b33ac38dc
UUID: ba4aac4f-5c22-456a-875c-12ec3766ca27
UUID: 21134c2b-45d4-46c0-b9e3-f2a21a78d2e0
[...]
```

Testing it with curl:
```
curl -X POST "http://localhost:8080/api/v1/upload"
      -F "file=@/home/user/TESTFILES/test.txt"
      -F "uuid=82b5ee60-c6dd-4f82-a102-c9a2ba357129"
File uploaded successfully: test.txt
```



## Disclaimer for "UploadAPI":

### Summary:
Exercise responsibility and abide by legal standards while using this software. Unauthorized penetration testing is prohibited and illegal.

### In depth:

- General Use: This software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
- Potential Misuse: The software is designed for legitimate purposes only. Any misuse, including but not limited to illegal, unethical, or unauthorized activities, is strictly discouraged and not the intention of the developers.
- User Responsibility: Any person, entity, or organization choosing to use this software bears the full responsibility for its actions while using the software. It is the user's responsibility to ensure that their use of this software complies with local, state, national, and international laws and regulations.
- No Liability: The creators, developers, and distributors of this software are not responsible for any harm or damage caused, directly or indirectly, by the misuse or use of this software.
- Updates and Monitoring: The developers reserve the right to update, modify, or discontinue the software at any time. Users are advised to always use the most recent version of the software. However, even with updates, the developers cannot guarantee that the software is completely secure or free from vulnerabilities.
- Third-Party Software/Links: This software may contain links to third-party sites or utilize third-party software/tools. The developers are not responsible for the content or privacy practices of those sites or software.
- Unauthorized Access: Using "UploadAPI" to access, probe, or connect to systems, networks, or data without explicit permission from appropriate parties is strictly discouraged, unethical, and illegal. Unauthorized access to systems, networks, or data breaches various local, national, and international laws, and can result in severe legal consequences. Always obtain the necessary permissions before accessing any systems or data. The developers of "UploadAPI" disavow any actions taken by individuals or entities that use this software for unauthorized activities.

By downloading, installing, or using "UploadAPI" you acknowledge that you have read, understood, and agreed to abide by this disclaimer. If you do not agree to these terms, do not use the software.
