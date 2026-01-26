```json
{
    "scripts": {
        "pre-install-cmd": [
            "curl -s -o patches.json https://raw.githubusercontent.com/awkirin/awk-patches/refs/heads/main/patches.json || echo 'Failed to download patches.json'"
        ],
        "pre-update-cmd": [
            "curl -s -o patches.json https://raw.githubusercontent.com/awkirin/awk-patches/refs/heads/main/patches.json || echo 'Failed to download patches.json'"
        ]
    }
}
```
