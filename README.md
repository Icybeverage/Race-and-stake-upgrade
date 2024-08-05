# The Race and Stake Game

The workshop demonstrates how to store, manage, and extend data using nested tokens within the Unique Network.


# The Race and Stake Game

Race and Stake game is a phygital experience where users can buy physical RC cars after minting all NFT car upgrades. Players engage in a digital platform to collect parts, which upon completion, qualify them for a real-world item.
- Run `npm install`

## Legend

Let's create a Race and Stake. 
In the game Race and Stake, players can mint NFTs that represent racing cars. Each NFT starts with an empty record—no wins, no losses. 
## Car Upgrades

In the game Race and Stake, players can mint NFTs that represent car parts as upgrades. Each of these parts enhances the car's performance in races.

- **Body Kit Upgrade:** Enhances aerodynamics. ![Body Kit Upgrade](./images/body_kit_upgrade.png)
- **Engine Upgrade:** Boosts engine power. ![Engine Upgrade](./images/engine_upgrade.png)
- **Wheel Upgrade:** Improves traction and speed. ![Wheel Upgrade](./images/wheel_upgrade.png)
- **Booster Upgrade:** Provides a temporary speed boost. ![Booster Upgrade](./images/booster_upgrade.png)

Collect all parts to build the ultimate racing car and compete for exclusive rewards.


Once a player collects all the necessary NFT parts (such as body kits, engines, wheels, and boosters), they can redeem these for a real RC car. This adds an exciting real-world reward to the virtual racing experience, motivating players to engage more deeply with the game and collect all the parts.


<img src="./images/img1.png">

Players can then compete against each other. When a car wins a race, its `Victories` counter increases. If it loses, the `Defeats` counter increments accordingly.

<img src="./images/img2.png">



<img src="./images/img3.png">

### Talking about restrictions

- All NFTs are owned by individual users
- The application can modify NFT properties
- Users cannot directly modify the properties of their NFTs

---


## 1. Create a Racing cars collection

```sh
node ./src/1-collection-cars.js
```

## 2. Create Achievements collection

```sh
node ./src/2-collection-achievement.js
```

## 3. Create at least two car NFTs

Pass the following arguments to the function
- collectionId (step 1)
- owner Substrate address
- owner nickname

For example:

```sh
node ./src/3-create-car.js 3135 5GrwvaEF5zXb26Fz9rcQpDWS57CtERHpNehXCPcNoHGKutQY FastGuy
node ./src/3-create-car.js 3135 5CPuU98SimxwoHZRZCi8hezgnfBwATs8vKo6haqkaP3hUj7X RaceQueen
```

## 4. Play the game

Pass the following arguments to the function
- Cars collectionId (step 1)
- Achievements collectionId (step 2)
- First player's tokenId 
- Second player's tokenId

```sh
node ./src/4-play.js 3132 3133 1 2
```
## Car Selection

Choose your starting car for the Race and Stake game:

- **Toyota Supra:** A sleek, high-performance vehicle perfect for racing. ![Toyota Supra](./images/Toyota_Supra.jpg)
- **Nissan Skyline:** Known for its agility and speed on the track. ![Nissan Skyline](./images/Nissan_skyline.jpg)
