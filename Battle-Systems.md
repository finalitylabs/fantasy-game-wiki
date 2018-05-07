# Battle Systems

**Mass unit resource battles (non-interactive):**

Buying and finding military units increases two global stats of the players, attack points AP and defense points DP.  Ethergoo handles units with arrays like *unitInfo[5] = Unit(5, 500, 250, 0, 20, 0, 0, 0, true); *while we are going to explore the option of tradable units. We will likely have base units as arrays of packed bytes and rare units as 721 objects. Mining units must provide the vok resources needed to fuel battle campaigns. Vok will need to be burned to amass and move armies into attacking positions against enemy strongholds.

Each mass unit combat results in one of three outcomes:

* Attacker Wins - In this case the attacker will take over or pillage the targets resources

* Defender Wins - Attacker loses all attacking units

* Draw - Both parties lose units 

Attacking and defending units are destroyed during the battle, so great care must be taken when deciding to attack another player. The winner is the one with units left after calculations have been conducted.

*Combat Example:*

Alice attacks Bob - Alice has amassed an army of variable units with a collective AP of 100. Bob has set an army with a collective DP of 90 to defend a resource outpost.  She calculates that she has enough AP, but will suffer heavy losses. Alice spends the necessary Vok to move her army within attack position. She will call the attack function and reduce Bob’s army to nothing, and reduce her own to 10% of what it was before attacking. The remaining troops that Alice have are now defending the resource outpost and she may now position her mining units there.

**Turn-style hero keep battles (interactive):**

Keeps allow players to build more units in parallel like having multiple bases of operation. Once a keeps mass units battle has been lost, the attackers may then initiate a hero battle that will decide whether or not the attackers will take over the defenders keep. These heroes will fight 1v1 turn-based battles until this first heroes HP reduces to 0 hit points declaring them the loser of the battle. The attacker must wait a certain amount of time for their opponent to come online and interactive battle to defend the keep. 
