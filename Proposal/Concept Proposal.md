# MTG Token Tracker

## Problem Statement
In Magic: The Gathering (MTG), `tokens` are "virtual" cards that are not a part of a player's library (deck) that are created by effects of other cards. Tokens are a crucial aspect of gameplay, but managing them can be cumbersome. In Limited games, players may not have access to the corresponding token cards, while in constructed formats, players must bring their own tokens. Players currently rely on manual methods for token management, such as using dice, temporary dry-erase cards, other objects to represent tokens, or official token cards.

These manual methods can add to the complexity, expense, room for error, and clutter of an already intricate game, making it difficult for players to focus on strategy, gameplay, and fun.

Token Tracker is a mobile app that streamlines token management to enhance MTG gameplay and allows players to be more efficient and organized to play the game with tokens.

## Ideal user
The ideal user is a Magic: the Gathering player who currently relies on one of the aforementioned manual methods to manage tokens. The player may be of any age, gender, income bracket, education level, or game skill.

![image of board state](./Assets/deck_board_state.jpeg)
*Real board state of a player's 6th turn. The top row are the tokens they have generated so far in the game. Note that the player has had to substitute dice and similar tokens for tokens they do not have enough of.*

## MVP Feature Set

1.  Search for cards
    - The app will allow users to search for tokens to add before or during gameplay
2. Token tracking
   - After a user adds a token from search, the app will 'create' tokens with features to increase or decrease the amount
3. Ouput log
    - Data of when, which, and how many tokens were created or destroyed

### Potential Additional Features

1.  User login to save data remotely
   - Allow users to save their token data remotely so they can access it across multiple devices
2.  Option to change token card art based on user preference
   - Allow users to customize the appearance of their tokens by selecting different card art

## Draft Technology Choices

- [Kotlin Multiplatform](https://kotlinlang.org/docs/multiplatform.html) for cross-platform mobile application development
- [Magic: The Gathering API](https://magicthegathering.io/) for card data
- [Wizard Gatherer](https://gatherer.wizards.com/) database for card images
- [Realm](http://realm.io.s3-website-us-east-1.amazonaws.com/products/realm-database/) for database that will store user's data
- [Gradle](https://gradle.org/) and [Xcode](https://developer.apple.com/xcode/) for deployment on mobile devices

## Additional content
- Wireframes
  - [Game selection view](./Assets/wireframe_select_game.png)
  - [Live game view](./Assets/wireframe_in_game.png)
  - [Card view](./Assets/wireframe_card_info.png)
- [MTG Fandom Wiki article](https://mtg.fandom.com/wiki/Token) on tokens