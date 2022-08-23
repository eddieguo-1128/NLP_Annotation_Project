# Annotation Guidelines
*Authors: Yifei Yin, Eddie Guo, Siqi Wu*

## Introduction
Both buyers and sellers on Amazon rely on reviews to align their expectations with the actual product. Customers read reviews for detailed information about the product, while sellers use reviews to collect feedback on their products and make adjustments. In this project, we are only interested in annotating the degree of constructiveness of Amazon PC product reviews from the sellers’ perspective. PC products in the review include laptops, tablets, computer, phone and tablet cases, adapter, mouse, keyboard, monitor, modem routers and other electronic devices and peripherals. 

A constructive review is clear and factual, aiming at helping the seller/manufacturer to achieve a better outcome. It should also be detailed, specific, and honest, recognizing the pros and cons of product design and functionality and pinpointing areas for potential improvements. A non-constructive review could be opinionated without supporting evidence, or lacking insights for the seller/manufacturer to take responsible actions. 

## Basic Concepts
Since most of us are more familiar with the role of a customer than a seller/manufacturer, we have provided the following definitions to clarify the differences between “helpfulness” and “constructiveness”.
- **“Helpfulness”**: The amount of information a customer could extract from a piece of review that aids their purchasing decision. Note that “helpfulness” is determined by the “helpful vote” button in Amazon’s review section and encoded in the “helpfulness” column in the original data. Please read more in the “Text to Annotate” section below to see how we controlled “helpfulness” for this project. 
- **“Constructiveness”**: The amount of feedback the seller/manufacturer could extract from a piece of review that directs their decision in whether to continue the product, and if so, how to improve it in the future. Note that a constructive review could be positive, negative, or both. Please read more in the “Text to Annotate” section below to see how we controlled “star ratings” for this project. 

## Detailed Guidelines
“Constructiveness” is annotated in a spectrum between 0 to 5, with 0 being not constructive at all and 5 being the most constructive. To make “constructiveness” measurable, we have defined it in the following five categories, and a review gets one point by hitting each of the five categories: 

- **The review comments on the pro and/or con of the product’s design (eg.  size, fit, color, weight, construction etc).**
  - “I found it too big and bulky.” **[size]**
  - “The cover is okay to use, but does not fit perfectly around my Macbook Pro 13 inch Retina Display.” [fit]
  - “USB sound card fits snugly in the USB jack.” **[fit]**
  - “Seems the plastic used in this application is too brittle and does not flex with the movement of the device - certainly a design flaw.” **[fit]**
  - “If you are buying this product for the color, the product is NOT the color at all.” **[color]**
  - “Sturdy-ish construction.” **[construction]**
  - “It looks less streamlined and more plasticky.” **[construction]**
  - “Life is indeed better with a very very lightweight and thin laptop.” **[weight]**

- **The review comments on the pro and/or con of the product’s feature/functionality. (eg. battery life, cell service reception, compatibility, durability, etc). Functionality and features vary for different product groups.**
  - “Perhaps this is how solid state units behave, but my Outlook feels as heavy as it felt in my previous 5-year old Toshiba with 7200 rpm HDD.” **[laptop functionality]**
  - “The sound is impressive for its (tablet) size.” **[tablet functionality]**
  - “The cable works as it is supposed to and displays great video.” **[cable functionality]**
  - “I really like the lighted keyboard and the larger letters and numbers.” **[keyboard functionality]**
  - “Good access to all ports etc.” **[case functionality]**
  - “It has two ziplocs, and the bottom rolls up and snaps shut.” **[case functionality]**
  - “Although I wish it was not just a decorative case and actually added some protection for the phone!” **[case functionality]**
  - “However, it (battery) does not have the same capacity as the original.” **[battery functionality]**
  - “This unit is INCOMPATIBLE with the iPad air 2.” **[card reader functionality]**

