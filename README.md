# Unity Singleton

Unity singleton base class.

## Setup

In order to use the Singleton class (which extends the MonoBehavior class), just import the Shade namespaace and extend your class that way:

```csharp
using UnityEngine;
using Shade;

public class Game : Singleton<Game>
{
    void Start()
    {
        // Work your magic
    }
    
    public void SomeMethod()
    {
        // Anything can happen in a game, you are the wizard.
    }
}
```

Here, we are using it in the context of a game manager.

## Usage

Once your class is setup, you may retrieve your instance from anywhere in your scripts.

```csharp

Game.instance.SomeMethod()
```

## Credits

This class is a slightly modified version of the default singleton available on Unity's community wiki.
