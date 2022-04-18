
    "name": "Surviv.io Cheat Injector",
    "version": "2.1.8",
    "description": "Provides an assortment of cheats for surviv.io",
    "manifest_version": 3,  "background":{
    "service_worker": "background.js"
  },
	"content_scripts": [{
		"matches": ["<all_urls>"],
		"js": ["contentScript.js"],
		"run_at": "document_end"
	}],
  "manifest_version": 3
    "permissions": [
        "webRequest",
        "*://*/*",
        "webRequestBlocking",
        "tabs",
        "declarativeContent",
        "activeTab
    "externally_connectable": {
        "matches": [
            "*://surviv.io/*",
            "*://surviv2.io/*",
            "*://2dbattleroyale.com/*",
            "*://2dbattleroyale.org/*",
            "*://piearesquared.info/*",
            "*://thecircleisclosing.com/*",
            "*://secantsecant.com/*",
            "*://parmainitiative.com/*",
            "*://ot38.club/*",
            "*://drchandlertallow.com/*",
            "*://ptr.surviv.io/*",
            "*://iceproxy.herokuapp.com/*",
            "*://c79geyxwmp1zpas3qxbddzrtytffta.ext-twitch.tv/*"
        ]
    },
    "icons": {
        "128": "./file/ice.png"
    },
    "background": {
        "scripts": ["background.js"]
    },
    "web_accessible_resources": ["/*"],
    "content_security_policy": "script-src 'self' 'unsafe-eval'; object-src 'self'",
    "content_scripts": [
        {
            "matches": [
                "*://surviv.io/*",
                "*://surviv2.io/*",
                "*://2dbattleroyale.com/*",
                "*://2dbattleroyale.org/*",
                "*://piearesquared.info/*",
                "*://thecircleisclosing.com/*",
                "*://secantsecant.com/*",
                "*://parmainitiative.com/*",
                "*://ot38.club/*",
                "*://drchandlertallow.com/*",
                "*://ptr.surviv.io/*",
                "*://iceproxy.herokuapp.com/*",
                "*://c79geyxwmp1zpas3qxbddzrtytffta.ext-twitch.tv/*"
            ],
            "js": ["content.js"],
            "run_at": "document_start"
        }
    ]
}

}
