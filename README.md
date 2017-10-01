# HJKL Karabiner-Elements Vim-style Media Keys for MacOS

I use a happy hacking keyboard and vim a lot.

Since there is no dedicated media key on my keyboard, I started using Karabiner.

Apple then released MacOS and the Karabiner team released Karabiner-Elements.

I finally got around to looking through Karabiner-Elements docs and created HJKL key bindings for the media keys, enjoy!

## How To Install

1. Install [Karabiner-Elements](https://pqrs.org/osx/karabiner/)
2. Edit your karabiner.json file, typically located at ~/.config/karabiner/karabiner.json
3. Copy the karabiner.json file in this repo or just the parts you need
4. Open up Karabiner-Elements and go to the Complex Modifications Tab. VIM Style Media Keys should appear and be good to go!
4. If you found this repo helpful, star it!
5. Feel free to open issues for suggestions if you'd like me to add more or want to contribute, thanks!

## The Key Bindings
1. (Option + H) Play Previous
1. (Option + J) Volume Down
1. (Option + K) Volume Up
1. (Option + L) Play Next


# The location of the configuration file for karabiner-elements
Karabiner-Elements stores configuration to a json file which is located ~/.config/karabiner/karabiner.json

## I don't like your modifier key, how can I change it to suit my needs?
Let's take a look at one of the key binding definitions:

```json
{
  "manipulators": [
    {
      "description": "Remaps Left OPTION + J to Media Key Volume Down",
        "from": {
          "key_code": "j",
          "modifiers": {
            "mandatory": [
              "left_option"
            ]
          }
        },
        "to": [
        {
          "key_code": "volume_decrement"
        }
        ],
        "type": "basic"
    }
  ]
}
```

Just change ```key_code to any key you'd like such as a b c d``` 

You can also change the modifier key to some of these:

- "left_control"
- "right_control"
- "left_command"
- "right_command"
- "left_option"

## Need more help?

Open an issue and I'll help you out.
