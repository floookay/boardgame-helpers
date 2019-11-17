# How to add new boardgame helpers

1. Copy the `new-helper.html`-template into the folder of the game where you want to contribute. Create a new folder if the game-folder does not exist yet.
2. Rename the template to the name of your helper.
3. Implement your helper!
4. Add your helper to the `folder` constant in the index file, like so:
```JS
const files = {
    // notice that "game1" has to exactly match the folder name
    "game1": {
        "label": "general name for all helpers of the game, should include the game name",
        "color": "color of the games cards: name, RGB or hex",
        "files": [
            {
                // name of the file of your helper
                "file": "my-new-helper.html",
                "label": "label of the helper"
            },
            {
                // ...
            }
        ]
    },
    "game2": {
        // ...
    }
}
```