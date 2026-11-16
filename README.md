# Durak

The Russian card game, in one web page. Play against card-counting bots, or with friends on their own phones.

**Play:** open the GitHub Pages link for this repo (Settings → Pages shows it).

## Playing with friends
1. Everyone opens the same link.
2. One person taps **Friends → Host a table** and shares the 4-letter code.
3. Everyone else taps **Friends**, types the code, and joins. Bots fill empty seats.

The host's phone runs the game, so keep it open while you play. Phones connect directly through [PeerJS](https://peerjs.com); if a school or work Wi-Fi blocks that, try mobile data.

## Rules in this version
- 36 cards (6 to Ace); the card under the deck sets trumps.
- Anyone except the defender can throw in matching ranks, first come, first served; a timer bar ends the bout when nobody adds a card.
- Defenders can pass the attack on with a card of the same rank before beating anything.
- At most 5 cards per bout. Last game's durak is attacked first and can't pass that attack on.
