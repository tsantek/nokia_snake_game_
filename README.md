 🐍 I Asked Amazon Q to “Write a Snake Game” — It Actually Did

So this happened: I opened Amazon Q and typed
q chat "write a pygame like snake game"

And within seconds… I had a working version of the classic Snake game. No back and forth. No setup. No tutorials. Just boom — game.
Honestly? That kind of blew my mind.
Here’s what happened after that:

    Why I even tried this in the first place
    What that one prompt gave me
    What I tweaked (with Q’s help)
    Some surprisingly clean code it wrote
    And how fast I had a playable version running

🎮 Why Snake?
I picked Snake for one reason: it’s simple, but not too simple.

    It’s nostalgic (hello, Nokia 3310 vibes)
    It’s got just enough going on — movement, collisions, food logic
    It’s a great test for how far an AI coding assistant can go without much hand-holding And it turns out? It can go really far.

🧠 One Prompt. That’s It.
I literally typed:

q chat "write a pygame like snake game"

And Amazon Q gave me a full script. Not partial. Not "here’s a snippet." A complete, playable game with:

    Snake that moves with arrow keys
    Food that randomly spawns
    Snake that grows when it eats
    Game over when the snake hits itself or the wall No bugs. No missing parts. It ran perfectly after installing pygame. That moment when the window opened and the snake started moving? Felt like magic.

🛠️ I Tweaked It a Bit — With Q’s Help
After that, I got curious. I asked Q to make a few upgrades:
🟩 “Make the snake move faster every 5 food pickups”
It added a speed-up mechanic tied to the score.
🟥 “Don’t let food spawn inside the snake”
Handled with a while loop until it found a safe spot.
🟨 “Add a Game Over screen with score”
Boom. Clean text render using pygame.font.
I didn’t have to write much. Just gave it small, direct prompts, and it adjusted the code instantly.

🧩 Cool Code Snippet
Here’s a small part of code that Q gave me — simple, readable, and solid:

        # Draw game over screen
        if self.game_over:
            game_over_text = self.font.render("GAME OVER!", True, WHITE)
            restart_text = self.font.render("Press SPACE to restart or ESC to quit", True, WHITE)

            # Center the text
            game_over_rect = game_over_text.get_rect(center=(WINDOW_WIDTH // 2, WINDOW_HEIGHT // 2 - 30))
            restart_rect = restart_text.get_rect(center=(WINDOW_WIDTH // 2, WINDOW_HEIGHT // 2 + 10))

            self.screen.blit(game_over_text, game_over_rect)
            self.screen.blit(restart_text, restart_rect)

Not fancy, but gets the job done perfectly. And it all came from that one prompt.

⚡ Time to First Playable: Like 2 Minutes
What blew me away was how fast I went from idea → game.

    No Googling
    No Stack Overflow diving
    No “why won’t this window open” debugging Just: ✅ Prompt ✅ Code ✅ Run It made me realize how useful AI assistants like Amazon Q are even for small, fun dev projects.

Image description

Image description

🧠 Final Thoughts
Sometimes you mess around with AI and expect it to kinda-help. This time? It delivered the entire thing right out of the gate.
I still had fun tweaking and customizing it, but Q basically removed all the friction. I got to just focus on improving and playing — not struggling to get things to work.
Now I’m wondering… what other games could I rebuild like this? Tetris? Pong? Flappy Bird?
Might try them all.
