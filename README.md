# 3DS-10.5-Downgrade
An untested downgrade of NATIVE-FIRM from 10.4/10.5 to 10.2

This is crossposted from [reddit](https://www.reddit.com/r/3dshacks/comments/43fj8t/wip_hardmod_users_only_an_untested_downgrade_of/).

*This is a summary / compilation of the information from [this](https://gbatemp.net/threads/possible-leadway-to-downgrade-10-5-0-30u.412735/) thread. Please don't follow any random instructions you find on that thread, there is quite a lot of misinformation going around. This is very much untested and a hardmod is necessary.*

**Do not ask if you can achieve this without a hardmod, you can't.**

This is an apparently working implementation of the "FIRM partitions known-plaintext" exploit detailed [here](https://www.3dbrew.org/wiki/3DS_System_Flaws). Reports of successful downgrades are sparse or unconfirmed, but seeing as anyone who tries this has a hardmod and a NAND backup (hopefully multiple backups kept in multiple locations), there isn't really much that can go wrong.

This should work on both a New and Old 3DS.

Keep in mind throughout this that 10.4 and 10.5 use the same NATIVE-FIRM. Also keep in mind that 10.3 does not have a unique NATIVE-FIRM, and we will be using the 10.2 NATIVE-FIRM.

~

*What you need:*

* Your 10.4 or 10.5 NAND extracted using your hardmod
* [Raugo's autofirm pack](https://mega.nz/#!8lFwxaTA!uxag4JB3wFgI6nPwrwWuwU8lKYsGxO7AjfpARr0Q8HQ) ([Mirror](https://mega.nz/#!MxMzRQKa!b3rugzgHvvMpmBkOKv_ZDW0CvZnRVnfjPpW2JSbFAx8))
* The appropriate decrypted NATIVE-FIRM CIAs downloadable from MEGA
    
    [Old 3DS 10.2 - 0004013800000002 v22313](https://mega.nz/#!osNSEJyL!jqfQJlhwTqmHLxvGfRyXNNUffgM0ze3ZTLdSf7MtkMk) ([Mirror](https://drive.google.com/open?id=0BzPfvjeuhqoDZENDVmR5QzBEMlE))    
    [Old 3DS 10.4 - 0004013800000002 v23341](https://mega.nz/#!Us1CFaKK!pU-bG9Esg30LINlasTP43Sei6aDNnTIzh1ojwECKOrU) ([Mirror](https://drive.google.com/open?id=0BzPfvjeuhqoDbGNDMllpaElpaDA))    
    [New 3DS 10.2 - 0004013820000002 v22313](https://mega.nz/#!tg9gUJKI!3ETGUCmWB_AKYlK5mKJhfMaNJoO_0gqEMFQTi0_65eM) ([Mirror](https://drive.google.com/open?id=0BzPfvjeuhqoDZklNUlQ2aHc1aHc))    
    [New 3DS 10.4 - 0004013820000002 v23341](https://mega.nz/#!t90AiCga!anu5UenuD-uEm6z14n680rQThEgViAsytWh5ZuTa_hc) ([Mirror](https://drive.google.com/open?id=0BzPfvjeuhqoDbFRnV0EtUFlma1E))    

*Instructions*

1. Extract the autofirm pack to a folder of your choice
2. Place a copy of your NAND file (named "nand.bin") in the autofirm folder
3. Download the appropriate decrypted 10.4/10.5 NATIVE-FIRM and the decrypted 10.2 NATIVE-FIRM as CIA files
4. Rename the 10.4/10.5 NATIVE_FIRM file to "firmoriginal.cia" then put it in the autofirm folder
5. Rename the 10.2 NATIVE_FIRM file to "firmnuevo.cia" then put it in the autofirm folder
6. Run "start.bat"
7. If everything worked, then you will have a modified "nand.bin" containing 10.2 NATIVE_FIRM on 10.4/10.5
8. Flash this "nand.bin"
9. Get [access](http://corbindavenport.com/?p=403&new1) to the homebrew channel ([Starter kit here](https://smealum.github.io/ninjhax2/starter.zip)) ([Mirror](https://mega.nz/#!MsUmSJ6b!tp8gNdd7oo9Q3aX3TUFiMoN9e-lfU-1Zx4t0t26UlwM))
10. [Downgrade](http://pastebin.com/m5C0jrVP) to 9.2 ([Mirror](http://pastebin.com/r0xZSgvZ))

~

Please reply with your bugs/issues or with confirmation of a successful downgrade either here or [on the IRC](https://www.rizon.net/chat) (#3dshacks)

~

Thanks to [@swarzesherz](https://gbatemp.net/members/swarzesherz.347970/) and [@ceapr]    (https://gbatemp.net/members/126563/) for their 3DSFat16tool, [/u/StillUsesWindowsXP](https://reddit.com/u/StillUsesWindowsXP) for his homebrew guide, [@Raugo](https://gbatemp.net/members/raugo.356694/) for his autofirm tool, and to the IRC channel for the 9.2 downgrade guide.
