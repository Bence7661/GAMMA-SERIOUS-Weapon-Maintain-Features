# [1.0.1] S.T.A.L.K.E.R G.A.M.M.A SERIOUS Weapon Maintain Features 'n fixes
Adds extra QoL features to the maintain weapon context menu

**Important note: This mod builds heavily on `zzzz_arti_jamming_repairs`. I by no means want to rip off his work.
I chose the file overwrite method instead of monkey patching since these seemed a lot cleaner/maintainable.**

Click this to view changes -> [Changelog](https://github.com/Bence7661/GAMMA-SERIOUS-Weapon-Maintain-Features/wiki)

## Detailed description
### Fixes
- **Fixed**: "Maintain parts" option appearing when there are no parts to clean or repair, preventing an empty menu box.
- **Fixed**: "Maintain parts" menu incorrectly stating that you can clean a part when no cleaning kits are available.
  - Previously, selecting this option would consume a repair kit charge for "cleaning."
  - Now, the menu correctly indicates whether a cleaning kit or repair kit charge will be used.

 ### New Features
- **Added**: A percentile display next to parts in the "Maintain Parts" menu (similar to the "Field Strip" menu). <br> (This is already present in G.A.M.M.A v0.9.3.1 courtesy of - [**SaloEater**](https://github.com/SaloEater))
- **Added**: Three new options to the "Maintain Parts" menu
  - **Clean All**: Cleans all parts or as many as possible based on available cleaning kit charges, starting from the worst-conditioned part to the best.
  - **Repair All**: Repairs all parts in the same manner, using available repair kits.
  - **Maintain All**: Performs a three-step process:
    - Cleans all possible parts.
    - Repairs all possible parts.
    - Repair uncleaned: If some parts were left uncleaned due to a lack of cleaning kit charges, repair kits will be used to complete the cleaning process.
    This process also follows a worst-to-best condition priority.

**All of the above will go from lowest charge kit in stack -> highest charge.**

**Also it will go from lowest condition part -> highest condition part.**
 ### Configurability
- **Clean all minimum condition** (default: 80%): Determines the minimum part condition threshold (%) for batch cleaning weapon parts. <br> So if this option is set to 80% "Clean all" will only clean parts that are equal to or lower than this threshold.
  
- **Replace all minimum condition** (default: 59%): Determines the minimum part condition threshold (%) for batch replacing weapon parts. <br> So if this option is set to 80% "Repair all" will only clean parts that are equal to or lower than this threshold.
  
- **Disable the "maintain all" option** (default: OFF): If you never want to use "maintain all" or if you're an avid misclicker then this one is for you! Removes the "maintain all" option from the "maintain parts" context menu.
  
- **Allow "maintain all" to use repair kits for cleaning** (default: OFF): Maintain all consists of 3 steps: Clean all, Repair all and Repair uncleaned (When clean kits run out, but there are still parts left to clean)
        Allows the "Repair uncleaned" step to consume charges of the repair kit to "replace parts".
        The part condition would still have to be below or equal to the "Clean all minimum condition" option.

- **Part replacing should prioritize barrel** (default: ON): The barrel will always be the first part to be replaced when batch replacing (if it is below or equal to the condition threshold configured).
        "Maintain all" will take this into consideration too!

- **De-clutter menu** (default: OFF): Removes the "&lt;= x %" part from the "clean all" and "replace all" menu options.
  
![image](https://github.com/user-attachments/assets/cc7e70ef-0106-417d-b60c-9dca100ae4ab)
 ## Feature showcase
 Context menu with all components present:
 
 ![image](https://github.com/user-attachments/assets/5a46c2b1-d90f-4e6e-96cc-ef90398e1435)

 After clicking the "maintain all [!]" option a message will pop up showing the maintenance results.
 
 The order of the parts displayed is the order in which they were cleaned/repaired.
 (*Part replacing should prioritize barrel* option is on. That's why it is replaced first):
 
 ![image](https://github.com/user-attachments/assets/1921f771-345f-439e-a335-20d1c6969852)

 Without any cleaning kits:

 ![image](https://github.com/user-attachments/assets/5ebd33cf-32ff-4005-a771-7949c417a866)

 ![image](https://github.com/user-attachments/assets/eac0a2c2-f90d-4c22-93d8-e47dfa5df0b4)

 And with a single cleaning kit charge:

 ![image](https://github.com/user-attachments/assets/ea91ebbe-735a-4bc4-b28e-c0ff3d99e524)

 Left image has the **Allow "maintain all" to use repair kits for cleaning** option off. Right image has it switched on.
 ![image](https://github.com/user-attachments/assets/a30e380c-6a8a-4cdb-b95a-9708dcddea5d)
 ![image](https://github.com/user-attachments/assets/d8305e7e-2797-42b9-af6c-10237423a31a)

 ## Installation

 *G.A.M.M.A v0.9.3.1 and v0.9.3*
 1. Click "Code" -> Download .zip

 ![image](https://github.com/user-attachments/assets/5a4c34cd-38be-45a1-85eb-fbe91686b13b)

 2. Open "Mod Organizer" and click "install a new mod from an archive" then select `GAMMA-SERIOUS-Weapon-Maintain-Features-main.zip`
 3. Tick the little box next to the mod.
 4. Right click mod -> Send to -> Priority:
    - For **v0.9.3.1** set the priority to **524**.
    - For **v0.9.3** set it to **510**
  
  NOTE: If you're using other mods than vanilla then you're probably still fine with the said priorities. If other non-vanilla mods occupy this priority just set mine to be higher (I mean if there's a non-vanilla mod at 524 just set mine to 525)

![image](https://github.com/user-attachments/assets/2324e888-97c8-47f8-a755-0ded5598a48d)

If you're using **v0.9.3** then that's it, you're all set!

For **v0.9.3.1** follow these 2 additional steps:

 5. In the bottom right search for "SaloEater's Replace Shows Parts Health" and disable it. Otherwise your game will crash as soon as you click "maintain parts" (The feature in this mod is also included in mine) (So sorry SaloEater, but the patch completely breaks my mod. This on the other hand breaks my hearth)
 6. Enjoy the cool new features :sunglasses:

## Special thanks to (W.I.P. waiting for consent)
