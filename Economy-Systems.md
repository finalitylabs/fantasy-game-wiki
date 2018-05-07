# Economy Systems

**_Decentraland Calculations:_**

Here we describe the contested battle arena as represented in 3D by the Decentraland client. This will need parcels of land to be owned and how much is calculated here. We should keep the number of contested keeps/strongholds to a finite N. N=1 is the simplest case and would require the least amount of land contested.

Current Max units of Parcels in DCL: 90,000 

Parcel area in meters: 10m x10m = 100 m^2

Genesis City area: 5592.34073 miles x 5592.34073 miles or 31,274,274.84 mi^2

(for reference the Earth is 196,600,000  mi^2, Genesis is ~16% of Earth’s surface)

A futbal field is ~70m x 100m with an area of (70x100=7000m) so for simplicity we will imagine that (7000/100=70) parcels of DCL land is about one soccer field. With this kind of scale in mind we could do a lot with ~5000 parcels.

**Scalability Technology:**

**_Generalized State-Channels:_**

[https://github.com/SpankChain/general-state-channels](https://github.com/SpankChain/general-state-channels)

State-channels gives the game the ability to play turn based combat in a trustless way that also escrows ether, tokens, and units. Heroes will partake in state-channel based fights.

**_Plasma:_**

We will be building an application specific plasma chain to run the game logic so that transaction fees and consensus lag can be averted. This chain will have a judge contract on the mainnet that can detect illegal state transitions in PLACEHOLDER. This technology will be the first (known) plasma construct that is not bound UTXO based state. 

**Access Token:**

The investors and Finality Labs combined FNT (total supply) will be considered locked in a staking contract during the Alpha and Beta development phase of the game, producing the initial QRT tokens that will be used to purchase access. These tokens represent a preorder voucher for the service provided (The Game). We will stake a finite supply to be issued to the public where ownership of the staked QRT will be proportionally divided between Finality Labs and any investors. All initial sales of QRT will go to paying back investor seed funding. Once seed funding is paid back we will sell QRT turn-based until the investor supply of QRT is depleted. Finality Labs will sell the remainder of the finite QRT supply from the staking event if there is any interest to purchase access remaining. The investor FNT may be unlocked or locked further to alleviate securities concerns.

--------------

