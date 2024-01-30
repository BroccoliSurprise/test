# Tittel på spillet
## Undertittel på steget du er på
Her skriver du **teksten** som skal vises. Du kan og ``||variables:skrive ting med formattering slik at de blir klikkbare||`` i veiledningen.


```blocks 
let mySprite = sprites.create(img`
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . 7 7 7 . 
    . . . . . . . . . . . 1 7 7 7 . 
    . . . . . . . . . . 1 7 7 7 7 . 
    . . . . . . . . . 7 7 7 7 7 . . 
    . . . . 1 . . . . 7 7 7 7 . . . 
    . . 7 7 7 1 . 7 7 7 7 7 6 . . . 
    . . 7 7 7 7 7 7 7 7 7 6 . . . . 
    . . 7 7 7 7 7 7 7 7 6 . . . . . 
    . . 6 7 7 7 7 7 7 6 . . . . . . 
    . . . 6 7 7 7 7 6 . . . . . . . 
    . . . . 6 7 7 6 . . . . . . . . 
    . . . . . 6 6 6 . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    `, SpriteKind.Player)
mySprite.setVelocity(50, 50)
```

```template
let mySprite = sprites.create(img`
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . 7 7 7 . 
    . . . . . . . . . . . 1 7 7 7 . 
    . . . . . . . . . . 1 7 7 7 7 . 
    . . . . . . . . . 7 7 7 7 7 . . 
    . . . . 1 . . . . 7 7 7 7 . . . 
    . . 7 7 7 1 . 7 7 7 7 7 6 . . . 
    . . 7 7 7 7 7 7 7 7 7 6 . . . . 
    . . 7 7 7 7 7 7 7 7 6 . . . . . 
    . . 6 7 7 7 7 7 7 6 . . . . . . 
    . . . 6 7 7 7 7 6 . . . . . . . 
    . . . . 6 7 7 6 . . . . . . . . 
    . . . . . 6 6 6 . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    `, SpriteKind.Player)
```





