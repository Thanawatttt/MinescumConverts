## Usage

### Item Icons

If you prepare 2D sprites for your 3D models, you can provide the converter with mappings for these sprites to be incorporated into item_texture.json and the exported Geyser mappings. To do so, simply include a file called `sprites.json` in the root of your Java resource pack. The format of this file is as follows:
```json
{
    "leather": [
        {
            "custom_model_data": 1,
            "sprite": "textures/path/to/texture_in_bedrock_rp/texture1"
        },
        {
            "custom_model_data": 2,
            "sprite": "textures/path/to/texture_in_bedrock_rp/texture2"
        }
    ],
    "diamond_axe": [
        {
            "damage_predicate": 2,
            "unbreakable": true,
            "sprite": "textures/path/to/texture_in_bedrock_rp/texture3"
        }
    ]
}
```

### Github Actions

You may also run the converter through Github Actions in this repository by creating an issue with the [Pack Conversion](https://github.com/thanawatttt/MinescumConverts/issues/new?assignees=&labels=conversion&template=pack-conversion.yml&title=%5BPack%5D%3A+) template. You are only required to enter the link to the Java pack, though the options described above may also be configured. Your pack will then be queued for conversion by Github Actions. After conversion is complete, the Github Actions bot will reply to your issue with a link to download your converted pack and associated mappings file. Included in the bundle is a behavior pack and addon to view the models in single player, as well as a configuration file containing the paths to the models converted from the Java resource pack and their corresponding identifiers in the Bedrock resource pack.
