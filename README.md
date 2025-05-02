

## 📋 Overview

QB-Scoreboard is an enhanced scoreboard resource for FiveM QBCore framework. This modern and feature-rich scoreboard provides server administrators and players with a clean interface to view server information, player lists, and job statistics.

## ✨ Features

- **Modern UI Design**: Clean, responsive interface with smooth animations
- **Multiple Tabs**: Organized information in separate tabs (Info, Players, Stats)
- **Player Information**: View player IDs, names, jobs, and playtime
- **Job Statistics**: Track the number of police, EMS, and civilian players
- **Activity Requirements**: Click on activities to view their requirements
- **Customizable**: Easily configure colors, activities, and requirements

## 📥 Installation

1. Download the resource
2. Place the `qb-scoreboard` folder in your server's resources directory
3. Add `ensure qb-scoreboard` to your server.cfg
4. Restart your server or use `refresh` followed by `ensure qb-scoreboard`

## ⚙️ Configuration

You can customize the scoreboard by editing the `config.lua` file:

```lua
Config = Config or {}

Config.Toggle = true               -- Toggle mode (true) or hold key mode (false)
Config.OpenKey = 'HOME'           -- Key to open/close the scoreboard
Config.ShowIDforALL = false       -- Show player IDs above all players when scoreboard is open
Config.MaxPlayers = 48            -- Maximum number of players (default: server max)

-- Configure illegal activities and their police requirements
Config.IllegalActions = {
    ['storerobbery'] = {
        minimumPolice = 1,
        busy = false,
        label = 'Store Robbery',
    },
    -- Add more activities as needed
}

-- Configure requirements for each activity
Config.Requirements = {
    ['storerobbery'] = {
        {name = "Lockpick", count = 1, icon = "fas fa-key"},
        {name = "Weapon", count = 1, icon = "fas fa-gun"},
        {name = "Bag", count = 1, icon = "fas fa-bag-shopping"}
    },
    -- Add more requirements as needed
}
```

## 🎮 Usage

- Press the configured key (default: HOME) to open/close the scoreboard
- Click on tabs to switch between different information views
- Click on activities in the Info tab to view their requirements

## 🔄 Dependencies

- QBCore Framework
- Font Awesome (included)

## 👨‍💻 Developer

### About Anas zreqat - Abo Ahmad 
### Ali hassoun

I am a passionate FiveM developer specializing in QBCore resources. With extensive experience in UI design and Lua scripting, I focus on creating high-quality, user-friendly resources for the FiveM community.

- **Discord**: [Abo Ahmad#1234][Ali hassoun] (https://discord.gg/AwYV28PjEa)
- **GitHub**: [github.com/aboahmad](https://github.com/aboahmad-dev)

## 📜 License

This resource is released under the MIT License. You are free to use, modify, and distribute this resource, provided you include the original copyright notice and permission notice in all copies or substantial portions of the software.

## 📞 Support

For support, feature requests, or bug reports, please join my Discord server or open an issue on GitHub.

---

Made with ❤️ by Anas zreqat - Abo Ahmad | © 2025
