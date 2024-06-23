# RFID Signal Blocking

In my previous project **RFID-Testing-and-Cloning**, I showed how to read data from a basic RFID card (e.g. your standard badge that you might use to clock in and out at work etc) and then clone it to another card using a simple $7 RFID tool available at Walmart. To a malicious actor, this would seem to be a fairly easy method to steal personal data by simply tapping the tool on the physical data source, accessing the information and potentially exploiting it for personal gain. While researching more secure alternatives, I suggested some simple options on a surface level to block the RFID signal from malicious actors - for example, the use of protective sleeves.

Coincindentally while doing some house cleaning, I discovered a wonderful piece of memorabilia during my journey in becoming a US Citizen: 

An **Anti-wireless-communication sleeve** that is usually included with Green Cards.

![Card_Blocker_Sleeve](https://github.com/nivvoudit/RFID-Blocking/assets/25519970/88f08fd3-4ecc-4968-811b-74215e9a22c8)

I know, right? At face value, one might say: *"This is literally just a small paper envelope. I can just take a long CVS receipt, cut it up, draw doodles with a sharpie and make a fun side hustle selling identity theft "protection envelopes" on Etsy. Gary Vaynerchuk is going to be so proud of me!"*

Well...in doing some research, I learned that in 2010, the USCIS began issuing "RFID enhanced" Green Cards. As a former greencard holder turned naturalized American citizen, I am aware of the importance of safeguarding such information as that data is *highly* sensitive. This little card holder is a sort of electromagnetically opaque sleeve that shields one's green card from external readers. At a minimum, it will make contactless access to one's RFID more difficult. One user claimed that *"the card holder definitely looks like a standard paper, but it is embedded with a very thin metal foil inside the 2 outside paper layers. I was able to scratch the corners of the paper and was able to see aluminum like thin foil."* 

**Interesting.** Let's test it out!

As previously mentioned, in my experiment **RFID-Testing-and-Cloning** I used a simple $7 RFID reader/writer from Walmart. This time, I'm going to attempt to read the card using a more advanced tool - a Flipper Zero.

![Flipper_Zero2](https://github.com/nivvoudit/RFID-Blocking/assets/25519970/acdc936f-78ba-485c-8acc-8bc9f1c1c42b)

More information about the Flipper Zero is available at https://flipperzero.one/, but in a nutshell, this is a portable multi-tool for pentesters and IT enthusiasts in a toy-like body. It can experiment with a variety of things including radio protocols, access control systems, hardware, and so much more. It's fully open-source and customizable, so you can extend it in whatever way you like. 

Unfortunately, there are currently numerous videos on the internet of people using it maliciously by modifying the public signs of gas prices at various petrol stations (https://www.youtube.com/watch?v=wtHr7x_wT40), using it as a universal remote control to turn off television/screens in public places like restaurants and shopping centers (https://youtube.com/shorts/aRjd-eK2Tqc?si=5WpuzgaUUG2dHQ6v) and even opening up random Tesla car ports (https://youtube.com/shorts/ibe9fjxs2ik?si=hXILEVGkfbND3FE1). 

**Please do not do this sort of stuff.** This is *highly* illegal. As Uncle Ben (and recently, Aunt May) said in Spiderman, **with great power comes great responsibility**. This leads me to my next point:

# Important Note:
*Legal Consequences:*
*Engaging in unauthorized RFID cloning/tampering is illegal and can result in severe penalties, including fines and imprisonment. Laws such as the Computer Fraud and Abuse Act (CFAA) and various state-specific regulations criminalize the unauthorized access and replication of RFID data, aiming to protect individuals and institutions from these disruptive activities. Penalties vary based on the severity of the offense, the extent of damage caused, and the jurisdiction, but they underscore the serious nature of this cybercrime.*
**Understanding the legal ramifications and implementing strong security measures are essential to safeguarding RFID technology from malicious exploitation.**


# My Process
1. I will attempt to read an RFID card using the Flipper Zero using direct physical contact.
2. I will attempt to read the RFID card again using the Anti-wireless-communication sleeve (Greencard sleeve).

# **1. Reading the Source Card with Flipper Zero - direct contact with no protective layer**

![RFID_Blocking_Flipper_Process](https://github.com/nivvoudit/RFID-Blocking/assets/25519970/f3bdf462-687e-47a6-a156-2c44795ba917)



# **2. Attempting to read the Source Card with Flipper Zero - but the source card is now in a protective layer (Anti-wireless communication sleeve aka Greencard sleeve)

![RFID_Blocking_With_Sleeve](https://github.com/nivvoudit/RFID-Blocking/assets/25519970/f3d518da-0eec-43c3-aeb8-e926adb995d2)

I have waited for over 10 minutes and still...the Flipper is unable to read the card in this protective sleeve. 

Can we conclude that this is a veritable solution? Not yet - more testing is required. The rabbit hole grows deeper...

Stay tuned as I explore additional options!






