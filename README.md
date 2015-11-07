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
	Medication and dosage
    Patient's publicKey
    Doctor's privateKey1
    ------ detach section -------
    PrivateKey1 at the bottom
    
User brings prescription to Pharmacy
User scans publicKey and privateKey1 in Pharmacy PC


Pharmacist frontend displays info on patient:
    Name, DOB, Address
    
Pharmacist checks data (Name, etc..)
Pharmacist enters privateKey2 for user's private wallet
Coin gets transferred from Patient's wallet to Pharmacy wallet
Coin gets transferred from Pharmacy wallet to Doctor's wallet
Pharmacist checks blockchain for "suspicious activity"
If "OK"
    Provide medication
Else
    ..... ?!!?!
End

Pharmacist keeps paper prescription.
User receives medication