```assetjson
{
  "README.md": " ",
  "assets.json": "",
  "main.blocks": "<xml xmlns=\"https://developers.google.com/blockly/xml\"><variables><variable id=\"#BO{hh_#Q/EE0[c:kHpL\">mySprite</variable><variable type=\"KIND_SpriteKind\" id=\"ZYv;0/.Uqnktsi5K,Zq!\">Player</variable><variable type=\"KIND_SpriteKind\" id=\"|7s$zzdS6906-s;+]RNt\">Projectile</variable><variable type=\"KIND_SpriteKind\" id=\"g5ZW90SeX^)KEpm/0yX]\">Food</variable><variable type=\"KIND_SpriteKind\" id=\"MH8{1:yLyB]Hfv{8c^=W\">Enemy</variable></variables><block type=\"pxt-on-start\" x=\"0\" y=\"0\"><statement name=\"HANDLER\"><block type=\"variables_set\"><field name=\"VAR\" id=\"#BO{hh_#Q/EE0[c:kHpL\">mySprite</field><value name=\"VALUE\"><shadow xmlns=\"http://www.w3.org/1999/xhtml\" type=\"math_number\"><field name=\"NUM\">0</field></shadow><block type=\"spritescreate\"><value name=\"img\"><shadow type=\"screen_image_picker\"><field name=\"img\">img`\n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . 7 7 7 . \n. . . . . . . . . . . 1 7 7 7 . \n. . . . . . . . . . 1 7 7 7 7 . \n. . . . . . . . . 7 7 7 7 7 . . \n. . . . 1 . . . . 7 7 7 7 . . . \n. . 7 7 7 1 . 7 7 7 7 7 6 . . . \n. . 7 7 7 7 7 7 7 7 7 6 . . . . \n. . 7 7 7 7 7 7 7 7 6 . . . . . \n. . 6 7 7 7 7 7 7 6 . . . . . . \n. . . 6 7 7 7 7 6 . . . . . . . \n. . . . 6 7 7 6 . . . . . . . . \n. . . . . 6 6 6 . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n. . . . . . . . . . . . . . . . \n`</field><data>{\"commentRefs\":[],\"fieldData\":{\"img\":null}}</data></shadow></value><value name=\"kind\"><shadow type=\"spritekind\"><field name=\"MEMBER\">Player</field></shadow></value></block></value><next><block type=\"spritesetvel\"><value name=\"sprite\"><block type=\"variables_get\"><field name=\"VAR\" id=\"#BO{hh_#Q/EE0[c:kHpL\">mySprite</field></block></value><value name=\"vx\"><shadow type=\"spriteSpeedPicker\"><field name=\"speed\">50</field></shadow></value><value name=\"vy\"><shadow type=\"spriteSpeedPicker\"><field name=\"speed\">50</field></shadow></value><next><block type=\"spritesetsetbounceonwall\"><value name=\"sprite\"><block type=\"variables_get\"><field name=\"VAR\" id=\"#BO{hh_#Q/EE0[c:kHpL\">mySprite</field></block></value><value name=\"on\"><shadow type=\"toggleOnOff\"><field name=\"on\">true</field></shadow></value><next><block type=\"set_current_tilemap\"><value name=\"tilemap\"><shadow type=\"tiles_tilemap_editor\"><field name=\"tilemap\">tilemap`level1`</field><data>{\"commentRefs\":[],\"fieldData\":{\"tilemap\":\"level1\"}}</data></shadow></value></block></next></block></next></block></next></block></statement></block></xml>",
  "main.ts": "let mySprite = sprites.create(img`\n    . . . . . . . . . . . . . . . . \n    . . . . . . . . . . . . 7 7 7 . \n    . . . . . . . . . . . 1 7 7 7 . \n    . . . . . . . . . . 1 7 7 7 7 . \n    . . . . . . . . . 7 7 7 7 7 . . \n    . . . . 1 . . . . 7 7 7 7 . . . \n    . . 7 7 7 1 . 7 7 7 7 7 6 . . . \n    . . 7 7 7 7 7 7 7 7 7 6 . . . . \n    . . 7 7 7 7 7 7 7 7 6 . . . . . \n    . . 6 7 7 7 7 7 7 6 . . . . . . \n    . . . 6 7 7 7 7 6 . . . . . . . \n    . . . . 6 7 7 6 . . . . . . . . \n    . . . . . 6 6 6 . . . . . . . . \n    . . . . . . . . . . . . . . . . \n    . . . . . . . . . . . . . . . . \n    . . . . . . . . . . . . . . . . \n    `, SpriteKind.Player)\nmySprite.setVelocity(50, 50)\nmySprite.setBounceOnWall(true)\ntiles.setCurrentTilemap(tilemap`level1`)\n",
  "pxt.json": "{\n    \"name\": \"Spillmaker-hvordan\",\n    \"description\": \"\",\n    \"dependencies\": {\n        \"device\": \"*\"\n    },\n    \"files\": [\n        \"main.blocks\",\n        \"main.ts\",\n        \"README.md\",\n        \"assets.json\",\n        \"tilemap.g.jres\",\n        \"tilemap.g.ts\"\n    ],\n    \"targetVersions\": {\n        \"branch\": \"v1.13.55\",\n        \"tag\": \"v1.13.55\",\n        \"commits\": \"https://github.com/microsoft/pxt-arcade/commits/1b3fc64620f77c6224e58f0d2efa9ce1db21f906\",\n        \"target\": \"1.13.55\",\n        \"pxt\": \"9.3.10\"\n    },\n    \"preferredEditor\": \"tsprj\"\n}\n",
  "tilemap.g.jres": "{\n    \"transparency16\": {\n        \"data\": \"hwQQABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA==\",\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"tilemapTile\": true\n    },\n    \"level1\": {\n        \"id\": \"level1\",\n        \"mimeType\": \"application/mkcd-tilemap\",\n        \"data\": \"MTAwYTAwMDgwMDAxMDEwMTAxMDEwMjAyMDIwMTAxMDEwMTAxMDEwMTAyMDIwMjAxMDEwMTAyMDIwMjAxMDIwMjAyMDEwMTAxMDIwMjAyMDEwMTAxMDEwMTAxMDEwMjAyMDIwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMTAxMDEwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMDAwMA==\",\n        \"tileset\": [\n            \"myTiles.transparency16\",\n            \"sprites.dungeon.hazardLava1\",\n            \"sprites.dungeon.hazardLava0\"\n        ],\n        \"displayName\": \"level1\"\n    },\n    \"*\": {\n        \"mimeType\": \"image/x-mkcd-f4\",\n        \"dataEncoding\": \"base64\",\n        \"namespace\": \"myTiles\"\n    }\n}",
  "tilemap.g.ts": "// Auto-generated code. Do not edit.\nnamespace myTiles {\n    //% fixedInstance jres blockIdentity=images._tile\n    export const transparency16 = image.ofBuffer(hex``);\n\n    helpers._registerFactory(\"tilemap\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n            case \"level1\":\n            case \"level1\":return tiles.createTilemap(hex`0a0008000101010101020202010101010101010202020101010202020102020201010102020201010101010101020202010101010101010101010101010101010101010101010101010101010101010101010101`, img`\n. . . . . . . . . . \n. . . . . . . . . . \n. . . . . . . . . . \n. . . . . . . . . . \n. . . . . . . . . . \n. . . . . . . . . . \n. . . . . . . . . . \n. . . . . . . . . . \n`, [myTiles.transparency16,sprites.dungeon.hazardLava1,sprites.dungeon.hazardLava0], TileScale.Sixteen);\n        }\n        return null;\n    })\n\n    helpers._registerFactory(\"tile\", function(name: string) {\n        switch(helpers.stringTrim(name)) {\n            case \"transparency16\":return transparency16;\n        }\n        return null;\n    })\n\n}\n// Auto-generated code. Do not edit.\n"
}
```