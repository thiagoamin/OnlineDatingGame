# Romantic Interaction Strategic Model

## 1: Introduction

This model examines the interactions between two individuals, Alex and Taylor, who have recently matched on an online dating platform. The dynamics of their interactions are influenced by their respective feelings and intentions, as well as the actions they choose to take based on incomplete information about the other's feelings.

## 2: Modeling the Scenario as a Game

We model this scenario as a game with the following parameters and rules:

1. **Players:**
   - **Alex:** Interested in a physical relationship with Taylor, regardless of emotional feelings.
   - **Taylor:** Interested in a physical relationship only if Alex demonstrates genuine emotional interest.

2. **Information:**
   - **Private Information:** Each player knows their own feelings but not the feelings of the other player.
   - **Public Actions:** Actions taken by each player (e.g., offering or accepting a gift) are observable.

3. **Actions:**
   - **Alex's Action:** Decide whether to offer a valuable gift to Taylor as a demonstration of genuine interest.
   - **Taylor's Action:** Decide whether to accept the gift and consider a physical relationship based on perceived interest.

4. **Payoffs:**
   - If both players are in love, they will end up dating, regardless of physical relationship status.
   - If only one or neither player is in love, they will not date.
   - If Taylor accepts the gift and a physical relationship occurs, and Alex is in love while Taylor is not, Alex may feel hurt and ask for the gift back.
   - If they date, the cost of the gift decreases to $\frac{1}{3}c$, reflecting Alex's happiness with the relationship.

---

### 2.1: Possible Outcomes

The table below summarizes the possible outcomes based on whether Alex and Taylor are in love, whether Alex offers a gift, and whether Taylor accepts the gift.

| Alex loves Taylor? | Taylor loves Alex? | Alex offers a gift? | Taylor accepts the gift? | Payoff for Alex | Payoff for Taylor |
|--------------------|--------------------|---------------------|--------------------------|-----------------|-------------------|
| Yes                | Yes                | Yes                 | Yes                      | $d(A)+s(A)-1/3c$ | $d(T) + s(T) + v$ |
| Yes                | Yes                | Yes                 | No                       | $d(A)$               | $d(T)$           |
| Yes                | Yes                | No                  | -                        | $d(A)$            |  $d(T)$          |
| Yes                | No                 | Yes                 | Yes                      |  $s(A) - c$            |  $s(T) + v - u$   |
| Yes                | No                 | Yes                 | No                       |  $0$                  |  $0$             |
| Yes                | No                 | No                  | -                        |  $0$                  |  $0$              |
| No                 | Yes                | Yes                 | Yes                      |  $s(A) - c$            |  $s(T) + v - u$|
| No                 | Yes                | Yes                 | No                       |  $0$                  |  $0$              |
| No                 | Yes                | No                  | -                        |  $0$                  |  $0$              |
| No                 | No                 | Yes                 | Yes                      |  $s(A) - c$            |  $s(T) + v - u$  |
| No                 | No                 | Yes                 | No                       |  $0$                  |  $0$              |
| No                 | No                 | No                  | -                        |  $0$                  |  $0$              |

Where:
- $d(A)$ and $d(T)$ are the utilities of dating for Alex and Taylor, respectively.
- $s(A)$ and $s(T)$ are the utilities of a physical relation for Alex and Taylor, respectively.
- $c$ is the cost of the gift.
- $v$ is the utility gained by Taylor from receiving the gift.
- $u$ is the cost suffered by Taylor if they have sex but do not end up dating.

---
**Intuition Behind the Payoffs:**

- If both players end up dating, they gain their respective utilities of dating.
- If they have a physical relationship, they gain their respective utilities of the physical relationship.
- If Alex offers a gift and Taylor rejects it, Alex returns the gift without any loss.
- If Taylor accepts the gift, Alex incurs the cost of the gift while Taylor gains utility from receiving it.
- If Taylor accepts the gift and they do not end up dating, Taylor suffers a cost.
- If they end up dating, the cost of the gift decreases to $\frac{1}{3}c$.
- If Alex loves Taylor but Taylor does not reciprocate, and they have a physical relationship, Alex's feelings get hurt, leading to a request to return the gift, which results in no utility change from the gift for both players.

### 2.2: Rules of the Game

1. This is a sequential game.
2. External factors determine whether Alex loves Taylor and whether Taylor loves Alex.
3. Alex and Taylor do not know the other's feelings (two-sided information asymmetry).
4. Alex must decide whether to give Taylor a gift.
5. Taylor must decide whether to accept the gift (and have a physical relationship) or not.
6. If both players love each other, they will end up dating.

### 2.3: Signalling Game

We want this to be a signalling game where Alex only buys the gift if genuinely in love with Taylor. The three elements of this signal are:

1. **Signal:** Alex buying the gift.
2. **Representation:** It signifies that Alex is in love with Taylor.
3. **Credibility:** For the signal to be credible, it must create a separating equilibrium, where different types of senders (in-love Alex and no-love Alex) send different signals (gift or no gift). This provides useful information to the receiver (Taylor).

The conditions for a separating equilibrium will be discussed later.

### 2.4: Modeling Uncertainty and Information Asymmetry

In our model, the uncertainty of whether the players love each other is represented by introducing a non-strategic player called Nature. Nature does not seek to maximize its payoff; rather, it chooses actions according to a probability distribution, thereby incorporating uncertainty into the game. This probabilistic choice by Nature is essential for modeling the external factors that influence the players' feelings. To represent this uncertainty and the resulting information asymmetry, we utilize information sets. An information set is essentially a node in the game tree that indicates a state of uncertainty. This situation exemplifies hidden information, where Alex and Taylor are unaware of the other's feelings. Both players possess a hidden attribute—being in love or not—which remains unobserved by the other.

## 3: Game Tree Representation

The following is a game tree representation of the aforementioned game. In the diagram:

- **Nodes (black dots):** These represent points where players make decisions.
- **Branches:** These represent the actions or choices available at each node.
- **Terminal Nodes:** The payoffs are shown in the terminal nodes and are listed in the order that players make decisions (first Alex, then Taylor).
- **Probabilities:** $p$ represents the probability that Alex loves Taylor, and $q$ represents the probability that Taylor loves Alex.
- **Information Sets:** There are two information sets:
  - One at Alex's nodes, representing Alex's uncertainty about Taylor's feelings.
  - One at Taylor's nodes, representing Taylor's uncertainty about Alex's feelings.
- **Branches:**
  - **P/NP:** Alex's decision to offer a gift (P) or not (NP).
  - **A/D:** Taylor's decision to accept the gift (A) or decline the gift (D).
  - 
**Figure 1:** Game Tree Representation of Online Dating

<img width="766" alt="Screenshot 2024-05-31 at 12 25 21 AM" src="https://github.com/thiagoamin/OnlineDatingGame/assets/122248078/b488ead5-6037-4629-b1d0-74c33b6e2eb0">


