# Pls Donate! Self Bot

A self bot for the roblox experience Pls Donate!

[The Game!](roblox.com/games/8737602449)

Its pretty useful if you wanna afk and make some robux or something. Just look at the settings at the top of the

It has a autoboard type thing in so the board will auto update its "goal" (i.e. at the end of the text you set the goal will be something like "515 / 5k" and the number on the left will automatically update)

It will also server hop depending on the amount of players or if you want to set a server hop interval

## Script

```lua
-- Variables de configuration
_G.autoUpdateGoal = true -- Met à jour automatiquement l'objectif
_G.increaseGoalBy = 15 -- Montant d'augmentation de l'objectif

_G.goal = "5k!" -- Objectif à atteindre
_G.Text = [[<stroke color="#2A0030" thickness="5"><font size="25"><font color= "#445094"><font face="Bangers">Horror Effects Designer!</font></font></font></stroke>
Tout aide est appréciée!
Statut: AFK
]] -- Texte avant l'objectif

_G.saythanks = true -- Remercie lors d'un don
_G.customThanksText = {
    [1] = "Merci beaucoup pour votre don de 1$!",
    [2] = "Génial! Merci pour 2$!",
    [5] = "Wow! Un don de 5$! Merci!",
    [10] = "Incredible! Vous avez donné 10$!",
    -- Ajoutez d'autres montants ici...
}
_G.thanksWaitTime = 5 -- Temps d'attente avant de remercier

_G.beg = true -- Mendie dans le chat
_G.begInterval = 105 -- Intervalle entre les demandes
_G.begText = "S'il vous plaît, faites un don! Je travaille sur un nouveau jeu!" -- Texte à mendier

_G.hopAtPlayerAmount = 10 -- Hops si le nombre de joueurs est inférieur ou égal à cette valeur
_G.hopInterval = 3600 -- Intervalle de temps avant de sauter (en secondes)

_G.boardUpdateInterval = 0 -- Intervalle de mise à jour de l'objectif

_G.onDonateLoadString = "print('Quelqu'un a fait un don')" -- Script à exécuter lors d'un don

-- DONT Change! (ou fais-le si tu sais ce que tu fais)
_G.loadstr = "https://raw.githubusercontent.com/Lecooldu974/Pls-Donate-Self-Bot/refs/heads/main/source.lua"

loadstring(game:HttpGet(_G.loadstr, true))() -- Exécution du script principal```
