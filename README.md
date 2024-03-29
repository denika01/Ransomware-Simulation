# Real-World Ransomware Project
![ransomware](https://github.com/denika01/Ransomware-Simulation/assets/152938905/fbde3ba0-eea3-4ac5-bbe6-15b9164c53ae)

# Description
In this project I took on the role of an Information Security Analyst for American International Group, Inc. - AIG.  During the simulation our team received an alert from the Cybersecurity & Infrastructure Security Agency (CISA), about an emerging vulnerability regarding the open source logging software Apache Log4j.

In response to this alert, my job was to research the zero-day vulnerability, then analyze our company's infrastructure list, and draft an email advisery to notify any affected teams.  In addition to informing affected teams, the email was to include a remediation program and assurances to prevent exploitations. 

Although actions were take to prevent exploitation, unfortunately one of our company's servers hosting Log4j was exploited with a ransomware attempt.  Our Incident Detection and Response team was able to stop the ransomware process by cutting off the server's network connection, and immediately powering down the device.  Despite the IDR team's efforts, the encryption process had already started and was able to encrypt important files of the Product Development team, which were not backed up.  As a result, in order to recover the encrypted files, my job was to write a Python script that will brute-force the file and break the encryption.

# Vulnerability Research
![Advisary](https://github.com/denika01/Ransomware-Simulation/assets/152938905/a3faa799-d76d-4799-9775-f766a431616e)

After learning about the Apache Log4j zero-day vulnerability through two publications that CISA released, I then investigated our company's infrastructure to find what devices had the Log4j software installed.  In my investigation I did find that one team did have infrastructure that may have been affected by the vulnerability.  Now having found that there is infrastructure that may have I been affected, my next steps were to contact the team that had ownership of that infrastructure to advise them on steps that needed to be taken in order to protect against that vulnerability.

# Email Advisery

The email advisory that I drafted was sent to the infrastructure owner.  It implicated the seriousness of the vulnerability, the risks/impact that the vulnerability posed if exploited, and steps on how to remediate it.

Below is the template that I used to draft the email advisery:

![Email_Template](https://github.com/denika01/Ransomware-Simulation/assets/152938905/dd762097-1ceb-44ad-9d65-728b0ab91671)

# Breaking the Ransomware Enryption
![ransomware_attack](https://github.com/denika01/Ransomware-Simulation/assets/152938905/ce641c3c-9608-4d12-a394-81237df48439)

Despite the efforts that the IDR team made to stop the ransomware from spreading, it was able to encrypt some important company files that were not backed up.  When dealing with a threat actor, especially in the case of ransomware, there are no guarantees that they will provide a decryption key, that they won't re-encrypt your files, or that they won't come back to attack again and demand more money.  For these reasons our company does not want to pay the ransom.

In order to recover the encrypted files I was tasked with brute-forcing the password to break the encryption.

Below is the Python script that I created for the brute-force: 
![bf_script](https://github.com/denika01/Ransomware-Simulation/assets/152938905/2f2c818b-c5b6-4d19-9c7c-0ec21145aaf1)

In the end I was glad to report that after running my brute-force script on the encrypted file, we were able to break the encryption and recover the company files!!

# Conclusion
I really enjoyed carrying out this project, taking on the role as an Information Security Analyst.  Through this project I was able to practice some of my existing skills,  and I also developed some new skills. Specifically the skills that I practiced and developed were:

 * Researching and reviewing CISA publications on known vulnerabilities
 * Reporting vulnerabilities by drafting clear and concise emails to guide teams on vulnerability awareness and remediation
 * Utilizing Python skills to write a script for ethical hacking, avoiding ransom payments by bruteforcing decryption keys
