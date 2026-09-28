# Events & Minigames

Besides [voting](voting.md) and [crates](crates.md), there are several smaller ways to earn rewards: chat games, piñata parties, the lottery, the AFK Pool, free kits, and referrals.

## Chat Games

Every **15 minutes** (when at least 2 players are online), a quick game pops up in chat. The first player to answer correctly wins.

Game types:

- **Math**: solve the sum
- **Trivia**: answer the question
- **Multiple choice**: pick the right option
- **Unscramble**: unscramble the word
- **Reaction**: be the first to type the phrase

**Prizes** are mostly **Gems** (3 to 50), with a chance at a **farm spawner** (pig, cow, or sheep) or an **Epic crate key**. It's one of the few ways to earn Gems just by playing.

## Piñata Party

When the server reaches **70 combined votes**, a **Piñata Party** starts. A piñata spawns, and everyone who hits it gets a shot at rewards.

```
/warp pinataparty
```

Every vote you cast counts toward the next party, so [voting daily](voting.md) helps everyone.

## Lottery

The server lottery is a **pick-your-numbers** game paid in money (`$`).

```
/lotto          # open the lottery
```

| | |
|---|---|
| **Price** | <span class="chip money">$1,000</span> per bet |
| **Numbers** | Pick from 1–15 |
| **Draws** | Every **6 hours** |
| **Limit** | Up to **100 tickets** per player, per draw |

Choose your numbers, place your bets, and wait for the draw. The more of the drawn numbers you match, the bigger your prize tier.

!!! warning "Gamble responsibly"
    The lottery is a money sink for most players. Treat tickets as entertainment, not as a way to get rich.

## AFK Pool

Stepping away for a while? Stand in one of the **AFK Pools** at `/warp crates` and keep earning.

| Pool | Reward | How often |
|------|--------|-----------|
| **Money pool** | <span class="chip money">$200–$1,000</span> | Every 60 minutes |
| **Key pool** | 1 **Vote Crate key** | Every 90 minutes |

```
/afkkey         # time left until the next Vote Key (also /afktime)
```

While you're in the key pool, your action bar shows a live countdown.

!!! note "AFK rules still apply"
    The AFK Pool is the **approved** way to earn while away. Using macros, autoclickers, or tricks to dodge AFK detection anywhere else breaks the [rules](../getting-started/rules.md#automation-macros).

## Kits

Free starter kits, refillable every **hour**:

```
/kit            # open the kits menu
```

| Kit | Requirement | Good for |
|-----|-------------|----------|
| **Starter Kit** | Free | Brand-new players |
| **Miner Kit** | Free | Mining trips |
| **Farmer Kit** | Free | Getting a farm going |
| **Dungeon Kit** | <span class="chip money">$25,000</span> | Running [dungeons](../world/dungeons.md) |
| **Ultimate Kit** | <span class="chip money">$150,000</span> | Endgame gear |

Donor ranks from the [Gem Store](../perks/store.md) unlock extra kits (Kit 1–4).

## Daily Rewards

Log in each day and claim your **login reward**. Rewards grow the longer your streak runs. See [Quests & Battle Pass](../progression/quests.md#daily-login-rewards).

```
/rewards
```

## Referral program

Bring a friend and get paid when they stick around.

```
/referralcode           # get your personal code to share
/referralredeem <code>  # (new players) enter a friend's code
/referralstatus         # check progress / trigger the payout
/referral               # help
```

How it works:

1. Share your **referral code** with a friend who has **never joined** before.
2. They run `/referralredeem <your code>` after they join. Each player can only redeem one code, ever.
3. Once they've played **2 hours**, **they** run `/referralstatus` and **you** get <span class="chip money">$250</span>.

!!! tip "Tell your friend to check their status"
    Playtime is only checked when the referred player runs `/referralstatus`. If they never run it, the reward never pays out.

---

**Related:** [Voting](voting.md) · [Crates](crates.md) · [Ways to Earn](../money/making-money.md)
