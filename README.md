# python-piper-tts-wrapper

A python package that wraps back around the [piper-tts](https://github.com/rhasspy/piper) app.


## Mission Primer

Imagine any machine to simply talk to you in your native language through the audio device in a natural language.

Simply by installing a package through pip, or running it in a container, giving your machine the ability to speak!

> I know, I'm overselling it, but on the other hand, I'm also a strong believer in setting obvious, but simple goals, and have my imagination run wild on the endless possibilities. ( Mantra: "I can't! Can only true when you I don't try!" ) 


### Basic CLI Wrapper

* CLI command : `mrrobot` (It's a bit corny, but also easy to customize.)

> This section declares the basic principle goal for the first thing to build.

* Create a simple CLI wrapper for the local piper command, this mitigates the end-user to have something like the `say` command on MacOs, but on other Unix-Like and Windows systems through python. Tinking about the game 'Simon Says' and combining that with our primary CLI command `mrrobot` it would become `mrrobot says` to sound out local and remote information by request.

#### Basic CLI Wrapper Requirements

- Ensure piper only runs in a Python Virtual Environment.
- When $VIRTUAL_ENV is null or '' Create a Virtual Environment at `$HOME/venv/

#### CLI Wrapper Self Building Bonus

> This section declares one of the endless possibilities when you're in-control yourself.

* Ensure the structure of this project is simply inherited by any end-user to build-their-own, but easily. For example; When a end-user wants to have a different cli-command, and run from source code on locally built binaries, This should also be made easy by having a command option like `mrrobot build self --cmd-name msrobot` an d a workflow to pulls the source code, build the package for cli command `msrobot`. Appending `--self-terminate` to remove the original command.
