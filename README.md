# MetinFarmBot

Metin2 Stone Bot (Created for educational and learning purposes)

This bot allows you to automate the collection of stones in Metin2 without using code injection. Instead, it uses image processing algorithms from the OpenCV library.

Main Features:

Metin stone recognition: Stones appear randomly in the world. After destroying them, the player gains items.
User Interface.
Configuration: The bot provides various configuration windows to differentiate the UI and speed up processing.
Navigation Problem: If the bot runs into movement problems (e.g. gets stuck), it uses teleportation scrolls to reset the player's position.
Additional Features: the bot can automatically reset buffs, change equipment, and checks if thief gauntlets are equipped to maximize loot yield.

Captcha Solution: The bot uses the AZCaptcha service to resolve captcha. When a captcha is detected, the bot takes a screenshot and sends it using the API. The service then returns a decoded number.

Technical Details:

The bot scans stones using image processing algorithms. After identifying a stone, it checks its name using OCR and then destroys it.
The captcha system is displayed on the Stellaria server every 15 minutes. In order for the bot to proceed, it sends the captcha image to the backend, where it is recognized by AZCaptcha and then filled in.
