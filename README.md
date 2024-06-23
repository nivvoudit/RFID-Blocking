# RFID Signal Blocking

In my previous project **RFID-Testing-and-Cloning**, I showed how to read data from a basic RFID card and then clone it to another card using a simple $7 RFID tool available at Walmart. To a malicious actor, this would seem to be a fairly easy method to steal personal data by simply tapping the tool on the physical data source, accessing the information and potentially exploiting it for personal gain. While researching more secure alternatives, I suggested some simple options on a surface level to block the RFID signal from malicious actors - for example, the use of protective sleeves.

Coincindentally while doing some house cleaning, I discovered a wonderful piece of memorabilia during my journey in becoming a US Citizen: 

An **Anti-wireless-communication sleeve** that is usually included with Green Cards.

![Card_Blocker_Sleeve](https://github.com/nivvoudit/RFID-Blocking/assets/25519970/88f08fd3-4ecc-4968-811b-74215e9a22c8)

I know, right? At face value, one might say: *"This is literally just a small paper envelope. I can just take a long CVS receipt, cut it up, draw doodles with a sharpie and make a fun side hustle selling identity theft "protection envelopes" on Etsy."*
While doing some research, I learned that in 2010, the USCIS began issuing "RFID enhanced" Green Cards. As a former greencard holder turned naturalized American citizen, I am aware of the importance of safeguarding such information as it is highly sensitive. 
This little card holder is a sort of electromagnetically opaque sleeve that shields one's green card from external readers. At a minimum, it will make contactless access to one's RFID more difficult. One user claimed that *"the card holder definitely looks like a standard paper, but it is embedded with a very thin metal foil inside the 2 outside paper layers. I was able to scratch the corners of the paper and was able to see aluminum like thin foil."* 

**Interesting.** Let's test it out!

As previously mentioned, in my experiment **RFID-Testing-and-Cloning** I used a simple $7 RFID reader/writer from Walmart. This time, I'm going to attempt to read the card using a more advanced tool - a Flipper Zero.

![Flipper_Zero2](https://github.com/nivvoudit/RFID-Blocking/assets/25519970/acdc936f-78ba-485c-8acc-8bc9f1c1c42b)

More information about the Flipper Zero is available at https://flipperzero.one/, but in a nutshell, this is a portable multi-tool for pentesters and IT enthusiasts in a toy-like body. It can experiment with a variety of things including radio protocols, access control systems, hardware, and so much more. It's fully open-source and customizable, so you can extend it in whatever way you like. 

Unfortunately, there are currently numerous videos on the internet of people using it maliciously by modifying the public signs of gas prices at various petrol stations (https://www.youtube.com/watch?v=wtHr7x_wT40), using it as a universal remote control to turn off television/screens in public places like restaurants and shopping centers (https://youtube.com/shorts/aRjd-eK2Tqc?si=5WpuzgaUUG2dHQ6v) and even opening up random Tesla car ports (https://youtube.com/shorts/ibe9fjxs2ik?si=hXILEVGkfbND3FE1). 

**Please do not do this sort of suff** This is highly illegal. As Uncle Ben (and recently, Aunt May) said in Spiderman, **with great power comes great responsibility**. This leads me to my next point:

# Important Note:
*Legal Consequences:*
*Engaging in unauthorized RFID cloning/tampering is illegal and can result in severe penalties, including fines and imprisonment. Laws such as the Computer Fraud and Abuse Act (CFAA) and various state-specific regulations criminalize the unauthorized access and replication of RFID data, aiming to protect individuals and institutions from these disruptive activities. Penalties vary based on the severity of the offense, the extent of damage caused, and the jurisdiction, but they underscore the serious nature of this cybercrime.*
**Understanding the legal ramifications and implementing strong security measures are essential to safeguarding RFID technology from malicious exploitation.**



# My Process
1. I will attempt to read an RFID card using the Flipper Zero using direct physical contact.
2. I will attempt to read the RFID card again using the Anti-wireless-communication sleeve (Greencard sleeve).

# **Reading the Source Card with Flipper Zero**......**SUCCESS!**


Now that we have captured the data from the source card, let's see if we can write it to a card of a similar type. 


# **Writing data from the source card to a CLONE card**.....**SUCCESS!**
![RFID_Write](https://github.com/nivvoudit/RFID_Testing/assets/25519970/18befdff-4106-412e-90d9-58907807e029)


For the purposes of this demonstration, I used a blank, similar RFID card. 

# However...

**There are also many different types of writeable media available e.g. key fobs, tags, wristbands and so forth - from travel cards, concert/event tags, to even medical patient wristbands.**

![OtherTypes](https://github.com/nivvoudit/RFID_Testing/assets/25519970/bcab6dd7-1418-40e7-9a69-964bd7b92e1e)


There was even a case where someone creatively turned his RFID chip into a wand (while dressed as Gandalf from Lord of the Rings), tapping his wand on the card readers to access travel:

![Wand_Clone_RFID](https://github.com/nivvoudit/RFID_Testing/assets/25519970/e6ef4f45-ad6a-42ae-a24e-f4cf1038530b)


# The Risks of RFID Cloning:
Radio Frequency Identification (RFID) technology is widely used in various sectors due to its convenience and efficiency in tracking and authenticating items and individuals. However, the ability to easily read and clone RFID devices poses significant cybersecurity risks, potentially causing severe disruptions in critical areas such as travel, banking, and healthcare.

**Travel**: RFID technology is commonly used in passports and boarding passes. Cloning these RFID tags can allow malicious actors to bypass security checks, leading to unauthorized access to secure areas, identity theft, and even the trafficking of illicit goods. Such breaches can compromise the safety of travelers and the integrity of border control systems.

**Banking**: Contactless payment cards and keycards utilize RFID technology for quick and secure transactions. Cloning these cards can lead to unauthorized access to financial accounts, resulting in significant financial losses for individuals and institutions. Furthermore, it undermines the trust in contactless payment systems, impacting the overall security of financial transactions.

**Medical**: RFID tags are used in patient identification, medical equipment tracking, and pharmaceutical management. Cloning these tags can result in severe consequences, including incorrect patient treatment, unauthorized access to medical facilities, and the distribution of counterfeit medications. This not only jeopardizes patient safety but also disrupts the integrity of healthcare services.

As RFID technology continues to integrate into our daily lives, it is crucial to address its vulnerabilities and implement robust security measures to prevent cloning and unauthorized access. Ensuring the integrity and security of RFID systems is essential to protect sensitive information and maintain trust in these critical sectors.

# Available Solutions

There are currently available solutions to protect malicious actors from cloning RFID devices. Most of these solutions involve a physical, protective layer surrounding the RFID source:

![Solutions](https://github.com/nivvoudit/RFID_Testing/assets/25519970/565ee377-3aeb-4b00-990d-40b452b31ae6)

# More secure alternatives

I will explore more secure, alternative solutions in upcoming projects including cards using different technologies (e.g. MiFare EV2). Stay tuned and thanks for reading!