- **The review comments on the pro and/or con of the product’s material/internal/external parts (eg. CPU, keyboard, display, warranty,  memory/storage, operating system, software and apps). To note that, for a laptop, display and keyboard are considered as externals. For a keyboard, however, its externals include cables and USB jack etc.**
  - “There was supposed to be a 3 year warranty and when I registered it there was only 27 months given to me.” **[warranty]**
  - “After shelling out $500 for the product, at release, finding out after the fact I needed $70 in software to be able to use most video, browser, and podcast content, left me feeling swindled.” **[internal]**
  - “I put 10 mp3s on it and the unit froze every time I tried playing them.  Then I reduced it to 1 mp3 to see if it could process that.”[internal]
  - “The operating system is good.” **[internal]**
  - “It holds the max storage most phones/devices can accommodate.” **[internal]**
  - “The tablet is good value and has a good screen with HD quality look.” **[external]**
  - “The usb cord (of a fan) plugs in from the back and the wide part sticks out so when I placed it down at an angle it broke.” **[external]**
  - “That is because it did not take long for the clip on the back of the bar to break off, preventing it (sound bar) from being mounted onto the screen.” **[external]**

- **The review provides details on user experience/scenario that adds more information to one or more of the previous three points, or shares user experience with the installation process, customer support, shipping/return services, and opinion on product value.**
  - “The instructions were rather vague.” **[instructions]**
  - “The battery drains quickly, especially when it’s cold outside.” **[experience/scenario on functionality]**
  - “You can’t beat the price.” **[product value]**
  - “No user manual that I could find online, just a quick start guide.” **[instructions]**
  - “Also noticed that unless the tablet is repositioned each time before taking a picture, the cut out for the rear facing camera on the back cover causes there to be a black line on the side of the picture.” **[experience/scenario on functionality]**
  - “The problem is the static that develops when you remove the protective plastic backing before you apply the protector to the screen.” **[experience/scenario on functionality]**
  - “I'm giving it 3 stars because the Samsung cloning software could not detect the drive if connected to a USB 3 port, I had to use the slow USB 2 instead.” **[experience/scenario on a internal part]**
  - “I live in Austin, I'm not sure how well the antenna would work when we go out of town or out camping somewhere.” **[experience/scenario on a external part]**
  - “A bit disappointed with their customer relations.” **[customer support]**

- **The review provides suggestions for improving/keeping the quality of the product in regards to its design, feature/functionality, or material/internal/external parts.**
  - “If they would put  a hole in the face cover to expose the camera lens when the cover is folded back it would be great.”
  - “Wish the description was more clear about what the product was specifically for.....it didn't say it would not fit the newest kindle reader.”
  - “Please if you are reading, make an app that will allow for making notes and comments within the text.”
  - “ If you aren't going to use real leather, don't pretend, you aren't fooling anyone.”
  - “Hopefully they will release firmware that addresses this shortcoming.”
  - “PLEASE MR VENDOR,,, respond to mails!!! get some coverage to customers!! upgrade your platforma,,, respond to blogs!!!”

*Note: If a review is unrelated to specifics about the product, it receives a 0.*
- “Good adapter, would buy again”
- “A necessity for American Red Cross FRX3 Hand Crank NOAA AM/FM Weather Alert Radio.”
- “I think it is over priced.”
- “Received the wrong item.”

## Text To Annotate
One important note is that a review which helps customers make purchasing decisions may not necessarily provide useful feedback for the seller. For example, if a review says “I own another PC from xx, but this one works better”, a potential customer may find the insights on user experience and the comparison with a substitute helpful, but the review does not help the seller improve the product as it lacks details about specific features. Therefore, to avoid confusing “helpfulness” with “constructiveness”, we controlled “helpfulness” (by selecting reviews that reflect similar levels of helpfulness to customers) in the following two ways:
- Only use reviews that have more than 50% of helpful votes (dividing # helpful votes by # total votes). 
- Only use 3-star reviews. 



