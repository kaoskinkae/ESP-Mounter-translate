# ESP-Mounter-translate

![AppIcon](https://github.com/user-attachments/assets/6f47e620-4947-431b-8dc4-f4432b8a7b83)


For me, ESP Mounter Pro is the best program for mounting and unmounting EFIs on our Hackintosh. We've been using it for a long time, I think, since Clover. However, the program is only available in English, and the way it's designed makes it impossible to easily translate it into other languages.

This guide is intended to show how we can try to translate our application into the languages ​​we use. In this case, it will be Spanish, since that's the default language on my computer.


Let's start by right-clicking on the program "Show Package Contents." Go to ESP Mounter Pro/Contents/Resources/Base.Iproj. Enter the selected folder and locate the file in question: "MainMenu.nib." Open it with the hexadecimal program "HexFied."

![Captura de pantalla 2025-04-26 a las 9 31 38](https://github.com/user-attachments/assets/17bd2022-cb76-4d5a-a2e6-33c00dcfd032)


Now, we begin converting what's displayed on the screen into readable files that we can convert, in my case, into Spanish.

## How to do this? Let's get to it.

We are going to need to create a file and a folder, the folder in my case as it is in Spanish will be "es.lproj" and the file in question will be "MainMenu.strings" we will open this file with Xcode

![Captura de pantalla 2025-04-26 a las 10 53 49](https://github.com/user-attachments/assets/f4d07d29-3f62-4ef3-9267-0f66f644d26c)


Let's open the file with the HexFied program and start searching for the content you need based on the English texts that appear in the program in question.

![Captura de pantalla 2025-04-26 a las 10 56 27](https://github.com/user-attachments/assets/7caadd36-2331-42ef-a000-509817b57670)


We will look for the three sections that are visually present and can be translated below. We must detail which ones they are. We only need to follow the visual indications we have, indicating first that it is an object to be marked. There are different types of its function "NSButtonCell". We locate the representative value and create a line:

${\color{red}"Intel Corporation, Series Chipset PCH Thermal Controller",}$ /* Class = "NSButtonCell"; title = "run at login"; ObjectID = "vFA-sV-1q0"; */

${\color{red}"Intel Corporation, Series Chipset PCH Thermal Controller",}$ vFA-sV-1q0.title" = "Iniciar sesión";



![Captura de pantalla 2025-04-26 a las 11 14 27](https://github.com/user-attachments/assets/6bd0df7d-e3f6-46aa-aa80-01fbeca401c1)


The entire process or part of it is explained on the Hackintosh Spain YouTube channel, although it is in Spanish, visually it is easy to understand.









