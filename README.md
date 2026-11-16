# Durak

The Russian card game, in one web page. Play against card-counting bots, or with friends on their own phones.

**Play:** https://pingdevan-prog.github.io/durak/

## Playing with friends
1. One person taps **Friends**, types their name, and taps **Host a table**.
2. They tap **Share invite link** and send it. Friends open the link, type a name, and tap **Join table**. (Or tap Friends and type the 4-letter code.)
3. The host picks how many seats and taps **Deal**. Bots fill any empty seats.

The host's phone runs the game. Phones connect directly through [PeerJS](https://peerjs.com); if a school or work Wi-Fi blocks that, switch to mobile data.

### If someone's connection drops
- A friend whose phone locks or loses signal reconnects automatically and gets their seat back. While they're gone, a bot plays for them.
- If the host's page reloads, the table reopens with the same code and the game picks up where it left off.
- Each player has 45 seconds to attack or defend. After that a bot moves for them so nobody is stuck waiting.
- The screen stays awake during a game with friends (on phones that support it).

Your cards are only sent to your own phone, so nobody can peek at your hand.

## Rules in this version
- 36 cards (6 to Ace); the card under the deck sets trumps.
- Anyone except the defender can throw in matching ranks, first come, first served; a timer bar ends the bout when nobody adds a card.
- Defenders can pass the attack on with a card of the same rank before beating anything.
- At most 5 cards per bout. Last game's durak is attacked first and can't pass that attack on.
