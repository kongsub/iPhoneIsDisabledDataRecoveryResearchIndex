# Collect information for all whose iPhone "is disabled,Connect to iTunes" Locked and want recover data

# Introduction : The extreme insecure in the extreme secure  
+ iPhone have special mechanism design "**permanent lock data if 10 times incorrect passcode attempt**" and **SEP** (Secure Enclave Processor) to make iPhone more **secure**.  
+ "**permanent lock data if 10 times incorrect passcode attempt**" means the after 10 times incorrect passcode attempted , your data lost forever. There is an option in iOS perference , **erase** it or not . but even you don't enable **erase** , after 10 times incorrect attempts, your iPhone is permanent disabled until you erase all data and reset it by iTunes then restore something from backup. Apple doesn't provide keep data re-enable service official way.  
+ It means that your data never back if you have no backup before , or even you have backup , the new data after backup still lost.  
+ So **iPhone's secure** just means it guarantee the data not be read by someone without permission , it not guarantee the data not be remove in unwanted way.  
+ In these scenarios , iPhone is **insecure** totally .  
   - a. You always unlock your phone by "Touch ID" or "Face ID" . but one day , these unlock systems not work , and you forgot passcode after a long time not use it.
   - b. You put your iPhone on desktop , some children want unlock your phone for play games , but failed.  
   - c. You record a crime or accident scene , but someone don't want the record exists , just need "10 times attempts".  
+ iPhone's special mechanism design prevent the data **can't be read** in **extreme secure** way , but make the data **can't be delete** in **extreme insecure** .  
+ Then , to know how to recover data on "disabled" iPhone is necessary .  
  
# F**k Apple!The problem may cause by hardware!  
Wrong passcode problem may cause by the design of iPhone and NFC . If so your phone may only fix by hardware.  
  
> Because Apple really put security is highest priority. The NFC is reporting directly to CPU, the communication of CPU and NFC is encrypted.
> If the NFC is not responding or somehow it failed to work, the CPU will tell the iOS to protect all the data by not letting anyone access the iOS.  
  
See here : https://www.iphone-repair.my/iphone/iphone-passcode-loop-fix/


# Problem at present  
## Only a few "disabled" iOS-device can be re-enable by paid  
https://checkm8.info provides a paid software for passcode lock screen removal , but it only for 12.3 – 13.x.x and 14.0 .  
  
## Jailbreak "disabled" iPhone by checkra1n , only can read part of files  
checkra1n (https://checkra.in) 0.11.0 beta can jailbreak 12.0 - 13.7 . it unlocked USB connection and provide SSH connect , but can't access important many files (e.g /private/var/mobile/Media/DCIM/* )  
  
# Resources  
## Projects  
### Jailbreak core
+ [ipwndfu] 
+ [checkra1n]
+ [Fugu]
+ [Clutch]
+ [Undecimus]

## Understanding iOS
### Application
+ PDF: [Hacking and Securing iOS Applications]
### SEP
+ PDF: [Attack Secure Boot of SEP]
+ PDF: [Demystifying the Secure Enclave Processor]
+ PDF: [(Presentation)Demystifying the Secure Enclave Processor]
+ PDF: [Apple Secure Key Store Cryptographic Module, v1.0 FIPS 140-2 Non-Proprietary Security Policy]
+ [Data Storage on iOS]
### SpringBoard
+ [Reverse-Engineering the iPhone X Home Indicator Color]
+ Q&A: [Restart Springboard without locking screen?] (**This method no longer work in iOS 5.x**)
### System
+ [darwin-XNU]
#### Boot
+ [\*OS:iBoot]
### File System
+ [APFS FUSE Driver for Linux]
### iOS 12
+ https://github.com/ichitaso/iOS-12.0-12.1.2-SpringBoard-Headers
+ https://github.com/nst/iOS-Runtime-Headers

## Debug
### Hardware
[Debugging an iPhone with Bonobo JTAG cable + OpenOCD + GDB demoted by checkm8]


[ipwndfu]: https://github.com/axi0mX/ipwndfu
[checkra1n]: https://github.com/checkra1n/
[Fugu]: https://github.com/LinusHenze/Fugu
[Hacking and Securing iOS Applications]: http://index-of.es/Hack/Oreilly.Hacking.and.Securing.iOS.Applications.Jan.2012.pdf
[Attack Secure Boot of SEP]: https://raw.githubusercontent.com/windknown/presentations/master/Attack_Secure_Boot_of_SEP.pdf
[Demystifying the Secure Enclave Processor]: http://mista.nu/research/sep-paper.pdf
[(Presentation)Demystifying the Secure Enclave Processor]: https://www.blackhat.com/docs/us-16/materials/us-16-Mandt-Demystifying-The-Secure-Enclave-Processor.pdf
[Restart Springboard without locking screen?]: https://stackoverflow.com/questions/1764492/restart-springboard-without-locking-screen/2021332
[Data Storage on iOS]: https://mobile-security.gitbook.io/mobile-security-testing-guide/ios-testing-guide/0x06d-testing-data-storage
[Apple Secure Key Store Cryptographic Module, v1.0 FIPS 140-2 Non-Proprietary Security Policy]: https://csrc.nist.gov/CSRC/media/projects/cryptographic-module-validation-program/documents/security-policies/140sp3223.pdf
[Reverse-Engineering the iPhone X Home Indicator Color]: https://medium.com/@nathangitter/reverse-engineering-the-iphone-x-home-indicator-color-a4c112f84d34
[Clutch]: https://github.com/KJCracks/Clutch
[Debugging an iPhone with Bonobo JTAG cable + OpenOCD + GDB demoted by checkm8]: https://www.youtube.com/watch?v=3zpwSUXlz6A
[Undecimus]: https://github.com/pwn20wndstuff/Undecimus
[\*OS:iBoot]: http://newosxbook.com/bonus/iBoot.pdf
[darwin-XNU]: https://github.com/apple/darwin-xnu
[APFS FUSE Driver for Linux]: https://github.com/sgan81/apfs-fuse
