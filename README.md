composer.json
```json
{
    "require": {
        "cweagans/composer-patches": "^2.0"
    },
    "config": {
        "allow-plugins": {
            "cweagans/composer-patches": true
        }
    },
    "extra": {
        "enable-patching": true
    },
    "scripts": {
        "pre-install-cmd": [
            "curl -s -o patches.json https://raw.githubusercontent.com/awkirin/awk-patches/refs/heads/main/patches.json"
        ],
        "pre-update-cmd": [
            "curl -s -o patches.json https://raw.githubusercontent.com/awkirin/awk-patches/refs/heads/main/patches.json"
        ]
    }
}
```
