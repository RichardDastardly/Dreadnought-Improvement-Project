# Key points
## Sizing
* Resized most British main guns using the bigger mk3 turrets as a baseline - now there should not be a need to rebuild a ship completely just for a turret upgrade ( it may be necessary to move something slightly, some turret rings are larger than others )
* Resized British cruiser/battleship secondaries a little - the Town class turrets were a bit too small, the Dido-type a bit too large. 4" mk5 is now /47 out of the box, mk4 /45. I'm looking for other suitable preset calbres. The light cruiser Town-class turrets got the same slight bump.
* Resized or model-swapped a few cruiser towers to stop them comically overhanging the hull. Swapped the tower from the modernised Dreads into the Armoured Cruiser V hull, it currently lacks the hopeless original Rebuild towers.
* Reworked Advanced Escort Cruiser I, because I could not find a use case for it as it was. Now it's more like the missing Light Cruiser III only with some higher tech stats, the hull is a completely different slimline flush deck cruiser hull, the rear towers were model swapped because the reversed main tower model is dire, and stats are more in line with a better Light Cruiser. I have no idea what to do with AEC II at all...
* Took a pass at reworking Adv Destroyers, because they were hopelessly expensive & useless - IMO the odd bump of accuracy & defensive stats does very little for a destroyer. I took the simple method of building my usual 1921 destroyer on the hull & then fiddling with it until I thought "I'd actually want to buy this", so it's not exactly thoroughly thought through yet. They will do 40kts without massive compromise with gas turbines, which will let them keep up with late model light cruisers. Once the British ones seem sane but something you'd actually want, I'll look at doing the same to the others. Swapped the gigantic front tower out from one from the Dido set ( the French claimed it too... ) and I'm looking for sensible funnels.
* Set USA up with their own Armoured Cruisers so they can lock down lattice masts - also removed the generic battleship flag from some other lattice masts, so I think they'll now just appear on US ships.
* Added some withdrawal chance to the unskippable destroyer ambush mission - I didn't ask anyone to start that mission, I'm fed up with running away in game. The obvious answer is to make them optional, but I haven't looked into that.


# Short guide how to use IDE / GITHUB
## Setup
* Download and install any IDE (eg. [IntelliJ IDEA](https://www.jetbrains.com/idea/download/?section=windows))
* Open Brother Munro's repository in [Github](https://github.com/brothermunro/Dreadnought-Improvement-Project)
  * on Tab **Code**, click on button **Code** and choose **Local** / **HTTPS** and copy the URL
* In IDE choose File / New / Project from Version control
  * Leave Version control on GIT, paste URL and choose a folder, where to save the project
  * if you choose UAD's Mods folder you don't need to copy and the state in the folder would correspond to what's in IDE

## IDE Operations
### Branches
* There's a Main branch, which is a copy of the project (main branch) from the repository
* New branch should be created in order to work on any change
  * You can switch between branches using operation **Checkout** on the branch
  * The current changes will "move" from branch to branch unless those are **shelved**
* You can do a **Checkout** to other person's branch - in Branches / Remote in order to check whatever is in that branch
  * List can be refreshed using **Fetch** operation to get current list
  * The branch needs to be in the Github, where it appears once a **Push** is performed from that branch
  
### Commit and Push changes
* Once the changes are done and ready you should do these operations
  * First you need to make sure the **Main** branch is up to date in order to be able to safely **Merge** it
    * Use operation **Update** on the Main branch
  * When checked out on your work branch use operation **Rebase** and choose **onto Main branch**
    * The operation can either finish successfully itself, if there are no conflicts between the branches, or you need to solve the conflicts -> choose what updates should be chosen
  * You can then use operation **Commit** to choose what files should be Merged into the Main branch (usually all)
    * Give it a description
    * Click on **Commit** if you want to continue to work on it later or **Commit and Push** if ready to be pushed to github and to be merged

### Merge changes
  * In Github repository you can then create a **Merge request** with your commit
    * It's usually prefilled otherwise you'd need to choose From and To branch
  * The merge request can be then reviewed
    * Comments can be created on any line to be checked by a creator and update if needed (ie. work on changes, create another Commit, which needs to be pushed)
  * Once there's no issue with the Merge request it can be **Merged** into the Main to have your changes included
    * Once done you can Update the Main branch on your PC to get the latest changes
    * The branch is at this point still kept in the repository but can be deleted if needed (or to clear the list of branches)

## CSV files
* In the IDE, eg. IntelliJ IDEA there's a plugin (couple of at least) to make editing of CSV files easier
  * Go to Settings / Plugins and search for **CSV Editor** and install it
  * It shows 2 tabs, one with differently coloured columns CSV file and 2nd one in a nice table
    * Edits are highlighted in the Text tab
