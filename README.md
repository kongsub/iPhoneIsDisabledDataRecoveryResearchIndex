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
## Understanding iOS
### Application
+ PDF: [Hacking and Securing iOS Applications]
### SEP
+ PDF: [Attack Secure Boot of SEP]
+ PDF: [Demystifying the Secure Enclave Processor]

[ipwndfu]: https://github.com/axi0mX/ipwndfu
[checkra1n]: https://github.com/checkra1n/
[Fugu]: https://github.com/LinusHenze/Fugu
[Hacking and Securing iOS Applications]: http://index-of.es/Hack/Oreilly.Hacking.and.Securing.iOS.Applications.Jan.2012.pdf
[Attack Secure Boot of SEP]: https://raw.githubusercontent.com/windknown/presentations/master/Attack_Secure_Boot_of_SEP.pdf
[Demystifying the Secure Enclave Processor]: http://mista.nu/research/sep-paper.pdf
