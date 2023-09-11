In order to create a new scenario, you need to update the game configurations.

Game configs can be found in the following path: `app/game_configs`.

```bash
game_configs
├── actors
│   ├── ACTOR1.yaml
│   └── ACTOR2.yaml
├── company.yaml
├── gameplay
│   ├── company_website_paths.txt
│   └── seed_text.txt
└── malware
    ├── malware1.yaml
    └── malware2.yaml
```

A brief description of the (mostly) required files
 
| File  | Description |
|---|---|
| ACTOR.yaml | This configuration is user to define the behavior of a threat actor that targets your company. You can have as many threat actors as you want but they must have a valid .yaml file extension. They should also all have different names. |
| company.yaml | This file defines who works are your company and how your company behaves. This is your opportunity to give the game some flavor. |
| company_website_paths.txt | Default paths that people can browse on the company's website. Ask chatgpt to make this for you based on the example.  |
| seed_text.txt | This is any seed text that the engine will used to create "background" subject and other writing. It should be themed after your company. E.g. for a vaccine company, you might try using an academic article about vaccines. |
| malware1.yaml | (optional) Defines the behavior of a malware family. The same malware can be used by multiple actors.  |

