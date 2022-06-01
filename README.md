
    "name": "TG-String-Session",
    "description": "A bot for Generating String Session of Telegram Account mostly for Userbots.",
    "repository": "https://github.com/Chandan7900/TG-String-Session",
    "logo": "https://telegra.ph/file/9d25c6bc85a8bfcca98df.jpg",
    "keywords": [
        "python",
        "telegram"
    ],
    "buildpacks": [{
    "url": "heroku/python"
  }],
    "formation": {
        "worker": {
            "quantity": 1,
            "size": "free"
        }
     },
       "addons": [
      {
         "options": {
            "version": "12"
         },
         "plan": "heroku-postgresql"
      }
   ],
    "env": {
        "APP_NAME": {
            "description": "Heroku App Name",
            "value": "",
            "required": true
        },
        "BOT_TOKEN": {
            "description": "Your bot token, as a string.",
            "value": "",
            "required": true
        },
        "API_KEY": {
            "description": "Your Heroku Account API Key from https://dashboard.heroku.com/account ",
            "value": "",
            "required": true
        },
        "API_ID": {
            "description": "Get from https://my.telegram.org",
            "value": "",
            "required": true
        },
        "API_HASH": {
            "description": "Get from https://my.telegram.org",
            "value": "",
            "required": true
        },
        "SUDO": {
            "description": "sudo ids here.",
            "value": "",
            "required": true
        }
    }
}
