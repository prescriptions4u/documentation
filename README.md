README for prescriptionsforyou
==========================

##Simplified Use Case


User generates wallet. Wallet must be configured so that it can only be operated with 2 private keys.
 2 keys are generated for the wallet.
 Doctor gets privateKey 1
 Pharmacy gets privateKey 2
    
    PublicKey, DOB, Address, Name is stored on both of DBs along with Private key

Person visits doctor, gets prescription.
Carries ID, woith Name, DOB, Addr, etc..
Doctor looks up public key.
With public key, Doctor puts token into user's wallet.
Prints prescription:
    Name, DOB, Addr
    Patient's publicKey
    Doctor's publicKey
    
    PrivateKey1 at the bottom
    
User brings prescription to Pharmacy
User scans publicKey and privateKey1 in Pharmacy PC


Pharmacist frontend displays info on patient:
    Name, DOB, Address
    
Pharmacist checks data (Name, etc..)
Pharmacist enters privateKey2 for user's private wallet
Coin gets transferred to Pharmacy wallet
Pharmacist checks blockchain for "suspicious activity"
If "OK"
    Provide medication
Else
    ..... ?!!?!
End

Pharmacy sends coin to Doctor's wallet.
Pharmacist keeps paper prescription.
User receives prescription    

