# tehoblivious.github.io

- i am not a dog
- i am a rabbit
- test test
- there should be a proper index.html now (although static)

TEST TEST LET'S TRY THIS IN VS CODE NOW... HMM.

double lines to get a newline just like \<br>\<br> would do (however, looks like this is true markdown, so it should work with HTML elements too :o hmmm -------> editediteditedit

doing git in vs code sure does make things more complicated, at least how vs code is treating me by using SSH also,

- first of all, working working tree isn't correct, OOOOOH WAIT, I CAN FIX THAT, just change vs code workspace folder to the proper folder since it's ```tehoblivious.github.io\tehoblivious.github.io``` to work properly, so doing ls lists tehoblivious.github.io only instead of the actual files, soooooo ***FIXED*** CORRECT, that DID fix it.
- now doing the ```ls``` command in git bash in vs code CTRL_SHIFT_` should list files instead
- commit some new files to change to add to the push: ```git add -A && git commit -m "Added a java file, updated index, added more readme"```
- do the above command again, since I updated it once again.
- do ```git show --color --pretty=format:%b $COMMIT``` to show differences visually
- then you keep pressing enter if the show is longer than just a few lines
- and it'll eventually mark (END), so type in ```q``` to exit the git show (q as in quit, of course)
- then of course, do ```git push``` (& enter passphrase for your SSH key) once you're ready to sync to your repository

test test 

(add a double line break otherwise it doesn't br)

ahaaaaaaa NICE, so, it seems everything works in VS CODE for GIT except for,

- open a powershell (admin) via windows, don't bother wasting time changing default shells in VS CODE cus then you'd just need to switch back to git bash anyway, waste of time.
- need to manually startup ssh-agent by doing ```Start-Service ssh-agent```
- and check it via ```Get-Service ssh-agent```, should say it's running now!
- try a ```git show --color --pretty=format:%b $COMMIT``` to make sure the staged files show up correctly from the VS CODE GUI (they should)
- hence the only thing really required to use CLI now seems to be a ```git push``` because it requires an SSH passphrase to be entered, which VS CODE seems to be weird with (also, maybe only if you have a passphrase, maybe it's fine if your SSH key doesn't have a passphrase)
